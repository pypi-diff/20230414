# Comparing `tmp/serverless-sdk-0.3.9.tar.gz` & `tmp/serverless-sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-etz6ci7s/serverless-sdk-0.3.9.tar", last modified: Tue Apr  4 07:17:33 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-klpnetyx/serverless-sdk-0.4.0.tar", last modified: Fri Apr 14 13:30:06 2023, max compression
```

## Comparing `serverless-sdk-0.3.9.tar` & `serverless-sdk-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/serverless_sdk/lib/warning_captured_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 07:17:33.000000 serverless-sdk-0.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-04 07:17:04.000000 serverless-sdk-0.3.9/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/sls_sdk/lib/warning_captured_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:30:06.000000 serverless-sdk-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-04-14 13:29:44.000000 serverless-sdk-0.4.0/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.3.9/PKG-INFO` & `serverless-sdk-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.3.9
+Version: 0.4.0
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
@@ -30,15 +30,15 @@
 ```shell
 pip install serverless-sdk
 ```
 
 ### Usage
 
 ```python
-from sls_sdk import serverlessSdk
+from serverless_sdk import serverlessSdk
 print(serverlessSdk.name)
 print(serverlessSdk.version)
 
 serverlessSdk.capture_error(Exception("Unexpected"))
 ```
 
 ### Setup
@@ -67,12 +67,14 @@
 
 ### Instrumentation
 
 This package comes with instrumentation for following areas.
 
 _Note: instrumentation is enabled via environment specific SDK instance, relying just on `serverless-sdk` doesn't enable any instrumentation)_
 
+- [HTTP(s) requests](docs/instrumentation/http.md)
+- [flask app](docs/instrumentation/flask-app.md)
 - [Python logging module](docs/instrumentation/python-logging.md)
 
 ### API
 
 - [serverlessSdk](docs/sdk.md)
```

### Comparing `serverless-sdk-0.3.9/README.md` & `serverless-sdk-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```shell
 pip install serverless-sdk
 ```
 
 ### Usage
 
 ```python
-from sls_sdk import serverlessSdk
+from serverless_sdk import serverlessSdk
 print(serverlessSdk.name)
 print(serverlessSdk.version)
 
 serverlessSdk.capture_error(Exception("Unexpected"))
 ```
 
 ### Setup
@@ -54,12 +54,14 @@
 
 ### Instrumentation
 
 This package comes with instrumentation for following areas.
 
 _Note: instrumentation is enabled via environment specific SDK instance, relying just on `serverless-sdk` doesn't enable any instrumentation)_
 
+- [HTTP(s) requests](docs/instrumentation/http.md)
+- [flask app](docs/instrumentation/flask-app.md)
 - [Python logging module](docs/instrumentation/python-logging.md)
 
 ### API
 
 - [serverlessSdk](docs/sdk.md)
```

### Comparing `serverless-sdk-0.3.9/pyproject.toml` & `serverless-sdk-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,38 +3,46 @@
 requires = [
     "setuptools>=65.6.3",
     "wheel>=0.38.4",
 ]
 
 [project]
 name = "serverless-sdk"
-version = "0.3.9"
+version = "0.4.0"
 description = "Serverless SDK for Python"
 readme = "README.md"
 authors = [{ name = "serverlessinc" }]
 requires-python = ">=3.7"
 dependencies = [
     "backports.cached-property", # included in Python >=3.8
     "blinker>=1.5",
     "importlib_metadata>=5.2", # included in Python >=3.8
     "js-regex<1.1.0,>=1.0.1",
     "typing-extensions>=4.4", # included in Python 3.8 - 3.11
 ]
 [project.optional-dependencies]
 tests = [
+    "aiohttp>=3.8.4",
     "black>=22.12",
+    "flask>=2.2.3",
     "pytest>=7.2",
+    "pytest-httpserver>=1.0.6",
+    "requests>=2.28.2",
     "ruff>=0.0.199",
+    "urllib3>=1.26.15",
 ]
 [project.urls]
 changelog = "https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md"
 documentation = "https://github.com/serverless/console/tree/main/python/packages/sdk"
 homepage = "https://www.serverless.com/console"
 repository = "https://github.com/serverless/console"
 
