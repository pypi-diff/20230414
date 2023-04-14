# Comparing `tmp/numalogic_prometheus-0.2.7.tar.gz` & `tmp/numalogic_prometheus-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic_prometheus-0.2.7.tar", max compression
+gzip compressed data, was "numalogic_prometheus-0.3.0.tar", max compression
```

## Comparing `numalogic_prometheus-0.2.7.tar` & `numalogic_prometheus-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/LICENSE
--rw-r--r--   0        0        0      855 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/__init__.py
--rw-r--r--   0        0        0      986 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/_config.py
--rw-r--r--   0        0        0      632 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/_constants.py
--rw-r--r--   0        0        0        0 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/clients/__init__.py
--rw-r--r--   0        0        0     3565 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/clients/prometheus.py
--rw-r--r--   0        0        0      950 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/clients/redis.py
--rw-r--r--   0        0        0     2145 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/configs/config.yaml
--rw-r--r--   0        0        0     1841 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/default-configs/config.yaml
--rw-r--r--   0        0        0      337 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/default-configs/numalogic_config.yaml
--rw-r--r--   0        0        0     4447 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/entities.py
--rw-r--r--   0        0        0      954 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/factory.py
--rw-r--r--   0        0        0    11284 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/tools.py
--rw-r--r--   0        0        0      366 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udf/__init__.py
--rw-r--r--   0        0        0      741 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udf/filter.py
--rw-r--r--   0        0        0     3668 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udf/inference.py
--rw-r--r--   0        0        0     6990 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udf/postprocess.py
--rw-r--r--   0        0        0     1925 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udf/preprocess.py
--rw-r--r--   0        0        0     3504 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udf/threshold.py
--rw-r--r--   0        0        0     4167 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udf/window.py
--rw-r--r--   0        0        0      134 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udsink/__init__.py
--rw-r--r--   0        0        0     5558 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udsink/train.py
--rw-r--r--   0        0        0     7776 2023-04-05 20:24:18.699662 numalogic_prometheus-0.2.7/numaprom/udsink/train_rollout.py
--rw-r--r--   0        0        0     1572 2023-04-05 20:24:18.703662 numalogic_prometheus-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 numalogic_prometheus-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/LICENSE
+-rw-r--r--   0        0        0      847 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/__init__.py
+-rw-r--r--   0        0        0      974 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/_config.py
+-rw-r--r--   0        0        0      756 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/_constants.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/clients/__init__.py
+-rw-r--r--   0        0        0     3565 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/clients/prometheus.py
+-rw-r--r--   0        0        0      950 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/clients/redis.py
+-rw-r--r--   0        0        0     2145 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/configs/config.yaml
+-rw-r--r--   0        0        0     1841 2023-04-14 20:31:14.070262 numalogic_prometheus-0.3.0/numaprom/default-configs/config.yaml
+-rw-r--r--   0        0        0      337 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/default-configs/numalogic_config.yaml
+-rw-r--r--   0        0        0     4447 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/entities.py
+-rw-r--r--   0        0        0      954 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/factory.py
+-rw-r--r--   0        0        0     8854 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/tools.py
+-rw-r--r--   0        0        0      366 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/__init__.py
+-rw-r--r--   0        0        0      741 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/filter.py
+-rw-r--r--   0        0        0     3628 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/inference.py
+-rw-r--r--   0        0        0     6866 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/postprocess.py
+-rw-r--r--   0        0        0     1889 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/preprocess.py
+-rw-r--r--   0        0        0     3476 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/threshold.py
+-rw-r--r--   0        0        0     4227 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udf/window.py
+-rw-r--r--   0        0        0      134 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udsink/__init__.py
+-rw-r--r--   0        0        0     5514 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udsink/train.py
+-rw-r--r--   0        0        0     7731 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/udsink/train_rollout.py
+-rw-r--r--   0        0        0     5026 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/numaprom/watcher.py
+-rw-r--r--   0        0        0     1592 2023-04-14 20:31:14.074262 numalogic_prometheus-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 numalogic_prometheus-0.3.0/PKG-INFO
```

### Comparing `numalogic_prometheus-0.2.7/LICENSE` & `numalogic_prometheus-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.2.7/numaprom/__init__.py` & `numalogic_prometheus-0.3.0/numaprom/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 
-from numaprom._config import UnifiedConf, MetricConf, ServiceConf, NumapromConf
+from numaprom._config import UnifiedConf, MetricConf, AppConf, NumapromConf
 
 
 def get_logger(name):
     formatter = logging.Formatter("%(asctime)s-%(levelname)s-%(message)s")
     logger = logging.getLogger(name)
     stream_handler = logging.StreamHandler()
     if os.getenv("DEBUG", False):
