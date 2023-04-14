# Comparing `tmp/fastkafka-0.4.0rc2.tar.gz` & `tmp/fastkafka-0.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.4.0rc2.tar", last modified: Fri Apr  7 15:11:08 2023, max compression
+gzip compressed data, was "fastkafka-0.5.0rc0.tar", last modified: Fri Apr 14 15:25:23 2023, max compression
```

## Comparing `fastkafka-0.4.0rc2.tar` & `fastkafka-0.5.0rc0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-07 15:11:08.736628 fastkafka-0.4.0rc2/
--rw-r--r--   0 davor     (1000) davor     (1000)    11357 2023-01-25 09:24:15.000000 fastkafka-0.4.0rc2/LICENSE
--rw-r--r--   0 davor     (1000) davor     (1000)      111 2023-01-25 09:24:15.000000 fastkafka-0.4.0rc2/MANIFEST.in
--rw-rw-r--   0 davor     (1000) davor     (1000)    32051 2023-04-07 15:11:08.736628 fastkafka-0.4.0rc2/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)    30644 2023-04-07 15:10:13.000000 fastkafka-0.4.0rc2/README.md
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-07 15:11:08.736628 fastkafka-0.4.0rc2/fastkafka/
--rw-rw-r--   0 davor     (1000) davor     (1000)      432 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/__init__.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-07 15:11:08.736628 fastkafka-0.4.0rc2/fastkafka/_application/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/_application/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    27864 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_application/app.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     7407 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_application/tester.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     1574 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_cli.py
--rw-r--r--   0 davor     (1000) davor     (1000)     3879 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_cli_docs.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      852 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_cli_testing.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-07 15:11:08.736628 fastkafka-0.4.0rc2/fastkafka/_components/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/_components/__init__.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     3705 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_components/_subprocess.py
--rw-r--r--   0 davor     (1000) davor     (1000)     8769 2023-04-07 14:00:33.000000 fastkafka-0.4.0rc2/fastkafka/_components/aiokafka_consumer_loop.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     2848 2023-04-07 14:00:33.000000 fastkafka-0.4.0rc2/fastkafka/_components/aiokafka_producer_manager.py
--rw-r--r--   0 davor     (1000) davor     (1000)    16362 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     2940 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_components/benchmarking.py
--rw-r--r--   0 davor     (1000) davor     (1000)     4686 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_components/docs_dependencies.py
--rw-r--r--   0 davor     (1000) davor     (1000)     2639 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/_components/helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     3952 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/_components/logger.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    12280 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_components/meta.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     3154 2023-04-07 14:00:33.000000 fastkafka-0.4.0rc2/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     5066 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/_components/test_dependencies.py
--rw-r--r--   0 davor     (1000) davor     (1000)    11215 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_docusaurus_helper.py
--rw-r--r--   0 davor     (1000) davor     (1000)    50547 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/_helpers.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    66827 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/_modidx.py
--rw-rw-r--   0 davor     (1000) davor     (1000)     6039 2023-04-07 14:00:34.000000 fastkafka-0.4.0rc2/fastkafka/_server.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-07 15:11:08.736628 fastkafka-0.4.0rc2/fastkafka/_testing/
--rw-rw-r--   0 davor     (1000) davor     (1000)        0 2023-04-07 14:00:35.000000 fastkafka-0.4.0rc2/fastkafka/_testing/__init__.py
--rw-r--r--   0 davor     (1000) davor     (1000)    19775 2023-04-07 14:00:33.000000 fastkafka-0.4.0rc2/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    18396 2023-04-07 14:00:33.000000 fastkafka-0.4.0rc2/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 davor     (1000) davor     (1000)    12382 2023-04-07 14:00:33.000000 fastkafka-0.4.0rc2/fastkafka/_testing/local_redpanda_broker.py
--rw-r--r--   0 davor     (1000) davor     (1000)     5031 2023-04-07 14:00:33.000000 fastkafka-0.4.0rc2/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 davor     (1000) davor     (1000)      849 2023-04-07 14:00:33.000000 fastkafka-0.4.0rc2/fastkafka/testing.py
-drwxrwxr-x   0 davor     (1000) davor     (1000)        0 2023-04-07 15:11:08.736628 fastkafka-0.4.0rc2/fastkafka.egg-info/
--rw-rw-r--   0 davor     (1000) davor     (1000)    32051 2023-04-07 15:11:08.000000 fastkafka-0.4.0rc2/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 davor     (1000) davor     (1000)     1243 2023-04-07 15:11:08.000000 fastkafka-0.4.0rc2/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-04-07 15:11:08.000000 fastkafka-0.4.0rc2/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)      146 2023-04-07 15:11:08.000000 fastkafka-0.4.0rc2/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)        1 2023-01-25 09:30:21.000000 fastkafka-0.4.0rc2/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 davor     (1000) davor     (1000)      578 2023-04-07 15:11:08.000000 fastkafka-0.4.0rc2/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)       10 2023-04-07 15:11:08.000000 fastkafka-0.4.0rc2/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 davor     (1000) davor     (1000)     1230 2023-04-07 15:06:44.000000 fastkafka-0.4.0rc2/settings.ini
--rw-rw-r--   0 davor     (1000) davor     (1000)       38 2023-04-07 15:11:08.736628 fastkafka-0.4.0rc2/setup.cfg
--rw-r--r--   0 davor     (1000) davor     (1000)     3570 2023-04-07 10:22:05.000000 fastkafka-0.4.0rc2/setup.py
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

### Comparing `fastkafka-0.4.0rc2/LICENSE` & `fastkafka-0.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/PKG-INFO` & `fastkafka-0.5.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.4.0rc2
+Version: 0.5.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: avro
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 FastKafka
 ================
@@ -75,15 +76,15 @@
 
 Your support helps us to stay in touch with you and encourages us to
 continue developing and improving the library. Thank you for your
 support!
 
 ------------------------------------------------------------------------
 
-We were busy lately, check it out yourself!
+#### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
 FastKafka works on macOS, Linux, and most Unix-style operating systems.
 You can install base version of `fastkafka` with `pip` as usual:
```

### Comparing `fastkafka-0.4.0rc2/README.md` & `fastkafka-0.5.0rc0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 Your support helps us to stay in touch with you and encourages us to
 continue developing and improving the library. Thank you for your
 support!
 
 ------------------------------------------------------------------------
 
-We were busy lately, check it out yourself!
+#### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
 FastKafka works on macOS, Linux, and most Unix-style operating systems.
 You can install base version of `fastkafka` with `pip` as usual:
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_application/app.py` & `fastkafka-0.5.0rc0/fastkafka/_application/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,25 @@
 from pathlib import Path
 from typing import *
 from unittest.mock import AsyncMock, MagicMock
 
 import anyio
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from pydantic import BaseModel
+from pydantic.main import ModelMetaclass
 
 import fastkafka._components.logger
 
 fastkafka._components.logger.should_supress_timestamps = True
 
 import fastkafka
 from fastkafka._components.aiokafka_consumer_loop import (
     aiokafka_consumer_loop,
     sanitize_kafka_config,
 )
