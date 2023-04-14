# Comparing `tmp/zimran-events-0.2.2.tar.gz` & `tmp/zimran-events-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.2.2.tar", last modified: Tue Apr 11 18:07:34 2023, max compression
+gzip compressed data, was "zimran-events-0.2.3.tar", last modified: Fri Apr 14 10:04:05 2023, max compression
```

## Comparing `zimran-events-0.2.2.tar` & `zimran-events-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.635647 zimran-events-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 18:07:26.000000 zimran-events-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 18:07:34.639647 zimran-events-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 18:07:26.000000 zimran-events-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 18:07:26.000000 zimran-events-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 18:07:26.000000 zimran-events-0.2.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:07:34.639647 zimran-events-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.635647 zimran-events-0.2.2/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.745556 zimran-events-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-14 10:03:56.000000 zimran-events-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 10:03:56.000000 zimran-events-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-14 10:04:05.757557 zimran-events-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-14 10:03:56.000000 zimran-events-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-14 10:03:56.000000 zimran-events-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 10:03:56.000000 zimran-events-0.2.3/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 10:04:05.757557 zimran-events-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.745556 zimran-events-0.2.3/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 10:03:56.000000 zimran-events-0.2.3/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:04:05.757557 zimran-events-0.2.3/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 10:04:05.000000 zimran-events-0.2.3/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.2.2/.github/scripts/release.py` & `zimran-events-0.2.3/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.2/.gitignore` & `zimran-events-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.2/.pre-commit-config.yaml` & `zimran-events-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.2/LICENSE` & `zimran-events-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.2/PKG-INFO` & `zimran-events-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.2
+Version: 0.2.3
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.2/README.md` & `zimran-events-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.2/pyproject.toml` & `zimran-events-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.2.2/zimran/events/connection.py` & `zimran-events-0.2.3/zimran/events/connection.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.2/zimran/events/consumer.py` & `zimran-events-0.2.3/zimran/events/consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
 
 from zimran.events.connection import AsyncConnection, Connection
-from zimran.events.constants import UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
+from zimran.events.constants import DEAD_LETTER_EXCHANGE_NAME, UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
 from zimran.events.schemas import ExchangeScheme
 from zimran.events.utils import cleanup_and_normalize_queue_name, retry_policy, validate_exchange
 
 
 class ConsumerMixin:
     def handle_event(self, name: str, *, exchange: ExchangeScheme | None = None):
         if exchange is not None:
@@ -61,15 +61,21 @@
             self.channel.basic_qos(prefetch_count=self._prefetch_count)
 
             self._declare_unroutable_exchange()
 
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
                 queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
-                self.channel.queue_declare(queue_name, durable=True)
+                self.channel.queue_declare(
+                    queue_name,
+                    durable=True,
+                    arguments={
+                        'x-dead-letter-exchange': DEAD_LETTER_EXCHANGE_NAME,
+                    },
+                )
 
                 if exchange := data['exchange']:
                     self.channel.exchange_declare(
                         exchange=exchange.name,
                         exchange_type=exchange.type,
                         **exchange.as_dict(exclude=['name', 'type', 'timeout']),
                     )
@@ -117,15 +123,21 @@
             channel = await self.channel
             tasks = [self._declare_unroutable_queue(channel), channel.set_qos(prefetch_count=self._prefetch_count)]
             await asyncio.gather(*tasks)
 
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
                 queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
-                queue = await channel.declare_queue(queue_name, durable=True)
+                queue = await channel.declare_queue(
+                    queue_name,
+                    durable=True,
+                    arguments={
+                        'x-dead-letter-exchange': DEAD_LETTER_EXCHANGE_NAME,
+                    },
+                )
                 if _exchange := data['exchange']:
                     exchange = await channel.declare_exchange(**_exchange.as_dict(exclude_none=True))
                     await queue.bind(exchange=exchange, routing_key=event_name)
 
                 await queue.consume(data['handler'])
 
                 logger.info(f'Registering consumer | queue: {queue_name} | routing_key: {event_name}')
```

### Comparing `zimran-events-0.2.2/zimran/events/producer.py` & `zimran-events-0.2.3/zimran/events/producer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 
 import aio_pika
+import pika
 from aioretry import retry
 
 
 try:
     from loguru import logger
 except ImportError:
     import logging
@@ -24,30 +25,41 @@
 
     def publish(self, routing_key: str, *, payload: dict, context: ContextScheme | None = None):
         if context is None:
             context = ContextScheme()
         else:
             validate_context(context)
 
+        properties = pika.BasicProperties(
+            content_type='application/json',
+            delivery_mode=pika.DeliveryMode.Persistent,
+            correlation_id=context.correlation_id,
+            headers=context.headers,
+        )
         body = json.dumps(payload, default=str)
         if context.exchange is None:
-            self.channel.basic_publish(exchange='', routing_key=routing_key, body=body)
+            self.channel.basic_publish(exchange='', routing_key=routing_key, body=body, properties=properties)
             logger.info(f'Message published to basic exchange | routing_key: {routing_key}')
             return
 
         self._declare_unroutable_queue()
 
         validate_exchange(context.exchange)
         self.channel.exchange_declare(
             exchange=context.exchange.name,
             exchange_type=context.exchange.type,
             **context.exchange.as_dict(exclude=['name', 'type', 'timeout'], exclude_none=True),
         )
 
-        self.channel.basic_publish(exchange=context.exchange.name, routing_key=routing_key, body=body)
+        self.channel.basic_publish(
+            exchange=context.exchange.name,
+            routing_key=routing_key,
+            body=body,
+            properties=properties,
+        )
         logger.info(f'Message published to {context.exchange.name} exchange | routing_key: {routing_key}')
 
     def _declare_unroutable_queue(self):
         self.channel.exchange_declare(exchange=UNROUTABLE_EXCHANGE_NAME, exchange_type='fanout', durable=True)
         self.channel.queue_declare(queue=UNROUTABLE_QUEUE_NAME, durable=True)
         self.channel.queue_bind(queue=UNROUTABLE_QUEUE_NAME, exchange=UNROUTABLE_EXCHANGE_NAME, routing_key='')
 
@@ -81,13 +93,14 @@
     @staticmethod
     def _get_message(context: ContextScheme, payload: dict):
         return aio_pika.Message(
             body=json.dumps(payload, default=str).encode(),
             headers=context.headers,
             content_type='application/json',
             correlation_id=context.correlation_id,
+            delivery_mode=aio_pika.DeliveryMode.PERSISTENT,
         )
 
     async def _declare_unroutable_queue(self, channel: aio_pika.abc.AbstractRobustChannel):
         exchange = await channel.declare_exchange(name=UNROUTABLE_EXCHANGE_NAME, type='fanout', durable=True)
         queue = await channel.declare_queue(name=UNROUTABLE_QUEUE_NAME, durable=True)
         await queue.bind(exchange=exchange, routing_key='')
```

### Comparing `zimran-events-0.2.2/zimran/events/schemas.py` & `zimran-events-0.2.3/zimran/events/schemas.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.2/zimran/events/utils.py` & `zimran-events-0.2.3/zimran/events/utils.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.2/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.2.3/zimran_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.2
+Version: 0.2.3
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.2/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.2.3/zimran_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