@@ -21,8 +21,8 @@
     pl_logger = logging.getLogger("pytorch_lightning")
     pl_logger.propagate = False
     pl_logger.setLevel(logging.ERROR)
     pl_logger.addHandler(stream_handler)
     return logger
 
 
-__all__ = ["UnifiedConf", "MetricConf", "ServiceConf", "NumapromConf", "get_logger"]
+__all__ = ["UnifiedConf", "MetricConf", "AppConf", "NumapromConf", "get_logger"]
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/_config.py` & `numalogic_prometheus-0.3.0/numaprom/_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     scrape_interval: int = 30
     retrain_freq_hr: int = 8
     resume_training: bool = False
     numalogic_conf: NumalogicConf = MISSING
 
 
 @dataclass
-class ServiceConf:
-    service: str = "default"
+class AppConf:
+    app: str = "default"
     namespace: str = "default"
     metric_configs: List[MetricConf] = field(default_factory=lambda: [MetricConf()])
     unified_configs: List[UnifiedConf] = field(default_factory=list)
 
 
 @dataclass
 class NumapromConf:
-    configs: List[ServiceConf]
+    configs: List[AppConf]
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/_constants.py` & `numalogic_prometheus-0.3.0/numaprom/_constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
 
 NUMAPROM_DIR = os.path.dirname(__file__)
 ROOT_DIR = os.path.split(NUMAPROM_DIR)[0]
 TESTS_DIR = os.path.join(ROOT_DIR, "tests")
+TESTS_RESOURCES = os.path.join(TESTS_DIR, "resources")
 DATA_DIR = os.path.join(NUMAPROM_DIR, "data")
 CONFIG_DIR = os.path.join(NUMAPROM_DIR, "configs")
 DEFAULT_CONFIG_DIR = os.path.join(NUMAPROM_DIR, "default-configs")
 
 # endpoints
 DEFAULT_PROMETHEUS_SERVER = "http://prometheus-service.monitoring.svc.cluster.local:8080"
 DEFAULT_TRACKING_URI = "http://mlflow-service.numalogic-prometheus.svc.cluster.local:5000"
 
 
 # UDF constants
 TRAIN_VTX_KEY = "train"
 INFERENCE_VTX_KEY = "inference"
 THRESHOLD_VTX_KEY = "threshold"
 POSTPROC_VTX_KEY = "postproc"
