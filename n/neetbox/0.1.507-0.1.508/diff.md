# Comparing `tmp/neetbox-0.1.507.tar.gz` & `tmp/neetbox-0.1.508.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.507.tar", max compression
+gzip compressed data, was "neetbox-0.1.508.tar", max compression
```

## Comparing `neetbox-0.1.507.tar` & `neetbox-0.1.508.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1067 2023-04-14 03:57:09.980247 neetbox-0.1.507/LICENSE
--rw-r--r--   0        0        0      397 2023-04-14 03:57:09.980247 neetbox-0.1.507/README.md
--rw-r--r--   0        0        0     2824 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/cli/parse.py
--rw-r--r--   0        0        0     1154 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/config/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/config/_config.py
--rw-r--r--   0        0        0     2327 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/daemon/__init__.py
--rw-r--r--   0        0        0      608 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/daemon/_apis.py
--rw-r--r--   0        0        0     1960 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/daemon/_daemon.py
--rw-r--r--   0        0        0     3776 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/daemon/_daemon_client.py
--rw-r--r--   0        0        0      409 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     7527 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/integrations/environment.py
--rw-r--r--   0        0        0     8229 2023-04-14 03:57:09.984247 neetbox-0.1.507/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      313 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0    12181 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18647 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/logging/logger.py
--rw-r--r--   0        0        0       54 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      281 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/pipeline/pipe.py
--rw-r--r--   0        0        0     5594 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/pipeline/registry.py
--rw-r--r--   0        0        0        0 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      115 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5227 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6437 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2319 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2440 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4481 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/torch/profile.py
--rw-r--r--   0        0        0        0 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2303 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/utils/framing.py
--rw-r--r--   0        0        0     2165 2023-04-14 03:57:09.988247 neetbox-0.1.507/neetbox/utils/utils.py
--rw-r--r--   0        0        0     1332 2023-04-14 03:57:09.988247 neetbox-0.1.507/pyproject.toml
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 neetbox-0.1.507/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-14 10:45:41.754661 neetbox-0.1.508/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-14 10:45:41.754661 neetbox-0.1.508/README.md
+-rw-r--r--   0        0        0     2824 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/cli/parse.py
+-rw-r--r--   0        0        0     1154 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/config/__init__.py
+-rw-r--r--   0        0        0     1385 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/config/_config.py
+-rw-r--r--   0        0        0     2541 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/daemon/__init__.py
+-rw-r--r--   0        0        0      608 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/daemon/_apis.py
+-rw-r--r--   0        0        0     1904 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/daemon/_daemon.py
+-rw-r--r--   0        0        0     4398 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/daemon/_daemon_client.py
+-rw-r--r--   0        0        0      409 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     7527 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/integrations/environment.py
+-rw-r--r--   0        0        0     8229 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      313 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0     2106 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/_colorama.py
+-rw-r--r--   0        0        0    12181 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     3921 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18647 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/logging/logger.py
+-rw-r--r--   0        0        0       54 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      281 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/pipeline/pipe.py
+-rw-r--r--   0        0        0     5594 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/pipeline/registry.py
+-rw-r--r--   0        0        0        0 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      115 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5227 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6437 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2319 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2440 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4481 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/torch/profile.py
+-rw-r--r--   0        0        0        0 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     2165 2023-04-14 10:45:41.762662 neetbox-0.1.508/neetbox/utils/utils.py
+-rw-r--r--   0        0        0     1332 2023-04-14 10:45:41.762662 neetbox-0.1.508/pyproject.toml
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 neetbox-0.1.508/PKG-INFO
```

### Comparing `neetbox-0.1.507/LICENSE` & `neetbox-0.1.508/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/__init__.py` & `neetbox-0.1.508/neetbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/cli/parse.py` & `neetbox-0.1.508/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/config/__init__.py` & `neetbox-0.1.508/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/config/_config.py` & `neetbox-0.1.508/neetbox/config/_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         "enable": True,
         "displayName": None,
         "server": "localhost",
         "port": 20202,
         "updateInterval": 10,
         "uploadInterval": 10,
         "info": ["log", "status"],