+[tool.setuptools.packages.find]
+include = ["sls_sdk*", "serverless_sdk*"]
+
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff]
 ignore = ["F401", "E722"]
```

### Comparing `serverless-sdk-0.3.9/serverless_sdk/__init__.py` & `serverless-sdk-0.4.0/sls_sdk/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,33 +28,44 @@
         return trace.root_span
 
 
 class ServerlessSdkSettings:
     disable_captured_events_stdout: bool
     disable_python_log_monitoring: bool
     disable_request_response_monitoring: bool
+    disable_http_monitoring: bool
+    disable_flask_monitoring: bool
 
     def __init__(
         self,
         disable_captured_events_stdout=False,
         disable_python_log_monitoring=False,
         disable_request_response_monitoring=False,
+        disable_http_monitoring=False,
+        disable_flask_monitoring=False,
     ):
         self.disable_captured_events_stdout = (
             bool(environ.get("SLS_DISABLE_CAPTURED_EVENTS_STDOUT"))
             or disable_captured_events_stdout
         )
         self.disable_python_log_monitoring = (
             bool(environ.get("SLS_DISABLE_PYTHON_LOG_MONITORING"))
             or disable_python_log_monitoring
         )
         self.disable_request_response_monitoring = (
             bool(environ.get("SLS_DISABLE_REQUEST_RESPONSE_MONITORING"))
             or disable_request_response_monitoring
         )
+        self.disable_http_monitoring = (
+            bool(environ.get("SLS_DISABLE_HTTP_MONITORING")) or disable_http_monitoring
+        )
+        self.disable_flask_monitoring = (
+            bool(environ.get("SLS_DISABLE_FLASK_MONITORING"))
+            or disable_flask_monitoring
+        )
 
 
 class ServerlessSdk:
     name: Final[str] = __name__
     version: Final[str] = __version__
     _event_emitter: EventEmitter
 
@@ -63,46 +74,62 @@
 
     org_id: Optional[str] = None
     _settings: ServerlessSdkSettings
     _custom_tags: Tags
     _is_initialized: bool
     _is_debug_mode: bool
     _is_dev_mode: bool
+    _maximum_body_byte_length: int
 
     def __init__(self):
         self._is_initialized = False
         self.trace_spans = TraceSpans()
         self._event_emitter = event_emitter
         self._custom_tags = Tags()
 
         self._report_error = report_error
         self._report_warning = report_warning
         self._report_notice = report_notice
+        self._maximum_body_byte_length = 1024 * 127  # 127 KB
 
     def _initialize(
         self,
         org_id: Optional[str] = None,
         disable_captured_events_stdout: Optional[bool] = False,
         disable_python_log_monitoring: Optional[bool] = False,
         disable_request_response_monitoring: Optional[bool] = False,
+        disable_http_monitoring: Optional[bool] = False,
+        disable_flask_monitoring: Optional[bool] = False,
     ):
         if self._is_initialized:
             return
         self.org_id = environ.get(SLS_ORG_ID, default=org_id)
         self._is_debug_mode = bool(environ.get("SLS_SDK_DEBUG"))
         self._is_dev_mode = bool(environ.get("SLS_DEV_MODE_ORG_ID"))
         self._settings = ServerlessSdkSettings(
             disable_captured_events_stdout,
             disable_python_log_monitoring,
             disable_request_response_monitoring,
+            disable_http_monitoring,
+            disable_flask_monitoring,
         )
 
         if not self._settings.disable_python_log_monitoring:
             install_logging()
 