+
+CONFIG_PATHS = ["./numaprom/configs", "./numaprom/default-configs"]
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/clients/prometheus.py` & `numalogic_prometheus-0.3.0/numaprom/clients/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.2.7/numaprom/clients/redis.py` & `numalogic_prometheus-0.3.0/numaprom/clients/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.2.7/numaprom/configs/config.yaml` & `numalogic_prometheus-0.3.0/numaprom/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.2.7/numaprom/default-configs/config.yaml` & `numalogic_prometheus-0.3.0/numaprom/default-configs/config.yaml`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.2.7/numaprom/entities.py` & `numalogic_prometheus-0.3.0/numaprom/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.2.7/numaprom/factory.py` & `numalogic_prometheus-0.3.0/numaprom/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.2.7/numaprom/tools.py` & `numalogic_prometheus-0.3.0/numaprom/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,26 +10,23 @@
 import boto3
 import numpy as np
 import pandas as pd
 import pytz
 from botocore.session import get_session
 from mlflow.entities.model_registry import ModelVersion
 from mlflow.exceptions import RestException
-from numalogic.config import NumalogicConf, PostprocessFactory
+from numalogic.config import PostprocessFactory
 from numalogic.models.threshold import SigmoidThreshold
 from numalogic.registry import MLflowRegistry, ArtifactData
-from omegaconf import OmegaConf
 from pynumaflow.function import Messages, Message
 
-from numaprom import get_logger, MetricConf, ServiceConf, NumapromConf, UnifiedConf
+from numaprom import get_logger, MetricConf
 from numaprom._constants import (
     DEFAULT_TRACKING_URI,
     DEFAULT_PROMETHEUS_SERVER,
-    CONFIG_DIR,
-    DEFAULT_CONFIG_DIR,
 )
 from numaprom.entities import TrainerPayload, StreamPayload
 from numaprom.clients.prometheus import Prometheus
 
 _LOGGER = get_logger(__name__)
 
 
@@ -151,77 +148,14 @@
     set_aws_session()
     tracking_uri = os.getenv("TRACKING_URI", DEFAULT_TRACKING_URI)
     ml_registry = MLflowRegistry(tracking_uri=tracking_uri, artifact_type=artifact_type)
     version = ml_registry.save(skeys=skeys, dkeys=dkeys, artifact=model, **metadata)
     return version
 
 
-def get_all_configs():
-    schema: NumapromConf = OmegaConf.structured(NumapromConf)
-
-    conf = OmegaConf.load(os.path.join(CONFIG_DIR, "config.yaml"))
-    given_configs = OmegaConf.merge(schema, conf).configs
-
-    conf = OmegaConf.load(os.path.join(DEFAULT_CONFIG_DIR, "config.yaml"))
-    default_configs = OmegaConf.merge(schema, conf).configs
-
-    conf = OmegaConf.load(os.path.join(DEFAULT_CONFIG_DIR, "numalogic_config.yaml"))
-    schema: NumalogicConf = OmegaConf.structured(NumalogicConf)
-    default_numalogic = OmegaConf.merge(schema, conf)
-
-    return given_configs, default_configs, default_numalogic
-
-
-def get_service_config(metric: str, namespace: str):
-    given_configs, default_configs, default_numalogic = get_all_configs()
-
-    # search and load from given configs
-    service_config = list(filter(lambda conf: (conf.namespace == namespace), given_configs))
-
-    # if not search and load from default configs
-    if not service_config:
-        for _conf in default_configs:
-            if metric in _conf.unified_configs[0].unified_metrics:
-                service_config = [_conf]
-                break
-
-    # if not in default configs, initialize Namespace conf with default values
-    if not service_config:
-        service_config = OmegaConf.structured(ServiceConf)
-    else:
-        service_config = service_config[0]
-
-    # loading and setting default numalogic config
-    for metric_config in service_config.metric_configs:
-        if OmegaConf.is_missing(metric_config, "numalogic_conf"):
-            metric_config.numalogic_conf = default_numalogic
-
-    return service_config
-
-
-def get_metric_config(metric: str, namespace: str) -> Optional[MetricConf]:
-    service_config = get_service_config(metric, namespace)
-    metric_config = list(
-        filter(lambda conf: (conf.metric == metric), service_config.metric_configs)
-    )
-    if not metric_config:
-        return service_config.metric_configs[0]
-    return metric_config[0]
-
-
-def get_unified_config(metric: str, namespace: str) -> Optional[UnifiedConf]:
-    service_config = get_service_config(metric, namespace)
-    unified_config = list(
-        filter(lambda conf: (metric in conf.unified_metrics), service_config.unified_configs)
-    )
-    if not unified_config:
-        return None
-    return unified_config[0]
-
-
 def fetch_data(
     payload: TrainerPayload, metric_config: MetricConf, labels: dict, return_labels=None
 ) -> pd.DataFrame:
     _start_time = time.time()
 
     prometheus_server = os.getenv("PROMETHEUS_SERVER", DEFAULT_PROMETHEUS_SERVER)
     datafetcher = Prometheus(prometheus_server)
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/udf/filter.py` & `numalogic_prometheus-0.3.0/numaprom/udf/filter.py`

 * *Files identical despite different names*

