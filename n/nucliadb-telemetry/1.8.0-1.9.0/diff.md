# Comparing `tmp/nucliadb_telemetry-1.8.0-py3-none-any.whl.zip` & `tmp/nucliadb_telemetry-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,29 @@
-Zip file size: 38415 bytes, number of entries: 26
--rw-r--r--  2.0 unx      899 b- defN 23-Apr-10 13:32 nucliadb_telemetry/__init__.py
--rw-r--r--  2.0 unx    12027 b- defN 23-Apr-10 13:32 nucliadb_telemetry/batch_span.py
--rw-r--r--  2.0 unx     1254 b- defN 23-Apr-10 13:32 nucliadb_telemetry/common.py
--rw-r--r--  2.0 unx     2925 b- defN 23-Apr-10 13:32 nucliadb_telemetry/errors.py
--rw-r--r--  2.0 unx     7739 b- defN 23-Apr-10 13:32 nucliadb_telemetry/fastapi.py
--rw-r--r--  2.0 unx    14809 b- defN 23-Apr-10 13:32 nucliadb_telemetry/grpc.py
--rw-r--r--  2.0 unx     5218 b- defN 23-Apr-10 13:32 nucliadb_telemetry/grpc_metrics.py
--rw-r--r--  2.0 unx     7231 b- defN 23-Apr-10 13:32 nucliadb_telemetry/jaeger.py
--rw-r--r--  2.0 unx     8226 b- defN 23-Apr-10 13:32 nucliadb_telemetry/jetstream.py
--rw-r--r--  2.0 unx     7106 b- defN 23-Apr-10 13:32 nucliadb_telemetry/metrics.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 13:32 nucliadb_telemetry/py.typed
--rw-r--r--  2.0 unx     1165 b- defN 23-Apr-10 13:32 nucliadb_telemetry/settings.py
--rw-r--r--  2.0 unx     3883 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tracerprovider.py
--rw-r--r--  2.0 unx     5187 b- defN 23-Apr-10 13:32 nucliadb_telemetry/utils.py
--rw-r--r--  2.0 unx      833 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tests/__init__.py
--rw-r--r--  2.0 unx      960 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tests/conftest.py
--rw-r--r--  2.0 unx    12593 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tests/telemetry.py
--rw-r--r--  2.0 unx      833 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tests/grpc/__init__.py
--rw-r--r--  2.0 unx     2340 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.py
--rw-r--r--  2.0 unx     2822 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.py
--rw-r--r--  2.0 unx     2290 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tests/grpc/helloworld_pb2.py
--rw-r--r--  2.0 unx     2677 b- defN 23-Apr-10 13:32 nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.py
--rw-r--r--  2.0 unx     7177 b- defN 23-Apr-10 13:32 nucliadb_telemetry-1.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 13:32 nucliadb_telemetry-1.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Apr-10 13:32 nucliadb_telemetry-1.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2373 b- defN 23-Apr-10 13:32 nucliadb_telemetry-1.8.0.dist-info/RECORD
-26 files, 112678 bytes uncompressed, 34511 bytes compressed:  69.4%
+Zip file size: 40835 bytes, number of entries: 27
+-rw-r--r--  2.0 unx      899 b- defN 23-Apr-14 13:52 nucliadb_telemetry/__init__.py
+-rw-r--r--  2.0 unx    12027 b- defN 23-Apr-14 13:52 nucliadb_telemetry/batch_span.py
+-rw-r--r--  2.0 unx     1254 b- defN 23-Apr-14 13:52 nucliadb_telemetry/common.py
+-rw-r--r--  2.0 unx     2925 b- defN 23-Apr-14 13:52 nucliadb_telemetry/errors.py
+-rw-r--r--  2.0 unx     7739 b- defN 23-Apr-14 13:52 nucliadb_telemetry/fastapi.py
+-rw-r--r--  2.0 unx    14809 b- defN 23-Apr-14 13:52 nucliadb_telemetry/grpc.py
+-rw-r--r--  2.0 unx     5218 b- defN 23-Apr-14 13:52 nucliadb_telemetry/grpc_metrics.py
+-rw-r--r--  2.0 unx     7231 b- defN 23-Apr-14 13:52 nucliadb_telemetry/jaeger.py
+-rw-r--r--  2.0 unx     8226 b- defN 23-Apr-14 13:52 nucliadb_telemetry/jetstream.py
+-rw-r--r--  2.0 unx     6181 b- defN 23-Apr-14 13:52 nucliadb_telemetry/logs.py
+-rw-r--r--  2.0 unx     7106 b- defN 23-Apr-14 13:52 nucliadb_telemetry/metrics.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 13:52 nucliadb_telemetry/py.typed
+-rw-r--r--  2.0 unx     1521 b- defN 23-Apr-14 13:52 nucliadb_telemetry/settings.py
+-rw-r--r--  2.0 unx     3883 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tracerprovider.py
+-rw-r--r--  2.0 unx     5187 b- defN 23-Apr-14 13:52 nucliadb_telemetry/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tests/__init__.py
+-rw-r--r--  2.0 unx      960 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tests/conftest.py
+-rw-r--r--  2.0 unx    12593 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tests/telemetry.py
+-rw-r--r--  2.0 unx      833 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tests/grpc/__init__.py
+-rw-r--r--  2.0 unx     2340 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.py
+-rw-r--r--  2.0 unx     2822 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.py
+-rw-r--r--  2.0 unx     2290 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tests/grpc/helloworld_pb2.py
+-rw-r--r--  2.0 unx     2677 b- defN 23-Apr-14 13:52 nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.py
+-rw-r--r--  2.0 unx     7209 b- defN 23-Apr-14 13:53 nucliadb_telemetry-1.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 13:53 nucliadb_telemetry-1.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Apr-14 13:53 nucliadb_telemetry-1.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2456 b- defN 23-Apr-14 13:53 nucliadb_telemetry-1.9.0.dist-info/RECORD
+27 files, 119330 bytes uncompressed, 36803 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -21,14 +21,17 @@
 
 Filename: nucliadb_telemetry/jaeger.py
 Comment: 
 
 Filename: nucliadb_telemetry/jetstream.py
 Comment: 
 