-from .._components.aiokafka_producer_manager import AIOKafkaProducerManager
 from fastkafka._components.asyncapi import (
     ConsumeCallable,
     ContactInfo,
     KafkaBroker,
     KafkaBrokers,
     KafkaServiceInfo,
     export_async_spec,
@@ -46,16 +46,16 @@
 from .._components.meta import delegates, export, filter_using_signature, patch
 from .._components.producer_decorator import ProduceCallable, producer_decorator
 
 # %% ../../nbs/015_FastKafka.ipynb 3
 logger = get_logger(__name__)
 
 # %% ../../nbs/015_FastKafka.ipynb 9
-@delegates(AIOKafkaConsumer)
-@delegates(AIOKafkaProducer, keep=True)
+@delegates(AIOKafkaConsumer, but=["bootstrap_servers"])
+@delegates(AIOKafkaProducer, but=["bootstrap_servers"], keep=True)
 def _get_kafka_config(
     **kwargs: Any,
 ) -> Dict[str, Any]:
     """Get kafka config"""
     allowed_keys = set(signature(_get_kafka_config).parameters.keys())
     if not set(kwargs.keys()) <= allowed_keys:
         unallowed_keys = ", ".join(
@@ -149,15 +149,14 @@
         *,
         title: Optional[str] = None,
         description: Optional[str] = None,
         version: Optional[str] = None,
         contact: Optional[Dict[str, str]] = None,
         kafka_brokers: Dict[str, Any],
         root_path: Optional[Union[Path, str]] = None,
-        bootstrap_servers: Optional[Union[str, List[str]]] = None,
         lifespan: Optional[Callable[["FastKafka"], AsyncContextManager[None]]] = None,
         **kwargs: Any,
     ):
         """Creates FastKafka application
 
         Args:
             title: optional title for the documentation. If None,
@@ -168,20 +167,14 @@
                 the version will be set to empty string
             contact: optional contact for the documentation. If None, the
                 contact will be set to placeholder values:
                 name='Author' url=HttpUrl('https://www.google.com', ) email='noreply@gmail.com'
             kafka_brokers: dictionary describing kafka brokers used for
                 generating documentation
             root_path: path to where documentation will be created
-            bootstrap_servers (str, list(str)): a ``host[:port]`` string or list of
-                ``host[:port]`` strings that the producer should contact to
-                bootstrap initial cluster metadata. This does not have to be the
-                full node list.  It just needs to have at least one broker that will
-                respond to a Metadata API Request. Default port is 9092. If no
-                servers are specified, will default to ``localhost:9092``.
             lifespan: asynccontextmanager that is used for setting lifespan hooks.
                 __aenter__ is called before app start and __aexit__ after app stop.
                 The lifespan is called whe application is started as async context
                 manager, e.g.:`async with kafka_app...`
 
         """
 
@@ -204,32 +197,30 @@
 
         self._root_path = Path(".") if root_path is None else Path(root_path)
 
         self._asyncapi_path = self._root_path / "asyncapi"
         (self._asyncapi_path / "docs").mkdir(exist_ok=True, parents=True)
         (self._asyncapi_path / "spec").mkdir(exist_ok=True, parents=True)
 
-        if bootstrap_servers is not None:
-            raise ValueError(
-                f"'bootstrap_servers' parameter is not supported, please use 'kafka_brokers' to set kafka server configuration"
-            )
-
         # this is used as default parameters for creating AIOProducer and AIOConsumer objects
         self._kafka_config = _get_kafka_config(**kwargs)
 
         #
-        self._consumers_store: Dict[str, Tuple[ConsumeCallable, Dict[str, Any]]] = {}
+        self._consumers_store: Dict[
+            str,
+            Tuple[
+                ConsumeCallable, Callable[[bytes, ModelMetaclass], Any], Dict[str, Any]
+            ],
+        ] = {}
 
         self._producers_store: Dict[  # type: ignore
             str, Tuple[ProduceCallable, AIOKafkaProducer, Dict[str, Any]]
         ] = {}
 
-        self._producers_list: List[  # type: ignore
-            Union[AIOKafkaProducer, AIOKafkaProducerManager]
-        ] = []
+        self._producers_list: List[AIOKafkaProducer] = []  # type: ignore
 
         self.benchmark_results: Dict[str, Dict[str, Any]] = {}
 
         # background tasks
         self._scheduled_bg_tasks: List[Callable[..., Coroutine[Any, Any, Any]]] = []
         self._bg_task_group_generator: Optional[anyio.abc.TaskGroup] = None
         self._bg_tasks_group: Optional[anyio.abc.TaskGroup] = None
@@ -294,23 +285,25 @@
 
     async def _stop(self) -> None:
         raise NotImplementedError
 
     def consumes(
         self,
         topic: Optional[str] = None,
+        decoder: str = "json",
         *,
         prefix: str = "on_",
         **kwargs: Dict[str, Any],
     ) -> ConsumeCallable:
         raise NotImplementedError
 
     def produces(  # type: ignore
         self,
         topic: Optional[str] = None,
+        encoder: str = "json",
         *,
         prefix: str = "to_",
         producer: Optional[AIOKafkaProducer] = None,
         **kwargs: Dict[str, Any],
     ) -> ProduceCallable:
         raise NotImplementedError
 
@@ -354,32 +347,57 @@
     async def _shutdown_producers(self) -> None:
         raise NotImplementedError
 
     async def _shutdown_bg_tasks(self) -> None:
         raise NotImplementedError
 
 # %% ../../nbs/015_FastKafka.ipynb 25
+def _get_decoder_fn(decoder: str) -> Callable[[bytes, ModelMetaclass], Any]:
+    """
+    Imports and returns decoder function based on input
+    """
+    if decoder == "json":
+        from fastkafka._components.encoder.json import json_decoder
+
+        return json_decoder
+    elif decoder == "avro":
+        try:
+            from fastkafka._components.encoder.avro import avro_decoder
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "Unable to import avro packages. Please install FastKafka using the command 'fastkafka[avro]'"
+            )
+        return avro_decoder
+    else:
+        raise ValueError(f"Unknown decoder - {decoder}")
+
+# %% ../../nbs/015_FastKafka.ipynb 27
 @patch
 @delegates(AIOKafkaConsumer)
 def consumes(
     self: FastKafka,
     topic: Optional[str] = None,
+    decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = "json",
     *,
     prefix: str = "on_",
     **kwargs: Dict[str, Any],
 ) -> Callable[[ConsumeCallable], ConsumeCallable]:
     """Decorator registering the callback called when a message is received in a topic.
 
     This function decorator is also responsible for registering topics for AsyncAPI specificiation and documentation.
 
     Args:
         topic: Kafka topic that the consumer will subscribe to and execute the
             decorated function when it receives a message from the topic,
             default: None. If the topic is not specified, topic name will be
             inferred from the decorated function name by stripping the defined prefix
+        decoder: Decoder to use to decode messages consumed from the topic,
+                default: json - By default, it uses json decoder to decode
+                bytes to json string and then it creates instance of pydantic
+                BaseModel. It also accepts custom decoder function.
         prefix: Prefix stripped from the decorated function to define a topic name
             if the topic argument is not passed, default: "on_". If the decorated
             function name is not prefixed with the defined prefix and topic argument
             is not passed, then this method will throw ValueError
 
     Returns:
         A function returning the same function
@@ -388,47 +406,74 @@
         ValueError
 
     """
 
     def _decorator(
         on_topic: ConsumeCallable,
         topic: Optional[str] = topic,
+        decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = decoder,
         kwargs: Dict[str, Any] = kwargs,
     ) -> ConsumeCallable:
         topic_resolved: str = (
             _get_topic_name(topic_callable=on_topic, prefix=prefix)
             if topic is None
             else topic
         )
 
-        self._consumers_store[topic_resolved] = (on_topic, kwargs)
+        decoder_fn = _get_decoder_fn(decoder) if isinstance(decoder, str) else decoder
+        self._consumers_store[topic_resolved] = (on_topic, decoder_fn, kwargs)
 
         return on_topic
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 27
+# %% ../../nbs/015_FastKafka.ipynb 29
+def _get_encoder_fn(encoder: str) -> Callable[[BaseModel], bytes]:
+    """
+    Imports and returns encoder function based on input
+    """
+    if encoder == "json":
+        from fastkafka._components.encoder.json import json_encoder
+
+        return json_encoder
+    elif encoder == "avro":
+        try:
+            from fastkafka._components.encoder.avro import avro_encoder
+        except ModuleNotFoundError:
+            raise ModuleNotFoundError(
+                "Unable to import avro packages. Please install FastKafka using the command 'fastkafka[avro]'"
+            )
+        return avro_encoder
+    else:
+        raise ValueError(f"Unknown encoder - {encoder}")
+
+# %% ../../nbs/015_FastKafka.ipynb 31
 @patch
 @delegates(AIOKafkaProducer)
 def produces(
     self: FastKafka,
     topic: Optional[str] = None,
+    encoder: Union[str, Callable[[BaseModel], bytes]] = "json",
     *,
     prefix: str = "to_",
     **kwargs: Dict[str, Any],
 ) -> Callable[[ProduceCallable], ProduceCallable]:
     """Decorator registering the callback called when delivery report for a produced message is received
 
     This function decorator is also responsible for registering topics for AsyncAPI specificiation and documentation.
 
     Args:
         topic: Kafka topic that the producer will send returned values from
             the decorated function to, default: None- If the topic is not
             specified, topic name will be inferred from the decorated function
             name by stripping the defined prefix.
+        encoder: Encoder to use to encode messages before sending it to topic,
+                default: json - By default, it uses json encoder to convert
+                pydantic basemodel to json string and then encodes the string to bytes
+                using 'utf-8' encoding. It also accepts custom encoder function.
         prefix: Prefix stripped from the decorated function to define a topic
             name if the topic argument is not passed, default: "to_". If the
             decorated function name is not prefixed with the defined prefix
             and topic argument is not passed, then this method will throw ValueError
 
     Returns:
         A function returning the same function
@@ -445,26 +490,29 @@
         topic_resolved: str = (
             _get_topic_name(topic_callable=on_topic, prefix=prefix)
             if topic is None
             else topic
         )
 
         self._producers_store[topic_resolved] = (on_topic, None, kwargs)
-        return producer_decorator(self._producers_store, on_topic, topic_resolved)
+        encoder_fn = _get_encoder_fn(encoder) if isinstance(encoder, str) else encoder
+        return producer_decorator(
+            self._producers_store, on_topic, topic_resolved, encoder_fn=encoder_fn
+        )
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 29
+# %% ../../nbs/015_FastKafka.ipynb 33
 @patch
 def get_topics(self: FastKafka) -> Iterable[str]:
     produce_topics = set(self._producers_store.keys())
     consume_topics = set(self._consumers_store.keys())
     return consume_topics.union(produce_topics)
 
-# %% ../../nbs/015_FastKafka.ipynb 31
+# %% ../../nbs/015_FastKafka.ipynb 35
 @patch
 def run_in_background(
     self: FastKafka,
 ) -> Callable[
     [Callable[..., Coroutine[Any, Any, Any]]], Callable[..., Coroutine[Any, Any, Any]]
 ]:
     """
@@ -493,53 +541,58 @@
         )
         self._scheduled_bg_tasks.append(bg_task)
 
         return bg_task
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 35
+# %% ../../nbs/015_FastKafka.ipynb 39
 @patch
 def _populate_consumers(
     self: FastKafka,
     is_shutting_down_f: Callable[[], bool],
 ) -> None:
     default_config: Dict[str, Any] = filter_using_signature(
         AIOKafkaConsumer, **self._kafka_config
     )
     self._kafka_consumer_tasks = [
         asyncio.create_task(
             aiokafka_consumer_loop(
                 topic=topic,
+                decoder_fn=decoder_fn,
                 callback=consumer,
                 msg_type=signature(consumer).parameters["msg"].annotation,
                 is_shutting_down_f=is_shutting_down_f,
                 **{**default_config, **override_config},
             )
         )
-        for topic, (consumer, override_config) in self._consumers_store.items()
+        for topic, (
+            consumer,
+            decoder_fn,
+            override_config,
+        ) in self._consumers_store.items()
     ]
 
 
 @patch
 async def _shutdown_consumers(
     self: FastKafka,
 ) -> None:
     if self._kafka_consumer_tasks:
         await asyncio.wait(self._kafka_consumer_tasks)
 