### Comparing `numalogic_prometheus-0.2.7/numaprom/udf/inference.py` & `numalogic_prometheus-0.3.0/numaprom/udf/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from torch.utils.data import DataLoader
 
 from numaprom import get_logger, MetricConf
 from numaprom.entities import PayloadFactory
 from numaprom.entities import Status, StreamPayload, Header
 from numaprom.tools import (
     load_model,
-    get_metric_config,
     msg_forward,
 )
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 
 def _run_inference(
     payload: StreamPayload, artifact_data: ArtifactData, numalogic_conf: NumalogicConf
 ) -> StreamPayload:
@@ -69,17 +69,15 @@
             "%s - Models not found in the previous steps, forwarding for static thresholding. Keys: %s",
             payload.uuid,
             payload.composite_keys,
         )
         return orjson.dumps(payload, option=orjson.OPT_SERIALIZE_NUMPY)
 
     # Load config
-    metric_config = get_metric_config(
-        metric=payload.composite_keys["name"], namespace=payload.composite_keys["namespace"]
-    )
+    metric_config = ConfigManager().get_metric_config(payload.composite_keys)
     numalogic_conf = metric_config.numalogic_conf
 
     # Load inference model
     artifact_data = load_model(
         skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
         dkeys=[numalogic_conf.model.name],
     )
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/udf/postprocess.py` & `numalogic_prometheus-0.3.0/numaprom/udf/postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from pynumaflow.function import Datum
 
 from numaprom import get_logger, UnifiedConf
 from numaprom.entities import Status, PrometheusPayload, StreamPayload, Header
 from numaprom.clients.redis import get_redis_client
 from numaprom.tools import (
     msgs_forward,
-    get_unified_config,
-    get_metric_config,
     WindowScorer,
 )
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 HOST = os.getenv("REDIS_HOST")
 PORT = os.getenv("REDIS_PORT")
 AUTH = os.getenv("REDIS_AUTH")
 
@@ -126,17 +125,15 @@
         type="Gauge",
         value=max_anomaly,
         labels=labels,
     )
 
 
 def _publish(final_score: float, payload: StreamPayload) -> List[bytes]:
-    unified_config = get_unified_config(
-        metric=payload.composite_keys["name"], namespace=payload.composite_keys["namespace"]
-    )
+    unified_config = ConfigManager().get_unified_config(payload.composite_keys)
 
     publisher_json = __construct_publisher_payload(payload, final_score).as_json()
     _LOGGER.info("%s - Payload sent to publisher: %s", payload.uuid, publisher_json)
 
     if not unified_config:
         _LOGGER.debug(
             "%s - Using default config, cannot generate a unified anomaly score", payload.uuid
@@ -177,17 +174,15 @@
     """
     _start_time = time.perf_counter()
 
     _in_msg = datum.value.decode("utf-8")
     payload = StreamPayload(**orjson.loads(_in_msg))
 
     # Load config
-    metric_config = get_metric_config(
-        metric=payload.composite_keys["name"], namespace=payload.composite_keys["namespace"]
-    )
+    metric_config = ConfigManager().get_metric_config(payload.composite_keys)
 
     _LOGGER.debug("%s - Received Payload: %r ", payload.uuid, payload)
 
     winscorer = WindowScorer(metric_config)
 
     # Use only using static thresholding
     if payload.header == Header.STATIC_INFERENCE:
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/udf/preprocess.py` & `numalogic_prometheus-0.3.0/numaprom/udf/preprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import time
 
 import orjson
 from pynumaflow.function import Datum
 
 from numaprom import get_logger
 from numaprom.entities import Status, StreamPayload, Header
-from numaprom.tools import msg_forward, load_model, get_metric_config
+from numaprom.tools import msg_forward, load_model
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 
 @msg_forward
 def preprocess(_: str, datum: Datum) -> bytes:
     _start_time = time.perf_counter()
     _in_msg = datum.value.decode("utf-8")
 
     payload = StreamPayload(**orjson.loads(_in_msg))
     _LOGGER.info("%s - Received Payload: %r ", payload.uuid, payload)
 
     # Load config
-    metric_config = get_metric_config(
-        metric=payload.composite_keys["name"], namespace=payload.composite_keys["namespace"]
-    )
+    metric_config = ConfigManager().get_metric_config(payload.composite_keys)
     preprocess_cfgs = metric_config.numalogic_conf.preprocess
 
     # Load preprocess artifact
     preproc_artifact = load_model(
         skeys=[payload.composite_keys["namespace"], payload.composite_keys["name"]],
         dkeys=[_conf.name for _conf in preprocess_cfgs],
         artifact_type="sklearn",
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/udf/threshold.py` & `numalogic_prometheus-0.3.0/numaprom/udf/threshold.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from numaprom import get_logger
 from numaprom._constants import TRAIN_VTX_KEY, POSTPROC_VTX_KEY
 from numaprom.entities import Status, TrainerPayload, PayloadFactory, Header
 from numaprom.tools import (
     conditional_forward,
     calculate_static_thresh,
     load_model,
-    get_metric_config,
 )
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 
 def _get_static_thresh_payload(payload, metric_config) -> bytes:
     """
     Calculates static thresholding, and returns a serialized json bytes payload.
@@ -40,17 +40,16 @@
     # Construct payload objects
     payload = PayloadFactory.from_json(_in_msg)
     train_payload = TrainerPayload(
         uuid=payload.uuid, composite_keys=OrderedDict(payload.composite_keys)
     )
 
     # Load config
-    metric_config = get_metric_config(
-        metric=payload.composite_keys["name"], namespace=payload.composite_keys["namespace"]
-    )
+    cm = ConfigManager()
+    metric_config = cm.get_metric_config(payload.composite_keys)
     thresh_cfg = metric_config.numalogic_conf.threshold
 
     # Check if payload needs static inference
     if payload.header == Header.STATIC_INFERENCE:
         _LOGGER.debug(
             "%s - Models not found in the previous steps, performing static thresholding. Keys: %s",
             payload.uuid,
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/udf/window.py` & `numalogic_prometheus-0.3.0/numaprom/udf/window.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from orjson import orjson
 from pynumaflow.function import Datum
 from redis.exceptions import RedisError, RedisClusterException
 
 from numaprom import get_logger
 from numaprom.entities import StreamPayload, Status, Header
 from numaprom.clients.redis import get_redis_client
-from numaprom.tools import msg_forward, create_composite_keys, get_metric_config
+from numaprom.tools import msg_forward, create_composite_keys
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 HOST = os.getenv("REDIS_HOST")
 PORT = os.getenv("REDIS_PORT")
 AUTH = os.getenv("REDIS_AUTH")
 
@@ -64,15 +65,17 @@
     UDF to construct windowing of the streaming input data, required by ML models.
     """
     _LOGGER.debug("Received Msg: %s ", datum.value)
 
     _start_time = time.perf_counter()
     msg = orjson.loads(datum.value)
 
-    metric_config = get_metric_config(metric=msg["name"], namespace=msg["labels"]["namespace"])
+    metric_config = ConfigManager().get_metric_config(
+        {"name": msg["name"], "namespace": msg["labels"]["namespace"]}
+    )
     win_size = metric_config.numalogic_conf.model.conf["seq_len"]
     buff_size = int(os.getenv("BUFF_SIZE", 10 * win_size))
 
     if buff_size < win_size:
         raise ValueError(
             f"Redis list buffer size: {buff_size} is less than window length: {win_size}"
         )
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/udsink/train.py` & `numalogic_prometheus-0.3.0/numaprom/udsink/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from numalogic.models.autoencoder import AutoencoderTrainer
 from numalogic.tools.data import StreamingDataset
 from pynumaflow.sink import Datum, Responses, Response
 
 from numaprom import get_logger
 from numaprom.entities import TrainerPayload
 from numaprom.clients.redis import get_redis_client
-from numaprom.tools import get_metric_config, save_model, fetch_data
+from numaprom.tools import save_model, fetch_data
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 HOST = os.getenv("REDIS_HOST")
 PORT = os.getenv("REDIS_PORT")
 AUTH = os.getenv("REDIS_AUTH")
 EXPIRY = int(os.getenv("REDIS_EXPIRY", 300))
@@ -99,17 +100,15 @@
         if not is_new:
             _LOGGER.debug(
                 "%s - Skipping train request with keys: %s", payload.uuid, payload.composite_keys
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
-        metric_config = get_metric_config(
-            metric=payload.composite_keys["name"], namespace=payload.composite_keys["namespace"]
-        )
+        metric_config = ConfigManager().get_metric_config(payload.composite_keys)
         model_cfg = metric_config.numalogic_conf.model
 
         train_df = fetch_data(
             payload, metric_config, {"namespace": payload.composite_keys["namespace"]}
         )
         train_df = clean_data(train_df)
```

### Comparing `numalogic_prometheus-0.2.7/numaprom/udsink/train_rollout.py` & `numalogic_prometheus-0.3.0/numaprom/udsink/train_rollout.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from pynumaflow.sink import Datum, Responses, Response
 from sklearn.pipeline import make_pipeline
 from torch.utils.data import DataLoader
 
 from numaprom import get_logger
 from numaprom.entities import TrainerPayload
 from numaprom.clients.redis import get_redis_client
-from numaprom.tools import get_metric_config, save_model, fetch_data
+from numaprom.tools import save_model, fetch_data
+from numaprom.watcher import ConfigManager
 
 _LOGGER = get_logger(__name__)
 
 HOST = os.getenv("REDIS_HOST")
 PORT = os.getenv("REDIS_PORT")
 AUTH = os.getenv("REDIS_AUTH")
 EXPIRY = int(os.getenv("REDIS_EXPIRY", 360))
@@ -113,18 +114,15 @@
                 "%s - Skipping rollouts train request with keys: %s",
                 payload.uuid,
                 payload.composite_keys,
             )
             responses.append(Response.as_success(_datum.id))
             continue
 
-        metric_config = get_metric_config(
-            metric=payload.composite_keys["name"], namespace=payload.composite_keys["namespace"]
-        )
-
+        metric_config = ConfigManager().get_metric_config(payload.composite_keys)
         model_cfg = metric_config.numalogic_conf.model
 
         # ToDo: standardize the label name
         if "rollouts_pod_template_hash" in payload.composite_keys:
             hash_label = "rollouts_pod_template_hash"
         else:
             hash_label = "hash_id"
```

### Comparing `numalogic_prometheus-0.2.7/pyproject.toml` & `numalogic_prometheus-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic-prometheus"
-version = "0.2.7"
+version = "0.3.0"
 description = "ML inference on numaflow using numalogic on Prometheus metrics"
 authors = ["Numalogic developers"]
 packages = [{ include = "numaprom" }]
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Nandita Koppisetty <nandita.iitkgp@gmail.com>",
 ]
@@ -22,14 +22,15 @@
 python = ">=3.9, <3.11"
 redis = "^4.3.1"
 pynumaflow = "~0.3"
 numalogic = {version = "~0.3.7", extras = ["mlflow"]}
 boto3 = "^1.25.2"
 orjson = "^3.8.4"
 omegaconf = "^2.3.0"
+watchdog = "^3.0.0"
 
 [tool.poetry.group.mlflowserver]
 optional = true
 
 [tool.poetry.group.mlflowserver.dependencies]
 mlflow = "^1.30.0"
```

### Comparing `numalogic_prometheus-0.2.7/PKG-INFO` & `numalogic_prometheus-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic-prometheus
-Version: 0.2.7
+Version: 0.3.0
 Summary: ML inference on numaflow using numalogic on Prometheus metrics
 Home-page: https://github.com/numaproj/numalogic-prometheus
 Author: Numalogic developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Developers
@@ -18,8 +18,9 @@
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: boto3 (>=1.25.2,<2.0.0)
 Requires-Dist: numalogic[mlflow] (>=0.3.7,<0.4.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: orjson (>=3.8.4,<4.0.0)
 Requires-Dist: pynumaflow (>=0.3,<0.4)
 Requires-Dist: redis (>=4.3.1,<5.0.0)
+Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/numaproj/numalogic-prometheus
```

