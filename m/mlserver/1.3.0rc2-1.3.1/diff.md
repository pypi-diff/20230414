# Comparing `tmp/mlserver-1.3.0rc2.tar.gz` & `tmp/mlserver-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlserver-1.3.0rc2.tar", last modified: Thu Apr  6 15:41:09 2023, max compression
+gzip compressed data, was "mlserver-1.3.1.tar", last modified: Fri Apr 14 18:06:37 2023, max compression
```

## Comparing `mlserver-1.3.0rc2.tar` & `mlserver-1.3.1.tar`

### file list

```diff
@@ -1,122 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.210648 mlserver-1.3.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-06 15:41:09.210648 mlserver-1.3.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.202648 mlserver-1.3.0rc2/mlserver/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/batch_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.202648 mlserver-1.3.0rc2/mlserver/batching/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/batching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/batching/adaptive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/batching/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/batching/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/batching/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.202648 mlserver-1.3.0rc2/mlserver/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/cli/init_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/cli/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/cloudevents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.206648 mlserver-1.3.0rc2/mlserver/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/codecs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.206648 mlserver-1.3.0rc2/mlserver/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/dataplane_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/dataplane_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/interceptors.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/model_repository_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/model_repository_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/servicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/grpc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.206648 mlserver-1.3.0rc2/mlserver/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/handlers/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/handlers/dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/handlers/model_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.206648 mlserver-1.3.0rc2/mlserver/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/kafka/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/kafka/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/kafka/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/kafka/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/kafka/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.206648 mlserver-1.3.0rc2/mlserver/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/metrics/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/metrics/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/metrics/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/metrics/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/metrics/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/metrics/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.210648 mlserver-1.3.0rc2/mlserver/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/parallel/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.210648 mlserver-1.3.0rc2/mlserver/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/repository/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/repository/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/repository/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.210648 mlserver-1.3.0rc2/mlserver/rest/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/rest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.210648 mlserver-1.3.0rc2/mlserver/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/types/dataplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/types/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/mlserver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.202648 mlserver-1.3.0rc2/mlserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-06 15:41:09.000000 mlserver-1.3.0rc2/mlserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-06 15:41:09.000000 mlserver-1.3.0rc2/mlserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:41:09.000000 mlserver-1.3.0rc2/mlserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-06 15:41:09.000000 mlserver-1.3.0rc2/mlserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-06 15:41:09.000000 mlserver-1.3.0rc2/mlserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 15:41:09.000000 mlserver-1.3.0rc2/mlserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:41:09.210648 mlserver-1.3.0rc2/openapi/
--rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/openapi/dataplane.json
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/openapi/model_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-06 15:41:09.214649 mlserver-1.3.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-06 15:40:28.000000 mlserver-1.3.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-04-14 18:05:57.000000 mlserver-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 18:05:57.000000 mlserver-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-14 18:06:37.578420 mlserver-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-14 18:05:57.000000 mlserver-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.566420 mlserver-1.3.1/mlserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batch_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.570420 mlserver-1.3.1/mlserver/batching/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/batching/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.570420 mlserver-1.3.1/mlserver/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/init_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cli/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/cloudevents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.570420 mlserver-1.3.1/mlserver/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/codecs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.574420 mlserver-1.3.1/mlserver/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31033 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/dataplane_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/dataplane_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/interceptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/model_repository_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/model_repository_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/servicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/grpc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.574420 mlserver-1.3.1/mlserver/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/handlers/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/handlers/dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/handlers/model_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.574420 mlserver-1.3.1/mlserver/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/kafka/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.574420 mlserver-1.3.1/mlserver/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/metrics/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7749 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/parallel/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/repository/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/repository/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/repository/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/rest/openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19065 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/openapi/dataplane.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/openapi/model_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/openapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/rest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.578420 mlserver-1.3.1/mlserver/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/types/dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/types/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 18:05:58.000000 mlserver-1.3.1/mlserver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:06:37.566420 mlserver-1.3.1/mlserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 18:06:37.000000 mlserver-1.3.1/mlserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-14 18:06:37.582420 mlserver-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-14 18:05:58.000000 mlserver-1.3.1/setup.py
```

### Comparing `mlserver-1.3.0rc2/LICENSE` & `mlserver-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/PKG-INFO` & `mlserver-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver
-Version: 1.3.0rc2
+Version: 1.3.1
 Summary: ML server
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLServer
```

### Comparing `mlserver-1.3.0rc2/README.md` & `mlserver-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/batch_processing.py` & `mlserver-1.3.1/mlserver/batch_processing.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/batching/adaptive.py` & `mlserver-1.3.1/mlserver/batching/adaptive.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/batching/hooks.py` & `mlserver-1.3.1/mlserver/batching/hooks.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/batching/requests.py` & `mlserver-1.3.1/mlserver/batching/requests.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/batching/shape.py` & `mlserver-1.3.1/mlserver/batching/shape.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/cli/build.py` & `mlserver-1.3.1/mlserver/cli/build.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/cli/constants.py` & `mlserver-1.3.1/mlserver/cli/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 
 USER root
 # Install dependencies system-wide, to ensure that they are available for every
 # user and give permissions to (future) environment folder.
 RUN ./hack/build-env.sh . && \\
     mkdir -p ./envs/base && \\
     chown -R 1000:0 ./envs/base && \\
