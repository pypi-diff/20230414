# Comparing `tmp/django-outbox-pattern-0.8.0.tar.gz` & `tmp/django-outbox-pattern-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-outbox-pattern-0.8.0.tar", max compression
+gzip compressed data, was "django-outbox-pattern-0.9.0.tar", max compression
```

## Comparing `django-outbox-pattern-0.8.0.tar` & `django-outbox-pattern-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1071 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/LICENSE
--rw-r--r--   0        0        0     9339 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/README.md
--rw-r--r--   0        0        0       22 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/__init__.py
--rw-r--r--   0        0        0      367 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/admin.py
--rw-r--r--   0        0        0      159 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/apps.py
--rw-r--r--   0        0        0     1354 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/bases.py
--rw-r--r--   0        0        0      125 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/choices.py
--rw-r--r--   0        0        0     4133 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/consumers.py
--rw-r--r--   0        0        0     1389 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/decorators.py
--rw-r--r--   0        0        0      244 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/exceptions.py
--rw-r--r--   0        0        0     1637 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/factories.py
--rw-r--r--   0        0        0      258 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/headers.py
--rw-r--r--   0        0        0     1608 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/listeners.py
--rw-r--r--   0        0        0        0 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/management/__init__.py
--rw-r--r--   0        0        0        0 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/management/commands/__init__.py
--rw-r--r--   0        0        0      552 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/management/commands/base.py
--rw-r--r--   0        0        0     2070 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/management/commands/publish.py
--rw-r--r--   0        0        0     1576 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/management/commands/subscribe.py
--rw-r--r--   0        0        0     2560 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/migrations/0001_initial.py
--rw-r--r--   0        0        0      459 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/migrations/0002_received_msg_id.py
--rw-r--r--   0        0        0        0 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/migrations/__init__.py
--rw-r--r--   0        0        0     2043 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/models.py
--rw-r--r--   0        0        0      396 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/payloads.py
--rw-r--r--   0        0        0     2361 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/producers.py
--rw-r--r--   0        0        0     4483 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/django_outbox_pattern/settings.py
--rw-r--r--   0        0        0     2000 2022-08-17 20:57:23.557470 django-outbox-pattern-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    10562 2022-08-17 20:57:41.165989 django-outbox-pattern-0.8.0/setup.py
--rw-r--r--   0        0        0    10729 2022-08-17 20:57:41.166668 django-outbox-pattern-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9339 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/__init__.py
+-rw-r--r--   0        0        0      367 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/admin.py
+-rw-r--r--   0        0        0      159 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/apps.py
+-rw-r--r--   0        0        0     1438 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/bases.py
+-rw-r--r--   0        0        0      125 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/choices.py
+-rw-r--r--   0        0        0     4111 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/consumers.py
+-rw-r--r--   0        0        0     1389 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/decorators.py
+-rw-r--r--   0        0        0      244 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/exceptions.py
+-rw-r--r--   0        0        0     1637 2022-09-10 08:30:38.003254 django-outbox-pattern-0.9.0/django_outbox_pattern/factories.py
+-rw-r--r--   0        0        0      274 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/headers.py
+-rw-r--r--   0        0        0     1608 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/listeners.py
+-rw-r--r--   0        0        0        0 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/management/commands/__init__.py
+-rw-r--r--   0        0        0      552 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/management/commands/base.py
+-rw-r--r--   0        0        0     2070 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/management/commands/publish.py
+-rw-r--r--   0        0        0     1576 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/management/commands/subscribe.py
+-rw-r--r--   0        0        0     2560 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/migrations/0001_initial.py
+-rw-r--r--   0        0        0      459 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/migrations/0002_received_msg_id.py
+-rw-r--r--   0        0        0        0 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/migrations/__init__.py
+-rw-r--r--   0        0        0     2043 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/models.py
+-rw-r--r--   0        0        0      396 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/payloads.py
+-rw-r--r--   0        0        0     2753 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/producers.py
+-rw-r--r--   0        0        0     4483 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/django_outbox_pattern/settings.py
+-rw-r--r--   0        0        0     2000 2022-09-10 08:30:38.007254 django-outbox-pattern-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10562 2022-09-10 08:31:03.110756 django-outbox-pattern-0.9.0/setup.py
+-rw-r--r--   0        0        0    10729 2022-09-10 08:31:03.111552 django-outbox-pattern-0.9.0/PKG-INFO
```

### Comparing `django-outbox-pattern-0.8.0/LICENSE` & `django-outbox-pattern-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/README.md` & `django-outbox-pattern-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/bases.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/bases.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
     def get_listener(self, name):
         return self.connection.get_listener(name)
 
     def set_listener(self, name, listener):
         self.connection.set_listener(name, listener)
 
