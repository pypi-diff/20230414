# Comparing `tmp/pyworxcloud-3.0.4.tar.gz` & `tmp/pyworxcloud-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-3.0.4.tar", max compression
+gzip compressed data, was "pyworxcloud-3.0.5.tar", max compression
```

## Comparing `pyworxcloud-3.0.4.tar` & `pyworxcloud-3.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2023-03-31 18:16:32.039904 pyworxcloud-3.0.4/LICENSE
--rw-r--r--   0        0        0      929 2023-03-31 18:16:32.039904 pyworxcloud-3.0.4/README.md
--rw-r--r--   0        0        0      627 2023-03-31 18:16:46.708138 pyworxcloud-3.0.4/pyproject.toml
--rw-r--r--   0        0        0    28586 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     3751 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/api.py
--rw-r--r--   0        0        0     1134 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      927 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/const.py
--rw-r--r--   0        0        0      204 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3647 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/events.py
--rw-r--r--   0        0        0     1756 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      204 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2794 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      838 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3338 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2091 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     1924 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3838 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      617 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      281 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      306 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      427 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     4793 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      411 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1348 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1109 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     2410 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6375 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2050 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      657 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      726 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     1423 2023-03-31 18:16:32.043904 pyworxcloud-3.0.4/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 pyworxcloud-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/LICENSE
+-rw-r--r--   0        0        0      929 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/README.md
+-rw-r--r--   0        0        0      629 2023-04-14 18:46:37.944752 pyworxcloud-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0    28586 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     3751 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1134 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      927 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/const.py
+-rw-r--r--   0        0        0      204 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3647 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/events.py
+-rw-r--r--   0        0        0     1756 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      204 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-04-14 18:46:24.360587 pyworxcloud-3.0.5/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2794 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      838 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3338 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2091 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     1924 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3838 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      617 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      281 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      306 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      427 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     4751 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      411 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1348 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1109 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     2410 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6375 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2050 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      657 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      726 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     1423 2023-04-14 18:46:24.364588 pyworxcloud-3.0.5/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 pyworxcloud-3.0.5/PKG-INFO
```

### Comparing `pyworxcloud-3.0.4/LICENSE` & `pyworxcloud-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/README.md` & `pyworxcloud-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyproject.toml` & `pyworxcloud-3.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v3.0.4"
+version = "v3.0.5"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
@@ -16,11 +16,11 @@
 readme = "README.md"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mtrab/pyworxcloud/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-awsiot = "0.1.3"
 urllib3 = "^1.26.10"
 requests = "^2.26.0"
-awsiotsdk = "1.12.6"
+awsiotsdk = "^1.12.6"
+cmake = "^3.26.3"
```

### Comparing `pyworxcloud-3.0.4/pyworxcloud/__init__.py` & `pyworxcloud-3.0.5/pyworxcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/api.py` & `pyworxcloud-3.0.5/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/clouds.py` & `pyworxcloud-3.0.5/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/const.py` & `pyworxcloud-3.0.5/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/events.py` & `pyworxcloud-3.0.5/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/exceptions.py` & `pyworxcloud-3.0.5/pyworxcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/helpers/logger.py` & `pyworxcloud-3.0.5/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/helpers/time_format.py` & `pyworxcloud-3.0.5/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/__init__.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/battery.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/blades.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/capability.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/devices.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/devices.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/firmware.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/mqtt.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/mqtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """MQTT information class."""
 from __future__ import annotations
 
 import json
 import logging
 import random
-import time
 import urllib.parse
 from datetime import datetime
 from typing import Any
 from uuid import uuid4
-from zoneinfo import ZoneInfo
 
 from awsiot import mqtt, mqtt_connection_builder
 
 from ..events import EventHandler
 from .landroid_class import LDict
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/product.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/requests.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/schedules.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/state.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/statistics.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/warranty.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/pyworxcloud/utils/zone.py` & `pyworxcloud-3.0.5/pyworxcloud/utils/zone.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-3.0.4/PKG-INFO` & `pyworxcloud-3.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 3.0.4
+Version: 3.0.5
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: awsiot (==0.1.3)
-Requires-Dist: awsiotsdk (==1.12.6)
+Requires-Dist: awsiotsdk (>=1.12.6,<2.0.0)
+Requires-Dist: cmake (>=3.26.3,<4.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26.10,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/mtrab/pyworxcloud/issues
 Project-URL: Documentation, https://github.com/mtrab/pyworxcloud
 Description-Content-Type: text/markdown
 
 <a href="https://www.buymeacoffee.com/mtrab" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 3.0.4 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 3.0.5 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Dist: awsiot (==0.1.3) Requires-Dist: awsiotsdk (==1.12.6)
-Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-Dist: urllib3
-(>=1.26.10,<2.0.0) Project-URL: Bug Tracker, https://github.com/mtrab/
+Modules Requires-Dist: awsiotsdk (>=1.12.6,<2.0.0) Requires-Dist: cmake
+(>=3.26.3,<4.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-Dist:
+urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug Tracker, https://github.com/mtrab/
 pyworxcloud/issues Project-URL: Documentation, https://github.com/mtrab/
 pyworxcloud Description-Content-Type: text/markdown [Buy_Me_A_Coffee] #
 pyWorxCloud This is a PyPI module for communicating with Worx Cloud mowers,
 primarily developed for use with [Home Assistant](https://home-assistant.io),
 but I try to keep it as widely usable as possible.
 
 The module are compatible with cloud enabled devices from [these vendors]
```