+        if not self._settings.disable_http_monitoring:
+            from .lib.instrumentation.http import install as install_http
+
+            install_http()
+
+        if not self._settings.disable_flask_monitoring:
+            from .lib.instrumentation.flask import install as install_flask
+
+            install_flask()
+
         self._is_initialized = True
 
     def _create_trace_span(
         self,
         name: str,
         input: Optional[str] = None,
         output: Optional[str] = None,
```

### Comparing `serverless-sdk-0.3.9/serverless_sdk/exceptions.py` & `serverless-sdk-0.4.0/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/captured_event.py` & `serverless-sdk-0.4.0/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/emitter.py` & `serverless-sdk-0.4.0/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/error.py` & `serverless-sdk-0.4.0/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.0/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.0/sls_sdk/lib/instrumentation/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from logging import Logger
+import json
 
 from ..error import report as report_error
 from ..error_captured_event import create as create_error_captured_event
 from ..warning_captured_event import create as create_warning_captured_event
 
 
 _is_installed = False
@@ -14,50 +15,53 @@
 
 
 def _resolve_message(*args) -> str:
     return args[0] % args[1:]
 
 
 def _error(self, *args, **kwargs):
-    _original_error(self, *args, **kwargs)
     try:
         if (
             len(args) == 1
             and type(args[0]) is dict
             and args[0].get("source") == "serverlessSdk"
         ):
+            args = (json.dumps(args[0], indent=2),) + args[1:]
             return
         if len(args) == 1 and isinstance(args[0], BaseException):
             message = args[0]
         else:
             message = _resolve_message(*args)
         create_error_captured_event(message, origin="pythonLogging")
     except Exception as ex:
         report_error(ex)
+    finally:
+        _original_error(self, *args, **kwargs)
 
 
 def _warning(call_warn: bool = False):
     def __warning(self, *args, **kwargs):
-        if call_warn:
-            _original_warn(self, *args, **kwargs)
-        else:
-            _original_warning(self, *args, **kwargs)
-
         try:
             if (
                 len(args) == 1
                 and type(args[0]) is dict
                 and args[0].get("source") == "serverlessSdk"
             ):
+                args = (json.dumps(args[0], indent=2),) + args[1:]
                 return
             create_warning_captured_event(
                 _resolve_message(*args), origin="pythonLogging"
             )
         except Exception as ex:
             report_error(ex)
+        finally:
+            if call_warn:
+                _original_warn(self, *args, **kwargs)
+            else:
+                _original_warning(self, *args, **kwargs)
 
     return __warning
 
 
 def install():
     global _is_installed
     if _is_installed:
```

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/name.py` & `serverless-sdk-0.4.0/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.4.0/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/tags.py` & `serverless-sdk-0.4.0/sls_sdk/lib/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from datetime import datetime
 from math import inf, nan
 from re import Pattern
 from typing import Dict, List, Mapping, Tuple, Optional
 from js_regex import compile
 from typing_extensions import Final, get_args
-
+from threading import Lock
 from .error import report as report_error
 from ..base import TagType, ValidTags
 from ..exceptions import (
     DuplicateTraceSpanName,
     InvalidTraceSpanTagName,
     InvalidTraceSpanTagValue,
     SdkException,
@@ -18,30 +18,35 @@
 
 # from https://github.com/serverless/console/blob/fe64a4f53529285e89a64f7d50ec9528a3c4ce57/node/packages/sdk/lib/tags.js#L12
 RE: Final[str] = r"^[a-zA-Z0-9_.-]+$"
 RE_C: Final[Pattern] = compile(RE)
 
 
 class Tags(Dict[str, ValidTags]):
+    def __init__(self):
+        super().__init__()
+        self._lock = Lock()
+
     def _set(self, key: str, value: ValidTags):
         if value is None:
             return
 
         name = ensure_tag_name(key)
         value = ensure_tag_value(name, value)
 
-        if name not in self:
-            super().__setitem__(name, value)
-            return
+        with self._lock:
+            if name not in self:
+                super().__setitem__(name, value)
+                return
 
-        current: ValidTags = self[name]
+            current: ValidTags = self[name]
 
-        if isinstance(current, list):
-            if value != current:
-                return
+            if isinstance(current, list):
+                if value != current:
+                    return
 
         raise DuplicateTraceSpanName(f"Cannot set tag: Tag {name} is already set")
 
     def set(self, key: str, value: ValidTags):
         try:
             self._set(key, value)
         except Exception as ex:
```

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/trace.py` & `serverless-sdk-0.4.0/sls_sdk/lib/trace.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from collections.abc import Iterable
 import logging
 import time
-from typing import List, Optional
+from typing import List, Optional, Callable
 from contextvars import ContextVar
 from backports.cached_property import cached_property  # available in Python >=3.8
 from typing_extensions import Final, Self
 import json
 from .timing import to_protobuf_epoch_timestamp
 from ..base import Nanoseconds, TraceId
 from ..exceptions import (
@@ -38,37 +38,40 @@
 
 
 class TraceSpan:
     parent_span: Self
     name: str
     start_time: Nanoseconds
     end_time: Optional[Nanoseconds] = None
-    input: Optional[str] = None
-    output: Optional[str] = None
+    _input: Optional[str] = None
+    _output: Optional[str] = None
     tags: Tags
     custom_tags: Tags
     sub_spans: List[Self]
+    _on_close_by_root: Optional[Callable] = None
 
     def __init__(
         self,
         name: str,
         input: Optional[str] = None,
         output: Optional[str] = None,
         start_time: Optional[Nanoseconds] = None,
         tags: Optional[Tags] = None,
         immediate_descendants: Optional[List[str]] = None,
+        on_close_by_root: Optional[Callable] = None,
     ):
-        self.name = get_resource_name(name)
+        self._set_name(name)
         self.input = input
         self.output = output
         self.sub_spans = []
 
         self._set_start_time(start_time)
         self._set_tags(tags)
         self._set_spans(immediate_descendants)
+        self._on_close_by_root = on_close_by_root
 
     @staticmethod
     def resolve_current_span() -> Optional[TraceSpan]:
         global root_span, ctx
         span = ctx.get(None)
 
         return span or root_span or None
@@ -99,14 +102,17 @@
         if self.parent_span:
             self.parent_span.sub_spans.append(self)
 
     def _set_ctx(self, override: Optional[TraceSpan] = None):
         global ctx
         ctx.set(override or self)
 
+    def _set_name(self, name):
+        self.name = get_resource_name(name)
+
     def _set_tags(self, tags: Optional[Tags]):
         self.tags = Tags()
         self.custom_tags = Tags()
 
         if tags is not None:
             self.tags.update(tags)
 
@@ -146,14 +152,25 @@
     @output.setter
     def output(self, value: str):
         if value is not None and not isinstance(value, str):
             raise InvalidType("`output` must be a string.")
 
         self._output = value
 
+    @property
+    def input(self) -> str:
+        return self._input
+
+    @input.setter
+    def input(self, value: str):
+        if value is not None and not isinstance(value, str):
+            raise InvalidType("`input` must be a string.")
+
+        self._input = value
+
     def close(self, end_time: Optional[Nanoseconds] = None):
         global root_span, ctx
         default: Nanoseconds = time.perf_counter_ns()
         target_end_time = end_time
 
         if self.end_time is not None:
             raise ClosureOnClosedSpan(
@@ -173,14 +190,16 @@
         self.end_time = default if end_time is None else end_time
         if self is root_span:
             # if this is the root span, check if there are any leftovers
             # and finally reset root_span and reset the context
             left_over_spans = []
             for sub_span in self.spans:
                 if not sub_span.end_time:
+                    if sub_span._on_close_by_root:
+                        sub_span._on_close_by_root()
                     sub_span.close(end_time=self.end_time)
                     left_over_spans.append(sub_span)
 
             if left_over_spans:
                 spans = ", ".join([s.name for s in left_over_spans])
                 logger.error(
                     "Serverless SDK Warning: Following trace spans didn't end before"
@@ -204,26 +223,28 @@
                 if not found:
                     self._set_ctx(root_span)
 
         event_emitter.emit("trace-span-close", self)
         return self
 
     def to_protobuf_dict(self):
-        return {
+        result = {
             "id": self.id,
             "traceId": self.trace_id,
             "parentSpanId": self.parent_span.id if self.parent_span else None,
             "name": self.name,
             "startTimeUnixNano": to_protobuf_epoch_timestamp(self.start_time),
             "endTimeUnixNano": to_protobuf_epoch_timestamp(self.end_time),
             "input": self.input,
             "output": self.output,
             "tags": convert_tags_to_protobuf(self.tags),
-            "customTags": json.dumps(self.custom_tags),
         }
+        if self.custom_tags:
+            result["customTags"] = json.dumps(self.custom_tags)
+        return result
 
 
 def _flatten(xs):
     # https://stackoverflow.com/a/2158532
     for x in xs:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
             yield from _flatten(x)
```

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/warning.py` & `serverless-sdk-0.4.0/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.0/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.3.9/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.0/serverless_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.3.9
+Version: 0.4.0
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
@@ -30,15 +30,15 @@
 ```shell
 pip install serverless-sdk
 ```
 
 ### Usage
 
 ```python
-from sls_sdk import serverlessSdk
+from serverless_sdk import serverlessSdk
 print(serverlessSdk.name)
 print(serverlessSdk.version)
 
 serverlessSdk.capture_error(Exception("Unexpected"))
 ```
 
 ### Setup
@@ -67,12 +67,14 @@
 
 ### Instrumentation
 
 This package comes with instrumentation for following areas.
 
 _Note: instrumentation is enabled via environment specific SDK instance, relying just on `serverless-sdk` doesn't enable any instrumentation)_
 
+- [HTTP(s) requests](docs/instrumentation/http.md)
+- [flask app](docs/instrumentation/flask-app.md)
 - [Python logging module](docs/instrumentation/python-logging.md)
 
 ### API
 
 - [serverlessSdk](docs/sdk.md)
```

### Comparing `serverless-sdk-0.3.9/tests/test_sdk.py` & `serverless-sdk-0.4.0/tests/test_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 from types import MethodType
 from unittest.mock import MagicMock
 import pytest
 
 from . import get_params
-import serverless_sdk
-from serverless_sdk import ServerlessSdk
-from serverless_sdk.base import SLS_ORG_ID
-from serverless_sdk.lib.error_captured_event import TYPE_MAP as ERROR_TYPE_MAP
-from serverless_sdk.lib.warning_captured_event import TYPE_MAP as WARNING_TYPE_MAP
-from serverless_sdk.lib.emitter import event_emitter
+import sls_sdk
+from sls_sdk import ServerlessSdk
+from sls_sdk.base import SLS_ORG_ID
+from sls_sdk.lib.error_captured_event import TYPE_MAP as ERROR_TYPE_MAP
+from sls_sdk.lib.warning_captured_event import TYPE_MAP as WARNING_TYPE_MAP
+from sls_sdk.lib.emitter import event_emitter
 
 
 @pytest.fixture
 def sdk() -> ServerlessSdk:
-    from serverless_sdk import serverlessSdk
+    from sls_sdk import serverlessSdk
 
     return serverlessSdk
 
 
 def test_can_import_serverless_sdk():
     try:
-        from serverless_sdk import serverlessSdk
+        from sls_sdk import serverlessSdk
 
     except ImportError as e:
         raise AssertionError("Cannot import `serverlessSdk`") from e
 
 
 def test_has_name(sdk: ServerlessSdk):
     assert hasattr(sdk, "name")
@@ -91,15 +91,15 @@
     params = get_params(sdk._create_trace_span)
 
     assert len(params) >= len(args)
     assert all(arg in params for arg in args)
 
 
 def test_create_trace_span_returns_trace_span(sdk: ServerlessSdk):
-    from serverless_sdk.lib.trace import TraceSpan
+    from sls_sdk.lib.trace import TraceSpan
 
     span = sdk._create_trace_span("name", "input", "output")
 
     assert isinstance(span, TraceSpan)
 
 
 def test_sdk_exposes_capture_error(sdk: ServerlessSdk):
@@ -170,15 +170,15 @@
     # then
     assert sdk._custom_tags[tag_name] == tag_value
 
 
 def test_sdk_set_tag_does_not_crash_on_invalid_input(sdk: ServerlessSdk, monkeypatch):
     # given
     mock = MagicMock()
-    monkeypatch.setattr(serverless_sdk, "report_error", mock)
+    monkeypatch.setattr(sls_sdk, "report_error", mock)
     tag_name = ""
     tag_value = "value"
 
     # when
     failed = False
     try:
         sdk.set_tag(tag_name, tag_value)
```

