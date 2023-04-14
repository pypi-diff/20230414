# Comparing `tmp/neetbox-0.1.506.tar.gz` & `tmp/neetbox-0.1.507.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.506.tar", max compression
+gzip compressed data, was "neetbox-0.1.507.tar", max compression
```

## Comparing `neetbox-0.1.506.tar` & `neetbox-0.1.507.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1067 2023-04-13 15:25:13.784400 neetbox-0.1.506/LICENSE
--rw-r--r--   0        0        0      397 2023-04-13 15:25:13.784400 neetbox-0.1.506/README.md
--rw-r--r--   0        0        0     2824 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/cli/parse.py
--rw-r--r--   0        0        0     1154 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/config/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/config/_config.py
--rw-r--r--   0        0        0     1094 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/daemon/__init__.py
--rw-r--r--   0        0        0      499 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/daemon/_apis.py
--rw-r--r--   0        0        0     1850 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/daemon/_daemon.py
--rw-r--r--   0        0        0     2989 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/daemon/_daemon_client.py
--rw-r--r--   0        0        0      409 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     7527 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8229 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      313 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0    12181 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18647 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/logging/logger.py
--rw-r--r--   0        0        0       54 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      281 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0     5594 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/pipeline/registry.py
--rw-r--r--   0        0        0        0 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      115 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2319 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4481 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/torch/profile.py
--rw-r--r--   0        0        0        0 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/utils/framing.py
--rw-r--r--   0        0        0     2165 2023-04-13 15:25:13.792400 neetbox-0.1.506/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1332 2023-04-13 15:25:13.792400 neetbox-0.1.506/pyproject.toml
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 neetbox-0.1.506/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-14 03:57:09.980247 neetbox-0.1.507/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-14 03:57:09.980247 neetbox-0.1.507/README.md
+-rw-r--r--   0        0        0     2824 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/cli/parse.py
+-rw-r--r--   0        0        0     1154 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/config/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/config/_config.py
+-rw-r--r--   0        0        0     2327 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/daemon/__init__.py
+-rw-r--r--   0        0        0      608 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/daemon/_apis.py
+-rw-r--r--   0        0        0     1960 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/daemon/_daemon.py
+-rw-r--r--   0        0        0     3776 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/daemon/_daemon_client.py
+-rw-r--r--   0        0        0      409 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     7527 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/integrations/environment.py
+-rw-r--r--   0        0        0     8229 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      313 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0    12181 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18647 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/logger.py
+-rw-r--r--   0        0        0       54 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0     5594 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/pipeline/registry.py
+-rw-r--r--   0        0        0        0 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      115 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5227 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6437 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2319 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2440 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4481 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/profile.py
+-rw-r--r--   0        0        0        0 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     2165 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/utils/utils.py
+-rw-r--r--   0        0        0     1332 2023-04-14 03:57:09.988247 neetbox-0.1.507/pyproject.toml
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 neetbox-0.1.507/PKG-INFO
```

### Comparing `neetbox-0.1.506/LICENSE` & `neetbox-0.1.507/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/__init__.py` & `neetbox-0.1.507/neetbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/cli/parse.py` & `neetbox-0.1.507/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/config/__init__.py` & `neetbox-0.1.507/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/config/_config.py` & `neetbox-0.1.507/neetbox/config/_config.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/daemon/_daemon.py` & `neetbox-0.1.507/neetbox/daemon/_daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,39 @@
+# -*- coding: utf-8 -*-
+#
+# Author: GavinGong aka VisualDust
+# URL:    https://gong.host
+# Date:   20230414
+
 from flask import Flask, json, abort, request
 import json as _json
 from neetbox.config import get_module_level_config
 from neetbox.logging import logger
 from threading import Thread
 import time
 import sys
 
 _STAT_POOL = {}
 __DAEMON_SHUTDOWN_IF_NO_UPLOAD_TIMEOUT_SEC = 60 * 60
 __COUNT_DOWN = __DAEMON_SHUTDOWN_IF_NO_UPLOAD_TIMEOUT_SEC
 __DAEMON_NAME = "NEETBOX DAEMON"
 
+
 def daemon_process(daemon_config=None):
     import setproctitle
+
     setproctitle.setproctitle(__DAEMON_NAME)
     daemon_config = daemon_config or get_module_level_config()
     api = Flask(__DAEMON_NAME)
 
     @api.route("/hello", methods=["GET"])
     def just_send_hello():
         return json.dumps({"hello": "hello"})
 
-    @api.route("/status", methods=["GET"],  defaults={'name': None})
+    @api.route("/status", methods=["GET"], defaults={"name": None})
     @api.route("/status/<name>", methods=["GET"])
     def return_status_of(name):
         global __COUNT_DOWN
         global _STAT_POOL
         __COUNT_DOWN = __DAEMON_SHUTDOWN_IF_NO_UPLOAD_TIMEOUT_SEC
         _returning_stat = dict(_STAT_POOL)
         if not name:
```

### Comparing `neetbox-0.1.506/neetbox/daemon/_daemon_client.py` & `neetbox-0.1.507/neetbox/daemon/_daemon_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,88 @@
+# -*- coding: utf-8 -*-
+#
+# Author: GavinGong aka VisualDust
+# URL:    https://gong.host
+# Date:   20230414
+
 import requests
 import time
 import json
 from datetime import datetime
 from typing import Callable
 from threading import Thread
 from functools import partial
 from neetbox.config import get_module_level_config
 from neetbox.logging import logger
 
 _update_queue_dict = {}
 __TIME_UNIT_SEC = 0.1