+        "allowIpython":False
     },
 }
 WORKSPACE_CONFIG: dict = DEFAULT_CONFIG.copy()
 
 
 def update_with(cfg: dict):
     def _update_dict_recursively(self: dict, the_other: dict):
```

### Comparing `neetbox-0.1.507/neetbox/daemon/__init__.py` & `neetbox-0.1.508/neetbox/daemon/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,55 +3,60 @@
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230414
 
 from neetbox.daemon._daemon_client import connect_daemon, watch
 from neetbox.daemon._daemon import daemon_process
 from neetbox.logging import logger
-from neetbox.integrations import pkg
 import time
 import os
 
 
 def __attach_daemon(daemon_config):
-    try:
-        __IPYTHON__
-    except NameError:
-        pass
-    else:
-        logger.log(f"NEETBOX DAEMON won't start when debugging in ipython console.")
-        return False  # ignore if debugging in ipython
+    if not daemon_config["allowIpython"]:
+        try:
+            __IPYTHON__
+        except NameError:
+            pass
+        else:
+            logger.log(
+                f"NEETBOX DAEMON won't start when debugging in ipython console. If you want to allow daemon run in ipython, try to set 'allowIpython' to True."
+            )
+            return False  # ignore if debugging in ipython
     _online_status = connect_daemon(daemon_config)  # try to connect daemon
     if not _online_status:  # if no daemon online
         logger.log(
             f"No daemon running at {daemon_config['server']}:{daemon_config['port']}, trying to create daemon..."
         )
         try:
             pid = os.fork()
         except Exception as e:
             logger.err(
                 f"Could not fork subprocess because {e}. NEETBOX daemon won't work on Windows."
             )
             return False  # do not run if could not fork
-        if pid <= 0:  # child process
-            assert pkg.is_installed(
-                "daemon", try_install_if_not="python-daemon"
-            ), "'python-daemon' is not installed, which is necessary for creating NEETBOX DAEMON"
+        if pid == 0:  # child process
             try:
                 import daemon
             except Exception as e:
                 logger.err(
                     f"Package 'python-daemon' not working because {e}. NEETBOX daemon won't work on Windows."
                 )
                 return False  # do not run if on windows
             with daemon.DaemonContext():
                 daemon_process(daemon_config)  # create daemon
+        elif pid < 0:
+            logger.err(
+                "Faild to spawn daemon process using os.fork. NEETBOX daemon will not start."
+            )
+            return False
         time.sleep(1)
         _retry = 3
         while not connect_daemon(daemon_config):  # try connect daemon
+            logger.warn(f"Could not connect to the daemon. {_retry} retries remaining.")
             time.sleep(1)
             _retry -= 1
             if not _retry:
                 logger.err(
                     "Connect daemon faild after 3 retries, daemon connector won't start."
                 )
                 return False
```

### Comparing `neetbox-0.1.507/neetbox/daemon/_apis.py` & `neetbox-0.1.508/neetbox/daemon/_apis.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/daemon/_daemon.py` & `neetbox-0.1.508/neetbox/daemon/_daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230414
 
 from flask import Flask, json, abort, request
-import json as _json
 from neetbox.config import get_module_level_config
-from neetbox.logging import logger
 from threading import Thread
 import time
 import sys
 
 _STAT_POOL = {}
 __DAEMON_SHUTDOWN_IF_NO_UPLOAD_TIMEOUT_SEC = 60 * 60
 __COUNT_DOWN = __DAEMON_SHUTDOWN_IF_NO_UPLOAD_TIMEOUT_SEC
```

### Comparing `neetbox-0.1.507/neetbox/daemon/_daemon_client.py` & `neetbox-0.1.508/neetbox/daemon/_daemon_client.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,67 +16,84 @@
 
 _update_queue_dict = {}
 __TIME_UNIT_SEC = 0.1
 __TIME_CTR_MAX_CYCLE = 9999999
 _update_value_dict = {}
 
 
+class _WatchConfig(dict):
+    def __init__(self, name, freq, initiative=False, to_log=False):
+        self["name"] = name
+        self["freq"] = freq
+        self["initiative"] = initiative
+        self["to_log"] = to_log
+
+
 def __get(name):
     _the_value = _update_value_dict.get(name, None)
     if _the_value and "value" in _the_value:
         _the_value = _the_value["value"]
     return _the_value
 
 
 def __update_and_get(name):
     _vtuple = _update_queue_dict[name]
