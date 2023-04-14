# Comparing `tmp/streampipes-0.0.2.dev0.tar.gz` & `tmp/streampipes-0.91.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streampipes-0.0.2.dev0.tar", last modified: Thu Feb  9 20:52:02 2023, max compression
+gzip compressed data, was "streampipes-0.91.0.tar", last modified: Fri Apr 14 06:09:38 2023, max compression
```

## Comparing `streampipes-0.0.2.dev0.tar` & `streampipes-0.91.0.tar`

### file list

```diff
@@ -1,75 +1,85 @@
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.968431 streampipes-0.0.2.dev0/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4468 2023-02-09 20:52:02.968278 streampipes-0.0.2.dev0/PKG-INFO
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     3369 2023-02-09 15:19:10.000000 streampipes-0.0.2.dev0/README.md
--rw-r--r--   0 tbossenmaier   (501) staff       (20)       38 2023-02-09 20:52:02.968477 streampipes-0.0.2.dev0/setup.cfg
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     3862 2023-02-09 20:50:54.000000 streampipes-0.0.2.dev0/setup.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.958171 streampipes-0.0.2.dev0/streampipes/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      903 2023-02-09 20:50:54.000000 streampipes-0.0.2.dev0/streampipes/__version__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.959816 streampipes-0.0.2.dev0/streampipes/client/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      863 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/client/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     7962 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/client/client.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2042 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/client/config.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4819 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/client/credential_provider.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.960468 streampipes-0.0.2.dev0/streampipes/endpoint/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      898 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/endpoint/__init__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.961077 streampipes-0.0.2.dev0/streampipes/endpoint/api/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      956 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/endpoint/api/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4347 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/endpoint/api/data_lake_measure.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2840 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/endpoint/api/data_stream.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)    10752 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/endpoint/endpoint.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2042 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/endpoint/exceptions.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.961311 streampipes-0.0.2.dev0/streampipes/endpoint/messaging/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/endpoint/messaging/__init__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.961667 streampipes-0.0.2.dev0/streampipes/function_zoo/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/function_zoo/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     7586 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/function_zoo/river_function.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.962463 streampipes-0.0.2.dev0/streampipes/functions/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/__init__.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.963330 streampipes-0.0.2.dev0/streampipes/functions/broker/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1007 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/broker/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     3474 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/broker/broker.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1845 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/broker/broker_handler.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2826 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/broker/nats_broker.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2333 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/broker/output_collector.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     7501 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/function_handler.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1688 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/registration.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4246 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/streampipes_function.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.964179 streampipes-0.0.2.dev0/streampipes/functions/utils/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/utils/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2577 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/utils/async_iter_handler.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1908 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/utils/data_stream_context.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     5174 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/utils/data_stream_generator.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2066 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/functions/utils/function_context.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.964614 streampipes-0.0.2.dev0/streampipes/model/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4762 2023-02-09 20:49:50.000000 streampipes-0.0.2.dev0/streampipes/model/common.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.965325 streampipes-0.0.2.dev0/streampipes/model/container/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      930 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/container/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1965 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/container/data_lake_measures.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1900 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/container/data_streams.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     8251 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/container/resource_container.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.966408 streampipes-0.0.2.dev0/streampipes/model/resource/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1069 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/resource/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2360 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/resource/data_lake_measure.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4366 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/resource/data_lake_series.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4153 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/resource/data_stream.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     3498 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/resource/function_definition.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2285 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/streampipes/model/resource/resource.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.958959 streampipes-0.0.2.dev0/streampipes.egg-info/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4468 2023-02-09 20:52:02.000000 streampipes-0.0.2.dev0/streampipes.egg-info/PKG-INFO
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     2120 2023-02-09 20:52:02.000000 streampipes-0.0.2.dev0/streampipes.egg-info/SOURCES.txt
--rw-r--r--   0 tbossenmaier   (501) staff       (20)        1 2023-02-09 20:52:02.000000 streampipes-0.0.2.dev0/streampipes.egg-info/dependency_links.txt
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1482 2023-02-09 20:52:02.000000 streampipes-0.0.2.dev0/streampipes.egg-info/requires.txt
--rw-r--r--   0 tbossenmaier   (501) staff       (20)       18 2023-02-09 20:52:02.000000 streampipes-0.0.2.dev0/streampipes.egg-info/top_level.txt
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.957501 streampipes-0.0.2.dev0/tests/
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.967339 streampipes-0.0.2.dev0/tests/client/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2022-11-19 07:10:51.000000 streampipes-0.0.2.dev0/tests/client/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     4780 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/tests/client/test_client.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     1964 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/tests/client/test_credential_provider.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     5464 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/tests/client/test_data_lake_series.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)    18361 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/tests/client/test_endpoint.py
-drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-02-09 20:52:02.968037 streampipes-0.0.2.dev0/tests/functions/
--rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2022-12-31 10:00:24.000000 streampipes-0.0.2.dev0/tests/functions/__init__.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)    17234 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/tests/functions/test_function_handler.py
--rw-r--r--   0 tbossenmaier   (501) staff       (20)     8047 2023-02-09 14:17:48.000000 streampipes-0.0.2.dev0/tests/functions/test_river_function.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.344386 streampipes-0.91.0/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     5323 2023-04-14 06:09:38.344162 streampipes-0.91.0/PKG-INFO
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     3994 2023-04-07 08:31:02.000000 streampipes-0.91.0/README.md
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)       38 2023-04-14 06:09:38.344467 streampipes-0.91.0/setup.cfg
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4253 2023-04-14 06:09:23.000000 streampipes-0.91.0/setup.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.321770 streampipes-0.91.0/streampipes/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      904 2023-04-14 05:54:46.000000 streampipes-0.91.0/streampipes/__version__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.323589 streampipes-0.91.0/streampipes/client/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      863 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/client/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     8765 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/client/client.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2078 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/client/config.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4889 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/client/credential_provider.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.324250 streampipes-0.91.0/streampipes/endpoint/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      898 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/endpoint/__init__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.324881 streampipes-0.91.0/streampipes/endpoint/api/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      956 2023-03-21 15:41:27.000000 streampipes-0.91.0/streampipes/endpoint/api/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)    14121 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/endpoint/api/data_lake_measure.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2775 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/endpoint/api/data_stream.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)    10562 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/endpoint/endpoint.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2042 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/endpoint/exceptions.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.325039 streampipes-0.91.0/streampipes/endpoint/messaging/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/endpoint/messaging/__init__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.325327 streampipes-0.91.0/streampipes/function_zoo/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/function_zoo/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     8227 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/function_zoo/river_function.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.326077 streampipes-0.91.0/streampipes/functions/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/functions/__init__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.334057 streampipes-0.91.0/streampipes/functions/broker/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1064 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     3428 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/broker.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2250 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/broker_handler.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2950 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/kafka_broker.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1468 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/kafka_message_fetcher.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2865 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/nats_broker.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2554 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/broker/output_collector.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     7689 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/function_handler.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1996 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/registration.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4538 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/streampipes_function.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.338746 streampipes-0.91.0/streampipes/functions/utils/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/functions/utils/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2660 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/utils/async_iter_handler.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1910 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/utils/data_stream_context.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2698 2023-04-14 05:54:46.000000 streampipes-0.91.0/streampipes/functions/utils/data_stream_generator.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2054 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/functions/utils/function_context.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.339206 streampipes-0.91.0/streampipes/model/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/streampipes/model/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     6193 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/common.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.339978 streampipes-0.91.0/streampipes/model/container/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      930 2023-03-21 15:41:27.000000 streampipes-0.91.0/streampipes/model/container/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1853 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/container/data_lake_measures.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1796 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/container/data_streams.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     8463 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/container/resource_container.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.341183 streampipes-0.91.0/streampipes/model/resource/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1069 2023-04-07 08:29:39.000000 streampipes-0.91.0/streampipes/model/resource/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2624 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/resource/data_lake_measure.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4463 2023-04-14 05:54:46.000000 streampipes-0.91.0/streampipes/model/resource/data_lake_series.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     5869 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/resource/data_stream.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4108 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/resource/function_definition.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2545 2023-04-07 08:31:02.000000 streampipes-0.91.0/streampipes/model/resource/resource.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.322487 streampipes-0.91.0/streampipes.egg-info/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     5323 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/PKG-INFO
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2385 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/SOURCES.txt
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)        1 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/dependency_links.txt
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1574 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/requires.txt
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)       18 2023-04-14 06:09:38.000000 streampipes-0.91.0/streampipes.egg-info/top_level.txt
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.320912 streampipes-0.91.0/tests/
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.342132 streampipes-0.91.0/tests/client/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/client/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     4780 2023-03-21 15:41:27.000000 streampipes-0.91.0/tests/client/test_client.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     1964 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/client/test_credential_provider.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     5475 2023-04-07 08:29:39.000000 streampipes-0.91.0/tests/client/test_data_lake_series.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)    18372 2023-03-21 15:41:27.000000 streampipes-0.91.0/tests/client/test_endpoint.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.342692 streampipes-0.91.0/tests/endpoint/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/endpoint/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     5128 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/endpoint/test_data_lake_measure.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.343237 streampipes-0.91.0/tests/functions/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/functions/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)    17234 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/functions/test_function_handler.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     8047 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/functions/test_river_function.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.343438 streampipes-0.91.0/tests/model/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/model/__init__.py
+drwxr-xr-x   0 tbossenmaier   (501) staff       (20)        0 2023-04-14 06:09:38.343872 streampipes-0.91.0/tests/model/resource/
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)      784 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/model/resource/__init__.py
+-rw-r--r--   0 tbossenmaier   (501) staff       (20)     2752 2023-03-13 14:44:48.000000 streampipes-0.91.0/tests/model/resource/test_data_stream.py
```

### Comparing `streampipes-0.0.2.dev0/PKG-INFO` & `streampipes-0.91.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: streampipes
-Version: 0.0.2.dev0
+Version: 0.91.0
 Summary: Python library for Apache StreamPipes
-Home-page: https://github.com/apache/streampipes/
+Home-page: https://streampipes.apache.org/docs/docs/python/latest/
 Author: Apache Software Foundation
 Author-email: dev@streampipes.apache.org
 License: Apache License 2.0
+Project-URL: Documentation, https://streampipes.apache.org/docs/docs/python/latest/
+Project-URL: Bug Tracker, https://github.com/apache/streampipes/issues
+Project-URL: Source Code, https://github.com/apache/streampipes
 Keywords: streampipes,iot,iiot,analytics,stream-processing,apache
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -67,45 +70,60 @@
 <br>
 
 **💡The current version of this Python client is still a beta version.**
 <br>
 **This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.**
 <br>
 