+__TIME_CTR_MAX_CYCLE = 9999999
 _update_value_dict = {}
 
 
-def _watch(func: Callable, name: str, freq: float):
+def __get(name):
+    _the_value = _update_value_dict.get(name, None)
+    if _the_value and "value" in _the_value:
+        _the_value = _the_value["value"]
+    return _the_value
+
+
+def __update_and_get(name):
+    _vtuple = _update_queue_dict[name]
+    _update_freq, _vfun = _vtuple
+    _the_value = _vfun()
+    _update_value_dict[name] = {
+        "value": _the_value,
+        "timestamp": datetime.timestamp(datetime.now()),
+        "interval": (_update_freq * __TIME_UNIT_SEC),
+    }
+    return _the_value
+
+
+def _watch(func: Callable, name: str, freq: float, initiative=False):
     """Function decorator to let the daemon watch a value of the function
 
     Args:
         func (function): A function returns a tuple '(name,value)'. 'name' represents the name of the value.
     """
     name = name or func.__name__
     _update_queue_dict[name] = (freq, func)
+    if (
+        initiative
+    ):  # initiatively update the value dict when the function was called manually
+        return partial(__update_and_get, name)
+    else:
+        return partial(__get, name)
+
+
+def watch(name=None, freq=None, initiative=False):
+    if not initiative:  # passively update
+        freq = freq or get_module_level_config()["updateInterval"]
+    else:
+        freq = __TIME_CTR_MAX_CYCLE + 1
+    return partial(_watch, name=name, freq=freq, initiative=initiative)
+
+
+def _update_thread():
+    # update values
+    _ctr = 0
+    while True:
+        _ctr = (_ctr + 1) % __TIME_CTR_MAX_CYCLE
+        time.sleep(__TIME_UNIT_SEC)
+        for _vname, _vtuple in _update_queue_dict.items():
+            _update_freq, _vfun = _vtuple
+            if (
+                _ctr % _update_freq == 0 and _update_freq <= __TIME_CTR_MAX_CYCLE
+            ):  # do update
+                _the_value = __update_and_get(_vname)
 
 
-def watch(name=None, freq=None):
-    _cfg = get_module_level_config()
-    freq = freq or _cfg["updateInterval"]
-    return partial(_watch, name=name, freq=freq)
+update_thread = Thread(target=_update_thread, daemon=True)
+update_thread.start()
 
 
 def connect_daemon(daemon_config):
     _display_name = get_module_level_config()["displayName"]
     _launch_config = get_module_level_config("@")
     _display_name = _display_name or _launch_config["name"]
     _update_value_dict = {"settings": _launch_config}
@@ -48,33 +100,14 @@
         r = requests.get(_api_addr)
 
     try:
         _check_daemon_alive()
     except Exception as e:
         return False
 
-    def _update_thread():
-        # update values
-        _ctr = 0
-        while True:
-            _ctr = (_ctr + 1) % 99999999
-            time.sleep(__TIME_UNIT_SEC)
-            for _vname, _vtuple in _update_queue_dict.items():
-                _update_freq, _vfun = _vtuple
-                if _ctr % _update_freq == 0:  # do update
-                    _the_value = _vfun()
-                    _update_value_dict[_vname] = {
-                        "value": _the_value,
-                        "timestamp": datetime.timestamp(datetime.now()),
-                        "interval": (_update_freq * __TIME_UNIT_SEC),
-                    }
-
-    update_thread = Thread(target=_update_thread, daemon=True)
-    update_thread.start()
-
     def _upload_thread():
         _ctr = 0
         _api_name = "sync"
         _api_addr = f"{base_addr}/{_api_name}/{_display_name}"
         while True:
             _ctr = (_ctr + 1) % 99999999
             _upload_interval = daemon_config["uploadInterval"]
```

### Comparing `neetbox-0.1.506/neetbox/integrations/engine.py` & `neetbox-0.1.507/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/integrations/environment.py` & `neetbox-0.1.507/neetbox/integrations/environment.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/integrations/resource.py` & `neetbox-0.1.507/neetbox/integrations/resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/logging/_colorama.py` & `neetbox-0.1.507/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.507/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.507/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.507/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.507/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.507/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/logging/formatting.py` & `neetbox-0.1.507/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/logging/logger.py` & `neetbox-0.1.507/neetbox/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/pipeline/registry.py` & `neetbox-0.1.507/neetbox/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/plotting/plot.py` & `neetbox-0.1.507/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/torch/arch/canny.py` & `neetbox-0.1.507/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/torch/arch/cnn.py` & `neetbox-0.1.507/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/torch/arch/kernels.py` & `neetbox-0.1.507/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.507/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/torch/nlp.py` & `neetbox-0.1.507/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/torch/profile.py` & `neetbox-0.1.507/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/utils/framing.py` & `neetbox-0.1.507/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/neetbox/utils/utils.py` & `neetbox-0.1.507/neetbox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.506/pyproject.toml` & `neetbox-0.1.507/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.506"
+version = "0.1.507"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
```

### Comparing `neetbox-0.1.506/PKG-INFO` & `neetbox-0.1.507/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.506
+Version: 0.1.507
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
```