+    def remove_listener(self, name):
+        self.connection.remove_listener(name)
+
     def _disconnect(self):
         self.connection.disconnect()
 
     def _exponential_backoff(self):
         return min(2**self.attempts + random.uniform(0, 1), settings.DEFAULT_MAXIMUM_BACKOFF)
 
     def _wait(self):
```

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/consumers.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/consumers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 
 logger = logging.getLogger("django_outbox_pattern")
 
 
 def _get_msg_id(headers):
     ret = None
     for key, value in headers.items():
-        if "msg-id" in key:
+        if key.endswith("-id"):
             ret = value
     return ret
 
 
 class Consumer(Base):
     listener_class = settings.DEFAULT_CONSUMER_LISTENER_CLASS
     received_class = settings.DEFAULT_RECEIVED_CLASS
     subscribe_headers = settings.DEFAULT_STOMP_QUEUE_HEADERS
 
     def __init__(self, connection, username, passcode):
         super().__init__(connection, username, passcode)
         self.callback = lambda p: p
         self.destination = None
         self.queue_name = None
-        self.is_stopped = False
         self.subscribe_id = None
-        self.set_listener(f"consumer-listener-{get_uuid()}", self.listener_class(self))
+        self.listener_name = f"consumer-listener-{get_uuid()}"
+        self.set_listener(self.listener_name, self.listener_class(self))
 
     def message_handler(self, body, headers):
         body = json.loads(body)
         payload = Payload(self.connection, body, headers)
         received, created = self.received_class.objects.get_or_create(msg_id=_get_msg_id(headers))
         if created:
             received.body = body
@@ -52,28 +52,27 @@
                 payload.ack()
             finally:
                 received.save()
         else:
             payload.ack()
 
     def start(self, callback, destination, queue_name=None):
-        if not self.is_stopped:
-            self.connect()
-            self.callback = callback
-            self.destination = destination
-            self.queue_name = queue_name
-            self._create_dlq_queue(destination, self.subscribe_headers, queue_name)
-            self._create_queue(destination, self.subscribe_headers, queue_name)
-            logger.info("Consumer started with id: %s", self.subscribe_id)
+        self.connect()
+        self.callback = callback
+        self.destination = destination
+        self.queue_name = queue_name
+        self._create_dlq_queue(destination, self.subscribe_headers, queue_name)
+        self._create_queue(destination, self.subscribe_headers, queue_name)
+        logger.info("Consumer started with id: %s", self.subscribe_id)
 
     def stop(self):
         if self.subscribe_id and self.is_connected():
             self._unsubscribe()
+            self.remove_listener(self.listener_name)
             self._disconnect()
-            self.is_stopped = True
         else:
             logger.info("Consumer not started")
 
     def _create_dlq_queue(self, destination, headers, queue_name=None):
         if not self.subscribe_id:
             subscribe_id = get_uuid()
             self._subscribe(destination, subscribe_id, headers, queue_name, dlq=True)
```

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/decorators.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/decorators.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/factories.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/factories.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/listeners.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/listeners.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/management/commands/base.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/management/commands/base.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/management/commands/publish.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/management/commands/publish.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/management/commands/subscribe.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/management/commands/subscribe.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/migrations/0001_initial.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/models.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/models.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/producers.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/producers.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,39 +15,53 @@
 
 class Producer(Base):
     settings = settings
     listener_class = settings.DEFAULT_PRODUCER_LISTENER_CLASS
 
     def __init__(self, connection, username, passcode):
         super().__init__(connection, username, passcode)
-        self.is_stopped = False
-        self.set_listener(f"producer-listener-{get_uuid()}", self.listener_class(self))
+        self.listener_name = f"producer-listener-{get_uuid()}"
+        self.set_listener(self.listener_name, self.listener_class(self))
+
+    def __enter__(self):
+        self.start()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.stop()
 
     def start(self):
-        if not self.is_stopped:
-            self.connect()
+        self.connect()
 
     def stop(self):
         if self.is_connected():
+            self.remove_listener(self.listener_name)
             self._disconnect()