+
+## 📚 Documentation
+Please visit our documentation: https://streampipes.apache.org/docs/docs/python/latest/
+There you can find information about how to [get started](https://streampipes.apache.org/docs/docs/python/latest/getting-started/first-steps/),
+follow some [tutorials](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/),
+or discover the library via our [references](https://streampipes.apache.org/docs/docs/python/latest/reference/client/client/).
+<br>
+
+In case you want to access the documentation of the current development state, you can go here:
+
+👉 [development docs 🤓](https://streampipes.apache.org/docs/docs/python/dev/)
+
 ## ⚡️ Quickstart
 
 As a quick example, we demonstrate how to set up and configure a StreamPipes client.
 
 You can simply install the StreamPipes library by running the following command
 ```bash
-%pip install streampipes
+pip install streampipes
 
 # if you want to have the current development state you can also execute
-%pip install git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-python
+pip install git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-python
 ```
 
 ```python
->> > from streampipes.client import StreamPipesClient
->> > from streampipes.client.client_config import StreamPipesClientConfig
->> > from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
-
->>> config = StreamPipesClientConfig(
-...     credential_provider = StreamPipesApiKeyCredentials(
-...         username = "test@streampipes.apache.org",
-...         api_key = "DEMO-KEY",
-...         ),
-...     host_address = "localhost",
-...     http_disabled = True,
-...     port = 80
-...)
+from streampipes.client import StreamPipesClient
+from streampipes.client.config import StreamPipesClientConfig
+from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+
+config = StreamPipesClientConfig(
+    credential_provider = StreamPipesApiKeyCredentials(
+        username = "test@streampipes.apache.org",
+        api_key = "DEMO-KEY",
+    ),
+    host_address = "localhost",
+    https_disabled = True,
+    port = 80
+)
 
->>> client = StreamPipesClient(client_config=config)
->>> client.describe()
+client = StreamPipesClient(client_config=config)
+client.describe()
+```
 
+Output:
+```
 Hi there!
-You are connected to a StreamPipes instance running at http://localhost: 80.
+You are connected to a StreamPipes instance running at http://localhost:80.
 The following StreamPipes resources are available with this client:
 6x DataStreams
 1x DataLakeMeasures
 ```
 
-For more information about how to use the StreamPipes client visit our [introduction example](https://github.com/apache/streampipes/blob/dev/streampipes-client-python/docs/examples/1-introduction-to-streampipes-python-client.ipynb).
+For more information about how to use the StreamPipes client visit our [introduction tutorial](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-Metadata-Version: 2.1 Name: streampipes Version: 0.0.2.dev0 Summary: Python
-library for Apache StreamPipes Home-page: https://github.com/apache/
-streampipes/ Author: Apache Software Foundation Author-email:
-dev@streampipes.apache.org License: Apache License 2.0 Keywords:
+Metadata-Version: 2.1 Name: streampipes Version: 0.91.0 Summary: Python library
+for Apache StreamPipes Home-page: https://streampipes.apache.org/docs/docs/
+python/latest/ Author: Apache Software Foundation Author-email:
+dev@streampipes.apache.org License: Apache License 2.0 Project-URL:
+Documentation, https://streampipes.apache.org/docs/docs/python/latest/ Project-
+URL: Bug Tracker, https://github.com/apache/streampipes/issues Project-URL:
+Source Code, https://github.com/apache/streampipes Keywords:
 streampipes,iot,iiot,analytics,stream-processing,apache Classifier: Development
-Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
+Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering
@@ -25,25 +28,35 @@
   power of StreamPipes to easily connect to and read different data sources,
    especially in the IoT domain, and the amazing universe of data analytics
                              libraries in Python.
 ---
 **ð¡The current version of this Python client is still a beta version.**
 **This means that it is still under development, which may result in frequent
 and extensive API changes, unstable behavior, etc.**
-## â¡ï¸ Quickstart As a quick example, we demonstrate how to set up and
-configure a StreamPipes client. You can simply install the StreamPipes library
-by running the following command ```bash %pip install streampipes # if you want
-to have the current development state you can also execute %pip install
-git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-
-python ``` ```python >> > from streampipes.client import StreamPipesClient >> >
-from streampipes.client.client_config import StreamPipesClientConfig >> > from
-streampipes.client.credential_provider import StreamPipesApiKeyCredentials >>>
-config = StreamPipesClientConfig( ... credential_provider =
-StreamPipesApiKeyCredentials( ... username = "test@streampipes.apache.org", ...
-api_key = "DEMO-KEY", ... ), ... host_address = "localhost", ... http_disabled
-= True, ... port = 80 ...) >>> client = StreamPipesClient(client_config=config)
->>> client.describe() Hi there! You are connected to a StreamPipes instance
-running at http://localhost: 80. The following StreamPipes resources are
-available with this client: 6x DataStreams 1x DataLakeMeasures ``` For more
-information about how to use the StreamPipes client visit our [introduction
-example](https://github.com/apache/streampipes/blob/dev/streampipes-client-
-python/docs/examples/1-introduction-to-streampipes-python-client.ipynb).
+## ð Documentation Please visit our documentation: https://
+streampipes.apache.org/docs/docs/python/latest/ There you can find information
+about how to [get started](https://streampipes.apache.org/docs/docs/python/
+latest/getting-started/first-steps/), follow some [tutorials](https://
+streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
+streampipes-python-client/), or discover the library via our [references]
+(https://streampipes.apache.org/docs/docs/python/latest/reference/client/
+client/).
+In case you want to access the documentation of the current development state,
+you can go here: ð [development docs ð¤](https://streampipes.apache.org/
+docs/docs/python/dev/) ## â¡ï¸ Quickstart As a quick example, we demonstrate
+how to set up and configure a StreamPipes client. You can simply install the
+StreamPipes library by running the following command ```bash pip install
+streampipes # if you want to have the current development state you can also
+execute pip install git+https://github.com/apache/
+streampipes.git#subdirectory=streampipes-client-python ``` ```python from
+streampipes.client import StreamPipesClient from streampipes.client.config
+import StreamPipesClientConfig from streampipes.client.credential_provider
+import StreamPipesApiKeyCredentials config = StreamPipesClientConfig
+( credential_provider = StreamPipesApiKeyCredentials( username =
+"test@streampipes.apache.org", api_key = "DEMO-KEY", ), host_address =
+"localhost", https_disabled = True, port = 80 ) client = StreamPipesClient
+(client_config=config) client.describe() ``` Output: ``` Hi there! You are
+connected to a StreamPipes instance running at http://localhost:80. The
+following StreamPipes resources are available with this client: 6x DataStreams
+1x DataLakeMeasures ``` For more information about how to use the StreamPipes
+client visit our [introduction tutorial](https://streampipes.apache.org/docs/
+docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
```

### Comparing `streampipes-0.0.2.dev0/README.md` & `streampipes-0.91.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -37,45 +37,60 @@
 <br>
 
 **💡The current version of this Python client is still a beta version.**
 <br>
 **This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.**
 <br>
 
+
+## 📚 Documentation
+Please visit our documentation: https://streampipes.apache.org/docs/docs/python/latest/
+There you can find information about how to [get started](https://streampipes.apache.org/docs/docs/python/latest/getting-started/first-steps/),
+follow some [tutorials](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/),
+or discover the library via our [references](https://streampipes.apache.org/docs/docs/python/latest/reference/client/client/).
+<br>
+
+In case you want to access the documentation of the current development state, you can go here:
+
+👉 [development docs 🤓](https://streampipes.apache.org/docs/docs/python/dev/)
+
 ## ⚡️ Quickstart
 
 As a quick example, we demonstrate how to set up and configure a StreamPipes client.
 
 You can simply install the StreamPipes library by running the following command
 ```bash
-%pip install streampipes
+pip install streampipes
 
 # if you want to have the current development state you can also execute
-%pip install git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-python
+pip install git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-python
 ```
 
 ```python
->> > from streampipes.client import StreamPipesClient
->> > from streampipes.client.client_config import StreamPipesClientConfig
->> > from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
-
->>> config = StreamPipesClientConfig(
-...     credential_provider = StreamPipesApiKeyCredentials(
-...         username = "test@streampipes.apache.org",
-...         api_key = "DEMO-KEY",
-...         ),
-...     host_address = "localhost",
-...     http_disabled = True,
-...     port = 80
-...)
+from streampipes.client import StreamPipesClient
+from streampipes.client.config import StreamPipesClientConfig
+from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+
+config = StreamPipesClientConfig(
+    credential_provider = StreamPipesApiKeyCredentials(
+        username = "test@streampipes.apache.org",
+        api_key = "DEMO-KEY",
+    ),
+    host_address = "localhost",
+    https_disabled = True,
+    port = 80
+)
 
->>> client = StreamPipesClient(client_config=config)
->>> client.describe()
+client = StreamPipesClient(client_config=config)
+client.describe()
+```
 
+Output:
+```
 Hi there!
-You are connected to a StreamPipes instance running at http://localhost: 80.
+You are connected to a StreamPipes instance running at http://localhost:80.
 The following StreamPipes resources are available with this client:
 6x DataStreams
 1x DataLakeMeasures
 ```
 
-For more information about how to use the StreamPipes client visit our [introduction example](https://github.com/apache/streampipes/blob/dev/streampipes-client-python/docs/examples/1-introduction-to-streampipes-python-client.ipynb).
+For more information about how to use the StreamPipes client visit our [introduction tutorial](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
```

#### html2text {}

```diff
@@ -10,25 +10,35 @@
   power of StreamPipes to easily connect to and read different data sources,
    especially in the IoT domain, and the amazing universe of data analytics
                              libraries in Python.
 ---
 **ð¡The current version of this Python client is still a beta version.**
 **This means that it is still under development, which may result in frequent
 and extensive API changes, unstable behavior, etc.**
-## â¡ï¸ Quickstart As a quick example, we demonstrate how to set up and
-configure a StreamPipes client. You can simply install the StreamPipes library
-by running the following command ```bash %pip install streampipes # if you want
-to have the current development state you can also execute %pip install
-git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-
-python ``` ```python >> > from streampipes.client import StreamPipesClient >> >
-from streampipes.client.client_config import StreamPipesClientConfig >> > from
-streampipes.client.credential_provider import StreamPipesApiKeyCredentials >>>
-config = StreamPipesClientConfig( ... credential_provider =
-StreamPipesApiKeyCredentials( ... username = "test@streampipes.apache.org", ...
-api_key = "DEMO-KEY", ... ), ... host_address = "localhost", ... http_disabled
-= True, ... port = 80 ...) >>> client = StreamPipesClient(client_config=config)
->>> client.describe() Hi there! You are connected to a StreamPipes instance
-running at http://localhost: 80. The following StreamPipes resources are
-available with this client: 6x DataStreams 1x DataLakeMeasures ``` For more
-information about how to use the StreamPipes client visit our [introduction
-example](https://github.com/apache/streampipes/blob/dev/streampipes-client-
-python/docs/examples/1-introduction-to-streampipes-python-client.ipynb).
+## ð Documentation Please visit our documentation: https://
+streampipes.apache.org/docs/docs/python/latest/ There you can find information
+about how to [get started](https://streampipes.apache.org/docs/docs/python/
+latest/getting-started/first-steps/), follow some [tutorials](https://
+streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
+streampipes-python-client/), or discover the library via our [references]
+(https://streampipes.apache.org/docs/docs/python/latest/reference/client/
+client/).
+In case you want to access the documentation of the current development state,
+you can go here: ð [development docs ð¤](https://streampipes.apache.org/
+docs/docs/python/dev/) ## â¡ï¸ Quickstart As a quick example, we demonstrate
+how to set up and configure a StreamPipes client. You can simply install the
+StreamPipes library by running the following command ```bash pip install
+streampipes # if you want to have the current development state you can also
+execute pip install git+https://github.com/apache/
+streampipes.git#subdirectory=streampipes-client-python ``` ```python from
+streampipes.client import StreamPipesClient from streampipes.client.config
+import StreamPipesClientConfig from streampipes.client.credential_provider
+import StreamPipesApiKeyCredentials config = StreamPipesClientConfig
+( credential_provider = StreamPipesApiKeyCredentials( username =
+"test@streampipes.apache.org", api_key = "DEMO-KEY", ), host_address =
+"localhost", https_disabled = True, port = 80 ) client = StreamPipesClient
+(client_config=config) client.describe() ``` Output: ``` Hi there! You are
+connected to a StreamPipes instance running at http://localhost:80. The
+following StreamPipes resources are available with this client: 6x DataStreams
+1x DataLakeMeasures ``` For more information about how to use the StreamPipes
+client visit our [introduction tutorial](https://streampipes.apache.org/docs/
+docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
```

### Comparing `streampipes-0.0.2.dev0/setup.py` & `streampipes-0.91.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,25 +20,32 @@
 
 import setuptools
 
 # Package meta-data.
 NAME = "streampipes"
 DESCRIPTION = "Python library for Apache StreamPipes"
 LONG_DESCRIPTION_CONTENT_TYPE = "text/markdown"
-URL = "https://github.com/apache/streampipes/"
+URL = "https://streampipes.apache.org/docs/docs/python/latest/"
 EMAIL = "dev@streampipes.apache.org"
 AUTHOR = "Apache Software Foundation"
 REQUIRES_PYTHON = ">=3.8.0"
 
+PROJECT_URLS = {
+    "Documentation": "https://streampipes.apache.org/docs/docs/python/latest/",
+    "Bug Tracker": "https://github.com/apache/streampipes/issues",
+    "Source Code": "https://github.com/apache/streampipes",
+}
+
 # Package requirements.
 base_packages = [
     "pandas>=1.5.1",
     "pydantic>=1.10.2",
     "requests>=2.28.1",
     "nats-py>=2.2.0",
+    "confluent-kafka>=2.0.2"
 ]
 
 dev_packages = base_packages + [
     "autoflake==2.0.0",
     "black==23.1.0",
     "blacken-docs==1.13.0",
     "flake8==6.0.0",
@@ -59,15 +66,16 @@
     "mkdocs-awesome-pages-plugin==2.8.0",
     "mkdocs-material==8.5.11",  # < 9.x.y is required by mkdocs-jupyter
     "mkdocstrings[python]==0.20.0",
     "pytkdocs[numpy-style]>=0.16.1",
     "mkdocs-gen-files==0.4.0",
     "mkdocs-literate-nav==0.6.0",
     "numpydoc==1.5.0",
-    "mkdocs-jupyter==0.22.0 "
+    "mkdocs-jupyter==0.22.0",
+#    "mike @ git+https://github.com/jimporter/mike.git@872f72def32f588908f8251fe512189e0c41f4e2"
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
@@ -76,36 +84,37 @@
 about = {}
 with open(os.path.join(here, "streampipes", "__version__.py")) as f:
     exec(f.read(), about)
 
 # Where the magic happens:
 setuptools.setup(
     name=NAME,
-    version=f'{about["__version__"]}-dev',
+    version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type=LONG_DESCRIPTION_CONTENT_TYPE,
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
+    project_urls=PROJECT_URLS,
     packages=setuptools.find_packages(exclude=("tests",)),
     install_requires=base_packages,
     extras_require={
         "dev": dev_packages,
         "test": dev_packages,
         "docs": docs_packages,
         "all": dev_packages + docs_packages,
     },
     include_package_data=True,
     license="Apache License 2.0",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Manufacturing",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `streampipes-0.0.2.dev0/streampipes/__init__.py` & `streampipes-0.91.0/streampipes/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/__version__.py` & `streampipes-0.91.0/streampipes/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #
 
-VERSION = (0, 0, 2)  # pragma: no cover
+VERSION = (0, 91, 0)  # pragma: no cover
 
 __version__ = ".".join(map(str, VERSION))  # noqa: F401 # pragma: no cover
```

### Comparing `streampipes-0.0.2.dev0/streampipes/client/__init__.py` & `streampipes-0.91.0/streampipes/client/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/client/client.py` & `streampipes-0.91.0/streampipes/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,61 +33,81 @@
 from streampipes.endpoint.endpoint import APIEndpoint
 
 logger = logging.getLogger(__name__)
 
 
 class StreamPipesClient:
     """The client to connect to StreamPipes.
+
     This is the central point of contact with StreamPipes and
     provides all the functionalities to interact with it.
 
     The client provides so-called "endpoints" each of which refers to
     an endpoint of the StreamPipes API, e.g. `.dataLakeMeasureApi`.
-    An endpoint provides the actual methods to interact with StreamPipes
-    API (see endpoint.endpoint.APIEndpoint).
+    An [endpoint][streampipes.endpoint.endpoint] provides the actual methods to interact with StreamPipes
+    API.
 
     Parameters
     ----------
     client_config: StreamPipesClientConfig
         Configures the client to connect properly to the StreamPipes instance.
     logging_level: Optional[int]
-        Influences the log messages emitted by the `StreamPipesClient`.
+        Influences the log messages emitted by the `StreamPipesClient`
+
+    Attributes
+    ----------
+    dataLakeMeasureApi: DataLakeMeasureEndpoint
+        Instance of the data lake measure endpoint
+    dataStreamApi: DataStreamEndpoint
+        Instance of the data stream endpoint
 
     Examples
     --------
 
-    >>> from streampipes.client import StreamPipesClient
-    >>> from streampipes.client.client_config import StreamPipesClientConfig
-    >>> from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
-
-    >>> client_config = StreamPipesClientConfig(
-    ...     credential_provider=StreamPipesApiKeyCredentials(
-    ...         username="test-user",
-    ...         api_key="api-key"
-    ...     ),
-    ...     host_address="localhost",
-    ...     https_disabled=True
-    ... )
+    ```python
+    from streampipes.client import StreamPipesClient
+    from streampipes.client.config import StreamPipesClientConfig
+    from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+    ```
+
+    ```python
+    client_config = StreamPipesClientConfig(
+        credential_provider=StreamPipesApiKeyCredentials(
+             username="test-user",
+             api_key="api-key"
+         ),
+         host_address="localhost",
+         https_disabled=True
+    )
+    ```
 
     The following way of instantiating a client instance is
     intended to be consistent with the StreamPipes Java client.
-    >>> client = StreamPipesClient.create(client_config=client_config)
+    ```python
+    client = StreamPipesClient.create(client_config=client_config)
+    ```
 
     If you prefer a more pythonic way, you can simply write:
-    >>> client = StreamPipesClient(client_config=client_config)
+    ```python
+    client = StreamPipesClient(client_config=client_config)
+    ```
 
     To interact with an endpoint:
-    >>> data_lake_measures = client.dataLakeMeasureApi.all()
+    ```python
+    data_lake_measures = client.dataLakeMeasureApi.all()
+    ```
 
     To inspect returned data as a pandas dataframe:
-    >>> data_lake_measures.to_pandas()
+    ```python
+    data_lake_measures.to_pandas()
     #
     #     measure_name timestamp_field  ... pipeline_is_running num_event_properties
     # 0           test   s0::timestamp  ...               False                    2
     # [1 rows x 6 columns]
+    ```
 
     """
 
     def __init__(
         self,
         client_config: StreamPipesClientConfig,
         logging_level: Optional[int] = logging.INFO,
@@ -95,15 +115,16 @@
         self.client_config = client_config
 
         # set up a requests session
         # this allows to centrally determine the behavior of all requests made
         self.request_session = Session()
         self.request_session.headers.update(self.http_headers)
 
-        self._set_up_logging(logging_level=logging_level)  # type: ignore
+        self.logging_level = logging_level
+        self._set_up_logging(logging_level=self.logging_level)  # type: ignore
 
         # provide all available endpoints here
         # name of the endpoint needs to be consistent with the Java client
         self.dataLakeMeasureApi = DataLakeMeasureEndpoint(parent_client=self)
         self.dataStreamApi = DataStreamEndpoint(parent_client=self)
 
     @staticmethod
@@ -130,15 +151,16 @@
     @classmethod
     def create(
         cls,
         client_config: StreamPipesClientConfig,
         logging_level: int = logging.INFO,
     ) -> StreamPipesClient:
         """Returns an instance of the `StreamPipesPythonClient`.
-        Provides consistency to the Java client.
+
+        Provides consistency to the StreamPipes Java client.
 
         Parameters
         ----------
         client_config: StreamPipesClientConfig
             Configures the client to connect properly to the StreamPipes instance.
         logging_level: Optional[int]
             Influences the log messages emitted by the `StreamPipesClient`.
@@ -147,48 +169,66 @@
         -------
         StreamPipesClient
         """
         return cls(client_config=client_config, logging_level=logging_level)
 
     @property
     def http_headers(self) -> Dict[str, str]:
-        """Returns the HTTP headers required for all requests.
+        """Returns the HTTP headers used for all requests.
+
         The HTTP headers are composed of the authentication headers supplied by the credential
         provider and additional required headers (currently this is only the application header).
 
         Returns
         -------
-        Dictionary with header information as string key-value pairs.
+        http_headers: Dict[str, str]
+            header information for HTTP requests as string key-value pairs.
         """
 
         # create HTTP headers from credential provider and add additional headers needed
         return self.client_config.credential_provider.make_headers(
             {"Application": "application/json"},
         )
 
     @property
     def base_api_path(self) -> str:
         """Constructs the basic API URL from the given `client_config`.
 
         Returns
         -------
-        str of the basic API URL
+        base_api_path: str
+            basic API path of the connected StreamPipes instance
         """
         return (
             f"{'http://' if self.client_config.https_disabled else 'https://'}"
             f"{self.client_config.host_address}:"
             f"{self.client_config.port}/streampipes-backend/"
         )
 
     def describe(self) -> None:
-        """Prints short description of the connected StreamPipes instance and the available resources to the console.
+        """Prints a short description of the connected StreamPipes instance and the available resources to the console.
 
         Returns
         -------
             None
+
+        Examples
+        --------
+
+        ```python
+        client.describe()
+        ```
+        Output:
+        ```
+        Hi there!
+        You are connected to a StreamPipes instance running at http://localhost:80.
+        The following StreamPipes resources are available with this client:
+        6x DataStreams
+        1x DataLakeMeasures
+        ```
         """
 
         # get all endpoints of this client
         available_endpoints = [
             attr_name for attr_name in dir(self) if isinstance(self.__getattribute__(attr_name), APIEndpoint)
         ]
```

### Comparing `streampipes-0.0.2.dev0/streampipes/client/config.py` & `streampipes-0.91.0/streampipes/client/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """
-Implementation of a config class for the StreamPipes client.
+Configuration class for the StreamPipes client.
 """
 
 
 from dataclasses import dataclass
 from typing import Optional
 
 __all__ = [
@@ -30,30 +30,34 @@
 
 from streampipes.client.credential_provider import CredentialProvider
 
 
 @dataclass
 class StreamPipesClientConfig:
     """Configure the StreamPipes client in accordance to the actual StreamPipes instance to connect to.
+
     An instance is provided to the `StreamPipesClient` to configure it properly.
 
     Parameters
     ----------
     credential_provider: CredentialProvider
         Provides the credentials to authenticate with the StreamPipes API.
     host_address:
         Host address of the StreamPipes instance to connect to.
         Should be provided without the protocol/scheme, e.g. as `localhost` or `streampipes.xyz`.
     https_disabled: Optional[bool]
         Determines whether https is used to connect to StreamPipes.
     port: Optional[int]
-        Specifies the port under which the StreamPipes API is available, e.g., `80` (with http) or `443` (with https)
+        Specifies the port under which the StreamPipes API is available,
+        e.g., `80` (with http) or `443` (with https)
 
     Examples
     --------
-    see `StreamPipesClient`
+
+    see [StreamPipesClient][streampipes.client.StreamPipesClient]
+
     """
 
     credential_provider: CredentialProvider
     host_address: str
     https_disabled: Optional[bool] = False
     port: Optional[int] = 80
```

### Comparing `streampipes-0.0.2.dev0/streampipes/client/credential_provider.py` & `streampipes-0.91.0/streampipes/client/credential_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,24 +36,28 @@
 class CredentialProvider(ABC):
     """Abstract implementation of a credential provider.
     Must be inherited by all credential providers.
     """
 
     def make_headers(self, http_headers: Optional[Dict[str, str]] = None) -> Dict[str, str]:
         """Creates the HTTP headers for the specific credential provider.
+
         Concrete authentication headers must be defined in the implementation of a credential provider.
 
         Parameters
         ----------
         http_headers: Optional[Dict[str, str]]
             Additional HTTP headers the generated headers are extended by.
 
         Returns
         -------
-        Dictionary with header information as string key-value pairs.
+        https_headers: Dict[str, str]
+            Dictionary with header information as string key-value pairs. <br>
+            Contains all pairs given as parameter plus the header pairs for authentication
+            determined by the credential provider.
 
         """
         if http_headers is None:
             http_headers = {}
 
         http_headers.update(self._authentication_headers)
 
@@ -69,32 +73,29 @@
         Dictionary with authentication headers as string key-value pairs.
 
         """
         raise NotImplementedError  # pragma: no cover
 
 
 class StreamPipesApiKeyCredentials(CredentialProvider):
-    """A Credential provider that allows authentication via a StreamPipes API Token.
-    This token can be generated via the StreamPipes UI (see how in the project's README).
+    """A credential provider that allows authentication via a StreamPipes API Token.
+
+    The required token can be generated via the StreamPipes UI (see the description on our [start-page](../../../).
 
     Parameters
     ----------
     username: str
         The username to which the API token is granted, e.g., `demo-user@streampipes.apche.org`.
     api_key: str
         The StreamPipes API key as it is displayed in the UI.
 
     Examples
     --------
-    see `StreamPipesClient`
+    see [StreamPipesClient][streampipes.client.StreamPipesClient]
 
-    References
-    ----------
-    [^1]: [StreamPipes Python Client README]
-    (https://github.com/apache/streampipes/blob/dev/streampipes-client-python/README.md#%EF%B8%8F-quickstart)
     """
 
     @classmethod
     def from_env(cls, username_env: str, api_key_env: str) -> StreamPipesApiKeyCredentials:
         """Returns an api key provider parameterized via environment variables.
 
         Parameters
```

### Comparing `streampipes-0.0.2.dev0/streampipes/endpoint/__init__.py` & `streampipes-0.91.0/streampipes/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/endpoint/api/__init__.py` & `streampipes-0.91.0/streampipes/endpoint/api/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/endpoint/api/data_lake_measure.py` & `streampipes-0.91.0/streampipes/model/resource/data_lake_series.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,111 +11,116 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-"""
-Specific implementation of the StreamPipes API's data lake measure endpoints.
-This endpoint allows to consume data stored in StreamPipes' data lake
-"""
-from typing import Tuple, Type
-
-from streampipes.endpoint.endpoint import APIEndpoint
-from streampipes.model.container import DataLakeMeasures
-from streampipes.model.container.resource_container import ResourceContainer
-from streampipes.model.resource import DataLakeSeries
+from __future__ import annotations
+
+import json
+from typing import Any, Dict, List, Optional, Union
+
+import pandas as pd
+from pydantic import StrictInt, StrictStr
+from streampipes.model.resource.resource import Resource
 
 __all__ = [
-    "DataLakeMeasureEndpoint",
+    "DataLakeSeries",
 ]
 
 
-class DataLakeMeasureEndpoint(APIEndpoint):
-    """Implementation of the DataLakeMeasure endpoint.
-    This endpoint provides an interfact to all data stored in the StreamPipes data lake.
-
-    Consequently, it allows uerying metadata about available data sets (see `all()` method).
-    The metadata is returned as an instance of `model.container.DataLakeMeasures`.
+class StreamPipesUnsupportedDataLakeSeries(Exception):
+    """Exception to be raised when the returned data lake series
+    cannot be parsed with the current implementation of the resource.
+    """
 
-    In addition, the endpoint provides direct access to the data stored in the data laka by querying a
-    specific data lake measure using the `get()` method.
+    def __init__(self):
+        super().__init__(
+            "The Data Lake series returned by the API appears "
+            "to have a structure that is not currently supported by the Python client."
+        )
 
-    Parameters
-    ----------
-    parent_client: StreamPipesClient
-        The instance of `client.StreamPipesClient` the endpoint is attached to.
 
-    Examples
-    --------
+class DataLakeSeries(Resource):
+    """Implementation of a resource for data lake series.
+    This resource defines the data model used by its resource container(`model.container.DataLakeMeasures`).
+    It inherits from Pydantic's BaseModel to get all its superpowers,
+    which are used to parse, validate the API response and to easily switch between
+    the Python representation (both serialized and deserialized) and Java representation (serialized only).
+
+    Notes
+    ------
+        This class will only exist temporarily it its current appearance since
+        there are some inconsistencies in the StreamPipes API.
 
-    >>> from streampipes.client import StreamPipesClient
-    >>> from streampipes.client.client_config import StreamPipesClientConfig
-    >>> from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+    """
 
-    >>> client_config = StreamPipesClientConfig(
-    ...     credential_provider=StreamPipesApiKeyCredentials(username="test-user", api_key="api-key"),
-    ...     host_address="localhost",
-    ...     port=8082,
-    ...     https_disabled=True
-    ... )
+    @classmethod
+    def from_json(cls, json_string: str) -> DataLakeSeries:
+        """Creates an instance of `DataLakeSeries` from a given JSON string.
+
+        This method is used by the resource container to parse the JSON response of
+        the StreamPipes API.
+        Currently, it only supports data lake series that consist of exactly one series of data.
 
-    >>> client = StreamPipesClient.create(client_config=client_config)
+        Parameters
+        ----------
+        json_string: str
+            The JSON string the data lake series should be created on.
 
-    >>> data_lake_measures = client.dataLakeMeasureApi.all()
+        Returns
+        -------
+        DataLakeSeries
+            Instance of `DataLakeSeries` that is created based on the given JSON string.
 
-    >>> len(data_lake_measures)
-    5
-    """
+        Raises
+        ------
+        StreamPipesUnsupportedDataLakeSeries
+            If the data lake series returned by the StreamPipes API cannot be parsed
+            with the current version of the Python client.
 
-    @property
-    def _resource_cls(self) -> Type[DataLakeSeries]:
         """
-        Additional reference to resource class.
-        This endpoint deviates from the desired relationship
-        that the resource class of the resource container is
-        the return type of the get endpoint.
-        Therefore, this is only a temporary implementation and will be removed soon.
-        """
-        return DataLakeSeries
 
-    @property
-    def _container_cls(self) -> Type[ResourceContainer]:
-        """Defines the model container class the endpoint refers to.
+        # deserialize JSON string
+        parsed_json = json.loads(json_string)
 
+        # check if the provided JSON has only one data series entry
+        # otherwise raise the proper exception
+        if len(parsed_json["allDataSeries"]) != 1:
+            raise StreamPipesUnsupportedDataLakeSeries()
 
-        Returns
-        -------
-        `model.container.DataLakeMeasures`
-        """
-        return DataLakeMeasures
+        # get the data data series
+        data_series = parsed_json["allDataSeries"][0]
+
+        return cls.parse_obj(data_series)
+
+    def convert_to_pandas_representation(self) -> Dict[str, Union[List[str], List[List[Any]]]]:
+        """Returns the dictionary representation of a data lake series
+        to be used when creating a pandas Dataframe.
 
-    @property
-    def _relative_api_path(self) -> Tuple[str, ...]:
-        """Defines the relative api path to the DataLakeMeasurement endpoint.
-        Each path within the URL is defined as an own string.
+        It contains only the "header rows" (the column names) and "rows" that contain the actual data.
 
         Returns
         -------
-        A tuple of strings of which every represents a path value of the endpoint's API URL.
+        pandas_repr: dict[str, Any]
+            Dictionary with the keys `headers` and `rows`
+
         """
+        return self.dict(include={"headers", "rows"})
 
-        return "api", "v4", "datalake", "measurements"
+    total: StrictInt
+    headers: List[StrictStr]
+    rows: List[List[Any]]
+    tags: Optional[str]
 
-    def get(self, identifier: str) -> DataLakeSeries:
-        """Queries the specified data lake measure from the API.
-
-        Parameters
-        ----------
-        identifier: str
-            The identifier of the data lake measure to be queried.
+    def to_pandas(self) -> pd.DataFrame:
+        """Returns the data lake series in representation of a Pandas Dataframe.
 
         Returns
         -------
-        The specified data lake measure as an instance of the corresponding model class (`model.DataLakeSeries`).
+        pd: pd.DataFrame
+            The data lake series in form of a pandas dataframe
         """
 
-        response = self._make_request(
-            request_method=self._parent_client.request_session.get, url=f"{self.build_url()}/{identifier}"
-        )
-        return self._resource_cls.from_json(json_string=response.text)
+        pandas_representation = self.convert_to_pandas_representation()
+        return pd.DataFrame(data=pandas_representation["rows"], columns=pandas_representation["headers"])
```

### Comparing `streampipes-0.0.2.dev0/streampipes/endpoint/api/data_stream.py` & `streampipes-0.91.0/streampipes/endpoint/api/data_stream.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,41 +30,42 @@
 from streampipes.model.container.resource_container import ResourceContainer
 
 
 class DataStreamEndpoint(APIEndpoint):
     """Implementation of the DataStream endpoint.
 
     Consequently, it allows querying metadata about available data streams (see `all()` method).
-    The metadata is returned as an instance of `model.container.DataStreams`.
-
-    Parameters
-    ----------
-    parent_client: StreamPipesClient
-        The instance of `client.StreamPipesClient` the endpoint is attached to.
+    The metadata is returned as an instance of [`DataStreams`][streampipes.model.container.DataStreams].
 
     Examples
     --------
 
-    >>> from streampipes.client import StreamPipesClient
-    >>> from streampipes.client.client_config import StreamPipesClientConfig
-    >>> from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
-
-    >>> client_config = StreamPipesClientConfig(
-    ...     credential_provider=StreamPipesApiKeyCredentials(username="test-user", api_key="api-key"),
-    ...     host_address="localhost",
-    ...     port=8082,
-    ...     https_disabled=True
-    ... )
-
-    >>> client = StreamPipesClient.create(client_config=client_config)
-
-    >>> data_streams = client.DataStreamEndpoint.all()
-
-    >>> len(data_streams)
+    ```python
+    from streampipes.client import StreamPipesClient
+    from streampipes.client.config import StreamPipesClientConfig
+    from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+
+    client_config = StreamPipesClientConfig(
+        credential_provider=StreamPipesApiKeyCredentials(username="test-user", api_key="api-key"),
+        host_address="localhost",
+        port=8082,
+        https_disabled=True
+    )
+    client = StreamPipesClient.create(client_config=client_config)
+    ```
+
+    ```python
+    # let's get all existing data streams in StreamPipes
+    data_streams = client.dataStreamApi.all()
+    len(data_streams)
+    ```
+    ```
     2
+    ```
+
     """
 
     @property
     def _container_cls(self) -> Type[ResourceContainer]:
         """Defines the model container class the endpoint refers to.
```

### Comparing `streampipes-0.0.2.dev0/streampipes/endpoint/endpoint.py` & `streampipes-0.91.0/streampipes/endpoint/endpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """
 General implementation for an endpoint.
 Provided classes and assets are aimed to be used for developing endpoints.
-An endpoint is provides all options to communicate with a central endpoint of the StreamPipes API in a handy way.
+An endpoint provides all options to communicate with ad dedicated part of StreamPipes in a handy way.
 """
 
 import json
 import logging
 from abc import ABC, abstractmethod
 from http import HTTPStatus
 from typing import Callable, Optional, Tuple, Type, final
@@ -50,47 +50,42 @@
     "Apparently, this user is not allowed to query the resource.\n"
     "Please check the user's permissions or contact your StreamPipes admin.",
     **dict.fromkeys(
         [404, 405],
         "\nOops, there seems to be an issue with the Python Client calling the API inappropriately.\n"
         "This should not happen, but unfortunately did.\n"
         "If you don't mind, it would be awesome to let us know by creating an issue"
-        " at github.com/apache/streampipes.\n"
+        " at https://github.com/apache/streampipes.\n"
         "Please paste the following information to the issue description:\n\n",
     ),
 }
 
 
 class Endpoint(ABC):
-    """Abstract implementation of an StreamPipes endpoint.
+    """Abstract implementation of a StreamPipes endpoint.
 
     Serves as template for all endpoints used for interaction with a StreamPipes instance.
     By design, endpoints are only instantiated within the `__init__` method of the StreamPipesClient.
 
     Parameters
     ----------
     parent_client: StreamPipesClient
-        This parameter expects the instance of the `client.StreamPipesClient` the endpoint is attached to.
+        This parameter expects the instance of `StreamPipesClient` the endpoint is attached to.
 
     """
 
     def __init__(self, parent_client: "StreamPipesClient"):  # type: ignore # noqa: F821
         self._parent_client = parent_client
 
 
 class APIEndpoint(Endpoint):
     """Abstract implementation of an API endpoint.
 
-    Serves as template for all endpoints for the StreamPipes API.
+    Serves as template for all endpoints of the StreamPipes API.
     By design, endpoints are only instantiated within the `__init__` method of the StreamPipesClient.
-
-    Parameters
-    ----------
-    parent_client: StreamPipesClient
-        This parameter expects the instance of the `client.StreamPipesClient` the endpoint is attached to.
     """
 
     @property
     @abstractmethod
     def _container_cls(self) -> Type[ResourceContainer]:
         """Defines the model container class the endpoint refers to.
         This model container class corresponds to the Python data model,
@@ -165,59 +160,63 @@
         else:
             logger.debug("Successfully retrieved resources from %s.", url)
             logger.info("Successfully retrieved all resources.")
 
         return response
 
     def build_url(self) -> str:
-        """Creates the URL of the API path for the endpoint.
+        """Builds the endpoint's URL of the API path.
 
         Returns
         -------
-        The URL of the Endpoint
+        url: str
+            The URL of the endpoint
         """
         return f"{self._parent_client.base_api_path}" f"{'/'.join(api_path for api_path in self._relative_api_path)}"
 
     def all(self) -> ResourceContainer:
         """Get all resources of this endpoint provided by the StreamPipes API.
-        Results are provided as an instance of a `model.container.ResourceContainer` that
+
+        Results are provided as an instance of a `ResourceContainer` that
         allows to handle the returned resources in a comfortable and pythonic way.
 
         Returns
         -------
-        A model container instance (`model.container.ResourceContainer`) bundling the resources returned.
+        container: ResourceContainer
+             container element that bundles the returned resources
         """
 
         response = self._make_request(
             request_method=self._parent_client.request_session.get,
             url=self.build_url(),
         )
         return self._container_cls.from_json(json_string=response.text)
 
-    def get(self, identifier: str) -> Resource:
+    def get(self, identifier: str, **kwargs) -> Resource:
         """Queries the specified resource from the API endpoint.
 
         Parameters
         ----------
         identifier: str
             The identifier of the resource to be queried.
 
         Returns
         -------
-        The specified resource as an instance of the corresponding model class (`model.Resource`).
+        resource: Resource
+            The specified resource as an instance of the corresponding model class.
         """
 
         response = self._make_request(
             request_method=self._parent_client.request_session.get, url=f"{self.build_url()}/{identifier}"
         )
 
         return self._container_cls._resource_cls()(**response.json())
 
     def post(self, resource: Resource) -> None:
-        """Post a resource to the StreamPipes API.
+        """Allows to post a resource to the StreamPipes API.
 
         Parameters
         ----------
         resource: Resource
             The resource to be posted.
 
         Returns
@@ -231,23 +230,19 @@
             data=json.dumps(resource.to_dict(use_source_names=True)),
             headers={"Content-type": "application/json"},
         )
 
 
 class MessagingEndpoint(Endpoint):
     """Abstract implementation of a StreamPipes messaging endpoint.
+
     Serves as template for all endpoints used for interacting with the StreamPipes messaging layer directly.
     Therefore, they need to provide the functionality to talk with the broker system running in StreamPipes.
     By design, endpoints are only instantiated within the `__init__` method of the StreamPipesClient.
 
-    Parameters
-    ----------
-    parent_client: StreamPipesClient
-        This parameter expects the instance of the `client.StreamPipesClient` the endpoint is attached to.
-
     """
 
     def __init__(self, parent_client: "StreamPipesClient"):  # type: ignore # noqa: F821
         self._broker: Optional[Broker] = None
         super().__init__(parent_client=parent_client)
 
     @property
@@ -260,16 +255,16 @@
         Raises
         ------
         MessagingEndpointNotConfiguredError
             If the endpoint is used before the broker instance is set via `configure()`
 
         Returns
         -------
-        The broker instance to be used to communicate with
-        StreamPipes' messaging layer.
+        broker: Broker
+            The broker instance to be used to communicate with StreamPipes' messaging layer.
         """
 
         if self._broker is not None:
             return self._broker
         raise MessagingEndpointNotConfiguredError(
             endpoint_name=f"{self=}".split("=")[0],
         )
@@ -282,14 +277,19 @@
     @final
     def configure(self, broker: Broker) -> None:
         """Configures the message endpoint by setting the broker instance to be used.
 
         This configuration step is required before the endpoint can be actually used.
         The based `broker` instance is passed to an internal property
 
+        Parameters
+        ----------
+        broker: Broker
+            Broker instance that should be used for this endpoint
+
         Returns
-        _______
+        -------
         None
 
         """
 
         self.broker = broker
```

### Comparing `streampipes-0.0.2.dev0/streampipes/endpoint/exceptions.py` & `streampipes-0.91.0/streampipes/endpoint/exceptions.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/endpoint/messaging/__init__.py` & `streampipes-0.91.0/streampipes/endpoint/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/function_zoo/__init__.py` & `streampipes-0.91.0/streampipes/function_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/function_zoo/river_function.py` & `streampipes-0.91.0/streampipes/function_zoo/river_function.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 )
 from streampipes.functions.utils.function_context import FunctionContext
 from streampipes.model.resource.function_definition import FunctionDefinition
 
 
 class RiverFunction(StreamPipesFunction):
     """Implementation of a StreamPipesFunction to enable an easy usage
-    for Online Machine Learning models of the River library.
+    for Online Machine Learning models of the [River library](https://riverml.xyz/).
 
     The function trains the model with the incoming events and publishes the prediction to an output data stream.
 
     Parameters
     ----------
     function_definition: FunctionDefinition
         The function definition which contains the output stream.
@@ -74,23 +74,54 @@
         self.on_start = on_start
         self.on_event = on_event
         self.on_stop = on_stop
 
         self.learning = True
 
     def requiredStreamIds(self) -> List[str]:
-        """Returns the the stream ids."""
+        """Returns the stream ids required by this function.
+
+        Returns
+        -------
+        stream_ids: List[str]
+            List of stream ids required by the function
+
+        """
         return self.stream_ids
 
     def onServiceStarted(self, context: FunctionContext):
-        """Executes the `on_start` function."""
+        """Executes the `on_start` method of the function.
+
+        Parameters
+        ----------
+        context: FunctionContext
+            The functions' context
+
+        Returns
+        -------
+        None
+
+        """
         self.on_start(self, context)
 
     def onEvent(self, event: Dict[str, Any], streamId: str):
-        """Trains the model with the incoming events and sends the prediction back to StreamPipes."""
+        """Trains the model with the incoming events and sends the prediction back to StreamPipes.
+
+        Parameters
+        ----------
+        event: Dict[str, Any]
+            The incoming event that serves as input for the function
+        streamId: str
+            Identifier of the corresponding data stream
+
+        Returns
+        -------
+        None
+
+        """
         self.on_event(self, event, streamId)
         output_event = {}
         if self.supervised:
             y = event.pop(self.target_label)  # type: ignore
             output_event["truth"] = y
         output_event["learning"] = self.learning
         output_event["prediction"] = self.model.predict_one(event)
@@ -107,15 +138,15 @@
         self.on_stop(self)
 
 
 class OnlineML:
     """Wrapper class to enable an easy usage for Online Machine Learning models of the River library.
 
     It creates a StreamPipesFunction to train a model with the incoming events of a data stream and
-    creates an output data stream to publishes the prediction to StreamPipes.
+    creates an output data stream that publishes the prediction to StreamPipes.
 
     Parameters
     ----------
     client: StreamPipesClient
         The client for the StreamPipes API.
     stream_ids: List[str]
         The ids of the data stream to train the model.
@@ -147,15 +178,15 @@
         target_label: Optional[str] = None,
         on_start: Callable[[Any, FunctionContext], None] = lambda self, context: None,
         on_event: Callable[[Any, Dict[str, Any], str], None] = lambda self, event, streamId: None,
         on_stop: Callable[[Any], None] = lambda self: None,
     ):
         self.client = client
 
-        attributes = {"learning": "boolean", "prediction": prediction_type}
+        attributes = {"learning": RuntimeType.BOOLEAN.value, "prediction": prediction_type}
         if supervised:
             attributes["truth"] = prediction_type
             if target_label is None:
                 raise ValueError("You must define a target attribute for a supervised model.")
         output_stream = create_data_stream("prediction", attributes)
         function_definition = FunctionDefinition().add_output_data_stream(output_stream)
         self.sp_function = RiverFunction(
@@ -176,9 +207,9 @@
         ----------
         learning: bool
             Defines if the training should be continued
         """
         self.sp_function.learning = learning
 
     def stop(self):
-        """Stops the function and ends the training for ever."""
+        """Stops the function and ends the training forever."""
         self.function_handler.disconnect()
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/__init__.py` & `streampipes-0.91.0/streampipes/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/broker/__init__.py` & `streampipes-0.91.0/streampipes/functions/broker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from .broker import Broker
+from .kafka_broker import KafkaBroker
 from .nats_broker import NatsBroker
 
 from .broker_handler import SupportedBroker, get_broker  # isort: skip
 
 __all__ = [
     "Broker",
+    "KafkaBroker",
     "NatsBroker",
     "SupportedBroker",
     "get_broker",
 ]
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/broker/broker.py` & `streampipes-0.91.0/streampipes/functions/broker/broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,28 +19,26 @@
 from typing import Any, AsyncIterator, Dict
 
 from streampipes.model.resource.data_stream import DataStream
 
 
 class Broker(ABC):
     """Abstract implementation of a broker.
-    A broker is used to subscribe to a data stream and to consume the published events.
+
+    A broker allows both to subscribe to a data stream and to publish events to a data stream.
     """
 
     async def connect(self, data_stream: DataStream) -> None:
-        """Connects the broker to a server.
+        """Connects to the broker running in StreamPipes.
 
         Parameters
         ----------
-         data_stream: DataStream
+        data_stream: DataStream
             Contains the meta information (resources) for a data stream.
 
-        host_address: str
-            The host address of the server, which the broker connects to.
-
         Returns
         -------
         None
         """
         self.stream_id = data_stream.element_id
         transport_protocol = data_stream.event_grounding.transport_protocols[0]
         self.topic_name = transport_protocol.topic_definition.actual_topic_name
@@ -51,18 +49,16 @@
 
     @abstractmethod
     async def _makeConnection(self, hostname: str, port: int) -> None:
         """Helper function to connect to a server.
 
         Parameters
         ----------
-
         hostname: str
-            The hostname of the of the server, which the broker connects to.
-
+            The hostname of the server, which the broker connects to.
         port: int
             The port number of the connection.
 
         Returns
         -------
         None
         """
@@ -75,20 +71,20 @@
         Returns
         -------
         None
         """
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
-    async def publish_event(self, event: Dict[str, Any]):
+    async def publish_event(self, event: Dict[str, Any]) -> None:
         """Publish an event to a connected data stream.
 
         Parameters
         ----------
-         event: Dict[str, Any]
+        event: Dict[str, Any]
             The event to be published.
 
         Returns
         -------
         None
         """
         raise NotImplementedError  # pragma: no cover
@@ -105,10 +101,11 @@
 
     @abstractmethod
     def get_message(self) -> AsyncIterator:
         """Get the published messages of the subscription.
 
         Returns
         -------
-        An async iterator for the messages.
+        iterator: AsyncIterator
+            An async iterator for the messages.
         """
         raise NotImplementedError  # pragma: no cover
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/broker/broker_handler.py` & `streampipes-0.91.0/streampipes/functions/broker/broker_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,42 +12,51 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from enum import Enum
 
-from streampipes.functions.broker import Broker, NatsBroker
+from streampipes.functions.broker import Broker, KafkaBroker, NatsBroker
 from streampipes.model.resource.data_stream import DataStream
 
 
 class SupportedBroker(Enum):
     """Enum for the supported brokers."""
 
     NATS = "NatsTransportProtocol"
+    KAFKA = "KafkaTransportProtocol"
 
 
 # TODO Exception should be removed once all brokers are implemented.
-class UnsupportedBroker(Exception):
+class UnsupportedBrokerError(Exception):
     """Exception if a broker isn't implemented yet."""
 
     def __init__(self, message):
         super().__init__(message)
 
 
 def get_broker(data_stream: DataStream) -> Broker:  # TODO implementation for more transport_protocols
-    """Get a broker by a name.
+    """Derive the broker for the given data stream.
 
     Parameters
     ----------
-    broker_name: str
-        A string that represents a broker.
+    data_stream: DataStream
+        Data stream instance from which the broker is inferred
 
     Returns
     -------
-    The broker which belongs to the name.
+    broker: Broker
+        The corresponding broker instance derived from data stream.
+
+    Raises
+    ------
+    UnsupportedBrokerError
+        Is raised when the given data stream belongs to a broker that is currently not supported by StreamPipes Python.
     """
     broker_name = data_stream.event_grounding.transport_protocols[0].class_name
     if SupportedBroker.NATS.value in broker_name:
         return NatsBroker()
+    elif SupportedBroker.KAFKA.value in broker_name:
+        return KafkaBroker()
     else:
-        raise UnsupportedBroker(f'The python client doesn\'t include the broker: "{broker_name}" yet')
+        raise UnsupportedBrokerError(f'The python client doesn\'t include the broker: "{broker_name}" yet')
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/broker/nats_broker.py` & `streampipes-0.91.0/streampipes/functions/broker/nats_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,48 +30,51 @@
     async def _makeConnection(self, hostname: str, port: int) -> None:
         """Helper function to connect to a server.
 
         Parameters
         ----------
 
         hostname: str
-            The hostname of the of the server, which the broker connects to.
+            The hostname of the server, which the broker connects to.
 
         port: int
             The port number of the connection.
 
         Returns
         -------
         None
+
         """
         self.nats_client = await connect(f"nats://{hostname}:{port}")
         if self.nats_client.connected_url is not None:
             logger.info(f"Connected to NATS at {self.nats_client.connected_url.netloc}")
 
     async def createSubscription(self) -> None:
         """Creates a subscription to a data stream.
 
         Returns
         -------
         None
+
         """
         self.subscription = await self.nats_client.subscribe(self.topic_name)
         logger.info(f"Subscribed to stream: {self.stream_id}")
 
     async def publish_event(self, event: Dict[str, Any]):
         """Publish an event to a connected data stream.
 
         Parameters
         ----------
-         event: Dict[str, Any]
+        event: Dict[str, Any]
             The event to be published.
 
         Returns
         -------
         None
+
         """
         await self.nats_client.publish(subject=self.topic_name, payload=json.dumps(event).encode("utf-8"))
 
     async def disconnect(self) -> None:
         """Closes the connection to the server.
 
         Returns
@@ -82,10 +85,11 @@
         logger.info(f"Stopped connection to stream: {self.stream_id}")
 
     def get_message(self) -> AsyncIterator:
         """Get the published messages of the subscription.
 
         Returns
         -------
-        An async iterator for the messages.
+        message_iterator: AsyncIterator
+            An async iterator for the messages.
         """
         return self.subscription.messages
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/broker/output_collector.py` & `streampipes-0.91.0/streampipes/functions/broker/output_collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,42 +18,58 @@
 from typing import Any, Coroutine, Dict
 
 from streampipes.functions.broker import get_broker
 from streampipes.model.resource.data_stream import DataStream
 
 
 class OutputCollector:
-    """Collector for output events.The events are published to an output data stream.
-    Therefore the output collector establishes a connection to the broker.
+    """Collector for output events. The events are published to an output data stream.
+    Therefore, the output collector establishes a connection to the broker.
 
     Parameters
     ----------
-        data_stream: DataStream
-            The output data stream that will receive the events.
+    data_stream: DataStream
+        The output data stream that will receive the events.
+
+    Attributes
+    ----------
+    broker: Broker
+        The broker instance that sends the data to StreamPipes
+
     """
 
     def __init__(self, data_stream: DataStream) -> None:
         self.broker = get_broker(data_stream)
         self._run_coroutine(self.broker.connect(data_stream))
 
     def collect(self, event: Dict[str, Any]) -> None:
         """Publishes an event to the output stream.
 
         Parameters
         ----------
         event: Dict[str, Any]
             The event to be published.
+
+        Returns
+        -------
+        None
         """
         self._run_coroutine(self.broker.publish_event(event))
 
     def disconnect(self) -> None:
-        """Disconnects the broker of the output collector."""
+        """Disconnects the broker of the output collector.
+
+        Returns
+        -------
+        None
+        """
         self._run_coroutine(self.broker.disconnect())
 
-    def _run_coroutine(self, coroutine: Coroutine) -> None:
+    @staticmethod
+    def _run_coroutine(coroutine: Coroutine) -> None:
         """Run a coroutine in the event loop or create a new one if there is a running event loop.
 
         Parameters
         ----------
         coroutine: Coroutine
             The coroutine to run.
         """
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/function_handler.py` & `streampipes-0.91.0/streampipes/functions/function_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,34 +27,42 @@
 from streampipes.functions.utils.function_context import FunctionContext
 from streampipes.model.resource.data_stream import DataStream
 
 logger = logging.getLogger(__name__)
 
 
 class FunctionHandler:
-    """The function handler manages the StreamPipesFunctions.
+    """The function handler manages the StreamPipes Functions.
+
     It controls the connection to the brokers, starts the functions, manages the broadcast of the live data
     and is able to stop the connection to the brokers and functions.
 
     Parameters
     ----------
     registration: Registration
         The registration, that contains the StreamPipesFunctions.
     client: StreamPipesClient
         The client to interact with the API.
+
+    Attributes
+    ----------
+    stream_contexts: Dict[str, DataStreamContext]
+        Map of all data stream contexts
+    brokers: List[Broker]
+        List of all registered brokers
     """
 
     def __init__(self, registration: Registration, client: StreamPipesClient) -> None:
         self.registration = registration
         self.client = client
         self.stream_contexts: Dict[str, DataStreamContext] = {}
         self.brokers: List[Broker] = []
 
     def initializeFunctions(self) -> None:
-        """Creates the context for every data stream and starts the event loop to manage the StreamPipesFunctions.
+        """Creates the context for every data stream and starts the event loop to manage the StreamPipes Functions.
 
         Returns
         -------
         None
         """
         for streampipes_function in self.registration.getFunctions():
             # Create the output data streams for every function
@@ -145,30 +153,30 @@
     def force_stop_functions(self) -> None:
         """Stops the StreamPipesFunctions when the event loop was stopped without stopping the functions.
 
         Returns
         -------
         None
 
-        Raises
+        Warns
         ------
         UserWarning
             If there is a running event loop and the functions should be stopped by disconnecting from the broker.
         """
         try:
             asyncio.get_running_loop()
         except RuntimeError:
             self._stop_functions()
         else:
             raise UserWarning(
                 "Don't stop the functions when the event loop is running. Use FunctionHandler().disconnect() instead"
             )
 
     def disconnect(self) -> None:
-        """Disconnects from the brokers and stops the functions.
+        """Disconnects from the brokers and stops all functions.
 
         Returns
         -------
         None
         """
         asyncio.get_event_loop().create_task(self._disconnect())
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/registration.py` & `streampipes-0.91.0/streampipes/functions/registration.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,35 +16,46 @@
 #
 from typing import List
 
 from streampipes.functions.streampipes_function import StreamPipesFunction
 
 
 class Registration:
-    """Manages the existing StreamPipesFunctions and registers them."""
+    """Manages the existing StreamPipesFunctions and registers them.
+
+    Attributes
+    ----------
+    functions: List[StreamPipesFunction]
+        List of all registered StreamPipesFunction
+
+    """
 
     def __init__(self) -> None:
         self.functions: List[StreamPipesFunction] = []
 
     def register(self, streampipes_function: StreamPipesFunction):
         """Registers a new function.
 
         Parameters
         ----------
         streampipes_function: StreamPipesFunction
             The function to register.
 
         Returns
         -------
-        Registration
+        self: Registration
+            The updated Registration instance
         """
         self.functions.append(streampipes_function)  # TODO register function to AdminAPI + consul
         return self
 
     def getFunctions(self) -> List[StreamPipesFunction]:
         """Get all registered functions.
 
+        This method exists to be consistent with the Java client.
+
         Returns
         -------
-        List of the functions.
+        functions: List[StreamPipesFunction]
+            List of all registered functions.
         """
         return self.functions
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/streampipes_function.py` & `streampipes-0.91.0/streampipes/functions/streampipes_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,27 +17,33 @@
 from abc import ABC, abstractmethod
 from time import time
 from typing import Any, Dict, List, Optional
 
 from streampipes.functions.broker.output_collector import OutputCollector
 from streampipes.functions.utils.function_context import FunctionContext
 from streampipes.model.resource import FunctionDefinition
+from streampipes.model.resource.function_definition import FunctionId
 
 
 class StreamPipesFunction(ABC):
     """Abstract implementation of a StreamPipesFunction.
 
     A StreamPipesFunction allows users to get the data of a StreamPipes data streams easily.
     It makes it possible to work with the live data in python and enables to use the powerful
     data analytics libraries there.
 
     Parameters
     ----------
     function_definition: FunctionDefinition
         the definition of the function that contains metadata about the connected function
+
+    Attributes
+    ----------
+    output_collectors: Dict[str, OutputCollector]
+        List of all output collectors which are created based on the provided function definitions.
     """
 
     def __init__(self, function_definition: Optional[FunctionDefinition] = None):
         self.function_definition = function_definition or FunctionDefinition()
         self.output_collectors = {
             stream_id: OutputCollector(data_stream)
             for stream_id, data_stream in self.function_definition.output_data_streams.items()
@@ -47,25 +53,29 @@
         """Send an event via an output data stream to StreamPipes
 
         Parameters
         ----------
         stream_id: str
             The id of the output data stream
         event: Dict[str, Any]
-            The event which should be sended
+            The event which should be sent
+
+        Returns
+        -------
+        None
         """
         event["timestamp"] = int(1000 * time())
         self.output_collectors[stream_id].collect(event)
 
-    def getFunctionId(self) -> FunctionDefinition.FunctionId:
+    def getFunctionId(self) -> FunctionId:
         """Returns the id of the function.
 
         Returns
         -------
-        FunctionId: FunctionDefinition.FunctionId
+        function_id: FunctionId
             Identification object of the StreamPipes function
         """
         return self.function_definition.function_id
 
     def stop(self) -> None:
         """Stops the function and disconnects from the output streams"""
 
@@ -75,15 +85,16 @@
 
     @abstractmethod
     def requiredStreamIds(self) -> List[str]:
         """Get the ids of the streams needed by the function.
 
         Returns
         -------
-        List of the stream ids
+        stream_ids: List[str]
+            List of the stream ids
         """
         raise NotImplementedError  # pragma: no cover
 
     @abstractmethod
     def onServiceStarted(self, context: FunctionContext) -> None:
         """Is called when the function gets started.
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/utils/__init__.py` & `streampipes-0.91.0/streampipes/functions/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/utils/async_iter_handler.py` & `streampipes-0.91.0/streampipes/functions/utils/async_iter_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,51 +15,50 @@
 # limitations under the License.
 #
 import asyncio
 from typing import Any, AsyncGenerator, AsyncIterator, Dict, Tuple
 
 
 class AsyncIterHandler:
-    """Handels asyncrone iterators to get every message after an other in parallel."""
+    """Handles asynchronous iterators to get every message after another in parallel."""
 
     @staticmethod
     async def anext(stream_id: str, message: AsyncIterator) -> Tuple[str, Any]:
-        """Gets the next message from an AsncIterator.
+        """Gets the next message from an AsyncIterator.
 
         Parameters
         ----------
-
         stream_id: str
             The id of the data stream which the message belongs to.
-
         message: AsyncIterator
-            An asyncrone iterator that contains the messages.
+            An asynchronous iterator that contains the messages.
 
         Returns
         -------
-        Tuple of the stream id und next message or ("stop", None) if no message is left.
+        result: Tuple[str, Optional[Any]]
+            Tuple of the stream id und next message or `("stop", None)` if no message is left.
         """
         try:
             return stream_id, await message.__anext__()
         except StopAsyncIteration:
             return "stop", None
 
     @staticmethod
     async def combine_async_messages(messages: Dict[str, AsyncIterator]) -> AsyncGenerator:
-        """Continuously gets the next published message from multiple AsncIterators in parallel.
+        """Continuously gets the next published message from multiple AsyncIterators in parallel.
 
         Parameters
         ----------
-
         messages: Dict[str, AsyncIterator]
-            A dictonary with an asyncrone iterator for every stream id.
+            A dictionary with an asynchronous iterator for every stream id.
 
-        Returns
-        -------
-        Generator that returns all recieved messages continuously.
+        Yields
+        ------
+        message: Tuple[str, Any]
+            Description of the anonymous integer return value.
         """
         pending = {AsyncIterHandler.anext(stream_id, message) for stream_id, message in messages.items()}
         while pending:
             done, pending = await asyncio.wait(pending, return_when=asyncio.FIRST_COMPLETED)  # type: ignore
             for i in done:
                 stream_id, msg = i.result()
                 if stream_id != "stop":
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/utils/data_stream_context.py` & `streampipes-0.91.0/streampipes/functions/utils/data_stream_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 
 class DataStreamContext:
     """Container for the context of a data stream.
 
     Parameters
     ----------
     functions: List[StreamPipesFunction]
-        StreamPipesFunctions which require the data of this data stream.
+        StreamPipes Functions which require the data of this data stream.
     schema: DataStream
         The schema of this data stream.
     broker: Broker
         The broker to connect to this data stream.
     """
 
     def __init__(self, functions: List[StreamPipesFunction], schema: DataStream, broker: Broker) -> None:
         self.functions = functions
         self.schema = schema
         self.broker = broker
 
     def add_function(self, function: StreamPipesFunction):
-        """Adds a new StreamPipesFunction.
+        """Adds a new StreamPipes Function.
 
         Parameters
         ----------
         function: StreamPipesFunction
             StreamPipesFunction which requires this data stream.
 
         Returns
```

### Comparing `streampipes-0.0.2.dev0/streampipes/functions/utils/function_context.py` & `streampipes-0.91.0/streampipes/functions/utils/function_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,37 +24,36 @@
     """Container for the context of a StreamPipesFunction.
 
     Parameters
     ----------
     function_id: str
         The id of this function.
     schema: Dict[str, DataStream]
-        A dictonary which contains the schema of a data stream for each stream id.
+        A dictionary which contains the schema of a data stream for each stream id.
     client: StreamPipesClient
         The client to interact with the API.
     streams: List[str]
         The ids of the streams needed by this function.
     """
 
-    def __init__(
-        self, function_id: str, schema: Dict[str, DataStream], client: StreamPipesClient, streams: List[str]
-    ) -> None:
+    def __init__(self, function_id: str, schema: Dict[str, DataStream], client: StreamPipesClient, streams: List[str]):
         self.function_id = function_id
         self.schema = schema
         self.client = client
         self.streams = streams
 
-    def add_data_stream_schema(self, stream_id: str, data_stream: DataStream):
+    def add_data_stream_schema(self, stream_id: str, data_stream: DataStream) -> None:
         """Adds a new data stream for a new stream id.
 
         Parameters
         ----------
         stream_id: str
             The id of the data stream.
         data_stream: DataStream
             The schema of the data stream.
 
         Returns
         -------
         None
+
         """
         self.schema[stream_id] = data_stream
```

### Comparing `streampipes-0.0.2.dev0/streampipes/model/__init__.py` & `streampipes-0.91.0/streampipes/model/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/model/container/__init__.py` & `streampipes-0.91.0/streampipes/model/container/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/model/container/data_lake_measures.py` & `streampipes-0.91.0/streampipes/model/container/data_lake_measures.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,24 @@
 __all__ = [
     "DataLakeMeasures",
 ]
 
 
 class DataLakeMeasures(ResourceContainer):
     """Implementation of the resource container for the data lake measures endpoint.
+
     This resource container is a collection of data lake measures returned by the StreamPipes API.
     It is capable of parsing the response content directly into a list of queried `DataLakeMeasure`.
     Furthermore, the resource container makes them accessible in a pythonic manner.
 
-    Parameters
-    ----------
-    resources: List[DataLakeMeasure]
-        A list of resources (`model.resource.DataLakeMeasure`) to be contained in the `ResourceContainer`.
-
     """
 
     @classmethod
     def _resource_cls(cls) -> Type[Resource]:
         """Returns the class of the resource that are bundled.
 
         Returns
         -------
-        DataLakeMeasure
+        type: DataLakeMeasure
+            class that describes an individual resource
         """
         return DataLakeMeasure
```

### Comparing `streampipes-0.0.2.dev0/streampipes/model/container/data_streams.py` & `streampipes-0.91.0/streampipes/model/container/data_streams.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,27 +27,24 @@
 __all__ = [
     "DataStreams",
 ]
 
 
 class DataStreams(ResourceContainer):
     """Implementation of the resource container for the data stream endpoint.
+
     This resource container is a collection of data streams returned by the StreamPipes API.
     It is capable of parsing the response content directly into a list of queried `DataStream`.
     Furthermore, the resource container makes them accessible in a pythonic manner.
 
-    Parameters
-    ----------
-    resources: List[DataStream]
-        A list of resources (`model.resource.DataStream`) to be contained in the `ResourceContainer`.
-
     """
 
     @classmethod
     def _resource_cls(cls) -> Type[Resource]:
         """Returns the class of the resource that are bundled.
 
         Returns
         -------
-        DataStream
+        type: DataStream
+            class that defines the contained resource
         """
         return DataStream
```

### Comparing `streampipes-0.0.2.dev0/streampipes/model/container/resource_container.py` & `streampipes-0.91.0/streampipes/model/container/resource_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """
 General and abstract implementation for a resource container.
+
 A resource container is a collection of resources returned by the StreamPipes API.
 It is capable of parsing the response content directly into a list of queried resources.
 Furthermore, the resource container makes them accessible in a pythonic manner.
 """
 
 from __future__ import annotations
 
@@ -63,15 +64,15 @@
         -------
         The error description (`str`)
         """
         return (
             f"\nOops, there seems to be a problem with our internal StreamPipes data model.\n"
             f"This should not occur, but unfortunately did.\n"
             f"Therefore, it would be great if you could report this problem as an issue at "
-            f"github.com/apache/streampipes.\n"
+            f"https://github.com/apache/streampipes.\n"
             f"Please don't forget to include the following information:\n\n"
             f"Affected Model class: {str(self.validation_error.model)}\n"
             f"Validation error log: {self.validation_error.json()}"
         )
 
 
 class StreamPipesResourceContainerJSONError(Exception):
@@ -103,31 +104,32 @@
         -------
         The error description (`str`)
         """
         return (
             f"\nOops, there seems to be a problem when parsing the response of the StreamPipes API."
             f"This should not occur, but unfortunately did.\n"
             f"Therefore, it would be great if you could report this problem as an issue at "
-            f"github.com/apache/streampipes.\n"
+            f"https://github.com/apache/streampipes.\n"
             f"Please don't forget to include the following information:\n\n"
             f"Affected container class: {str(self.container_name)}\n"
             f"JSON string: {self.json_string}"
         )
 
 
 class ResourceContainer(ABC):
     """General and abstract implementation for a resource container.
+
     A resource container is a collection of resources returned by the StreamPipes API.
     It is capable of parsing the response content directly into a list of queried resources.
     Furthermore, the resource container makes them accessible in a pythonic manner.
 
     Parameters
     ----------
     resources: List[Resource]
-        A list of resources (`model.resource.Resource`) to be contained in the `ResourceContainer`.
+        A list of resources to be contained in the `ResourceContainer`.
 
     """
 
     def __init__(self, resources: List[Resource]):
         self._resources = resources
 
     def __getitem__(self, position: int) -> Resource:
@@ -143,30 +145,32 @@
     @classmethod
     @abstractmethod
     def _resource_cls(cls) -> Type[Resource]:
         """Returns the class of the resource that are bundled.
 
         Returns
         -------
-        model.resource.Resource
+        cls: Resource
+            class that defines the resource type contained by the container
         """
         raise NotImplementedError  # pragma: no cover
 
     @classmethod
     def from_json(cls, json_string: str) -> ResourceContainer:
         """Creates a `ResourceContainer` from the given JSON string.
 
         Parameters
         ----------
         json_string: str
             The JSON string returned from the StreamPipes API.
 
         Returns
         -------
-        ResourceContainer
+        container: ResourceContainer
+            instance of the container derived from the JSON definition
 
         Raises
         ------
         StreamPipesDataModelError
             If a resource cannot be mapped to the corresponding Python data model.
         StreamPipesResourceContainerJSONError
             If JSON response cannot be parsed to a `ResourceContainer`.
@@ -205,26 +209,27 @@
         return [resource.to_dict(use_source_names=use_source_names) for resource in self._resources]
 
     def to_json(self) -> str:
         """Returns the resource container in the StreamPipes JSON representation.
 
         Returns
         -------
-        JSON string: str
+         json_string: str
             JSON representation of the resource container where key names are equal to
             keys used in the StreamPipes backend
         """
 
         return json.dumps(self.to_dicts(use_source_names=True))
 
     def to_pandas(self) -> pd.DataFrame:
         """Returns the resource container in representation of a Pandas Dataframe.
 
         Returns
         -------
         resource_container_df: pd.DataFrame
+            Representation of the resource container as pandas DataFrame
         """
         return pd.DataFrame.from_records(
             # ResourceContainer is iterable itself via __get_item__
             # (ignore mypy's expectation of __iter__ here)
             data=[resource_item.convert_to_pandas_representation() for resource_item in self]  # type: ignore
         )
```

### Comparing `streampipes-0.0.2.dev0/streampipes/model/resource/__init__.py` & `streampipes-0.91.0/streampipes/model/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/streampipes/model/resource/data_lake_measure.py` & `streampipes-0.91.0/streampipes/model/resource/data_lake_measure.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,33 +23,43 @@
 __all__ = [
     "DataLakeMeasure",
 ]
 
 
 class DataLakeMeasure(Resource):
     """Implementation of a resource for data lake measures.
+
     This resource defines the data model used by resource container (`model.container.DataLakeMeasures`).
     It inherits from Pydantic's BaseModel to get all its superpowers,
-    which are used to parse, validate the API response and to easily switch between
+    which are used to parse, validate the API response, and to easily switch between
     the Python representation (both serialized and deserialized) and Java representation (serialized only).
     """
 
     def convert_to_pandas_representation(self):
         """Returns the dictionary representation of a data lake measure
         to be used when creating a pandas Dataframe.
+
         It excludes the following fields: `element_id`, `event_schema`, `schema_version`.
         Instead of the whole event schema the number of event properties contained
         is returned with the column name `num_event_properties`.
+
+        Returns
+        -------
+        pandas_repr: Dict[str, Any]
+            Pandas representation of the resource as a dictionary, which is then used by the respource container
+            to create a data frame from a collection of resources.
+
         """
+
         return {
             **self.dict(exclude={"element_id", "event_schema", "schema_version"}),
             "num_event_properties": len(self.event_schema.event_properties),
         }
 
     element_id: Optional[StrictStr]
     measure_name: StrictStr
     timestamp_field: StrictStr
     event_schema: Optional[EventSchema]
     pipeline_id: Optional[StrictStr]
     pipeline_name: Optional[StrictStr]
     pipeline_is_running: StrictBool
-    schema_version: StrictStr
+    schema_version: Optional[StrictStr]
```

### Comparing `streampipes-0.0.2.dev0/streampipes/model/resource/function_definition.py` & `streampipes-0.91.0/streampipes/model/resource/function_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,79 +24,106 @@
 
 from pydantic import Field, StrictInt, StrictStr
 from streampipes.model.common import BasicModel
 from streampipes.model.resource.data_stream import DataStream
 from streampipes.model.resource.resource import Resource
 
 
+class FunctionId(BasicModel):
+    """Identification object for a StreamPipes function.
+
+    Maps to the `FunctionId` class defined in the StreamPipes model.
+
+    Parameters
+    ----------
+    id: str
+        unique identifier of the function instance
+    version: int
+        version of the corresponding function
+
+    """
+
+    id: StrictStr = Field(default_factory=lambda: str(uuid4()))
+    version: StrictInt = Field(default=1)
+
+    def __hash__(self):
+        return hash((self.id, self.version))
+
+
 class FunctionDefinition(Resource):
     """Configuration for a StreamPipes Function.
 
     This class maps to the `FunctionDefinition` class in the StreamPipes model.
     It contains all metadata that are required to register a function at the StreamPipes backend.
 
     Parameters
     ----------
+    consumed_streams: List[str]
+        List of data streams the function is consuming from
     function_id: FunctionId
         identifier object of a StreamPipes function
-    consumed_streams: List[str]
-        list of data streams the function is consuming from
+
+    Attributes
+    ----------
+    output_data_streams: Dict[str, DataStream]
+        Map off all output data streams added to the function definition
+
     """
 
+    function_id: FunctionId = Field(default_factory=FunctionId)
+    consumed_streams: List[str] = Field(default_factory=list)
+    output_data_streams: Dict[str, DataStream] = Field(default_factory=dict)
+
     def convert_to_pandas_representation(self) -> Dict:
         """Returns the dictionary representation of a function definition
         to be used when creating a pandas Dataframe.
+
+        Returns
+        -------
+        pandas_repr: Dict[str, Any]
+            Pandas representation of the resource as a dictionary, which is then used by the respource container
+            to create a data frame from a collection of resources.
         """
 
         return self.to_dict(use_source_names=False)
 
     def add_output_data_stream(self, data_stream: DataStream):
         """Adds an output data stream to the function which makes it possible to write data back to StreamPipes.
 
         Parameters
         ----------
         data_stream: DataStream
             The schema of the output data stream.
+
+        Returns
+        -------
+        self: FunctionDefinition
+            Instance of the function definition that is extended by the provided `DataStream`
+
         """
+
         self.output_data_streams[data_stream.element_id] = data_stream
         return self
 
     def get_output_data_streams(self) -> Dict[str, DataStream]:
         """Get the output data streams of the function.
 
         Returns
         -------
-        Dictonary with every stream id and the related output stream.
+        output_streams: Dict[str, DataStream]
+            Dictionary with every known stream id and the related output stream.
+
         """
+
         return self.output_data_streams
 
     def get_output_stream_ids(self) -> List[str]:
         """Get the stream ids of the output data streams.
 
         Returns
         -------
-        List of all stream ids.
-        """
-        return list(self.output_data_streams.keys())
+        output_stream_ids: List[str]
+            List of all stream ids
 
-    class FunctionId(BasicModel):
-        """Identification object for a StreamPipes function.
-
-        Maps to the `FunctionId` class defined in the StreamPipes model.
-
-        Parameters
-        ----------
-        id: str
-            unique identifier of the function instance
-        version: int
-            version of the corresponding function
         """
 
-        id: StrictStr = Field(default_factory=lambda: str(uuid4()))
-        version: StrictInt = Field(default=1)
-
-        def __hash__(self):
-            return hash((self.id, self.version))
-
-    function_id: FunctionId = Field(default_factory=FunctionId)
-    consumed_streams: List[str] = Field(default_factory=list)
-    output_data_streams: Dict[str, DataStream] = Field(default_factory=dict)
+        return list(self.output_data_streams.keys())
```

### Comparing `streampipes-0.0.2.dev0/streampipes/model/resource/resource.py` & `streampipes-0.91.0/streampipes/model/resource/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """
 General and abstract implementation for a resource.
+
 A resource defines the data model that is used by a resource container (`model.container.resourceContainer`).
 """
 from abc import ABC, abstractmethod
 from typing import Dict
 
 from streampipes.model.common import BasicModel
 
@@ -32,19 +33,27 @@
 class Resource(ABC, BasicModel):
     """General and abstract implementation for a resource.
 
     A resource defines the data model used by a resource container (`model.container.resourceContainer`).
     It inherits from Pydantic's BaseModel to get all its superpowers,
     which are used to parse, validate the API response and to easily switch between
     the Python representation (both serialized and deserialized) and Java representation (serialized only).
+
     """
 
     @abstractmethod
     def convert_to_pandas_representation(self) -> Dict:
-        """Returns a dictionary representation to be used when creating a pandas Dataframe."""
+        """Returns a dictionary representation to be used when creating a pandas Dataframe.
+
+        Returns
+        -------
+        pandas_repr: Dict[str, Any]
+            Pandas representation of the resource as a dictionary, which is then used by the respource container
+            to create a data frame from a collection of resources.
+        """
         raise NotImplementedError  # pragma: no cover
 
     def to_dict(self, use_source_names=True):
         """Returns the resource in dictionary representation.
 
         Parameters
         ----------
```

### Comparing `streampipes-0.0.2.dev0/streampipes.egg-info/PKG-INFO` & `streampipes-0.91.0/streampipes.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: streampipes
-Version: 0.0.2.dev0
+Version: 0.91.0
 Summary: Python library for Apache StreamPipes
-Home-page: https://github.com/apache/streampipes/
+Home-page: https://streampipes.apache.org/docs/docs/python/latest/
 Author: Apache Software Foundation
 Author-email: dev@streampipes.apache.org
 License: Apache License 2.0
+Project-URL: Documentation, https://streampipes.apache.org/docs/docs/python/latest/
+Project-URL: Bug Tracker, https://github.com/apache/streampipes/issues
+Project-URL: Source Code, https://github.com/apache/streampipes
 Keywords: streampipes,iot,iiot,analytics,stream-processing,apache
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -67,45 +70,60 @@
 <br>
 
 **💡The current version of this Python client is still a beta version.**
 <br>
 **This means that it is still under development, which may result in frequent and extensive API changes, unstable behavior, etc.**
 <br>
 
+
+## 📚 Documentation
+Please visit our documentation: https://streampipes.apache.org/docs/docs/python/latest/
+There you can find information about how to [get started](https://streampipes.apache.org/docs/docs/python/latest/getting-started/first-steps/),
+follow some [tutorials](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/),
+or discover the library via our [references](https://streampipes.apache.org/docs/docs/python/latest/reference/client/client/).
+<br>
+
+In case you want to access the documentation of the current development state, you can go here:
+
+👉 [development docs 🤓](https://streampipes.apache.org/docs/docs/python/dev/)
+
 ## ⚡️ Quickstart
 
 As a quick example, we demonstrate how to set up and configure a StreamPipes client.
 
 You can simply install the StreamPipes library by running the following command
 ```bash
-%pip install streampipes
+pip install streampipes
 
 # if you want to have the current development state you can also execute
-%pip install git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-python
+pip install git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-python
 ```
 
 ```python
->> > from streampipes.client import StreamPipesClient
->> > from streampipes.client.client_config import StreamPipesClientConfig
->> > from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
-
->>> config = StreamPipesClientConfig(
-...     credential_provider = StreamPipesApiKeyCredentials(
-...         username = "test@streampipes.apache.org",
-...         api_key = "DEMO-KEY",
-...         ),
-...     host_address = "localhost",
-...     http_disabled = True,
-...     port = 80
-...)
+from streampipes.client import StreamPipesClient
+from streampipes.client.config import StreamPipesClientConfig
+from streampipes.client.credential_provider import StreamPipesApiKeyCredentials
+
+config = StreamPipesClientConfig(
+    credential_provider = StreamPipesApiKeyCredentials(
+        username = "test@streampipes.apache.org",
+        api_key = "DEMO-KEY",
+    ),
+    host_address = "localhost",
+    https_disabled = True,
+    port = 80
+)
 
->>> client = StreamPipesClient(client_config=config)
->>> client.describe()
+client = StreamPipesClient(client_config=config)
+client.describe()
+```
 
+Output:
+```
 Hi there!
-You are connected to a StreamPipes instance running at http://localhost: 80.
+You are connected to a StreamPipes instance running at http://localhost:80.
 The following StreamPipes resources are available with this client:
 6x DataStreams
 1x DataLakeMeasures
 ```
 
-For more information about how to use the StreamPipes client visit our [introduction example](https://github.com/apache/streampipes/blob/dev/streampipes-client-python/docs/examples/1-introduction-to-streampipes-python-client.ipynb).
+For more information about how to use the StreamPipes client visit our [introduction tutorial](https://streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-Metadata-Version: 2.1 Name: streampipes Version: 0.0.2.dev0 Summary: Python
-library for Apache StreamPipes Home-page: https://github.com/apache/
-streampipes/ Author: Apache Software Foundation Author-email:
-dev@streampipes.apache.org License: Apache License 2.0 Keywords:
+Metadata-Version: 2.1 Name: streampipes Version: 0.91.0 Summary: Python library
+for Apache StreamPipes Home-page: https://streampipes.apache.org/docs/docs/
+python/latest/ Author: Apache Software Foundation Author-email:
+dev@streampipes.apache.org License: Apache License 2.0 Project-URL:
+Documentation, https://streampipes.apache.org/docs/docs/python/latest/ Project-
+URL: Bug Tracker, https://github.com/apache/streampipes/issues Project-URL:
+Source Code, https://github.com/apache/streampipes Keywords:
 streampipes,iot,iiot,analytics,stream-processing,apache Classifier: Development
-Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
+Status :: 4 - Beta Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Manufacturing Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: Scientific/Engineering
@@ -25,25 +28,35 @@
   power of StreamPipes to easily connect to and read different data sources,
    especially in the IoT domain, and the amazing universe of data analytics
                              libraries in Python.
 ---
 **ð¡The current version of this Python client is still a beta version.**
 **This means that it is still under development, which may result in frequent
 and extensive API changes, unstable behavior, etc.**
-## â¡ï¸ Quickstart As a quick example, we demonstrate how to set up and
-configure a StreamPipes client. You can simply install the StreamPipes library
-by running the following command ```bash %pip install streampipes # if you want
-to have the current development state you can also execute %pip install
-git+https://github.com/apache/streampipes.git#subdirectory=streampipes-client-
-python ``` ```python >> > from streampipes.client import StreamPipesClient >> >
-from streampipes.client.client_config import StreamPipesClientConfig >> > from
-streampipes.client.credential_provider import StreamPipesApiKeyCredentials >>>
-config = StreamPipesClientConfig( ... credential_provider =
-StreamPipesApiKeyCredentials( ... username = "test@streampipes.apache.org", ...
-api_key = "DEMO-KEY", ... ), ... host_address = "localhost", ... http_disabled
-= True, ... port = 80 ...) >>> client = StreamPipesClient(client_config=config)
->>> client.describe() Hi there! You are connected to a StreamPipes instance
-running at http://localhost: 80. The following StreamPipes resources are
-available with this client: 6x DataStreams 1x DataLakeMeasures ``` For more
-information about how to use the StreamPipes client visit our [introduction
-example](https://github.com/apache/streampipes/blob/dev/streampipes-client-
-python/docs/examples/1-introduction-to-streampipes-python-client.ipynb).
+## ð Documentation Please visit our documentation: https://
+streampipes.apache.org/docs/docs/python/latest/ There you can find information
+about how to [get started](https://streampipes.apache.org/docs/docs/python/
+latest/getting-started/first-steps/), follow some [tutorials](https://
+streampipes.apache.org/docs/docs/python/latest/tutorials/1-introduction-to-
+streampipes-python-client/), or discover the library via our [references]
+(https://streampipes.apache.org/docs/docs/python/latest/reference/client/
+client/).
+In case you want to access the documentation of the current development state,
+you can go here: ð [development docs ð¤](https://streampipes.apache.org/
+docs/docs/python/dev/) ## â¡ï¸ Quickstart As a quick example, we demonstrate
+how to set up and configure a StreamPipes client. You can simply install the
+StreamPipes library by running the following command ```bash pip install
+streampipes # if you want to have the current development state you can also
+execute pip install git+https://github.com/apache/
+streampipes.git#subdirectory=streampipes-client-python ``` ```python from
+streampipes.client import StreamPipesClient from streampipes.client.config
+import StreamPipesClientConfig from streampipes.client.credential_provider
+import StreamPipesApiKeyCredentials config = StreamPipesClientConfig
+( credential_provider = StreamPipesApiKeyCredentials( username =
+"test@streampipes.apache.org", api_key = "DEMO-KEY", ), host_address =
+"localhost", https_disabled = True, port = 80 ) client = StreamPipesClient
+(client_config=config) client.describe() ``` Output: ``` Hi there! You are
+connected to a StreamPipes instance running at http://localhost:80. The
+following StreamPipes resources are available with this client: 6x DataStreams
+1x DataLakeMeasures ``` For more information about how to use the StreamPipes
+client visit our [introduction tutorial](https://streampipes.apache.org/docs/
+docs/python/latest/tutorials/1-introduction-to-streampipes-python-client/).
```

### Comparing `streampipes-0.0.2.dev0/streampipes.egg-info/SOURCES.txt` & `streampipes-0.91.0/streampipes.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 streampipes/functions/__init__.py
 streampipes/functions/function_handler.py
 streampipes/functions/registration.py
 streampipes/functions/streampipes_function.py
 streampipes/functions/broker/__init__.py
 streampipes/functions/broker/broker.py
 streampipes/functions/broker/broker_handler.py
+streampipes/functions/broker/kafka_broker.py
+streampipes/functions/broker/kafka_message_fetcher.py
 streampipes/functions/broker/nats_broker.py
 streampipes/functions/broker/output_collector.py
 streampipes/functions/utils/__init__.py
 streampipes/functions/utils/async_iter_handler.py
 streampipes/functions/utils/data_stream_context.py
 streampipes/functions/utils/data_stream_generator.py
 streampipes/functions/utils/function_context.py
@@ -47,10 +49,15 @@
 streampipes/model/resource/function_definition.py
 streampipes/model/resource/resource.py
 tests/client/__init__.py
 tests/client/test_client.py
 tests/client/test_credential_provider.py
 tests/client/test_data_lake_series.py
 tests/client/test_endpoint.py
+tests/endpoint/__init__.py
+tests/endpoint/test_data_lake_measure.py
 tests/functions/__init__.py
 tests/functions/test_function_handler.py
-tests/functions/test_river_function.py
+tests/functions/test_river_function.py
+tests/model/__init__.py
+tests/model/resource/__init__.py
+tests/model/resource/test_data_stream.py
```

### Comparing `streampipes-0.0.2.dev0/streampipes.egg-info/requires.txt` & `streampipes-0.91.0/streampipes.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 pandas>=1.5.1
 pydantic>=1.10.2
 requests>=2.28.1
 nats-py>=2.2.0
+confluent-kafka>=2.0.2
 
 [all]
 pandas>=1.5.1
 pydantic>=1.10.2
 requests>=2.28.1
 nats-py>=2.2.0
+confluent-kafka>=2.0.2
 autoflake==2.0.0
 black==23.1.0
 blacken-docs==1.13.0
 flake8==6.0.0
 interrogate==1.5.0
 isort==5.12.0
 mypy==1.0.0
@@ -33,14 +35,15 @@
 mkdocs-jupyter==0.22.0
 
 [dev]
 pandas>=1.5.1
 pydantic>=1.10.2
 requests>=2.28.1
 nats-py>=2.2.0
+confluent-kafka>=2.0.2
 autoflake==2.0.0
 black==23.1.0
 blacken-docs==1.13.0
 flake8==6.0.0
 interrogate==1.5.0
 isort==5.12.0
 mypy==1.0.0
@@ -64,14 +67,15 @@
 mkdocs-jupyter==0.22.0
 
 [test]
 pandas>=1.5.1
 pydantic>=1.10.2
 requests>=2.28.1
 nats-py>=2.2.0
+confluent-kafka>=2.0.2
 autoflake==2.0.0
 black==23.1.0
 blacken-docs==1.13.0
 flake8==6.0.0
 interrogate==1.5.0
 isort==5.12.0
 mypy==1.0.0
```

### Comparing `streampipes-0.0.2.dev0/tests/client/__init__.py` & `streampipes-0.91.0/tests/client/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/tests/client/test_client.py` & `streampipes-0.91.0/tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/tests/client/test_credential_provider.py` & `streampipes-0.91.0/tests/client/test_credential_provider.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/tests/client/test_data_lake_series.py` & `streampipes-0.91.0/tests/client/test_data_lake_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                 credential_provider=StreamPipesApiKeyCredentials(username="user", api_key="key"),
                 host_address="localhost",
             )
         )
         result = client.dataLakeMeasureApi.get(identifier="test")
 
         http_session.assert_has_calls(
-            [call().get(url="https://localhost:80/streampipes-backend/api/v4/datalake/measurements/test")],
+            [call().get(url="https://localhost:80/streampipes-backend/api/v4/datalake/measurements/test?limit=1000")],
             any_order=True,
         )
 
         result_pd = result.to_pandas()
 
         self.assertEqual(2, len(result_pd))
         self.assertListEqual(
```

### Comparing `streampipes-0.0.2.dev0/tests/client/test_endpoint.py` & `streampipes-0.91.0/tests/client/test_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
                     url="https://localhost:80/streampipes-backend/api/v2/streams/urn:streampipes."
                     "apache.org:eventstream:uPDKLI"
                 )
             ],
             any_order=True,
         )
         self.assertTrue(isinstance(result, DataStream))
-        self.assertEqual(result.dict(by_alias=True), self.data_stream_get)
+        self.assertEqual(result.to_dict(use_source_names=True), self.data_stream_get)
 
     @patch("streampipes.client.client.Session", autospec=True)
     def test_endpoint_post(self, http_session: MagicMock):
         http_session_mock = MagicMock()
         http_session.return_value = http_session_mock
 
         client = StreamPipesClient(
```

### Comparing `streampipes-0.0.2.dev0/tests/functions/__init__.py` & `streampipes-0.91.0/tests/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/tests/functions/test_function_handler.py` & `streampipes-0.91.0/tests/functions/test_function_handler.py`

 * *Files identical despite different names*

### Comparing `streampipes-0.0.2.dev0/tests/functions/test_river_function.py` & `streampipes-0.91.0/tests/functions/test_river_function.py`

 * *Files identical despite different names*