-    chmod -R 776 ./envs/base
+    chmod -R 776 ./envs/base && \\
+    rm -rf /root/.cache/pip
 USER 1000
 
 # Copy everything else
 COPY . .
 
 # Override MLServer's own `CMD` to activate the embedded environment
 # (optionally activating the hot-loaded one as well).
```

### Comparing `mlserver-1.3.0rc2/mlserver/cli/main.py` & `mlserver-1.3.1/mlserver/cli/main.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/cli/serve.py` & `mlserver-1.3.1/mlserver/cli/serve.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/cloudevents.py` & `mlserver-1.3.1/mlserver/cloudevents.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/__init__.py` & `mlserver-1.3.1/mlserver/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/base.py` & `mlserver-1.3.1/mlserver/codecs/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/base64.py` & `mlserver-1.3.1/mlserver/codecs/base64.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/datetime.py` & `mlserver-1.3.1/mlserver/codecs/datetime.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/decorator.py` & `mlserver-1.3.1/mlserver/codecs/decorator.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/errors.py` & `mlserver-1.3.1/mlserver/codecs/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/lists.py` & `mlserver-1.3.1/mlserver/codecs/lists.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/numpy.py` & `mlserver-1.3.1/mlserver/codecs/numpy.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/pandas.py` & `mlserver-1.3.1/mlserver/codecs/pandas.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/string.py` & `mlserver-1.3.1/mlserver/codecs/string.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/codecs/utils.py` & `mlserver-1.3.1/mlserver/codecs/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/env.py` & `mlserver-1.3.1/mlserver/env.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/errors.py` & `mlserver-1.3.1/mlserver/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/converters.py` & `mlserver-1.3.1/mlserver/grpc/converters.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/dataplane_pb2.py` & `mlserver-1.3.1/mlserver/grpc/dataplane_pb2.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/dataplane_pb2_grpc.py` & `mlserver-1.3.1/mlserver/grpc/dataplane_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/interceptors.py` & `mlserver-1.3.1/mlserver/grpc/interceptors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/model_repository.py` & `mlserver-1.3.1/mlserver/grpc/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/model_repository_pb2.py` & `mlserver-1.3.1/mlserver/grpc/model_repository_pb2.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/model_repository_pb2_grpc.py` & `mlserver-1.3.1/mlserver/grpc/model_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/server.py` & `mlserver-1.3.1/mlserver/grpc/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/servicers.py` & `mlserver-1.3.1/mlserver/grpc/servicers.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/grpc/utils.py` & `mlserver-1.3.1/mlserver/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/handlers/custom.py` & `mlserver-1.3.1/mlserver/handlers/custom.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/handlers/dataplane.py` & `mlserver-1.3.1/mlserver/handlers/dataplane.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/handlers/model_repository.py` & `mlserver-1.3.1/mlserver/handlers/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/kafka/handlers.py` & `mlserver-1.3.1/mlserver/kafka/handlers.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/kafka/message.py` & `mlserver-1.3.1/mlserver/kafka/message.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/kafka/server.py` & `mlserver-1.3.1/mlserver/kafka/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/logging.py` & `mlserver-1.3.1/mlserver/logging.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/metrics/context.py` & `mlserver-1.3.1/mlserver/metrics/context.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/metrics/errors.py` & `mlserver-1.3.1/mlserver/metrics/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/metrics/prometheus.py` & `mlserver-1.3.1/mlserver/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/metrics/registry.py` & `mlserver-1.3.1/mlserver/metrics/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/metrics/server.py` & `mlserver-1.3.1/mlserver/metrics/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/middleware.py` & `mlserver-1.3.1/mlserver/middleware.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/model.py` & `mlserver-1.3.1/mlserver/model.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/parallel/dispatcher.py` & `mlserver-1.3.1/mlserver/parallel/dispatcher.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/parallel/errors.py` & `mlserver-1.3.1/mlserver/parallel/errors.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/parallel/messages.py` & `mlserver-1.3.1/mlserver/parallel/messages.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/parallel/model.py` & `mlserver-1.3.1/mlserver/parallel/model.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/parallel/pool.py` & `mlserver-1.3.1/mlserver/parallel/pool.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/parallel/registry.py` & `mlserver-1.3.1/mlserver/parallel/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/parallel/utils.py` & `mlserver-1.3.1/mlserver/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/parallel/worker.py` & `mlserver-1.3.1/mlserver/parallel/worker.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/raw.py` & `mlserver-1.3.1/mlserver/raw.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/registry.py` & `mlserver-1.3.1/mlserver/registry.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/repository/factory.py` & `mlserver-1.3.1/mlserver/repository/factory.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/repository/load.py` & `mlserver-1.3.1/mlserver/repository/load.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/repository/repository.py` & `mlserver-1.3.1/mlserver/repository/repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/rest/app.py` & `mlserver-1.3.1/mlserver/rest/app.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/rest/endpoints.py` & `mlserver-1.3.1/mlserver/rest/endpoints.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/rest/logging.py` & `mlserver-1.3.1/mlserver/rest/logging.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/rest/openapi.py` & `mlserver-1.3.1/mlserver/rest/openapi/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import orjson
 
 from functools import lru_cache
 from typing import Optional, Tuple
 from importlib_resources import files
 