-# %% ../../nbs/015_FastKafka.ipynb 37
+# %% ../../nbs/015_FastKafka.ipynb 41
 # TODO: Add passing of vars
 async def _create_producer(  # type: ignore
     *,
     callback: ProduceCallable,
     default_config: Dict[str, Any],
     override_config: Dict[str, Any],
-    producers_list: List[Union[AIOKafkaProducer, AIOKafkaProducerManager]],
-) -> Union[AIOKafkaProducer, AIOKafkaProducerManager]:
+    producers_list: List[AIOKafkaProducer],
+) -> AIOKafkaProducer:
     """Creates a producer
 
     Args:
         callback: A callback function that is called when the producer is ready.
         producer: An existing producer to use.
         default_config: A dictionary of default configuration values.
         override_config: A dictionary of configuration values to override.
@@ -547,24 +600,21 @@
 
     Returns:
         A producer.
     """
 
     config = {
         **filter_using_signature(AIOKafkaProducer, **default_config),
-        **override_config,
+        **filter_using_signature(AIOKafkaProducer, **override_config),
     }
     producer = AIOKafkaProducer(**config)
     logger.info(
         f"_create_producer() : created producer using the config: '{sanitize_kafka_config(**config)}'"
     )
 
-    if not iscoroutinefunction(callback):
-        producer = AIOKafkaProducerManager(producer)
-
     await producer.start()
 
     producers_list.append(producer)
 
     return producer
 
 
