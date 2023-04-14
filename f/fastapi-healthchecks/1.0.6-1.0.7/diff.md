# Comparing `tmp/fastapi-healthchecks-1.0.6.tar.gz` & `tmp/fastapi_healthchecks-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-healthchecks-1.0.6.tar", max compression
+gzip compressed data, was "fastapi_healthchecks-1.0.7.tar", max compression
```

## Comparing `fastapi-healthchecks-1.0.6.tar` & `fastapi_healthchecks-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1075 2022-11-22 13:08:47.299887 fastapi-healthchecks-1.0.6/LICENSE
--rw-r--r--   0        0        0     1485 2022-11-22 13:08:47.299887 fastapi-healthchecks-1.0.6/README.md
--rw-r--r--   0        0        0        0 2022-11-22 13:08:47.299887 fastapi-healthchecks-1.0.6/fastapi_healthchecks/__init__.py
--rw-r--r--   0        0        0        0 2022-07-29 11:17:32.635406 fastapi-healthchecks-1.0.6/fastapi_healthchecks/api/__init__.py
--rw-r--r--   0        0        0      170 2022-07-29 11:17:32.636406 fastapi-healthchecks-1.0.6/fastapi_healthchecks/api/models.py
--rw-r--r--   0        0        0     1877 2022-11-22 13:08:47.300887 fastapi-healthchecks-1.0.6/fastapi_healthchecks/api/router.py
--rw-r--r--   0        0        0       85 2022-07-25 11:11:01.832911 fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/__init__.py
--rw-r--r--   0        0        0      259 2022-07-25 11:11:01.832911 fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/_base.py
--rw-r--r--   0        0        0     2217 2022-11-22 13:08:47.300887 fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/ceph.py
--rw-r--r--   0        0        0     1967 2022-07-29 11:17:32.636406 fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/http.py
--rw-r--r--   0        0        0     2467 2022-07-29 11:17:32.636406 fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/postgres.py
--rw-r--r--   0        0        0     1712 2022-07-29 11:17:32.636406 fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/rabbit_mq.py
--rw-r--r--   0        0        0     2162 2022-07-25 11:11:01.832911 fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/redis.py
--rw-r--r--   0        0        0     1174 2022-07-25 11:11:01.833911 fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/settings.py
--rw-r--r--   0        0        0     2326 2022-11-22 13:08:47.301887 fastapi-healthchecks-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     2572 2022-11-22 13:08:49.034265 fastapi-healthchecks-1.0.6/setup.py
--rw-r--r--   0        0        0     2414 2022-11-22 13:08:49.034578 fastapi-healthchecks-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-11-21 12:11:10.745541 fastapi_healthchecks-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1485 2022-09-08 06:17:52.184411 fastapi_healthchecks-1.0.7/README.md
+-rw-r--r--   0        0        0        0 2022-07-29 15:29:34.146823 fastapi_healthchecks-1.0.7/fastapi_healthchecks/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-26 09:14:56.017837 fastapi_healthchecks-1.0.7/fastapi_healthchecks/api/__init__.py
+-rw-r--r--   0        0        0      170 2022-07-26 09:14:56.017837 fastapi_healthchecks-1.0.7/fastapi_healthchecks/api/models.py
+-rw-r--r--   0        0        0     1877 2022-08-02 10:46:11.292528 fastapi_healthchecks-1.0.7/fastapi_healthchecks/api/router.py
+-rw-r--r--   0        0        0       85 2022-07-25 09:06:52.373979 fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/__init__.py
+-rw-r--r--   0        0        0      259 2022-07-25 09:06:52.373979 fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/_base.py
+-rw-r--r--   0        0        0     2217 2022-11-21 14:10:04.882952 fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/ceph.py
+-rw-r--r--   0        0        0     1967 2022-07-26 08:57:32.364953 fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/http.py
+-rw-r--r--   0        0        0     2467 2022-07-25 16:28:06.246097 fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/postgres.py
+-rw-r--r--   0        0        0     1728 2023-04-14 07:38:17.734138 fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/rabbit_mq.py
+-rw-r--r--   0        0        0     2162 2022-07-25 09:53:22.724534 fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/redis.py
+-rw-r--r--   0        0        0     1174 2022-07-25 09:06:52.374979 fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/settings.py
+-rw-r--r--   0        0        0     2326 2023-04-14 07:38:17.734138 fastapi_healthchecks-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2580 1970-01-01 00:00:00.000000 fastapi_healthchecks-1.0.7/setup.py
+-rw-r--r--   0        0        0     2465 1970-01-01 00:00:00.000000 fastapi_healthchecks-1.0.7/PKG-INFO
```

### Comparing `fastapi-healthchecks-1.0.6/LICENSE` & `fastapi_healthchecks-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-healthchecks-1.0.6/README.md` & `fastapi_healthchecks-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-healthchecks-1.0.6/fastapi_healthchecks/api/router.py` & `fastapi_healthchecks-1.0.7/fastapi_healthchecks/api/router.py`

 * *Files identical despite different names*

### Comparing `fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/ceph.py` & `fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/ceph.py`

 * *Files identical despite different names*

### Comparing `fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/http.py` & `fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/http.py`

 * *Files identical despite different names*

### Comparing `fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/postgres.py` & `fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/postgres.py`

 * *Files identical despite different names*

### Comparing `fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/rabbit_mq.py` & `fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/rabbit_mq.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,17 +46,17 @@
             secure=ampq_url.scheme == "amqps",
             timeout=timeout,
             name=name,
         )
 
     async def __call__(self) -> CheckResult:
         try:
-            await aio_pika.connect_robust(
+            async with await aio_pika.connect_robust(
                 host=self._host,
                 port=self._port,
                 login=self._user,
                 password=self._password,
                 ssl=self._secure,
-            )
-            return CheckResult(name=self._name, passed=True)
+            ):
+                return CheckResult(name=self._name, passed=True)
         except Exception as exception:
             return CheckResult(name=self._name, passed=False, details=str(exception))
```

### Comparing `fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/redis.py` & `fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-healthchecks-1.0.6/fastapi_healthchecks/checks/settings.py` & `fastapi_healthchecks-1.0.7/fastapi_healthchecks/checks/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi-healthchecks-1.0.6/pyproject.toml` & `fastapi_healthchecks-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-healthchecks"
-version = "1.0.6"
+version = "1.0.7"
 authors = ["RockITSoft", "Victor Tsykanov", "Andrey Malchuk", "Mikhail Pachurin"]
 description = "FastAPI Healthchecks"
 keywords = ["fastapi", "healthcheck"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `fastapi-healthchecks-1.0.6/setup.py` & `fastapi_healthchecks-1.0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,22 +22,22 @@
  'http': ['aiohttp[speedups]>=3,<4'],
  'postgres': ['asyncpg>=0.25.0'],
  'rabbitmq': ['aio-pika>=7'],
  'redis': ['redis>=4,<5']}
 
 setup_kwargs = {
     'name': 'fastapi-healthchecks',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'FastAPI Healthchecks',
     'long_description': '# FastAPI health checks\n\nConfigurable health checks endpoints for FastAPI applications.\n\n## Quickstart\n\n```python\napp = FastAPI()\napp.include_router(\n    HealthcheckRouter(\n        Probe(\n            name="readiness",\n            checks=[\n                PostgreSqlCheck(host="db.example.com", username=..., password=...),\n                RedisCheck(host="redis.example.com", username=..., password=...),\n            ],\n        ),\n        Probe(\n            name="liveness",\n            checks=[\n                ...,\n            ],\n        ),\n    ),\n    prefix="/health",\n)\n```\n\nThe probes from this example will be available as `GET /health/readiness` and `GET /health/liveness`.\n\n## Bundled checks\n\n* `PostgreSqlCheck` – checks PostgreSQL server availability\n* `RedisCheck` – checks Redis server availability\n* `RabbitMqCheck` – checks RabbitMQ server availability\n* `SettingsCheck` – validates settings models based on pydantic BaseModel\n* `HttpCheck` – checks availability of specified URL\n* `CephCheck` – checks Ceph server availability\n\n## Custom checks\n\nYou can create your own checks by providing custom `fastapi_healthchecks.checks.Check` implementations. Like this:\n\n```python\nclass MaintenanceCheck(Check):\n    async def __call__(self) -> CheckResult:\n        if is_maintenance():\n            return CheckResult(name="Maintenance", passed=False, details="Closed for maintenance")\n        else:\n            return CheckResult(name="Maintenance", passed=True)\n```\n',
     'author': 'RockITSoft',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `fastapi-healthchecks-1.0.6/PKG-INFO` & `fastapi_healthchecks-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: fastapi-healthchecks
-Version: 1.0.6
+Version: 1.0.7
 Summary: FastAPI Healthchecks
 License: MIT
 Keywords: fastapi,healthcheck
 Author: RockITSoft
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: ceph
 Provides-Extra: http
 Provides-Extra: postgres
 Provides-Extra: rabbitmq
 Provides-Extra: redis
 Requires-Dist: aio-pika (>=7); extra == "all" or extra == "rabbitmq"
```