-OPENAPI_SCHEMA_RELATIVE_PATH = "../openapi/dataplane.json"
 MODEL_NAME_PARAMETER = "model_name"
 MODEL_VERSION_PARAMETER = "model_version"
 
 
 @lru_cache
 def get_openapi_schema() -> dict:
-    mlserver_package = __package__.split(".")[0]
-    openapi_schema_path = files(mlserver_package).joinpath(OPENAPI_SCHEMA_RELATIVE_PATH)
+    openapi_schema_path = files(__package__).joinpath("dataplane.json")
     return orjson.loads(openapi_schema_path.read_bytes())
 
 
 def get_model_schema_uri(model_name: str, model_version: Optional[str]) -> str:
     base = f"/v2/models/{model_name}"
     if model_version:
         base = f"{base}/versions/{model_version}"
```

### Comparing `mlserver-1.3.0rc2/mlserver/rest/requests.py` & `mlserver-1.3.1/mlserver/rest/requests.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/rest/responses.py` & `mlserver-1.3.1/mlserver/rest/responses.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/rest/server.py` & `mlserver-1.3.1/mlserver/rest/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/rest/utils.py` & `mlserver-1.3.1/mlserver/rest/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/server.py` & `mlserver-1.3.1/mlserver/server.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/settings.py` & `mlserver-1.3.1/mlserver/settings.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/types/__init__.py` & `mlserver-1.3.1/mlserver/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/types/base.py` & `mlserver-1.3.1/mlserver/types/base.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/types/dataplane.py` & `mlserver-1.3.1/mlserver/types/dataplane.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/types/model_repository.py` & `mlserver-1.3.1/mlserver/types/model_repository.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver/utils.py` & `mlserver-1.3.1/mlserver/utils.py`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/mlserver.egg-info/PKG-INFO` & `mlserver-1.3.1/mlserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlserver
-Version: 1.3.0rc2
+Version: 1.3.1
 Summary: ML server
 Home-page: https://github.com/SeldonIO/MLServer.git
 Author: Seldon Technologies Ltd.
 Author-email: hello@seldon.io
 License: Apache 2.0
 Description: # MLServer
```

### Comparing `mlserver-1.3.0rc2/mlserver.egg-info/SOURCES.txt` & `mlserver-1.3.1/mlserver.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -89,18 +89,19 @@
 mlserver/repository/load.py
 mlserver/repository/repository.py
 mlserver/rest/__init__.py
 mlserver/rest/app.py
 mlserver/rest/endpoints.py
 mlserver/rest/errors.py
 mlserver/rest/logging.py
-mlserver/rest/openapi.py
 mlserver/rest/requests.py
 mlserver/rest/responses.py
 mlserver/rest/server.py
 mlserver/rest/utils.py
+mlserver/rest/openapi/__init__.py
+mlserver/rest/openapi/dataplane.json
+mlserver/rest/openapi/model_repository.json
+mlserver/rest/openapi/schema.py
 mlserver/types/__init__.py
 mlserver/types/base.py
 mlserver/types/dataplane.py
-mlserver/types/model_repository.py
-openapi/dataplane.json
-openapi/model_repository.json
+mlserver/types/model_repository.py
```

### Comparing `mlserver-1.3.0rc2/openapi/dataplane.json` & `mlserver-1.3.1/mlserver/rest/openapi/dataplane.json`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/openapi/model_repository.json` & `mlserver-1.3.1/mlserver/rest/openapi/model_repository.json`

 * *Files identical despite different names*

### Comparing `mlserver-1.3.0rc2/setup.cfg` & `mlserver-1.3.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -30,84 +30,91 @@
 	alibi-detect
 	all-runtimes
 
 [testenv:mlserver]
 deps = 
 	-e{toxinidir}
 	-r{toxinidir}/requirements/dev.txt