@@ -620,15 +670,15 @@
                 callback,
                 _,
                 override_config,
             ) in self._producers_store.items()
         }
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 39
+# %% ../../nbs/015_FastKafka.ipynb 43
 @patch
 async def _populate_bg_tasks(
     self: FastKafka,
 ) -> None:
     def _start_bg_task(task: Callable[..., Coroutine[Any, Any, Any]]) -> asyncio.Task:
         logger.info(
             f"_populate_bg_tasks() : Starting background task '{task.__name__}'"
@@ -656,15 +706,15 @@
             await task
         except asyncio.CancelledError:
             pass
         logger.info(
             f"_shutdown_bg_tasks() : Execution finished for background task '{task.get_name()}'"
         )
 
-# %% ../../nbs/015_FastKafka.ipynb 41
+# %% ../../nbs/015_FastKafka.ipynb 45
 @patch
 async def _start(self: FastKafka) -> None:
     def is_shutting_down_f(self: FastKafka = self) -> bool:
         return self._is_shutting_down
 
     #     self.create_docs()
     await self._populate_producers()
@@ -681,30 +731,30 @@
     await self._shutdown_bg_tasks()
     await self._shutdown_consumers()
     await self._shutdown_producers()
 
     self._is_shutting_down = False
     self._is_started = False
 
-# %% ../../nbs/015_FastKafka.ipynb 47
+# %% ../../nbs/015_FastKafka.ipynb 51
 @patch
 def create_docs(self: FastKafka) -> None:
     export_async_spec(
         consumers={
-            topic: callback for topic, (callback, _) in self._consumers_store.items()
+            topic: callback for topic, (callback, _, _) in self._consumers_store.items()
         },
         producers={
             topic: callback for topic, (callback, _, _) in self._producers_store.items()
         },
         kafka_brokers=self._kafka_brokers,
         kafka_service_info=self._kafka_service_info,
         asyncapi_path=self._asyncapi_path,
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 51
+# %% ../../nbs/015_FastKafka.ipynb 55
 class AwaitedMock:
     @staticmethod
     def _await_for(f: Callable[..., Any]) -> Callable[..., Any]:
         @delegates(f)
         async def inner(
             *args: Any, f: Callable[..., Any] = f, timeout: int = 60, **kwargs: Any
         ) -> Any:
@@ -732,19 +782,19 @@
 
         for name in o.__dir__():
             if not name.startswith("_"):
                 f = getattr(o, name)
                 if inspect.ismethod(f):
                     setattr(self, name, self._await_for(f))
 
-# %% ../../nbs/015_FastKafka.ipynb 52
+# %% ../../nbs/015_FastKafka.ipynb 56
 @patch
 def create_mocks(self: FastKafka) -> None:
     """Creates self.mocks as a named tuple mapping a new function obtained by calling the original functions and a mock"""
-    app_methods = [f for f, _ in self._consumers_store.values()] + [
+    app_methods = [f for f, _, _ in self._consumers_store.values()] + [
         f for f, _, _ in self._producers_store.values()
     ]
     self.AppMocks = namedtuple(  # type: ignore
         f"{self.__class__.__name__}Mocks", [f.__name__ for f in app_methods]
     )
 
     self.mocks = self.AppMocks(  # type: ignore
@@ -782,32 +832,33 @@
         else:
             return sync_inner
 
     self._consumers_store.update(
         {
             name: (
                 add_mock(f, getattr(self.mocks, f.__name__)),
+                decoder_fn,
                 kwargs,
             )
-            for name, (f, kwargs) in self._consumers_store.items()
+            for name, (f, decoder_fn, kwargs) in self._consumers_store.items()
         }
     )
 
     self._producers_store.update(
         {
             name: (
                 add_mock(f, getattr(self.mocks, f.__name__)),
                 producer,
                 kwargs,
             )
             for name, (f, producer, kwargs) in self._producers_store.items()
         }
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 58
+# %% ../../nbs/015_FastKafka.ipynb 62
 @patch
 def benchmark(
     self: FastKafka,
     interval: Union[int, timedelta] = 1,
     *,
     sliding_window_size: Optional[int] = None,
 ) -> Callable[[Callable[[I], Optional[O]]], Callable[[I], Optional[O]]]:
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_application/tester.py` & `fastkafka-0.5.0rc0/fastkafka/_application/tester.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from .._components.meta import delegates, patch
 from .._testing.apache_kafka_broker import ApacheKafkaBroker
 from .._testing.in_memory_broker import InMemoryBroker
 from .._testing.local_redpanda_broker import LocalRedpandaBroker
 
 # %% ../../nbs/016_Tester.ipynb 6
 class Tester(FastKafka):
+    __test__ = False
+
     @delegates(ApacheKafkaBroker.__init__)
     def __init__(
         self,
         app: Union[FastKafka, List[FastKafka]],
         *,
         broker: Optional[
             Union[ApacheKafkaBroker, LocalRedpandaBroker, InMemoryBroker]
@@ -190,15 +192,15 @@
     mirror_func.__signature__ = sig  # type: ignore
     return mirror_func
 
 # %% ../../nbs/016_Tester.ipynb 15
 @patch
 def create_mirrors(self: Tester) -> None:
     for app in self.apps:
-        for topic, (consumer_f, _) in app._consumers_store.items():
+        for topic, (consumer_f, _, _) in app._consumers_store.items():
             mirror_f = mirror_consumer(topic, consumer_f)
             mirror_f = self.produces()(mirror_f)  # type: ignore
             setattr(self, mirror_f.__name__, mirror_f)
         for topic, (producer_f, _, _) in app._producers_store.items():
             mirror_f = mirror_producer(topic, producer_f)
             mirror_f = self.consumes()(mirror_f)  # type: ignore
             setattr(self, mirror_f.__name__, mirror_f)
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_cli.py` & `fastkafka-0.5.0rc0/fastkafka/_cli.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_cli_docs.py` & `fastkafka-0.5.0rc0/fastkafka/_cli_docs.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_cli_testing.py` & `fastkafka-0.5.0rc0/fastkafka/_cli_testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/_subprocess.py` & `fastkafka-0.5.0rc0/fastkafka/_components/_subprocess.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.5.0rc0/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import anyio
 import asyncer
 from aiokafka import AIOKafkaConsumer
 from aiokafka.structs import ConsumerRecord, TopicPartition
 from anyio.streams.memory import MemoryObjectReceiveStream
 from pydantic import BaseModel
+from pydantic.main import ModelMetaclass
 
 from .logger import get_logger
 from .meta import delegates
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 5
 logger = get_logger(__name__)
 
@@ -106,46 +107,50 @@
 
 
 @delegates(AIOKafkaConsumer.getmany)
 async def _aiokafka_consumer_loop(  # type: ignore
     consumer: AIOKafkaConsumer,
     *,
     topic: str,
+    decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     callback: Callable[[BaseModel], Union[None, Awaitable[None]]],
     max_buffer_size: int = 100_000,
     msg_type: Type[BaseModel],
     is_shutting_down_f: Callable[[], bool],
     **kwargs: Any,
 ) -> None:
     """
     Consumer loop for infinite pooling of the AIOKafka consumer for new messages. Calls consumer.getmany()
     and after the consumer return messages or times out, messages are decoded and streamed to defined callback.
 
     Params:
+        topic: Topic to subscribe
+        decoder_fn: Function to decode the messages consumed from the topic
         callbacks: Dict of callbacks mapped to their respective topics
         timeout_ms: Time to timeut the getmany request by the consumer
         max_buffer_size: Maximum number of unconsumed messages in the callback buffer
         msg_types: Dict of message types mapped to their respective topics
         is_shutting_down_f: Function for controlling the shutdown of consumer loop
     """
 
     prepared_callback = _prepare_callback(callback)
 
     async def process_message_callback(
         receive_stream: MemoryObjectReceiveStream[Any],
         callback: Callable[[BaseModel], Awaitable[None]] = prepared_callback,
         msg_type: Type[BaseModel] = msg_type,
         topic: str = topic,
+        decoder_fn: Callable[[bytes, ModelMetaclass], Any] = decoder_fn,
     ) -> None:
         async with receive_stream:
             try:
                 async for record in _streamed_records(receive_stream):
                     try:
                         msg = record.value
-                        decoded_msg = msg_type.parse_raw(msg.decode("utf-8"))
+                        decoded_msg = decoder_fn(msg, msg_type)
                         await callback(decoded_msg)
                     except Exception as e:
                         logger.warning(
                             f"process_message_callback(): Unexpected exception '{e.__repr__()}' caught and ignored for topic='{topic}' and message: {msg}"
                         )
             except Exception as e:
                 logger.warning(
@@ -163,38 +168,43 @@
                 msgs = await consumer.getmany(**kwargs)
                 try:
                     await send_stream.send(msgs.values())
                 except Exception as e:
                     logger.warning(
                         f"_aiokafka_consumer_loop(): Unexpected exception '{e}' caught and ignored for messages: {msgs}"
                     )
+            logger.info(
+                f"_aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain..."
+            )
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 24
 def sanitize_kafka_config(**kwargs: Any) -> Dict[str, Any]:
     """Sanitize Kafka config"""
     return {k: "*" * len(v) if "pass" in k.lower() else v for k, v in kwargs.items()}
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 26
 @delegates(AIOKafkaConsumer)
 @delegates(_aiokafka_consumer_loop, keep=True)
 async def aiokafka_consumer_loop(
     topic: str,
+    decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     *,
     timeout_ms: int = 100,
     max_buffer_size: int = 100_000,
     callback: Callable[[BaseModel], Union[None, Awaitable[None]]],
     msg_type: Type[BaseModel],
     is_shutting_down_f: Callable[[], bool],
     **kwargs: Any,
 ) -> None:
     """Consumer loop for infinite pooling of the AIOKafka consumer for new messages. Creates and starts AIOKafkaConsumer
     and runs _aio_kafka_consumer loop fo infinite poling of the consumer for new messages.
 
     Args:
         topic: name of the topic to subscribe to
+        decoder_fn: Function to decode the messages consumed from the topic
         callback: callback function to be called after decoding and parsing a consumed message
         timeout_ms: Time to timeut the getmany request by the consumer
         max_buffer_size: Maximum number of unconsumed messages in the callback buffer
         msg_type: Type with `parse_json` method used for parsing a decoded message
         is_shutting_down_f: Function for controlling the shutdown of consumer loop
     """
     logger.info(f"aiokafka_consumer_loop() starting...")
@@ -211,14 +221,15 @@
         consumer.subscribe([topic])
         logger.info("aiokafka_consumer_loop(): Consumer subscribed.")
 
         try:
             await _aiokafka_consumer_loop(
                 consumer=consumer,
                 topic=topic,
+                decoder_fn=decoder_fn,
                 max_buffer_size=max_buffer_size,
                 timeout_ms=timeout_ms,
                 callback=callback,
                 msg_type=msg_type,
                 is_shutting_down_f=is_shutting_down_f,
             )
         finally:
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/asyncapi.py` & `fastkafka-0.5.0rc0/fastkafka/_components/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/benchmarking.py` & `fastkafka-0.5.0rc0/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.5.0rc0/fastkafka/_components/docs_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/helpers.py` & `fastkafka-0.5.0rc0/fastkafka/_components/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/998_Internal_Helpers.ipynb.
 
 # %% auto 0
-__all__ = ['logger', 'in_notebook', 'change_dir', 'ImportFromStringError']
+__all__ = ['in_notebook', 'change_dir', 'ImportFromStringError', 'true_after']
 
 # %% ../../nbs/998_Internal_Helpers.ipynb 2
 def in_notebook() -> bool:
     try:
         from IPython import get_ipython
 
         if "IPKernelApp" not in get_ipython().config:
@@ -21,35 +21,32 @@
 import importlib
 import os
 import sys
 from functools import wraps
 from inspect import signature
 from pathlib import Path
 from typing import *
+from datetime import datetime, timedelta
 
 import docstring_parser
 import typer
 
-from .logger import get_logger
 from .meta import delegates
 
 # %% ../../nbs/998_Internal_Helpers.ipynb 6
-logger = get_logger(__name__)
-
-# %% ../../nbs/998_Internal_Helpers.ipynb 8
 @contextlib.contextmanager
 def change_dir(d: str) -> Generator[None, None, None]:
     curdir = os.getcwd()
     os.chdir(d)
     try:
         yield
     finally:
         os.chdir(curdir)
 
-# %% ../../nbs/998_Internal_Helpers.ipynb 10
+# %% ../../nbs/998_Internal_Helpers.ipynb 8
 class ImportFromStringError(Exception):
     pass
 
 
 def _import_from_string(import_str: str) -> Any:
     """Imports library from string
 
@@ -89,7 +86,17 @@
     except AttributeError:
         message = 'Attribute "{attrs_str}" not found in module "{module_str}".'
         raise ImportFromStringError(
             message.format(attrs_str=attrs_str, module_str=module_str)
         )
 
     return instance
+
+# %% ../../nbs/998_Internal_Helpers.ipynb 10
+def true_after(seconds: Union[int, float]) -> Callable[[], bool]:
+    """Function returning True after a given number of seconds"""
+    t = datetime.now()
+
+    def _true_after(seconds: Union[int, float] = seconds, t: datetime = t) -> bool:
+        return (datetime.now() - t) > timedelta(seconds=seconds)
+
+    return _true_after
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/logger.py` & `fastkafka-0.5.0rc0/fastkafka/_components/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/Logger.ipynb.
 
 # %% auto 0
 __all__ = ['should_supress_timestamps', 'logger_spaces_added', 'supress_timestamps', 'get_default_logger_configuration',
-           'get_logger', 'set_level']
+           'get_logger', 'set_level', 'cached_log']
 
 # %% ../../nbs/Logger.ipynb 2
 import logging
 import logging.config
 from typing import *
+from .meta import patch
+from .helpers import true_after
 
 # %% ../../nbs/Logger.ipynb 4
 # Logger Levels
 # CRITICAL = 50
 # ERROR = 40
 # WARNING = 30
 # INFO = 20
@@ -127,7 +129,19 @@
         logging.getLogger(name)
         for name in logging.root.manager.loggerDict
         if ("airt" in name) or ("__main__" in name)
     ]
 
     for logger in loggers:
         logger.setLevel(level)
+
+# %% ../../nbs/Logger.ipynb 18
+def cached_log(
+    self: logging.Logger, msg: str, level: int, timeout: Union[int, float] = 5
+) -> None:
+    if not hasattr(self, "_timeouted_msgs"):
+        self._timeouted_msgs = {}  # type: ignore
+
+    if msg not in self._timeouted_msgs or self._timeouted_msgs[msg]():  # type: ignore
+        self._timeouted_msgs[msg] = true_after(timeout)  # type: ignore
+
+        self.log(level, msg)
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/meta.py` & `fastkafka-0.5.0rc0/fastkafka/_components/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,76 +218,89 @@
 # %% ../../nbs/096_Meta.ipynb 45
 def _format_args(xs: List[docstring_parser.DocstringParam]) -> str:
     return "\nArgs:\n - " + "\n - ".join(
         [f"{x.arg_name} ({x.type_name}): {x.description}" for x in xs]
     )
 
 
-def combine_params(f: F, o: Union[Type, Callable[..., Any]]) -> F:
+def combine_params(
+    f: F, o: Union[Type, Callable[..., Any]], but: Optional[List[str]] = None
+) -> F:
     """Combines docstring arguments of a function and another object or function
 
     Args:
         f: destination functions where combined arguments will end up
         o: source function from which arguments are taken from
 
     Returns:
         Function f with augumented docstring including arguments from both functions/objects
     """
+    if but is None:
+        but = []
+
     src_params = docstring_parser.parse_from_object(o).params
     #     logger.info(f"combine_params(): source:{_format_args(src_params)}")
     docs = docstring_parser.parse_from_object(f)
     #     logger.info(f"combine_params(): destination:{_format_args(docs.params)}")
     dst_params_names = [p.arg_name for p in docs.params]
 
     combined_params = docs.params + [
-        x for x in src_params if not x.arg_name in dst_params_names
+        x
+        for x in src_params
+        if x.arg_name not in dst_params_names and x.arg_name not in but
     ]
     #     logger.info(f"combine_params(): combined:{_format_args(combined_params)}")
 
     docs.meta = [
         x for x in docs.meta if not isinstance(x, docstring_parser.DocstringParam)
     ] + combined_params  # type: ignore
 
     f.__doc__ = docstring_parser.compose(
         docs, style=docstring_parser.DocstringStyle.GOOGLE
     )
     return f
 
-# %% ../../nbs/096_Meta.ipynb 47
+# %% ../../nbs/096_Meta.ipynb 48
 def delegates(
     o: Union[Type, Callable[..., Any]],
     keep: bool = False,
     but: Optional[List[str]] = None,
 ) -> Callable[[F], F]:
     """Delegates keyword agruments from o to the function the decorator is applied to
 
     Args:
         o: object (class or function) with default kwargs
         keep: Keep `kwargs` in decorated function?
         but: argument names not to include
     """
 
     def _inner(f: F, keep: bool = keep, but: Optional[List[str]] = but) -> F:
-        def _combine_params(o: Union[Type, Callable[..., Any]]) -> Callable[[F], F]:
-            def __combine_params(f: F, o: Union[Type, Callable[..., Any]] = o) -> F:
-                return combine_params(f=f, o=o)
+        def _combine_params(
+            o: Union[Type, Callable[..., Any]], but: Optional[List[str]] = None
+        ) -> Callable[[F], F]:
+            def __combine_params(
+                f: F,
+                o: Union[Type, Callable[..., Any]] = o,
+                but: Optional[List[str]] = but,
+            ) -> F:
+                return combine_params(f=f, o=o, but=but)
 
             return __combine_params
 
-        @_combine_params(o)  # type: ignore
+        @_combine_params(o, but=but)  # type: ignore
         @_delegates_without_docs(o, keep=keep, but=but)  # type: ignore
         @wraps(f)
         def _f(*args: Any, **kwargs: Any) -> Any:
             return f(*args, **kwargs)
 
         return _f
 
     return _inner
 
-# %% ../../nbs/096_Meta.ipynb 64
+# %% ../../nbs/096_Meta.ipynb 66
 def use_parameters_of(
     o: Union[Type, Callable[..., Any]], **kwargs: Dict[str, Any]
 ) -> Dict[str, Any]:
     """Restrict parameters passwed as keyword arguments to parameters from the signature of ``o``
 
     Args:
         o: object or callable which signature is used for restricting keyword arguments
@@ -296,32 +309,32 @@
     Returns:
         restricted keyword arguments
 
     """
     allowed_keys = set(inspect.signature(o).parameters.keys())
     return {k: v for k, v in kwargs.items() if k in allowed_keys}
 
-# %% ../../nbs/096_Meta.ipynb 66
+# %% ../../nbs/096_Meta.ipynb 68
 def filter_using_signature(f: Callable, **kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """todo: write docs"""
     param_names = list(inspect.signature(f).parameters.keys())
     return {k: v for k, v in kwargs.items() if k in param_names}
 
-# %% ../../nbs/096_Meta.ipynb 68
+# %% ../../nbs/096_Meta.ipynb 70
 TorF = TypeVar("TorF", Type, Callable[..., Any])
 
 
 def export(module_name: str) -> Callable[[TorF], TorF]:
     def _inner(o: TorF, module_name: str = module_name) -> TorF:
         o.__module__ = module_name
         return o
 
     return _inner
 
-# %% ../../nbs/096_Meta.ipynb 71
+# %% ../../nbs/096_Meta.ipynb 73
 T = TypeVar("T")
 
 
 def classcontextmanager(name: str = "lifecycle") -> Callable[[Type[T]], Type[T]]:
     def _classcontextmanager(cls: Type[T], name: str = name) -> Type[T]:
         if not hasattr(cls, name):
             raise ValueError
@@ -338,15 +351,15 @@
         def __exit__(self: cls, *args: Any) -> None:  # type: ignore
             self._lifecycle_ctx.pop(-1).__exit__(*args)  # type: ignore
 
         return cls
 
     return _classcontextmanager
 
-# %% ../../nbs/096_Meta.ipynb 74
+# %% ../../nbs/096_Meta.ipynb 76
 def _get_default_kwargs_from_sig(f: F, **kwargs: Any) -> Dict[str, Any]:
     """
     Get default values for function **kwargs
 
     Args:
         f: Function to extract default values from
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/producer_decorator.py` & `fastkafka-0.5.0rc0/fastkafka/_components/producer_decorator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/013_ProducerDecorator.ipynb.
 
 # %% auto 0
-__all__ = ['BaseSubmodel', 'ProduceReturnTypes', 'ProduceCallable', 'KafkaEvent', 'producer_decorator']
+__all__ = ['BaseSubmodel', 'ProduceReturnTypes', 'ProduceCallable', 'KafkaEvent', 'get_loop', 'producer_decorator']
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 1
 import functools
 import json
+import asyncio
 from asyncio import iscoroutinefunction  # do not use the version from inspect
 from collections import namedtuple
 from dataclasses import dataclass
 from typing import *
 
+import nest_asyncio
+
 from aiokafka import AIOKafkaProducer
 from pydantic import BaseModel
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 3
 BaseSubmodel = TypeVar("BaseSubmodel", bound=BaseModel)
 BaseSubmodel
 
@@ -38,55 +41,71 @@
 # %% ../../nbs/013_ProducerDecorator.ipynb 5
 ProduceReturnTypes = Union[BaseModel, KafkaEvent[BaseModel]]
 
 ProduceCallable = Union[
     Callable[..., ProduceReturnTypes], Callable[..., Awaitable[ProduceReturnTypes]]
 ]
 
-# %% ../../nbs/013_ProducerDecorator.ipynb 6
-def _to_json_utf8(o: Any) -> bytes:
-    """Converts to JSON and then encodes with UTF-8"""
-    if hasattr(o, "json"):
-        return o.json().encode("utf-8")  # type: ignore
-    else:
-        return json.dumps(o).encode("utf-8")
-
 # %% ../../nbs/013_ProducerDecorator.ipynb 8
 def _wrap_in_event(message: Union[BaseModel, KafkaEvent]) -> KafkaEvent:
     return message if type(message) == KafkaEvent else KafkaEvent(message)
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 11
+def get_loop() -> asyncio.AbstractEventLoop:
+    try:
+        loop: asyncio.AbstractEventLoop = asyncio.get_event_loop()
+    except RuntimeError as e:
+        loop = asyncio.new_event_loop()
+
+    if loop.is_running():
+        nest_asyncio.apply(loop)
+
+    return loop
+
+# %% ../../nbs/013_ProducerDecorator.ipynb 13
 def producer_decorator(
-    producer_store: Dict[str, Any], func: ProduceCallable, topic: str
+    producer_store: Dict[str, Any],
+    func: ProduceCallable,
+    topic: str,
+    encoder_fn: Callable[[BaseModel], bytes],
 ) -> ProduceCallable:
     """todo: write documentation"""
 
+    loop = get_loop()
+
+    def release_callback(fut: asyncio.Future) -> None:
+        pass
+
     @functools.wraps(func)
     async def _produce_async(
         *args: List[Any],
         producer_store: Dict[str, Any] = producer_store,
         f: Callable[..., Awaitable[ProduceReturnTypes]] = func,  # type: ignore
         **kwargs: Any
     ) -> ProduceReturnTypes:
         return_val = await f(*args, **kwargs)
         wrapped_val = _wrap_in_event(return_val)
         _, producer, _ = producer_store[topic]
         fut = await producer.send(
-            topic, _to_json_utf8(wrapped_val.message), key=wrapped_val.key
+            topic, encoder_fn(wrapped_val.message), key=wrapped_val.key
         )
-        msg = await fut
+        fut.add_done_callback(release_callback)
         return return_val
 
     @functools.wraps(func)
     def _produce_sync(
         *args: List[Any],
         producer_store: Dict[str, Any] = producer_store,
         f: Callable[..., ProduceReturnTypes] = func,  # type: ignore
+        loop: asyncio.AbstractEventLoop = loop,
         **kwargs: Any
     ) -> ProduceReturnTypes:
         return_val = f(*args, **kwargs)
         wrapped_val = _wrap_in_event(return_val)
         _, producer, _ = producer_store[topic]
-        producer.send(topic, _to_json_utf8(wrapped_val.message), key=wrapped_val.key)
+        fut = loop.run_until_complete(
+            producer.send(topic, encoder_fn(wrapped_val.message), key=wrapped_val.key)
+        )
+        fut.add_done_callback(release_callback)
         return return_val
 
     return _produce_async if iscoroutinefunction(func) else _produce_sync
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_components/test_dependencies.py` & `fastkafka-0.5.0rc0/fastkafka/_components/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_docusaurus_helper.py` & `fastkafka-0.5.0rc0/fastkafka/_docusaurus_helper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/096_Docusaurus_Helper.ipynb.
 
 # %% auto 0
-__all__ = ['fix_invalid_syntax_in_markdown', 'generate_markdown_docs']
+__all__ = ['SidebarT', 'fix_invalid_syntax_in_markdown', 'generate_markdown_docs', 'parse_contents', 'remove_section_contents',
+           'generate_sidebar']
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 2
 import itertools
 import re
 import types
 from inspect import Signature, getmembers, isclass, isfunction, signature
 from pathlib import Path
+from urllib.parse import urljoin
 from typing import *
 
+import yaml
+
 from docstring_parser import parse
 from docstring_parser.common import DocstringParam, DocstringRaises, DocstringReturns
 from nbdev.config import get_config
 from nbdev_mkdocs.mkdocs import (
     _add_all_submodules,
     _get_api_summary,
     _import_all_members,
@@ -165,29 +169,30 @@
         A string representing the function definition
     """
     _signature = signature(symbol)
     arg_list = _get_arg_list_with_signature(_signature)
     ret_val = ""
 
     if isfunction(symbol):
-        ret_val = f"`def {symbol.__name__}({arg_list})"
+        ret_val = f"### `{symbol.__name__}`" + f" {{#{symbol.__name__.strip('_')}}}\n\n"
+        ret_val = ret_val + f"`def {symbol.__name__}({arg_list})"
         if _signature.return_annotation and "inspect._empty" not in str(
             _signature.return_annotation
         ):
             if isinstance(_signature.return_annotation, type):
                 ret_val = ret_val + f" -> {_signature.return_annotation.__name__}`\n"
             else:
                 ret_val = ret_val + f" -> {_signature.return_annotation}`\n"
 
         else:
             ret_val = ret_val + " -> None`\n"
 
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 27
+# %% ../nbs/096_Docusaurus_Helper.ipynb 28
 def _get_formatted_docstring_for_symbol(
     symbol: Union[types.FunctionType, Type[Any]]
 ) -> str:
     """Recursively parses and get formatted docstring of a symbol.
 
     Args:
         symbol: A Python class or function object to parse the docstring for.
@@ -222,15 +227,15 @@
         if symbol.__doc__ is not None
         else ""
     )
     if isclass(symbol):
         contents = traverse(symbol, contents)
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 31
+# %% ../nbs/096_Docusaurus_Helper.ipynb 32
 def _convert_html_style_attribute_to_jsx(contents: str) -> str:
     """Converts the inline style attributes in an HTML string to JSX compatible format.
 
     Args:
         contents: A string containing an HTML document or fragment.
 
     Returns:
@@ -254,63 +259,167 @@
         for key, value in style_dict.items():
             replacement += f"{key}: '{value}', "
         replacement = replacement[:-2] + "}}"
         contents = contents.replace(f'style="{style_match}"', replacement)
 
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 33
+# %% ../nbs/096_Docusaurus_Helper.ipynb 34
 def _get_all_markdown_files_path(docs_path: Path) -> List[Path]:
     """Get all Markdown files in a directory and its subdirectories.
 
     Args:
         directory: The path to the directory to search in.
 
     Returns:
         A list of paths to all Markdown files found in the directory and its subdirectories.
     """
     markdown_files = [file_path for file_path in docs_path.glob("**/*.md")]
     return markdown_files
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 35
+# %% ../nbs/096_Docusaurus_Helper.ipynb 36
 def _fix_special_symbols_in_html(contents: str) -> str:
     contents = contents.replace("”", '"')
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 37
+# %% ../nbs/096_Docusaurus_Helper.ipynb 38
+def _remove_redundant_segment_from_link(url: str) -> str:
+    """Remove redundant segment from the end of a URL.
+
+    Args:
+        url: The URL to remove the a redundant segment.
+
+    Returns:
+        The updated URL with the redundant segment removed, or the original URL if no redundant segment was found.
+    """
+    segments = url.split("/#")[0].split("/")[-2:]
+    return (
+        url.replace(f"/{segments[1]}", "")
+        if segments[0] == segments[1].lower()
+        else url
+    )
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 42
+def _fix_symbol_links(contents: str) -> str:
+    """Fix symbol links in Markdown content.
+
+    Args:
+        contents: The Markdown content to search for symbol links.
+
+    Returns:
+        str: The Markdown content with updated symbol links.
+    """
+    cfg = get_config()
+    prefix = re.escape(urljoin(cfg["doc_host"] + "/", cfg["doc_baseurl"] + "/api"))
+    pattern = re.compile(rf"\[(.*?)\]\(({prefix}[^)]+)\)")
+    matches = pattern.findall(contents)
+    for match in matches:
+        old_url = match[1]
+        new_url = _remove_redundant_segment_from_link(old_url).replace(
+            "/api/", "/docs/api/"
+        )
+        contents = contents.replace(old_url, new_url)
+    return contents
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 48
 def fix_invalid_syntax_in_markdown(docs_path: str) -> None:
     """Fix invalid HTML syntax in markdown files and converts inline style attributes to JSX-compatible format.
 
     Args:
         docs_path: The path to the root directory to search for markdown files.
     """
     markdown_files = _get_all_markdown_files_path(Path(docs_path))
-    updated_contents = [
-        _convert_html_style_attribute_to_jsx(Path(file).read_text())
-        for file in markdown_files
-    ]
-    updated_contents = [
-        _fix_special_symbols_in_html(contents) for contents in updated_contents
-    ]
-    for i, file_path in enumerate(markdown_files):
-        file_path.write_text(updated_contents[i])
+    for file in markdown_files:
+        contents = Path(file).read_text()
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 39
+        contents = _convert_html_style_attribute_to_jsx(contents)
+        contents = _fix_special_symbols_in_html(contents)
+        contents = _fix_symbol_links(contents)
+
+        file.write_text(contents)
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 50
 def generate_markdown_docs(module_name: str, docs_path: str) -> None:
     """Generates Markdown documentation files for the symbols in the given module and save them to the given directory.
 
     Args:
         module_name: The name of the module to generate documentation for.
         docs_path: The path to the directory where the documentation files will be saved.
     """
     members_with_submodules = _get_submodules(module_name)
     symbols = _load_submodules(module_name, members_with_submodules)
 
     for symbol in symbols:
-        content = f"`{symbol.__module__}.{symbol.__name__}`\n\n"
+        content = f"## `{symbol.__module__}.{symbol.__name__}` {{#{symbol.__module__}.{symbol.__name__}}}\n\n"
         content += _get_formatted_docstring_for_symbol(symbol)
         target_file_path = (
             "/".join(f"{symbol.__module__}.{symbol.__name__}".split(".")) + ".md"
         )
 
         with open((Path(docs_path) / "api" / target_file_path), "w") as f:
             f.write(content)
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 52
+SidebarT = Union[str, List["SidebarT"], Dict[str, "SidebarT"]]
+
+
+def parse_contents(contents: List[SidebarT]) -> List[SidebarT]:
+    new: List[SidebarT] = []
+    for content in contents:
+        if isinstance(content, str):
+            new.append(content.split(".")[0])
+        if isinstance(content, dict):
+            new.append(remove_section_contents(content))  # type: ignore
+    return new
+
+
+def remove_section_contents(
+    section: Dict[str, "SidebarT"]
+) -> Dict[str, List[SidebarT]]:
+    new_section: Dict[str, List["SidebarT"]] = {}
+    new_section[section["section"]] = parse_contents(section["contents"])  # type: ignore
+    return new_section
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 54
+def generate_sidebar(
+    nbs_sidebar: str = "/work/fastkafka/nbs/sidebar.yml",
+    target: str = "./docusaurus/sidebars.js",
+) -> None:
+    with open(nbs_sidebar, "r") as stream, open(target, "w") as target_stream:
+        try:
+            sidebar = yaml.safe_load(stream)
+            parsed_sidebar = parse_contents(sidebar["website"]["sidebar"]["contents"])
+            sidebar_str = str(parsed_sidebar)[1:-1] + ","
+            target_stream.write(
+                """module.exports = {
+tutorialSidebar: [
+    """
+                + sidebar_str
+                + """
+//         [require("./docs/reference/sidebar.json")],
+    {
+        "items": [
+            "api/fastkafka/FastKafka",
+            "api/fastkafka/KafkaEvent",
+            {
+              "items": [
+                "api/fastkafka/testing/ApacheKafkaBroker",
+                "api/fastkafka/testing/LocalRedpandaBroker",
+                "api/fastkafka/testing/Tester"
+              ],
+              "label": "testing",
+              "type": "category"
+            },
+        ],
+        "label": "API",
+        "type": "category"
+    },
+    {
+        "CLI": ['cli/fastkafka', 'cli/run_fastkafka_server_process'],
+    },
+
+    "CHANGELOG",
+],
+};"""
+            )
+        except yaml.YAMLError as exc:
+            print(exc)
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_helpers.py` & `fastkafka-0.5.0rc0/fastkafka/_helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_modidx.py` & `fastkafka-0.5.0rc0/fastkafka/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,18 @@
                                                                                                         'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.set_kafka_broker': ( 'fastkafka.html#fastkafka.set_kafka_broker',
                                                                                                        'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._create_producer': ( 'fastkafka.html#_create_producer',
                                                                                              'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_contact_info': ( 'fastkafka.html#_get_contact_info',
                                                                                               'fastkafka/_application/app.py'),
+                                            'fastkafka._application.app._get_decoder_fn': ( 'fastkafka.html#_get_decoder_fn',
+                                                                                            'fastkafka/_application/app.py'),
+                                            'fastkafka._application.app._get_encoder_fn': ( 'fastkafka.html#_get_encoder_fn',
+                                                                                            'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_kafka_brokers': ( 'fastkafka.html#_get_kafka_brokers',
                                                                                                'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_kafka_config': ( 'fastkafka.html#_get_kafka_config',
                                                                                               'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_topic_name': ( 'fastkafka.html#_get_topic_name',
                                                                                             'fastkafka/_application/app.py')},
             'fastkafka._application.tester': { 'fastkafka._application.tester.Tester': ( 'tester.html#tester',
@@ -101,26 +105,14 @@
                                                                                                                              'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._streamed_records': ( 'consumerloop.html#_streamed_records',
                                                                                                                                   'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop.aiokafka_consumer_loop': ( 'consumerloop.html#aiokafka_consumer_loop',
                                                                                                                                        'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop.sanitize_kafka_config': ( 'consumerloop.html#sanitize_kafka_config',
                                                                                                                                       'fastkafka/_components/aiokafka_consumer_loop.py')},
-            'fastkafka._components.aiokafka_producer_manager': { 'fastkafka._components.aiokafka_producer_manager.AIOKafkaProducerManager': ( 'producermanager.html#aiokafkaproducermanager',
-                                                                                                                                              'fastkafka/_components/aiokafka_producer_manager.py'),
-                                                                 'fastkafka._components.aiokafka_producer_manager.AIOKafkaProducerManager.__init__': ( 'producermanager.html#aiokafkaproducermanager.__init__',
-                                                                                                                                                       'fastkafka/_components/aiokafka_producer_manager.py'),
-                                                                 'fastkafka._components.aiokafka_producer_manager.AIOKafkaProducerManager.send': ( 'producermanager.html#aiokafkaproducermanager.send',
-                                                                                                                                                   'fastkafka/_components/aiokafka_producer_manager.py'),
-                                                                 'fastkafka._components.aiokafka_producer_manager.AIOKafkaProducerManager.start': ( 'producermanager.html#aiokafkaproducermanager.start',
-                                                                                                                                                    'fastkafka/_components/aiokafka_producer_manager.py'),
-                                                                 'fastkafka._components.aiokafka_producer_manager.AIOKafkaProducerManager.stop': ( 'producermanager.html#aiokafkaproducermanager.stop',
-                                                                                                                                                   'fastkafka/_components/aiokafka_producer_manager.py'),
-                                                                 'fastkafka._components.aiokafka_producer_manager._aiokafka_producer_manager': ( 'producermanager.html#_aiokafka_producer_manager',
-                                                                                                                                                 'fastkafka/_components/aiokafka_producer_manager.py')},
             'fastkafka._components.asyncapi': { 'fastkafka._components.asyncapi.APIKeyLocation': ( 'asyncapi.html#apikeylocation',
                                                                                                    'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.ContactInfo': ( 'asyncapi.html#contactinfo',
                                                                                                 'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaBroker': ( 'asyncapi.html#kafkabroker',
                                                                                                 'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaBroker.dict': ( 'asyncapi.html#kafkabroker.dict',
@@ -185,23 +177,47 @@
                                                                                                                  'fastkafka/_components/docs_dependencies.py'),
                                                          'fastkafka._components.docs_dependencies._check_npm_with_local': ( 'docs_dependencies.html#_check_npm_with_local',
                                                                                                                             'fastkafka/_components/docs_dependencies.py'),
                                                          'fastkafka._components.docs_dependencies._install_docs_npm_deps': ( 'docs_dependencies.html#_install_docs_npm_deps',
                                                                                                                              'fastkafka/_components/docs_dependencies.py'),
                                                          'fastkafka._components.docs_dependencies._install_node': ( 'docs_dependencies.html#_install_node',
                                                                                                                     'fastkafka/_components/docs_dependencies.py')},
+            'fastkafka._components.encoder.avro': { 'fastkafka._components.encoder.avro.AvroBase': ( 'avro_encode_decoder.html#avrobase',
+                                                                                                     'fastkafka/_components/encoder/avro.py'),
+                                                    'fastkafka._components.encoder.avro.AvroBase._avro_schema': ( 'avro_encode_decoder.html#avrobase._avro_schema',
+                                                                                                                  'fastkafka/_components/encoder/avro.py'),
+                                                    'fastkafka._components.encoder.avro.AvroBase.avro_schema': ( 'avro_encode_decoder.html#avrobase.avro_schema',
+                                                                                                                 'fastkafka/_components/encoder/avro.py'),
+                                                    'fastkafka._components.encoder.avro.AvroBase.avro_schema_for_pydantic': ( 'avro_encode_decoder.html#avrobase.avro_schema_for_pydantic',
+                                                                                                                              'fastkafka/_components/encoder/avro.py'),
+                                                    'fastkafka._components.encoder.avro.avro_decoder': ( 'avro_encode_decoder.html#avro_decoder',
+                                                                                                         'fastkafka/_components/encoder/avro.py'),
+                                                    'fastkafka._components.encoder.avro.avro_encoder': ( 'avro_encode_decoder.html#avro_encoder',
+                                                                                                         'fastkafka/_components/encoder/avro.py'),
+                                                    'fastkafka._components.encoder.avro.avsc_to_pydantic': ( 'avro_encode_decoder.html#avsc_to_pydantic',
+                                                                                                             'fastkafka/_components/encoder/avro.py')},
+            'fastkafka._components.encoder.json': { 'fastkafka._components.encoder.json._to_json_utf8': ( 'json_encode_decoder.html#_to_json_utf8',
+                                                                                                          'fastkafka/_components/encoder/json.py'),
+                                                    'fastkafka._components.encoder.json.json_decoder': ( 'json_encode_decoder.html#json_decoder',
+                                                                                                         'fastkafka/_components/encoder/json.py'),
+                                                    'fastkafka._components.encoder.json.json_encoder': ( 'json_encode_decoder.html#json_encoder',
+                                                                                                         'fastkafka/_components/encoder/json.py')},
             'fastkafka._components.helpers': { 'fastkafka._components.helpers.ImportFromStringError': ( 'internal_helpers.html#importfromstringerror',
                                                                                                         'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers._import_from_string': ( 'internal_helpers.html#_import_from_string',
                                                                                                       'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.change_dir': ( 'internal_helpers.html#change_dir',
                                                                                              'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.in_notebook': ( 'internal_helpers.html#in_notebook',
-                                                                                              'fastkafka/_components/helpers.py')},
-            'fastkafka._components.logger': { 'fastkafka._components.logger.get_default_logger_configuration': ( 'logger.html#get_default_logger_configuration',
+                                                                                              'fastkafka/_components/helpers.py'),
+                                               'fastkafka._components.helpers.true_after': ( 'internal_helpers.html#true_after',
+                                                                                             'fastkafka/_components/helpers.py')},
+            'fastkafka._components.logger': { 'fastkafka._components.logger.cached_log': ( 'logger.html#cached_log',
+                                                                                           'fastkafka/_components/logger.py'),
+                                              'fastkafka._components.logger.get_default_logger_configuration': ( 'logger.html#get_default_logger_configuration',
                                                                                                                  'fastkafka/_components/logger.py'),
                                               'fastkafka._components.logger.get_logger': ( 'logger.html#get_logger',
                                                                                            'fastkafka/_components/logger.py'),
                                               'fastkafka._components.logger.set_level': ( 'logger.html#set_level',
                                                                                           'fastkafka/_components/logger.py'),
                                               'fastkafka._components.logger.supress_timestamps': ( 'logger.html#supress_timestamps',
                                                                                                    'fastkafka/_components/logger.py')},
@@ -231,18 +247,18 @@
                                             'fastkafka._components.meta.test_eq': ('meta.html#test_eq', 'fastkafka/_components/meta.py'),
                                             'fastkafka._components.meta.union2tuple': ( 'meta.html#union2tuple',
                                                                                         'fastkafka/_components/meta.py'),
                                             'fastkafka._components.meta.use_parameters_of': ( 'meta.html#use_parameters_of',
                                                                                               'fastkafka/_components/meta.py')},
             'fastkafka._components.producer_decorator': { 'fastkafka._components.producer_decorator.KafkaEvent': ( 'producerdecorator.html#kafkaevent',
                                                                                                                    'fastkafka/_components/producer_decorator.py'),
-                                                          'fastkafka._components.producer_decorator._to_json_utf8': ( 'producerdecorator.html#_to_json_utf8',
-                                                                                                                      'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator._wrap_in_event': ( 'producerdecorator.html#_wrap_in_event',
                                                                                                                        'fastkafka/_components/producer_decorator.py'),
+                                                          'fastkafka._components.producer_decorator.get_loop': ( 'producerdecorator.html#get_loop',
+                                                                                                                 'fastkafka/_components/producer_decorator.py'),
                                                           'fastkafka._components.producer_decorator.producer_decorator': ( 'producerdecorator.html#producer_decorator',
                                                                                                                            'fastkafka/_components/producer_decorator.py')},
             'fastkafka._components.test_dependencies': { 'fastkafka._components.test_dependencies._install_java': ( 'test_dependencies.html#_install_java',
                                                                                                                     'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies._install_kafka': ( 'test_dependencies.html#_install_kafka',
                                                                                                                      'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies._install_testing_deps': ( 'test_dependencies.html#_install_testing_deps',
@@ -428,11 +444,9 @@
             'fastkafka._testing.test_utils': { 'fastkafka._testing.test_utils.display_docs': ( 'test_utils.html#display_docs',
                                                                                                'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.mock_AIOKafkaProducer_send': ( 'test_utils.html#mock_aiokafkaproducer_send',
                                                                                                              'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.nb_safe_seed': ( 'test_utils.html#nb_safe_seed',
                                                                                                'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.run_script_and_cancel': ( 'test_utils.html#run_script_and_cancel',
-                                                                                                        'fastkafka/_testing/test_utils.py'),
-                                               'fastkafka._testing.test_utils.true_after': ( 'test_utils.html#true_after',
-                                                                                             'fastkafka/_testing/test_utils.py')},
+                                                                                                        'fastkafka/_testing/test_utils.py')},
             'fastkafka.testing': {'fastkafka.testing.dummy': ('testing_export.html#dummy', 'fastkafka/testing.py')}}}
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_server.py` & `fastkafka-0.5.0rc0/fastkafka/_server.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.5.0rc0/fastkafka/_testing/apache_kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.5.0rc0/fastkafka/_testing/in_memory_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,25 @@
 # %% ../../nbs/001_InMemoryBroker.ipynb 1
 import asyncio
 import copy
 import hashlib
 import inspect
 import random
 import string
-
 import uuid
 from collections import namedtuple
 from contextlib import contextmanager
 from dataclasses import dataclass
 from typing import *
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord, RecordMetadata, TopicPartition
 
 import fastkafka._application.app
 import fastkafka._components.aiokafka_consumer_loop
-import fastkafka._components.aiokafka_producer_manager
 from .._components.logger import get_logger
 from fastkafka._components.meta import (
     _get_default_kwargs_from_sig,
     classcontextmanager,
     copy_func,
     delegates,
     patch,
@@ -523,35 +521,26 @@
         logger.info("InMemoryBroker starting")
 
         old_consumer_app = fastkafka._application.app.AIOKafkaConsumer
         old_producer_app = fastkafka._application.app.AIOKafkaProducer
         old_consumer_loop = (
             fastkafka._components.aiokafka_consumer_loop.AIOKafkaConsumer
         )
-        old_producer_manager = (
-            fastkafka._components.aiokafka_producer_manager.AIOKafkaProducer
-        )
 
         fastkafka._application.app.AIOKafkaConsumer = InMemoryConsumer(self)
         fastkafka._application.app.AIOKafkaProducer = InMemoryProducer(self)
         fastkafka._components.aiokafka_consumer_loop.AIOKafkaConsumer = (
             InMemoryConsumer(self)
         )
-        fastkafka._components.aiokafka_producer_manager.AIOKafkaProducer = (
-            InMemoryProducer(self)
-        )
 
         self.is_started = True
         yield self
     finally:
         logger.info("InMemoryBroker stopping")
 
         fastkafka._application.app.AIOKafkaConsumer = old_consumer_app
         fastkafka._application.app.AIOKafkaProducer = old_producer_app
         fastkafka._components.aiokafka_consumer_loop.AIOKafkaConsumer = (
             old_consumer_loop
         )
-        fastkafka._components.aiokafka_producer_manager.AIOKafkaProducer = (
-            old_producer_manager
-        )
 
         self.is_started = False
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.5.0rc0/fastkafka/_testing/local_redpanda_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.4.0rc2/fastkafka/_testing/test_utils.py` & `fastkafka-0.5.0rc0/fastkafka/_testing/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/004_Test_Utils.ipynb.
 
 # %% auto 0
-__all__ = ['logger', 'nb_safe_seed', 'true_after', 'mock_AIOKafkaProducer_send', 'run_script_and_cancel', 'display_docs']
+__all__ = ['logger', 'nb_safe_seed', 'mock_AIOKafkaProducer_send', 'run_script_and_cancel', 'display_docs']
 
 # %% ../../nbs/004_Test_Utils.ipynb 1
 import asyncio
 import hashlib
 import shlex
 import subprocess  # nosec
 import unittest
@@ -42,37 +42,27 @@
 
     def _get_seed(x: int = 0, *, init_seed: int = init_seed) -> int:
         return init_seed + x
 
     return _get_seed
 
 # %% ../../nbs/004_Test_Utils.ipynb 8
-def true_after(seconds: float) -> Callable[[], bool]:
-    """Function returning True after a given number of seconds"""
-    t = datetime.now()
-
-    def _true_after(seconds: float = seconds, t: datetime = t) -> bool:
-        return (datetime.now() - t) > timedelta(seconds=seconds)
-
-    return _true_after
-
-# %% ../../nbs/004_Test_Utils.ipynb 10
 @contextmanager
 def mock_AIOKafkaProducer_send() -> Generator[unittest.mock.Mock, None, None]:
     """Mocks **send** method of **AIOKafkaProducer**"""
     with unittest.mock.patch("__main__.AIOKafkaProducer.send") as mock:
 
         async def _f() -> None:
             pass
 
         mock.return_value = asyncio.create_task(_f())
 
         yield mock
 
-# %% ../../nbs/004_Test_Utils.ipynb 11
+# %% ../../nbs/004_Test_Utils.ipynb 9
 async def run_script_and_cancel(
     script: str,
     *,
     script_file: Optional[str] = None,
     cmd: Optional[str] = None,
     cancel_after: int = 10,
     app_name: str = "app",
@@ -121,15 +111,15 @@
         )
         await asyncio.sleep(cancel_after)
         proc.terminate()
         output, _ = proc.communicate()
 
         return (proc.returncode, output)
 
-# %% ../../nbs/004_Test_Utils.ipynb 16
+# %% ../../nbs/004_Test_Utils.ipynb 14
 async def display_docs(docs_path: str, port: int = 4000) -> None:
     with change_dir(docs_path):
         process = await asyncio.create_subprocess_exec(
             "python3",
             "-m",
             "http.server",
             f"{port}",
```

### Comparing `fastkafka-0.4.0rc2/fastkafka/testing.py` & `fastkafka-0.5.0rc0/fastkafka/testing.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ._testing.in_memory_broker import InMemoryBroker
 from ._testing.local_redpanda_broker import LocalRedpandaBroker
 from fastkafka._testing.test_utils import (
     display_docs,
     mock_AIOKafkaProducer_send,
     nb_safe_seed,
     run_script_and_cancel,
-    true_after,
 )
 
 __all__ = [
     "InMemoryBroker",
     "ApacheKafkaBroker",
     "LocalRedpandaBroker",
     "Tester",
```

### Comparing `fastkafka-0.4.0rc2/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.5.0rc0/fastkafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.4.0rc2
+Version: 0.5.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: avro
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 FastKafka
 ================
@@ -75,15 +76,15 @@
 
 Your support helps us to stay in touch with you and encourages us to
 continue developing and improving the library. Thank you for your
 support!
 
 ------------------------------------------------------------------------
 
-We were busy lately, check it out yourself!
+#### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
 FastKafka works on macOS, Linux, and most Unix-style operating systems.
 You can install base version of `fastkafka` with `pip` as usual:
```

### Comparing `fastkafka-0.4.0rc2/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.5.0rc0/fastkafka.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,21 +21,23 @@
 fastkafka.egg-info/top_level.txt
 fastkafka/_application/__init__.py
 fastkafka/_application/app.py
 fastkafka/_application/tester.py
 fastkafka/_components/__init__.py
 fastkafka/_components/_subprocess.py
 fastkafka/_components/aiokafka_consumer_loop.py
-fastkafka/_components/aiokafka_producer_manager.py
 fastkafka/_components/asyncapi.py
 fastkafka/_components/benchmarking.py
 fastkafka/_components/docs_dependencies.py
 fastkafka/_components/helpers.py
 fastkafka/_components/logger.py
 fastkafka/_components/meta.py
 fastkafka/_components/producer_decorator.py
 fastkafka/_components/test_dependencies.py
+fastkafka/_components/encoder/__init__.py
+fastkafka/_components/encoder/avro.py
+fastkafka/_components/encoder/json.py
 fastkafka/_testing/__init__.py
 fastkafka/_testing/apache_kafka_broker.py
 fastkafka/_testing/in_memory_broker.py
 fastkafka/_testing/local_redpanda_broker.py
 fastkafka/_testing/test_utils.py
```

### Comparing `fastkafka-0.4.0rc2/fastkafka.egg-info/requires.txt` & `fastkafka-0.5.0rc0/fastkafka.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 aiokafka>=0.8.0
 anyio>=3.0
 asyncer>=0.0.2
 docstring-parser>=0.15
+nest-asyncio>=1.5.6
 pydantic>=1.9
 tqdm>=4.62
 typer>=0.7.0
 
+[avro]
+fastavro>=1.7.3
+
 [dev]
 PyYAML>=5.3.1
 aiohttp>=3.8.4
 bandit==1.7.4
 black==23.1.0
 email-validator==1.3.1
+fastavro>=1.7.3
 install-jdk==0.3.0
 ipywidgets<=8.0.4,>=8.0
 isort==5.12.0
 mypy==1.0.1
 nbconvert>=7.2.9
 nbdev-mkdocs==0.3.0
 nbformat>=5.7.3
 nbqa==1.6.3
-nest-asyncio>=1.5.6
 numpy>=1.21.0
 pandas>=1.2.0
 pre-commit==3.0.4
 pytest==7.2.1
 requests>=2.20
 scikit-learn==1.2.1
 semgrep==1.14.0
@@ -32,9 +36,8 @@
 [docs]
 PyYAML>=5.3.1
 aiohttp>=3.8.4
 
 [test]
 install-jdk==0.3.0
 ipywidgets<=8.0.4,>=8.0
-nest-asyncio>=1.5.6
 requests>=2.20
```

### Comparing `fastkafka-0.4.0rc2/settings.ini` & `fastkafka-0.5.0rc0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.4.0rc2
+version = 0.5.0rc0
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.4.0rc2/setup.py` & `fastkafka-0.5.0rc0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,21 @@
     "pydantic>=1.9",
     "anyio>=3.0",
     "aiokafka>=0.8.0",
     "asyncer>=0.0.2",
     "tqdm>=4.62",
     "docstring-parser>=0.15",
     "typer>=0.7.0",
+    "nest-asyncio>=1.5.6",
+]
+avro_requirements = [
+    "fastavro>=1.7.3"
 ]
 test_requirements = [
     "install-jdk==0.3.0",
-    "nest-asyncio>=1.5.6",
     "ipywidgets>=8.0,<=8.0.4",
     "requests>=2.20",
 ]
 docs_requirements = [
     "PyYAML>=5.3.1",
     "aiohttp>=3.8.4"
 ]
@@ -82,15 +85,15 @@
         'Natural Language :: ' + cfg['language'].title(),
     ] + ['Programming Language :: Python :: '+o for o in py_versions[py_versions.index(min_python):]] + (['License :: ' + lic[1] ] if lic[1] else []),
     url = cfg['git_url'],
     project_urls=project_urls,
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
-    extras_require={ 'dev': dev_requirements + test_requirements + docs_requirements, "test": test_requirements, "docs": docs_requirements },
+    extras_require={ 'dev': dev_requirements + avro_requirements + test_requirements + docs_requirements, "avro": avro_requirements, "test": test_requirements, "docs": docs_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
     long_description = open('README.md', encoding="UTF-8").read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     entry_points = {
         'console_scripts': cfg.get('console_scripts','').split(),
```

