# Comparing `tmp/apibara-0.6.6a2.tar.gz` & `tmp/apibara-0.6.6a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apibara-0.6.6a2.tar", max compression
+gzip compressed data, was "apibara-0.6.6a3.tar", max compression
```

## Comparing `apibara-0.6.6a2.tar` & `apibara-0.6.6a3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.6.6a2/LICENSE.txt
--rw-r--r--   0        0        0     1342 2023-01-18 12:16:07.977321 apibara-0.6.6a2/README.rst
--rw-r--r--   0        0        0     1075 2023-03-22 12:46:13.567643 apibara-0.6.6a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.124336 apibara-0.6.6a2/src/apibara/__init__.py
--rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.6.6a2/src/apibara/cursor.py
--rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.6.6a2/src/apibara/indexer/__init__.py
--rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.6.6a2/src/apibara/indexer/configuration.py
--rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.6.6a2/src/apibara/indexer/indexer.py
--rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.6.6a2/src/apibara/indexer/info.py
--rw-r--r--   0        0        0    10489 2023-03-22 12:45:45.277347 apibara-0.6.6a2/src/apibara/indexer/runner.py
--rw-r--r--   0        0        0    10496 2023-03-22 12:29:40.778494 apibara-0.6.6a2/src/apibara/indexer/storage.py
--rw-r--r--   0        0        0      687 2023-03-20 22:42:06.349998 apibara-0.6.6a2/src/apibara/protocol/__init__.py
--rw-r--r--   0        0        0     3521 2023-03-20 22:42:06.414999 apibara-0.6.6a2/src/apibara/protocol/client.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/protocol/proto/__init__.py
--rw-r--r--   0        0        0     3107 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/protocol/proto/stream_pb2.py
--rw-r--r--   0        0        0     9814 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/protocol/proto/stream_pb2.pyi
--rw-r--r--   0        0        0     2517 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/protocol/proto/stream_pb2_grpc.py
--rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/protocol/proto/stream_pb2_grpc.pyi
--rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/__init__.py
--rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/cursor.py
--rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/felt.py
--rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.6.6a2/src/apibara/starknet/filter.py
--rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/indexer.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/proto/__init__.py
--rw-r--r--   0        0        0     7060 2023-01-18 12:09:05.990737 apibara-0.6.6a2/src/apibara/starknet/proto/filter_pb2.py
--rw-r--r--   0        0        0    11215 2023-01-18 12:08:22.304579 apibara-0.6.6a2/src/apibara/starknet/proto/filter_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/proto/filter_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/proto/filter_pb2_grpc.pyi
--rw-r--r--   0        0        0    10601 2023-03-20 22:42:06.408999 apibara-0.6.6a2/src/apibara/starknet/proto/starknet_pb2.py
--rw-r--r--   0        0        0    17756 2023-01-18 12:08:07.126530 apibara-0.6.6a2/src/apibara/starknet/proto/starknet_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/proto/starknet_pb2_grpc.py
--rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1096 2023-01-18 12:07:16.874395 apibara-0.6.6a2/src/apibara/starknet/proto/types_pb2.py
--rw-r--r--   0        0        0      732 2023-01-18 12:07:16.871395 apibara-0.6.6a2/src/apibara/starknet/proto/types_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/proto/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.6.6a2/src/apibara/starknet/proto/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 apibara-0.6.6a2/setup.py
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 apibara-0.6.6a2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.6.6a3/LICENSE.txt
+-rw-r--r--   0        0        0     1342 2023-01-18 12:16:07.977321 apibara-0.6.6a3/README.rst
+-rw-r--r--   0        0        0     1075 2023-03-26 09:47:19.074267 apibara-0.6.6a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.124336 apibara-0.6.6a3/src/apibara/__init__.py
+-rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.6.6a3/src/apibara/cursor.py
+-rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.6.6a3/src/apibara/indexer/__init__.py
+-rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.6.6a3/src/apibara/indexer/configuration.py
+-rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.6.6a3/src/apibara/indexer/indexer.py
+-rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.6.6a3/src/apibara/indexer/info.py
+-rw-r--r--   0        0        0    10488 2023-03-26 09:46:17.305447 apibara-0.6.6a3/src/apibara/indexer/runner.py
+-rw-r--r--   0        0        0    10496 2023-03-22 12:29:40.778494 apibara-0.6.6a3/src/apibara/indexer/storage.py
+-rw-r--r--   0        0        0      687 2023-03-20 22:42:06.349998 apibara-0.6.6a3/src/apibara/protocol/__init__.py
+-rw-r--r--   0        0        0     3521 2023-03-20 22:42:06.414999 apibara-0.6.6a3/src/apibara/protocol/client.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/protocol/proto/__init__.py
+-rw-r--r--   0        0        0     3107 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/protocol/proto/stream_pb2.py
+-rw-r--r--   0        0        0     9814 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/protocol/proto/stream_pb2.pyi
+-rw-r--r--   0        0        0     2517 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/protocol/proto/stream_pb2_grpc.py
+-rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/protocol/proto/stream_pb2_grpc.pyi
+-rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/__init__.py
+-rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/cursor.py
+-rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/felt.py
+-rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.6.6a3/src/apibara/starknet/filter.py
+-rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/indexer.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/proto/__init__.py
+-rw-r--r--   0        0        0     7060 2023-01-18 12:09:05.990737 apibara-0.6.6a3/src/apibara/starknet/proto/filter_pb2.py
+-rw-r--r--   0        0        0    11215 2023-01-18 12:08:22.304579 apibara-0.6.6a3/src/apibara/starknet/proto/filter_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/proto/filter_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/proto/filter_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10601 2023-03-20 22:42:06.408999 apibara-0.6.6a3/src/apibara/starknet/proto/starknet_pb2.py
+-rw-r--r--   0        0        0    17756 2023-01-18 12:08:07.126530 apibara-0.6.6a3/src/apibara/starknet/proto/starknet_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/proto/starknet_pb2_grpc.py
+-rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1096 2023-01-18 12:07:16.874395 apibara-0.6.6a3/src/apibara/starknet/proto/types_pb2.py
+-rw-r--r--   0        0        0      732 2023-01-18 12:07:16.871395 apibara-0.6.6a3/src/apibara/starknet/proto/types_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/proto/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.6.6a3/src/apibara/starknet/proto/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 apibara-0.6.6a3/setup.py
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 apibara-0.6.6a3/PKG-INFO
```

### Comparing `apibara-0.6.6a2/LICENSE.txt` & `apibara-0.6.6a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/README.rst` & `apibara-0.6.6a3/README.rst`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/pyproject.toml` & `apibara-0.6.6a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apibara"
-version = "0.6.6a2"
+version = "0.6.6a3"
 description = "Apibara cliend SDK. Stream and transform on-chain data with Python."
 authors = ["Francesco Ceccon <francesco@apibara.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://www.apibara.com"
 repository= "https://github.com/apibara/python-sdk"
 keywords = [
```