-            self.is_stopped = True
         else:
             logger.info("Producer not started")
 
     def send(self, message, **kwargs):
         generate_headers = self.settings.DEFAULT_GENERATE_HEADERS
         headers = generate_headers(message)
         kwargs = {
             "body": json.dumps(message.body, cls=DjangoJSONEncoder),
             "destination": message.destination,
             "headers": headers,
             **kwargs,
         }
         return self._send_with_retry(**kwargs)
 
+    def send_event(self, body, destination, **kwargs):
+        kwargs = {
+            "body": json.dumps(body, cls=DjangoJSONEncoder),
+            "destination": destination,
+            **kwargs,
+        }
+        return self._send_with_retry(**kwargs)
+
     def _send_with_retry(self, **kwargs):
         """
         During the message sending process, when the broker crashes or the connection fails or an abnormality occurs,
         will retry the sending. Retry 3 times for the first time, retry every minute after 4 minutes.
         When the total number of retries reaches 50 (DEFAULT_MAXIMUM_RETRY_ATTEMPTS), will stop retrying.
         """
```

### Comparing `django-outbox-pattern-0.8.0/django_outbox_pattern/settings.py` & `django-outbox-pattern-0.9.0/django_outbox_pattern/settings.py`

 * *Files identical despite different names*

### Comparing `django-outbox-pattern-0.8.0/pyproject.toml` & `django-outbox-pattern-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-outbox-pattern"
-version = "0.8.0"
+version = "0.9.0"
 description = "A django application to make it easier to use the transactional outbox pattern"
 license = "MIT"
 authors = ["Hugo Brilhante <hugobrilhante@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/juntossomosmais/django-outbox-pattern"
 repository = "https://github.com/juntossomosmais/django-outbox-pattern"
 documentation = "https://github.com/juntossomosmais/django-outbox-pattern"
```

### Comparing `django-outbox-pattern-0.8.0/setup.py` & `django-outbox-pattern-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['django>=3.2', 'stomp.py>=8.0.1,<9']
 
 setup_kwargs = {
     'name': 'django-outbox-pattern',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'A django application to make it easier to use the transactional outbox pattern',
     'long_description': '# Django outbox pattern\n\n[![Build Status](https://dev.azure.com/juntos-somos-mais-loyalty/python/_apis/build/status/juntossomosmais.django-outbox-pattern?branchName=main)](https://dev.azure.com/juntos-somos-mais-loyalty/python/_build/latest?definitionId=307&branchName=main)\n[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=juntossomosmais_django-outbox-pattern&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=juntossomosmais_django-outbox-pattern)\n[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=juntossomosmais_django-outbox-pattern&metric=coverage)](https://sonarcloud.io/summary/new_code?id=juntossomosmais_django-outbox-pattern)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/ambv/black)\n[![Downloads](https://pepy.tech/badge/django-outbox-pattern)](https://pepy.tech/project/django-outbox-pattern)\n[![Downloads](https://pepy.tech/badge/django-outbox-pattern/month)](https://pepy.tech/project/django-outbox-pattern/month)\n[![Downloads](https://pepy.tech/badge/django-outbox-pattern/week)](https://pepy.tech/project/django-outbox-pattern/week)\n[![PyPI version](https://badge.fury.io/py/django-outbox-pattern.svg)](https://badge.fury.io/py/django-outbox-pattern)\n[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/juntossomosmais/django-outbox-pattern/blob/master/LICENSE)\n\nA django application to make it easier to use\nthe [transactional outbox pattern](https://microservices.io/patterns/data/transactional-outbox.html)\n\n## Installation\n\nInstall django-outbox-pattern with pip\n\n```bash\npip install django-outbox-pattern\n```\n\nAdd to settings\n\n```python\n# settings.py\n\nINSTALLED_APPS = [\n    "django_outbox_pattern",\n]\n\nDJANGO_OUTBOX_PATTERN = {\n    "DEFAULT_STOMP_HOST_AND_PORTS": [("127.0.0.1", 61613)],\n    "DEFAULT_STOMP_USERNAME": "guest",\n    "DEFAULT_STOMP_PASSCODE": "guest",\n}\n\n```\n\nRum migrations\n\n```shell\npython manage.py migrate\n```\n\n## Usage/Examples\n\nThe `publish` decorator adds the outbox table to the model. `\npublish` accepts list of Config. The Config accepts four params the `destination` which is required,\n`fields` which the default are all the fields of the model, `serializer` which by default adds the `id` in the message\nto be sent and `version` which by default is `v1`.\n\n> Note: `fields` and `serializer` are mutually exclusive, serializer overwrites the fields.\n\n### The Config typing\n\n```python\nfrom typing import List\nfrom typing import NamedTuple\nfrom typing import Optional\n\nclass Config(NamedTuple):\n    destination: str\n    fields: Optional[List[str]] = None\n    serializer: Optional[str] = None\n    version: Optional[str] = "v1"\n```\n\n_**Only destination in config**_\n\n```python\nfrom django.db import models\nfrom django_outbox_pattern.decorators import Config\nfrom django_outbox_pattern.decorators import publish\n\n\n@publish([Config(destination=\'/topic/my_route_key\')])\nclass MyModel(models.Model):\n    field_one = models.CharField(max_length=100)\n    field_two = models.CharField(max_length=100)\n```\n\nThis generates the following data to be sent.\n\n```text\nproducer.send(destination=\'/topic/my_route_key.v1\', body=\'{"id": 1, "field_one": "Field One", "field_two": "Field Two"}\')\n```\n\n_**With destinations and fields**_\n\n```python\nfrom django.db import models\nfrom django_outbox_pattern.decorators import Config\nfrom django_outbox_pattern.decorators import publish\n\n\n@publish([Config(destination=\'/topic/my_route_key\', fields=["field_one"])])\nclass MyModel(models.Model):\n    field_one = models.CharField(max_length=100)\n    field_two = models.CharField(max_length=100)\n```\n\nThis generates the following data to be sent.\n\n```text\nproducer.send(destination=\'/topic/my_route_key.v1\', body=\'{"id": 1, "field_one": "Field One"}\')\n```\n\n_**With destinations and serializer**_\n\n```python\nfrom django.db import models\nfrom django_outbox_pattern.decorators import Config\nfrom django_outbox_pattern.decorators import publish\n\n\n@publish([Config(destination=\'/topic/my_route_key\', serializer=\'my_serializer\')])\nclass MyModel(models.Model):\n    field_one = models.CharField(max_length=100)\n    field_two = models.CharField(max_length=100)\n\n    def my_serializer(self):\n        return {\n            "id": self.id,\n            "one": self.field_one,\n            "two": self.field_two\n        }\n```\n\nThis generates the following data to be sent.\n\n```text\nproducer.send(destination=\'/topic/my_route_key.v1\', body=\'{"id": 1, "one": "Field One", "two": "Field Two"}\')\n```\n\n_**With multi destinations and serializers**_\n\n```python\nfrom django.db import models\nfrom django_outbox_pattern.decorators import Config\nfrom django_outbox_pattern.decorators import publish\n\n\n@publish([\n    Config(destination=\'/topic/my_route_key_1\', serializer="my_serializer_1"),\n    Config(destination=\'/topic/my_route_key_2\', serializer="my_serializer_2"),\n])\nclass MyModel(models.Model):\n    field_one = models.CharField(max_length=100)\n    field_two = models.CharField(max_length=100)\n\n    def my_serializer_1(self):\n        return {\n            "id": self.id,\n            "one": self.field_one,\n        }\n\n    def my_serializer_2(self):\n        return {\n            "id": self.id,\n            "two": self.field_two\n        }\n```\n\nThis generates the following data to be sent.\n\n```text\nproducer.send(destination=\'/topic/my_route_key_1.v1\', body=\'{"id": 1, "one": "Field One"}\')\nproducer.send(destination=\'/topic/my_route_key_2.v1\', body=\'{"id": 1, "two": "Field Two"}\')\n```\n\n## Publish/Subscribe commands\n\n##### Publish command\n\nTo send the messages added to the outbox table it is necessary to start the producer with the following command.\n\n```shell\npython manage.py publish\n```\n\n##### Subscribe command\n\nDjango outbox pattern also provides a consumer that can be used to receive outgoing messages.\n\nCreate a function that receives an instance of `django_outbox_pattern.payloads.Payload`\n\n```python\n# callbacks.py\n\ndef callback(payload):\n    try:\n        # Do anything\n        payload.ack()\n    except Exception:\n        # Nack is automatically called in case of errors, but you might want to handle the error in another way\n        payload.nack()\n```\n\nTo start the consumer, after creating the callback, it is necessary to execute the following command.\n\n```shell\npython manage.py subscribe \'dotted.path.to.callback` \'destination\' \'queue_name\'\n```\nThe command takes three parameters:\n\n`callback` : the path to the callback function.\n\n`destination` : the destination where messages will be consumed following one of the [stomp](https://www.rabbitmq.com/stomp.html) patterns\n\n`queue_name`(optional): the name of the queue that will be consumed. If not provided, the routing_key of the destination will be used.\n\n## Settings\n\n**DEFAULT_CONNECTION_CLASS**\n\nThe stomp.py class responsible for connecting to the broker. Default: `stomp.StompConnection12`\n\n**DEFAULT_CONSUMER_LISTENER_CLASS**\n\nThe consumer listener class. Default: `django_outbox_pattern.listeners.ConsumerListener`\n\n**DEFAULT_GENERATE_HEADERS**\n\nA function to add headers to the message. Default: `django_outbox_pattern.headers.generate_headers`\n\n**DEFAULT_MAXIMUM_BACKOFF**:\n\nMaximum wait time for connection attempts in seconds. Default: `3600` (1 hour)\n\n**DEFAULT_MAXIMUM_RETRY_ATTEMPTS**\n\nMaximum number of message resend attempts. Default: `50`\n\n**DEFAULT_PAUSE_FOR_RETRY**\n\nPausing for attempts to resend messages in seconds. Defualt: `240` (4 minutes)\n\n**DEFAULT_WAIT_RETRY**\n\nTime between attempts to send messages after the pause. Default: `60` (1 minute)\n\n**DEFAULT_PRODUCER_LISTENER_CLASS**:\n\nThe producer listener class. Default: `django_outbox_pattern.listeners.ProducerListener`\n\n**DEFAULT_STOMP_HOST_AND_PORTS**\n\nList of host and port tuples to try to connect to the broker. Default `[("127.0.0.1", 61613)]`\n\n**DEFAULT_STOMP_QUEUE_HEADERS**\n\nHeaders for queues. Default: `{"durable": "true", "auto-delete": "false", "prefetch-count": "1"}`\n\n**DEFAULT_STOMP_HEARTBEATS**\n\nTime tuples for input and output heartbeats. Default:  `(10000, 10000)`\n\n**DEFAULT_STOMP_VHOST**\n\nVirtual host. Default: "/"\n\n**DEFAULT_STOMP_USERNAME**\n\nUsername for connection. Default: `"guest"`\n\n**DEFAULT_STOMP_PASSCODE**\n\nPassword for connection. Default: `"guest"`\n\n**DEFAULT_STOMP_USE_SSL**\n\nFor ssl connections. Default: False\n\n**DEFAULT_STOMP_KEY_FILE**\n\nThe path to a X509 key file. Default: None\n\n**DEFAULT_STOMP_CERT_FILE**\n\nThe path to a X509 certificate. Default: None\n\n\n**DEFAULT_STOMP_CA_CERTS**\n\nThe path to the a file containing CA certificates to validate the server against.\nIf this is not set, server side certificate validation is not done. Default: None\n\n**DEFAULT_STOMP_CERT_VALIDATOR**\n\nFunction which performs extra validation on the client certificate, for example\nchecking the returned certificate has a commonName attribute equal to the\nhostname (to avoid man in the middle attacks).\nThe signature is: (OK, err_msg) = validation_function(cert, hostname)\nwhere OK is a boolean, and cert is a certificate structure\nas returned by ssl.SSLSocket.getpeercert(). Default: None\n\n**DEFAULT_STOMP_SSL_VERSION**\n\nSSL protocol to use for the connection. This should be one of the PROTOCOL_x\nconstants provided by the ssl module. The default is ssl.PROTOCOL_TLSv1.\n\n**DEFAULT_STOMP_SSL_PASSWORD**\n\nSSL password\n',
     'author': 'Hugo Brilhante',
     'author_email': 'hugobrilhante@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/juntossomosmais/django-outbox-pattern',
```

### Comparing `django-outbox-pattern-0.8.0/PKG-INFO` & `django-outbox-pattern-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-outbox-pattern
-Version: 0.8.0
+Version: 0.9.0
 Summary: A django application to make it easier to use the transactional outbox pattern
 Home-page: https://github.com/juntossomosmais/django-outbox-pattern
 License: MIT
 Keywords: transactional outbox patterns,application events,microservices
 Author: Hugo Brilhante
 Author-email: hugobrilhante@gmail.com
 Requires-Python: >=3.7,<4.0
```