+	-r{toxinidir}/requirements/docker.txt
 commands = 
 	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} {toxinidir}/tests
 
 [testenv:sklearn]
 deps = 
 	-e{toxinidir}
 	-e{toxinidir}/runtimes/sklearn
 	-r{toxinidir}/requirements/dev.txt
+	-r{toxinidir}/requirements/docker.txt
 commands = 
 	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} {toxinidir}/runtimes/sklearn
 
 [testenv:xgboost]
 deps = 
 	-e{toxinidir}
 	-e{toxinidir}/runtimes/xgboost
 	-r{toxinidir}/requirements/dev.txt
+	-r{toxinidir}/requirements/docker.txt
 commands = 
 	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} {toxinidir}/runtimes/xgboost
 
 [testenv:lightgbm]
 deps = 
 	-e{toxinidir}
 	-e{toxinidir}/runtimes/lightgbm
 	-r{toxinidir}/requirements/dev.txt
+	-r{toxinidir}/requirements/docker.txt
 commands = 
 	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} {toxinidir}/runtimes/lightgbm
 
 [testenv:mlflow]
 deps = 
 	-e{toxinidir}
 	-e{toxinidir}/runtimes/mlflow
 	-r{toxinidir}/requirements/dev.txt
+	-r{toxinidir}/requirements/docker.txt
 	-r{toxinidir}/runtimes/mlflow/requirements/dev.txt
 commands = 
 	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} {toxinidir}/runtimes/mlflow
 
 [testenv:huggingface]
 deps = 
 	-e{toxinidir}/runtimes/huggingface
 	-r{toxinidir}/requirements/dev.txt
 commands = 
-	pip install -e{toxinidir}
+	pip install -e{toxinidir} -r{toxinidir}/requirements/docker.txt
 	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} {toxinidir}/runtimes/huggingface
 
 [testenv:alibi-explain]
 deps = 
 	-e{toxinidir}/runtimes/alibi-explain
 	-e{toxinidir}
 	-r{toxinidir}/requirements/dev.txt
+	-r{toxinidir}/requirements/docker.txt
 	-r{toxinidir}/runtimes/alibi-explain/requirements/dev.txt
 setenv = 
 	CUDA_VISIBLE_DEVICES =
 commands = 
 	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} {toxinidir}/runtimes/alibi-explain
 
 [testenv:alibi-detect]
 deps = 
 	-e{toxinidir}/runtimes/alibi-detect
 	-r{toxinidir}/requirements/dev.txt
+	-r{toxinidir}/runtimes/alibi-detect/requirements/dev.txt
 setenv = 
 	CUDA_VISIBLE_DEVICES =
 commands = 
-	pip install -e{toxinidir}
+	pip install -e{toxinidir} -r{toxinidir}/requirements/docker.txt
 	pip install --upgrade setuptools pip wheel
 	python -m pytest {posargs} {toxinidir}/runtimes/alibi-detect
 
 [testenv:all-runtimes]
 deps = 
 	-e{toxinidir}/runtimes/alibi-explain
 	-e{toxinidir}/runtimes/alibi-detect
@@ -120,15 +127,16 @@
 	-r{toxinidir}/requirements/dev.txt
 commands = 
 	pip install \
 	-r{toxinidir}/runtimes/mlflow/requirements/dev.txt \
 	-r{toxinidir}/runtimes/alibi-explain/requirements/dev.txt \
 	-r{toxinidir}/runtimes/alibi-detect/requirements/dev.txt
 	pip install \
-	-e{toxinidir}
+	-e{toxinidir} \
+	-r{toxinidir}/requirements/docker.txt
 	python -m pytest {posargs} \
 	{toxinidir}/tests \
 	{toxinidir}/runtimes/alibi-explain \
 	{toxinidir}/runtimes/alibi-detect \
 	{toxinidir}/runtimes/sklearn \
 	{toxinidir}/runtimes/xgboost \
 	{toxinidir}/runtimes/mllib \
```

### Comparing `mlserver-1.3.0rc2/setup.py` & `mlserver-1.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,17 +48,15 @@
         "grpcio",
         # The importlib-resources backport is required to use some
         # functionality added in Python 3.10
         # https://setuptools.pypa.io/en/latest/userguide/datafiles.html#accessing-data-files-at-runtime
         "importlib-resources",
         "numpy",
         "pandas",
-        # Force patch for CVE-2022-1941
-        # https://github.com/huggingface/optimum/issues/733
-        "protobuf == 3.20.3",
+        "protobuf",
         "uvicorn",
         "starlette_exporter",
         "py-grpc-prometheus",
         "uvloop;" + env_marker_cpython,
         "aiokafka",
         "tritonclient[http]>=2.24",
         "aiofiles",
```

