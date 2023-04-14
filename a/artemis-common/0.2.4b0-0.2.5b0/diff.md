# Comparing `tmp/artemis-common-0.2.4b0.tar.gz` & `tmp/artemis-common-0.2.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artemis-common-0.2.4b0.tar", last modified: Fri Apr 14 18:23:07 2023, max compression
+gzip compressed data, was "artemis-common-0.2.5b0.tar", last modified: Fri Apr 14 19:02:11 2023, max compression
```

## Comparing `artemis-common-0.2.4b0.tar` & `artemis-common-0.2.5b0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.324436 artemis-common-0.2.4b0/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/clients/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/clients/params_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/clients/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common/config/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/config/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/config/pem.key
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/config/uvicorn_disable_logging.json
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/custom_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common/models/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common/models/dal/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/dal/fred.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/dal/user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/model_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common/models/server/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/server/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/models/server/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common/server/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/server/exception_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common/server/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/server/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/server/middlewares/logging_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/server/swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/artemis_common/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:23:07.320435 artemis-common-0.2.4b0/artemis_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-14 18:23:07.000000 artemis-common-0.2.4b0/artemis_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 18:23:07.000000 artemis-common-0.2.4b0/artemis_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:23:07.000000 artemis-common-0.2.4b0/artemis_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 18:23:07.000000 artemis-common-0.2.4b0/artemis_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 18:23:07.000000 artemis-common-0.2.4b0/artemis_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:23:07.324436 artemis-common-0.2.4b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-14 18:22:58.000000 artemis-common-0.2.4b0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 18:23:06.000000 artemis-common-0.2.4b0/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.640840 artemis-common-0.2.5b0/artemis_common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/clients/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/clients/params_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/clients/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/pem.key
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/config/uvicorn_disable_logging.json
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/custom_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/models/dal/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/dal/fred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/dal/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/model_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/models/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/server/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/models/server/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/exception_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/artemis_common/server/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/middlewares/logging_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/artemis_common/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:02:11.640840 artemis-common-0.2.5b0/artemis_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 19:02:11.000000 artemis-common-0.2.5b0/artemis_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:02:11.644840 artemis-common-0.2.5b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-14 19:02:03.000000 artemis-common-0.2.5b0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 19:02:10.000000 artemis-common-0.2.5b0/version
```

### Comparing `artemis-common-0.2.4b0/artemis_common/clients/async_client.py` & `artemis-common-0.2.5b0/artemis_common/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/clients/params_model.py` & `artemis-common-0.2.5b0/artemis_common/clients/params_model.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/config/config.py` & `artemis-common-0.2.5b0/artemis_common/config/config.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/config/config_loader.py` & `artemis-common-0.2.5b0/artemis_common/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/config/uvicorn_disable_logging.json` & `artemis-common-0.2.5b0/artemis_common/config/uvicorn_disable_logging.json`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/consts.py` & `artemis-common-0.2.5b0/artemis_common/consts.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/custom_logging.py` & `artemis-common-0.2.5b0/artemis_common/custom_logging.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/exceptions.py` & `artemis-common-0.2.5b0/artemis_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/models/bases.py` & `artemis-common-0.2.5b0/artemis_common/models/bases.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/models/dal/fred.py` & `artemis-common-0.2.5b0/artemis_common/models/dal/fred.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/models/jwt.py` & `artemis-common-0.2.5b0/artemis_common/models/jwt.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/models/model_parser.py` & `artemis-common-0.2.5b0/artemis_common/models/model_parser.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/models/server/response.py` & `artemis-common-0.2.5b0/artemis_common/models/server/response.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/server/exception_handlers.py` & `artemis-common-0.2.5b0/artemis_common/server/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/server/middlewares/logging_middleware.py` & `artemis-common-0.2.5b0/artemis_common/server/middlewares/logging_middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
-import logging
 from time import perf_counter
 from typing import Callable
 
+import structlog
 from asgi_correlation_id.context import correlation_id
 from fastapi import FastAPI
 from fastapi import Request
 from fastapi import Response
 from starlette.middleware.base import BaseHTTPMiddleware
+from structlog.contextvars import bind_contextvars
+from structlog.contextvars import clear_contextvars
 
 from artemis_common.server import get_client_address
 
 
 REQUEST_KEY = 'REQUEST'
 RESPONSE_KEY = 'RESPONSE'
 
@@ -33,25 +35,32 @@
 
 
 class LoggingMiddleware(BaseHTTPMiddleware):
     def __init__(
         self,
         app: FastAPI,
         *,
-        logger: logging.Logger,
+        logger: structlog.BoundLogger,
     ) -> None:
         self._logger = logger
         super().__init__(app)
 
     async def dispatch(
         self,
         request: Request,
         call_next: Callable,
     ) -> Response:
         request_id = correlation_id.get()
+        client_address = get_client_address(request)
+
+        clear_contextvars()
+        bind_contextvars(
+            request_id=request_id,
+            client_address=client_address,
+        )
 
         await self._log_request(request, request_id)
 
         start_time = perf_counter()
         response = await self._execute_request(request, call_next, request_id)
         end_time = perf_counter()
 
@@ -72,32 +81,28 @@
             return response
 
         except Exception as ex:
             message = 'Failed to process response'
             self._logger.exception(
                 message,
                 http_transaction_type=RESPONSE_KEY,
-                request_id=request_id,
-                client_address=get_client_address(request),
                 request_method=request.method,
                 exc_message=str(ex),
             )
             raise
 
     async def _log_request(
         self,
         request: Request,
         request_id: str,
     ):
         message = f'Request {request.method} {request.url}'
         self._logger.info(
             message,
             http_transaction_type=REQUEST_KEY,
-            request_id=request_id,
-            client_address=get_client_address(request),
             request_method=request.method,
             request_headers=dict(request.headers),
             request_path=request.url.path,
             request_query=request.url.query,
         )
 
     async def _log_response(
@@ -116,14 +121,12 @@
         for response_item in response_body:
             response_length += len(response_item)
 
         message = f'Response {request.method} {request.url}'
         self._logger.info(
             message,
             http_transaction_type=RESPONSE_KEY,
-            request_id=request_id,
-            client_address=get_client_address(request),
             request_method=request.method,
             response_time=process_time,
             response_length=response_length,
             status_code=response.status_code,
         )
```

### Comparing `artemis-common-0.2.4b0/artemis_common/server/swagger.py` & `artemis-common-0.2.5b0/artemis_common/server/swagger.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/server/utils.py` & `artemis-common-0.2.5b0/artemis_common/server/utils.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common/token.py` & `artemis-common-0.2.5b0/artemis_common/token.py`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/artemis_common.egg-info/SOURCES.txt` & `artemis-common-0.2.5b0/artemis_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artemis-common-0.2.4b0/setup.py` & `artemis-common-0.2.5b0/setup.py`

 * *Files identical despite different names*