+Filename: nucliadb_telemetry/logs.py
+Comment: 
+
 Filename: nucliadb_telemetry/metrics.py
 Comment: 
 
 Filename: nucliadb_telemetry/py.typed
 Comment: 
 
 Filename: nucliadb_telemetry/settings.py
@@ -60,20 +63,20 @@
 
 Filename: nucliadb_telemetry/tests/grpc/helloworld_pb2.py
 Comment: 
 
 Filename: nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.py
 Comment: 
 
-Filename: nucliadb_telemetry-1.8.0.dist-info/METADATA
+Filename: nucliadb_telemetry-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb_telemetry-1.8.0.dist-info/WHEEL
+Filename: nucliadb_telemetry-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb_telemetry-1.8.0.dist-info/top_level.txt
+Filename: nucliadb_telemetry-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb_telemetry-1.8.0.dist-info/RECORD
+Filename: nucliadb_telemetry-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb_telemetry/settings.py

```diff
@@ -13,19 +13,37 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
+import enum
+from typing import Optional
+
 from pydantic import BaseSettings
 
 
 class TelemetrySettings(BaseSettings):
     jaeger_agent_host: str = "localhost"
     jaeger_agent_port: int = 6831
     jaeger_enabled: bool = False
     jaeger_query_port: int = 16686
     jaeger_query_host: str = "jaeger.observability.svc.cluster.local"
 
 
 telemetry_settings = TelemetrySettings()
+
+
+class LogLevel(enum.Enum):
+    DEBUG = "DEBUG"
+    INFO = "INFO"
+    WARNING = "WARNING"
+    ERROR = "ERROR"
+    FATAL = "FATAL"
+    CRITICAL = "CRITICAL"
+
+
+class LogSettings(BaseSettings):
+    debug: bool = False
+    log_level: LogLevel = LogLevel.WARNING
+    logger_levels: Optional[dict[str, LogLevel]] = None
```

## Comparing `nucliadb_telemetry-1.8.0.dist-info/METADATA` & `nucliadb_telemetry-1.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb-telemetry
-Version: 1.8.0
+Version: 1.9.0
 Summary: NucliaDB Telemetry Library Python process
 Home-page: https://github.com/nuclia/nucliadb
 Author: nucliadb Authors
 Author-email: nucliadb@nuclia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -34,14 +34,15 @@
 Requires-Dist: opentelemetry-instrumentation-fastapi (==0.30b1)
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: fastapi
 Requires-Dist: types-protobuf (<4.0,>=3.19.5)
 Requires-Dist: types-requests
 Requires-Dist: prometheus-client (>=0.12.0)
+Requires-Dist: orjson (>=3.6.7)
 
 # NucliaDB Telemetry
 
 Open telemetry compatible plugin to propagate traceid on FastAPI, Nats and GRPC with Asyncio.
 
 ENV vars:
```

## Comparing `nucliadb_telemetry-1.8.0.dist-info/RECORD` & `nucliadb_telemetry-1.9.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 nucliadb_telemetry/common.py,sha256=ZIvQTk_-xiaqNURBocz14w4cLoMyxXVg3Yk9oWCYKpc,1254
 nucliadb_telemetry/errors.py,sha256=kYovtISME_1V-_xbaQy1Jz0maqA6Ovga4CYUg3-XeWQ,2925
 nucliadb_telemetry/fastapi.py,sha256=1_O5ROvptiAUW8uAVJw1T7TPNzxoYI-2NXq0pFZAMo4,7739
 nucliadb_telemetry/grpc.py,sha256=qJ0YayPHQSymP2RKQnrOKM5s7TVvZmWz5jY7Rr8UzR0,14809
 nucliadb_telemetry/grpc_metrics.py,sha256=kIHdvHXGNEGM4e4GcWLionk4JTIQPQutISdlLQesX28,5218
 nucliadb_telemetry/jaeger.py,sha256=iiG1_5wq_8vP_dChFa0CU98S6C7rvMm_LYwZXLPrGlA,7231
 nucliadb_telemetry/jetstream.py,sha256=rr2iKgnm7nWMrBETNlEteMvNhMcYGS5k5aT6kJwoETE,8226
+nucliadb_telemetry/logs.py,sha256=0qzRsSQVl79PcZ_iBNx1e_JwKZvIV4QIMLEMpPB7va8,6181
 nucliadb_telemetry/metrics.py,sha256=32g7RwM5ekaM11V9mN9-Bw4J-oqkqSJLG2B8cZS1jlA,7106
 nucliadb_telemetry/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-nucliadb_telemetry/settings.py,sha256=Cz6EMH3MQ3zAdspXomDrvGcxYokiHI4RDi-xlVoAAF8,1165
+nucliadb_telemetry/settings.py,sha256=72hXo9UAvMtMGzbguJ6lZI_4Ljc2V2fudijyP5uHcMQ,1521
 nucliadb_telemetry/tracerprovider.py,sha256=4_4PR_V5SyA4daoX-2W5elv7y2OBbhlJBS_zZnLUPAM,3883
 nucliadb_telemetry/utils.py,sha256=ou3LRjeOGDVN0_EfHQpOVjH-0n5y-Ytqzm42ZSaHuos,5187
 nucliadb_telemetry/tests/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb_telemetry/tests/conftest.py,sha256=38jA3yjjHqTcITCIogWUp05w7p_VfdSGhczi91REt8c,960
 nucliadb_telemetry/tests/telemetry.py,sha256=kdmmY513GgtSslUkvrKHs7XW_nANd42LrCgTMv2_Ymo,12593
 nucliadb_telemetry/tests/grpc/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2.py,sha256=ieRO-vJCBnbZHxgzOMkcbravm106w6gIaSk2Rn2yFCk,2340
 nucliadb_telemetry/tests/grpc/hellostreamingworld_pb2_grpc.py,sha256=t0AUJC2DgtMwFZUGs8dGlMlb2k4YmvXgzWRg029-m0k,2822
 nucliadb_telemetry/tests/grpc/helloworld_pb2.py,sha256=GLe7zEa6k4UqwZTrp34DFeg7R0_INvWSEUf_vudIdJ8,2290
 nucliadb_telemetry/tests/grpc/helloworld_pb2_grpc.py,sha256=_jxUNxl4Fx-JztK9RO5R6osjNP2sVNVPAxLnmczEYOc,2677
-nucliadb_telemetry-1.8.0.dist-info/METADATA,sha256=KsQMl_VfpJ_56rE8po1hSfoMNzFHE7jA84vtcx9I-E4,7177
-nucliadb_telemetry-1.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-nucliadb_telemetry-1.8.0.dist-info/top_level.txt,sha256=3qEHI_5ttqQIL2gkNYwSlKsFyBBiEzDiIy9UKISzOaQ,19
-nucliadb_telemetry-1.8.0.dist-info/RECORD,,
+nucliadb_telemetry-1.9.0.dist-info/METADATA,sha256=VtVy-s7i7qH1b-qazehQfMmB3SnjtpGhtTkaRA7_IBk,7209
+nucliadb_telemetry-1.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+nucliadb_telemetry-1.9.0.dist-info/top_level.txt,sha256=3qEHI_5ttqQIL2gkNYwSlKsFyBBiEzDiIy9UKISzOaQ,19
+nucliadb_telemetry-1.9.0.dist-info/RECORD,,
```