-    _update_freq, _vfun = _vtuple
+    _watch_config, _vfun = _vtuple
     _the_value = _vfun()
     _update_value_dict[name] = {
         "value": _the_value,
         "timestamp": datetime.timestamp(datetime.now()),
-        "interval": (_update_freq * __TIME_UNIT_SEC),
+        "interval": (_watch_config["freq"] * __TIME_UNIT_SEC),
     }
     return _the_value
 
 
-def _watch(func: Callable, name: str, freq: float, initiative=False):
+def _watch(func: Callable, name: str, freq: float, initiative=False, to_log=False):
     """Function decorator to let the daemon watch a value of the function
 
     Args:
         func (function): A function returns a tuple '(name,value)'. 'name' represents the name of the value.
     """
     name = name or func.__name__
-    _update_queue_dict[name] = (freq, func)
+    _update_queue_dict[name] = (
+        _WatchConfig(name, freq=freq, initiative=initiative, to_log=to_log),
+        func,
+    )
     if (
         initiative
     ):  # initiatively update the value dict when the function was called manually
+        logger.log(
+            f"added {name} to daemon monitor. It will update on each call of the function."
+        )
         return partial(__update_and_get, name)
     else:
+        logger.log(
+            f"added {name} to daemon monitor. It will update every {freq*__TIME_UNIT_SEC} second(s)."
+        )
         return partial(__get, name)
 
 
-def watch(name=None, freq=None, initiative=False):
+def watch(name=None, freq=None, initiative=False, to_log=False):
     if not initiative:  # passively update
         freq = freq or get_module_level_config()["updateInterval"]
     else:
         freq = __TIME_CTR_MAX_CYCLE + 1
-    return partial(_watch, name=name, freq=freq, initiative=initiative)
+    return partial(_watch, name=name, freq=freq, initiative=initiative, to_log=to_log)
 
 
 def _update_thread():
     # update values
     _ctr = 0
     while True:
         _ctr = (_ctr + 1) % __TIME_CTR_MAX_CYCLE
         time.sleep(__TIME_UNIT_SEC)
         for _vname, _vtuple in _update_queue_dict.items():
-            _update_freq, _vfun = _vtuple
+            _watch_config, _vfun = _vtuple
             if (
-                _ctr % _update_freq == 0 and _update_freq <= __TIME_CTR_MAX_CYCLE
+                not _watch_config["initiative"] and _ctr % _watch_config["freq"] == 0
             ):  # do update
                 _the_value = __update_and_get(_vname)
 
 
 update_thread = Thread(target=_update_thread, daemon=True)
 update_thread.start()
```

### Comparing `neetbox-0.1.507/neetbox/integrations/engine.py` & `neetbox-0.1.508/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/integrations/environment.py` & `neetbox-0.1.508/neetbox/integrations/environment.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/integrations/resource.py` & `neetbox-0.1.508/neetbox/integrations/resource.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/logging/_colorama.py` & `neetbox-0.1.508/neetbox/logging/_colorama.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.508/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.508/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.508/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.508/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.508/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/logging/formatting.py` & `neetbox-0.1.508/neetbox/logging/formatting.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/logging/logger.py` & `neetbox-0.1.508/neetbox/logging/logger.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/pipeline/registry.py` & `neetbox-0.1.508/neetbox/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/plotting/plot.py` & `neetbox-0.1.508/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/torch/arch/canny.py` & `neetbox-0.1.508/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/torch/arch/cnn.py` & `neetbox-0.1.508/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/torch/arch/kernels.py` & `neetbox-0.1.508/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.508/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/torch/nlp.py` & `neetbox-0.1.508/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/torch/profile.py` & `neetbox-0.1.508/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/utils/framing.py` & `neetbox-0.1.508/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/neetbox/utils/utils.py` & `neetbox-0.1.508/neetbox/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.507/pyproject.toml` & `neetbox-0.1.508/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.507"
+version = "0.1.508"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
```

### Comparing `neetbox-0.1.507/PKG-INFO` & `neetbox-0.1.508/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.507
+Version: 0.1.508
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
```