### Comparing `apibara-0.6.6a2/src/apibara/cursor.py` & `apibara-0.6.6a3/src/apibara/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/indexer/indexer.py` & `apibara-0.6.6a3/src/apibara/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/indexer/info.py` & `apibara-0.6.6a3/src/apibara/indexer/info.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/indexer/runner.py` & `apibara-0.6.6a3/src/apibara/indexer/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         self._retry_count = 0
 
         logger.debug("starting indexer")
         while True:
             try:
                 await self._connect_and_stream(indexer, ctx)
             except Exception as exc:
-                logger.debug("indexer exception %A", exc)
+                logger.debug(f"indexer exception {exc}")
                 self._retry_count += 1
                 reconnect = await indexer.handle_reconnect(exc, self._retry_count)
 
                 if not reconnect.reconnect:
                     raise
 
     async def _connect_and_stream(self, indexer: Indexer, ctx: Optional[UserContext]):
```

### Comparing `apibara-0.6.6a2/src/apibara/indexer/storage.py` & `apibara-0.6.6a3/src/apibara/indexer/storage.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/protocol/__init__.py` & `apibara-0.6.6a3/src/apibara/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/protocol/client.py` & `apibara-0.6.6a3/src/apibara/protocol/client.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/protocol/proto/stream_pb2.py` & `apibara-0.6.6a3/src/apibara/protocol/proto/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/protocol/proto/stream_pb2.pyi` & `apibara-0.6.6a3/src/apibara/protocol/proto/stream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/protocol/proto/stream_pb2_grpc.py` & `apibara-0.6.6a3/src/apibara/protocol/proto/stream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/protocol/proto/stream_pb2_grpc.pyi` & `apibara-0.6.6a3/src/apibara/protocol/proto/stream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/cursor.py` & `apibara-0.6.6a3/src/apibara/starknet/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/felt.py` & `apibara-0.6.6a3/src/apibara/starknet/felt.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/filter.py` & `apibara-0.6.6a3/src/apibara/starknet/filter.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/proto/filter_pb2.py` & `apibara-0.6.6a3/src/apibara/starknet/proto/filter_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/proto/filter_pb2.pyi` & `apibara-0.6.6a3/src/apibara/starknet/proto/filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/proto/starknet_pb2.py` & `apibara-0.6.6a3/src/apibara/starknet/proto/starknet_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/proto/starknet_pb2.pyi` & `apibara-0.6.6a3/src/apibara/starknet/proto/starknet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/proto/types_pb2.py` & `apibara-0.6.6a3/src/apibara/starknet/proto/types_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/src/apibara/starknet/proto/types_pb2.pyi` & `apibara-0.6.6a3/src/apibara/starknet/proto/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.6.6a2/setup.py` & `apibara-0.6.6a3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ['grpcio>=1.50,<2.0', 'protobuf>=4.20,<5']
 
 extras_require = \
 {':extra == "indexer"': ['pymongo>=4.3.3,<5.0.0']}
 
 setup_kwargs = {
     'name': 'apibara',
-    'version': '0.6.6a2',
+    'version': '0.6.6a3',
     'description': 'Apibara cliend SDK. Stream and transform on-chain data with Python.',
     'long_description': 'Apibara Python SDK\n==================\n\n.. warning::\n    This SDK is alpha software. The API will change drastically until the beta.\n\n    `Open an issue on GitHub <https://github.com/apibara/python-sdk>`_ to report bugs or provide feedback.\n\n\nBuild web3-powered applications in Python. \n\nDevelopment\n-----------\n\nInstall all dependencies with:\n\n.. code::\n\n    poetry install\n\nRun tests with:\n\n.. code::\n\n    poetry run pytest tests\n\nFormat code with:\n\n.. code::\n\n    poetry run black src examples test\n    poetry run isort src examples test\n\nTo update the protobuf definitions:\n\n.. code::\n\n    protoc -I=protos/starknet/ \\\n        --python_out=src/apibara/starknet/proto/ \\\n        --pyi_out=src/apibara/starknet/proto protos/starknet/*\n\n\nLicense\n-------\n\n   Copyright 2022 GNC Labs Limited\n\n   Licensed under the Apache License, Version 2.0 (the "License");\n   you may not use this file except in compliance with the License.\n   You may obtain a copy of the License at\n\n       http://www.apache.org/licenses/LICENSE-2.0\n\n   Unless required by applicable law or agreed to in writing, software\n   distributed under the License is distributed on an "AS IS" BASIS,\n   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n   See the License for the specific language governing permissions and\n   limitations under the License.\n',
     'author': 'Francesco Ceccon',
     'author_email': 'francesco@apibara.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.apibara.com',
```

### Comparing `apibara-0.6.6a2/PKG-INFO` & `apibara-0.6.6a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apibara
-Version: 0.6.6a2
+Version: 0.6.6a3
 Summary: Apibara cliend SDK. Stream and transform on-chain data with Python.
 Home-page: https://www.apibara.com
 License: Apache-2.0
 Keywords: ethereum,web3,starknet
 Author: Francesco Ceccon
 Author-email: francesco@apibara.com
 Requires-Python: >=3.8,<3.11
```

