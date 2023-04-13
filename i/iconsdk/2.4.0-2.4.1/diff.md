# Comparing `tmp/iconsdk-2.4.0.tar.gz` & `tmp/iconsdk-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iconsdk-2.4.0.tar", last modified: Thu Apr 13 08:23:05 2023, max compression
+gzip compressed data, was "dist/iconsdk-2.4.1.tar", last modified: Thu Apr 13 23:54:47 2023, max compression
```

## Comparing `iconsdk-2.4.0.tar` & `iconsdk-2.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-13 08:23:05.000000 iconsdk-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-04-13 08:23:00.000000 iconsdk-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/builder/call_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/builder/transaction_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    22207 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/icon_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/libs/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/libs/in_memory_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/libs/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/libs/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/providers/http_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/providers/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/signed_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/convert_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/hexadecimal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/utils/typing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/typing/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-13 08:23:00.000000 iconsdk-2.4.0/iconsdk/wallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 08:23:05.000000 iconsdk-2.4.0/iconsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 08:23:05.000000 iconsdk-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-13 08:23:00.000000 iconsdk-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-13 23:54:47.000000 iconsdk-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33506 2023-04-13 23:54:42.000000 iconsdk-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/builder/call_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/builder/transaction_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/icon_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/libs/in_memory_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/libs/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/libs/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7839 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/providers/http_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/providers/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/signed_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/convert_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/hexadecimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/utils/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/typing/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-13 23:54:42.000000 iconsdk-2.4.1/iconsdk/wallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45290 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 23:54:47.000000 iconsdk-2.4.1/iconsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 23:54:47.000000 iconsdk-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-13 23:54:42.000000 iconsdk-2.4.1/setup.py
```

### Comparing `iconsdk-2.4.0/PKG-INFO` & `iconsdk-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconsdk
-Version: 2.4.0
+Version: 2.4.1
 Summary: ICON SDK for Python is a collection of libraries which allow you to interact with a local or remote ICON node using an HTTP connection.
 Home-page: https://github.com/icon-project/icon-sdk-python
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
 Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/icon-sdk-python/iconsdk-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/icon-sdk-python/actions/workflows/iconsdk-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/iconsdk?label=latest&logo=pypi)](https://pypi.org/project/iconsdk)
```

### Comparing `iconsdk-2.4.0/README.md` & `iconsdk-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/__init__.py` & `iconsdk-2.4.1/iconsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/builder/__init__.py` & `iconsdk-2.4.1/iconsdk/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/builder/call_builder.py` & `iconsdk-2.4.1/iconsdk/builder/call_builder.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/builder/transaction_builder.py` & `iconsdk-2.4.1/iconsdk/builder/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/exception.py` & `iconsdk-2.4.1/iconsdk/exception.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/icon_service.py` & `iconsdk-2.4.1/iconsdk/icon_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -517,15 +517,15 @@
         Delegates to btp_getSourceInformation RPC method.
         https://github.com/icon-project/goloop/blob/master/doc/btp2_extension.md#btp_getSourceInformation
 
         :return: A BTP network information object
         """
         return self.__provider.make_request('btp_getSourceInformation')
 
-    def monitor(self, spec: MonitorSpec, keep_alive: Optional[float]) -> Monitor:
+    def monitor(self, spec: MonitorSpec, keep_alive: Optional[float] = None) -> Monitor:
         """
         Monitor events specified in the spec
 
         :param spec: Monitor specification
         :param keep_alive: interval to send keep-alive while it reads a message
         in fraction of seconds
         :return: Monitoring handle
```

### Comparing `iconsdk-2.4.0/iconsdk/libs/__init__.py` & `iconsdk-2.4.1/iconsdk/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/libs/in_memory_zip.py` & `iconsdk-2.4.1/iconsdk/libs/in_memory_zip.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/libs/serializer.py` & `iconsdk-2.4.1/iconsdk/libs/serializer.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/libs/signer.py` & `iconsdk-2.4.1/iconsdk/libs/signer.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/monitor.py` & `iconsdk-2.4.1/iconsdk/monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,39 +21,39 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from __future__ import annotations
 
-from typing import List
+from typing import List, Dict, Any
 
 from iconsdk.providers.provider import MonitorSpec
 from iconsdk.utils.typing.conversion import object_to_str
 
 
 class EventFilter:
     def __init__(self, addr: str, event: str, indexed: int, *args):
         self.__addr = addr
         self.__event = event
         self.__indexed = list(args[0:indexed])
         self.__data = list(args[indexed:])
 
-    def apply_to(self, obj: dict):
+    def apply_to(self, obj: Dict[str, Any]):
         obj.update({
             "event": self.__event,
             "indexed": self.__indexed,
             "data": self.__data,
         })
         if self.__addr is not None:
             obj.update({
                 "addr": self.__addr
             })
 
-    def as_dict(self) -> dict:
+    def as_dict(self) -> Dict[str, Any]:
         obj = {}
         self.apply_to(obj)
         return obj
 
 
 class EventMonitorSpec(MonitorSpec):
     def __init__(self, height: int | None,
@@ -103,15 +103,15 @@
             self.__filters = list([filters])
         else:
             self.__filters = filters
 
     def get_path(self) -> str:
         return 'block'
 
-    def get_request(self) -> any:
+    def get_request(self) -> Dict[str, Any]:
         params = {}
         if self.__height is not None:
             params["height"] = self.__height
         if self.__logs:
             params["logs"] = True
         if len(self.__filters) == 1:
             self.__filters[0].apply_to(params)
@@ -138,15 +138,15 @@
         self.__network_id = network_id
         self.__proof_flag = proof_flag
         self.__progress_interval = progress_interval
 
     def get_path(self) -> str:
         return 'btp'
 
-    def get_request(self) -> any:
+    def get_request(self) -> Dict[str, Any]:
         params = {
             "networkID": self.__network_id,
         }
         if self.__height is not None:
             params["height"] = self.__height
         if self.__proof_flag:
             params['proofFlag'] = True
```

### Comparing `iconsdk-2.4.0/iconsdk/providers/__init__.py` & `iconsdk-2.4.1/iconsdk/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/providers/http_provider.py` & `iconsdk-2.4.1/iconsdk/providers/http_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,41 +151,40 @@
         content = json.loads(response.content)
         if full_response:
             return content
         if response.ok:
             return content['result']
         raise JSONRPCException(content["error"])
 
-    def make_monitor(self, spec: MonitorSpec, keep_alive: float = 30.0) -> Monitor:
+    def make_monitor(self, spec: MonitorSpec, keep_alive: Optional[float] = None) -> Monitor:
         if self._WS_MAP is None:
             raise Exception(f'Channel must be set for socket')
         path = spec.get_path()
         params = spec.get_request()
         if path not in self._WS_MAP:
             raise Exception(f'No available socket for {path}')
         return WebSocketMonitor(self._WS_MAP[path], params, keep_alive=keep_alive)
 
 
 class WebSocketMonitor(Monitor):
-    def __init__(self, url: str, params: dict, keep_alive: float):
+    def __init__(self, url: str, params: dict, keep_alive: Optional[float] = None):
         self.__client = WebSocket()
-        self.__keep_alive = keep_alive
-        self.__client.timeout = keep_alive
+        self.__keep_alive = keep_alive or 30
         self.__client.connect(url)
         self.__client.send(json.dumps(params))
         result = self.__read_json(None)
         if 'code' not in result:
             raise Exception(f'invalid response={json.dumps(result)}')
         if result['code'] != 0:
             raise Exception(f'fail to monitor err={result["message"]}')
 
     def close(self):
         self.__client.close()
 
-    def __read_json(self, timeout: Optional[float]) -> any:
+    def __read_json(self, timeout: Optional[float] = None) -> any:
         now = monotonic()
         limit = None
         if timeout is not None:
             limit = now + timeout
 
         while True:
             try:
@@ -198,9 +197,9 @@
                 now = monotonic()
                 if limit is None or now < limit:
                     self.__client.send(json.dumps({"keepalive": "0x1"}))
                     continue
                 else:
                     raise MonitorTimeoutException()
 
-    def read(self, timeout: Optional[float]) -> any:
+    def read(self, timeout: Optional[float] = None) -> any:
         return self.__read_json(timeout=timeout)
```

### Comparing `iconsdk-2.4.0/iconsdk/providers/provider.py` & `iconsdk-2.4.1/iconsdk/providers/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABCMeta, abstractmethod
-from typing import Optional
+from typing import Optional, Dict, Any
 
 
 class MonitorSpec(metaclass=ABCMeta):
     @abstractmethod
     def get_request(self) -> any:
         """
         Request object to send to the websocket
@@ -44,33 +44,33 @@
         Close the monitor
 
         It releases related resources.
         """
         pass
 
     @abstractmethod
-    def read(self, timeout: Optional[float]) -> any:
+    def read(self, timeout: Optional[float] = None) -> any:
         """
         Read the notification
 
         :param timeout: Timeout to wait for the message in fraction of seconds
         :except MonitorTimeoutException: if it passes the timeout
         """
         pass
 
 
 class Provider(metaclass=ABCMeta):
     """The provider defines how the IconService connects to RPC server."""
 
     @abstractmethod
-    def make_request(self, method: str, params=None, full_response: bool = False):
+    def make_request(self, method: str, params: Optional[Dict[str, Any]] = None, full_response: bool = False):
         raise NotImplementedError("Providers must implement this method")
 
     @abstractmethod
-    def make_monitor(self, spec: MonitorSpec, keep_alive: float = 30.0) -> Monitor:
+    def make_monitor(self, spec: MonitorSpec, keep_alive: Optional[float] = None) -> Monitor:
         """
         Make monitor for the spec
         :param spec: Monitoring spec
         :param keep_alive: Keep-alive message interval in fraction of seconds
         """
         raise NotImplementedError()
```

### Comparing `iconsdk-2.4.0/iconsdk/signed_transaction.py` & `iconsdk-2.4.1/iconsdk/signed_transaction.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/__init__.py` & `iconsdk-2.4.1/iconsdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/convert_type.py` & `iconsdk-2.4.1/iconsdk/utils/convert_type.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/converter.py` & `iconsdk-2.4.1/iconsdk/utils/converter.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/hexadecimal.py` & `iconsdk-2.4.1/iconsdk/utils/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/templates.py` & `iconsdk-2.4.1/iconsdk/utils/templates.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/type.py` & `iconsdk-2.4.1/iconsdk/utils/type.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/typing/__init__.py` & `iconsdk-2.4.1/iconsdk/utils/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/typing/conversion.py` & `iconsdk-2.4.1/iconsdk/utils/typing/conversion.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/utils/validation.py` & `iconsdk-2.4.1/iconsdk/utils/validation.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/wallet/__init__.py` & `iconsdk-2.4.1/iconsdk/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk/wallet/wallet.py` & `iconsdk-2.4.1/iconsdk/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/iconsdk.egg-info/PKG-INFO` & `iconsdk-2.4.1/iconsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iconsdk
-Version: 2.4.0
+Version: 2.4.1
 Summary: ICON SDK for Python is a collection of libraries which allow you to interact with a local or remote ICON node using an HTTP connection.
 Home-page: https://github.com/icon-project/icon-sdk-python
 Author: ICON Foundation
 Author-email: foo@icon.foundation
 License: Apache License 2.0
 Description: [![unittest](https://img.shields.io/github/actions/workflow/status/icon-project/icon-sdk-python/iconsdk-workflow.yml?branch=master&label=unittest&logo=github)](https://github.com/icon-project/icon-sdk-python/actions/workflows/iconsdk-workflow.yml)
         [![PyPI - latest](https://img.shields.io/pypi/v/iconsdk?label=latest&logo=pypi)](https://pypi.org/project/iconsdk)
```

### Comparing `iconsdk-2.4.0/iconsdk.egg-info/SOURCES.txt` & `iconsdk-2.4.1/iconsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iconsdk-2.4.0/setup.py` & `iconsdk-2.4.1/setup.py`

 * *Files identical despite different names*

