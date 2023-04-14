# Comparing `tmp/fastkafka-0.5.0.tar.gz` & `tmp/fastkafka-0.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.5.0.tar", last modified: Fri Apr 14 15:27:36 2023, max compression
+gzip compressed data, was "fastkafka-0.5.0rc0.tar", last modified: Fri Apr 14 15:25:23 2023, max compression
```

## Comparing `fastkafka-0.5.0.tar` & `fastkafka-0.5.0rc0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:36.492123 fastkafka-0.5.0/
--rw-r--r--   0 davor     (1000) davor     (1000)    11357 2023-01-25 09:24:15.000000 fastkafka-0.5.0/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-01-25 09:24:15.000000 fastkafka-0.5.0/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    32076 2023-04-14 15:27:36.492123 fastkafka-0.5.0/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)    30651 2023-04-14 15:23:47.000000 fastkafka-0.5.0/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:36.488123 fastkafka-0.5.0/fastkafka/
--rw-rw-r--   0 davor     (1000) davor     (1000)      429 2023-04-14 15:27:30.000000 fastkafka-0.5.0/fastkafka/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:36.488123 fastkafka-0.5.0/fastkafka/_application/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:30.000000 fastkafka-0.5.0/fastkafka/_application/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    29758 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_application/app.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     7432 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_application/tester.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     1574 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_cli.py
--rw-r--r--   0 davor     (1000) davor     (1000)     3879 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_cli_docs.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      852 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_cli_testing.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:36.488123 fastkafka-0.5.0/fastkafka/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:30.000000 fastkafka-0.5.0/fastkafka/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     3705 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_components/_subprocess.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     9356 2023-04-14 15:27:28.000000 fastkafka-0.5.0/fastkafka/_components/aiokafka_consumer_loop.py
--rw-r--r--   0 davor     (1000) davor     (1000)    16362 2023-04-14 15:27:28.000000 fastkafka-0.5.0/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     2940 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_components/benchmarking.py
--rw-r--r--   0 davor     (1000) davor     (1000)     4686 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:36.492123 fastkafka-0.5.0/fastkafka/_components/encoder/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:30.000000 fastkafka-0.5.0/fastkafka/_components/encoder/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    13092 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_components/encoder/avro.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     1026 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_components/encoder/json.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     2952 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     4445 2023-04-14 15:27:30.000000 fastkafka-0.5.0/fastkafka/_components/logger.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    12567 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_components/meta.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     3556 2023-04-14 15:27:28.000000 fastkafka-0.5.0/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     5066 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_components/test_dependencies.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    14740 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_docusaurus_helper.py
--rw-r--r--   0 davor     (1000) davor     (1000)    50547 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    68208 2023-04-14 15:27:30.000000 fastkafka-0.5.0/fastkafka/_modidx.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     6039 2023-04-14 15:27:29.000000 fastkafka-0.5.0/fastkafka/_server.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:36.492123 fastkafka-0.5.0/fastkafka/_testing/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:30.000000 fastkafka-0.5.0/fastkafka/_testing/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)    19775 2023-04-14 15:27:28.000000 fastkafka-0.5.0/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    17978 2023-04-14 15:27:28.000000 fastkafka-0.5.0/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    12382 2023-04-14 15:27:28.000000 fastkafka-0.5.0/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     4671 2023-04-14 15:27:28.000000 fastkafka-0.5.0/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      833 2023-04-14 15:27:27.000000 fastkafka-0.5.0/fastkafka/testing.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:27:36.488123 fastkafka-0.5.0/fastkafka.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    32076 2023-04-14 15:27:36.000000 fastkafka-0.5.0/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     1310 2023-04-14 15:27:36.000000 fastkafka-0.5.0/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-04-14 15:27:36.000000 fastkafka-0.5.0/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      146 2023-04-14 15:27:36.000000 fastkafka-0.5.0/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-01-25 09:30:21.000000 fastkafka-0.5.0/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      598 2023-04-14 15:27:36.000000 fastkafka-0.5.0/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       10 2023-04-14 15:27:36.000000 fastkafka-0.5.0/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)     1227 2023-04-14 15:27:17.000000 fastkafka-0.5.0/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-04-14 15:27:36.492123 fastkafka-0.5.0/setup.cfg
--rw-rw-r--   0 davor     (1000) davor     (1000)     3663 2023-04-14 15:19:15.000000 fastkafka-0.5.0/setup.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/
+-rw-r--r--   0 davor     (1000) davor     (1000)    11357 2023-01-25 09:24:15.000000 fastkafka-0.5.0rc0/LICENSE
+-rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-01-25 09:24:15.000000 fastkafka-0.5.0rc0/MANIFEST.in
+-rw-rw-r--   0 davor     (1000) davor     (1000)    32079 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)    30651 2023-04-14 15:23:47.000000 fastkafka-0.5.0rc0/README.md
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.768181 fastkafka-0.5.0rc0/fastkafka/
+-rw-rw-r--   0 davor     (1000) davor     (1000)      432 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/__init__.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/fastkafka/_application/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_application/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    29758 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_application/app.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     7432 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_application/tester.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     1574 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_cli.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     3879 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_cli_docs.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      852 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_cli_testing.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/fastkafka/_components/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_components/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3705 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/_subprocess.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     9356 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    16362 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     2940 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/benchmarking.py
+-rw-r--r--   0 davor     (1000) davor     (1000)     4686 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/fastkafka/_components/encoder/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_components/encoder/__init__.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    13092 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/encoder/avro.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     1026 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/encoder/json.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     2952 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     4445 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_components/logger.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12567 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/meta.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3556 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_components/producer_decorator.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     5066 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_components/test_dependencies.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    14740 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_docusaurus_helper.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    50547 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_helpers.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    68208 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_modidx.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     6039 2023-04-14 15:21:02.000000 fastkafka-0.5.0rc0/fastkafka/_server.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/fastkafka/_testing/
+-rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-14 15:21:03.000000 fastkafka-0.5.0rc0/fastkafka/_testing/__init__.py
+-rw-r--r--   0 davor     (1000) davor     (1000)    19775 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    17978 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_testing/in_memory_broker.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)    12382 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)     4671 2023-04-14 15:21:01.000000 fastkafka-0.5.0rc0/fastkafka/_testing/test_utils.py
+-rw-rw-r--   0 davor     (1000) davor     (1000)      833 2023-04-14 15:21:00.000000 fastkafka-0.5.0rc0/fastkafka/testing.py
+drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-14 15:25:23.768181 fastkafka-0.5.0rc0/fastkafka.egg-info/
+-rw-rw-r--   0 davor     (1000) davor     (1000)    32079 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 davor     (1000) davor     (1000)     1310 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)      146 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-01-25 09:30:21.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 davor     (1000) davor     (1000)      598 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)       10 2023-04-14 15:25:23.000000 fastkafka-0.5.0rc0/fastkafka.egg-info/top_level.txt
+-rw-rw-r--   0 davor     (1000) davor     (1000)     1230 2023-04-14 15:19:31.000000 fastkafka-0.5.0rc0/settings.ini
+-rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-04-14 15:25:23.772182 fastkafka-0.5.0rc0/setup.cfg
+-rw-rw-r--   0 davor     (1000) davor     (1000)     3663 2023-04-14 15:19:15.000000 fastkafka-0.5.0rc0/setup.py
```

### Comparing `fastkafka-0.5.0/LICENSE` & `fastkafka-0.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/PKG-INFO` & `fastkafka-0.5.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.5.0
+Version: 0.5.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
```

### Comparing `fastkafka-0.5.0/README.md` & `fastkafka-0.5.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_application/app.py` & `fastkafka-0.5.0rc0/fastkafka/_application/app.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_application/tester.py` & `fastkafka-0.5.0rc0/fastkafka/_application/tester.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_cli.py` & `fastkafka-0.5.0rc0/fastkafka/_cli.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_cli_docs.py` & `fastkafka-0.5.0rc0/fastkafka/_cli_docs.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_cli_testing.py` & `fastkafka-0.5.0rc0/fastkafka/_cli_testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/_subprocess.py` & `fastkafka-0.5.0rc0/fastkafka/_components/_subprocess.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.5.0rc0/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/asyncapi.py` & `fastkafka-0.5.0rc0/fastkafka/_components/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/benchmarking.py` & `fastkafka-0.5.0rc0/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.5.0rc0/fastkafka/_components/docs_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/encoder/avro.py` & `fastkafka-0.5.0rc0/fastkafka/_components/encoder/avro.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/encoder/json.py` & `fastkafka-0.5.0rc0/fastkafka/_components/encoder/json.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/helpers.py` & `fastkafka-0.5.0rc0/fastkafka/_components/helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/logger.py` & `fastkafka-0.5.0rc0/fastkafka/_components/logger.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/meta.py` & `fastkafka-0.5.0rc0/fastkafka/_components/meta.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/producer_decorator.py` & `fastkafka-0.5.0rc0/fastkafka/_components/producer_decorator.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_components/test_dependencies.py` & `fastkafka-0.5.0rc0/fastkafka/_components/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_docusaurus_helper.py` & `fastkafka-0.5.0rc0/fastkafka/_docusaurus_helper.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_helpers.py` & `fastkafka-0.5.0rc0/fastkafka/_helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_modidx.py` & `fastkafka-0.5.0rc0/fastkafka/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_server.py` & `fastkafka-0.5.0rc0/fastkafka/_server.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.5.0rc0/fastkafka/_testing/apache_kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.5.0rc0/fastkafka/_testing/in_memory_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.5.0rc0/fastkafka/_testing/local_redpanda_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/_testing/test_utils.py` & `fastkafka-0.5.0rc0/fastkafka/_testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka/testing.py` & `fastkafka-0.5.0rc0/fastkafka/testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.5.0rc0/fastkafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.5.0
+Version: 0.5.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
```

### Comparing `fastkafka-0.5.0/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.5.0rc0/fastkafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/fastkafka.egg-info/requires.txt` & `fastkafka-0.5.0rc0/fastkafka.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.5.0/settings.ini` & `fastkafka-0.5.0rc0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.5.0
+version = 0.5.0rc0
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.5.0/setup.py` & `fastkafka-0.5.0rc0/setup.py`

 * *Files identical despite different names*

