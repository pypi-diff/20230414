# Comparing `tmp/elkpy-1.1.0.tar.gz` & `tmp/elkpy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkpy-1.1.0.tar", last modified: Thu Apr 13 12:09:51 2023, max compression
+gzip compressed data, was "elkpy-1.1.1.tar", last modified: Fri Apr 14 14:09:56 2023, max compression
```

## Comparing `elkpy-1.1.0.tar` & `elkpy-1.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-13 12:09:51.102546 elkpy-1.1.0/
--rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.0/COPYING
--rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.0/LICENSE
--rw-r--r--   0 max        (501) staff       (20)     5142 2023-04-13 12:09:51.102616 elkpy-1.1.0/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.0/README.md
--rw-r--r--   0 max        (501) staff       (20)      694 2023-03-30 14:23:24.000000 elkpy-1.1.0/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)      330 2023-04-13 12:09:51.102852 elkpy-1.1.0/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.0/setup.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-13 12:09:51.096992 elkpy-1.1.0/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-13 12:09:51.101844 elkpy-1.1.0/src/elkpy/
--rw-r--r--   0 max        (501) staff       (20)        0 2023-03-30 13:21:26.000000 elkpy-1.1.0/src/elkpy/__init__.py
--rw-r--r--   0 max        (501) staff       (20)    19388 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/audiographcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     9934 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/audioroutingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    16365 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/cvgatecontroller.py
--rw-r--r--   0 max        (501) staff       (20)     1989 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/grpc_gen.py
--rw-r--r--   0 max        (501) staff       (20)     8021 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/keyboardcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    19656 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/midicontroller.py
--rw-r--r--   0 max        (501) staff       (20)    15224 2023-04-06 14:39:28.000000 elkpy-1.1.0/src/elkpy/notificationcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     5032 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/osccontroller.py
--rw-r--r--   0 max        (501) staff       (20)    15841 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/parametercontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6506 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/programcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     3056 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sessioncontroller.py
--rw-r--r--   0 max        (501) staff       (20)    22973 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sushi_info_types.py
--rw-r--r--   0 max        (501) staff       (20)     6191 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sushicontroller.py
--rw-r--r--   0 max        (501) staff       (20)     1994 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sushierrors.py
--rw-r--r--   0 max        (501) staff       (20)     9701 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/sushiprocessor.py
--rw-r--r--   0 max        (501) staff       (20)     3024 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/systemcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6641 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/timingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     7011 2023-03-30 13:19:14.000000 elkpy-1.1.0/src/elkpy/transportcontroller.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-13 12:09:51.102451 elkpy-1.1.0/src/elkpy.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     5142 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      790 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)        9 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        6 2023-04-13 12:09:51.000000 elkpy-1.1.0/src/elkpy.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-14 14:09:56.864838 elkpy-1.1.1/
+-rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.1/COPYING
+-rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.1/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-04-14 14:09:56.864956 elkpy-1.1.1/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.1/README.md
+-rw-r--r--   0 max        (501) staff       (20)      694 2023-04-14 14:07:40.000000 elkpy-1.1.1/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)      330 2023-04-14 14:09:56.865267 elkpy-1.1.1/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.1/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-14 14:09:56.858639 elkpy-1.1.1/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-14 14:09:56.864071 elkpy-1.1.1/src/elkpy/
+-rw-r--r--   0 max        (501) staff       (20)        0 2023-03-30 13:21:26.000000 elkpy-1.1.1/src/elkpy/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    19388 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/audiographcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     9934 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/audioroutingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16365 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/cvgatecontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     1989 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/grpc_gen.py
+-rw-r--r--   0 max        (501) staff       (20)     8021 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/keyboardcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    19656 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/midicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16178 2023-04-14 14:06:32.000000 elkpy-1.1.1/src/elkpy/notificationcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     5032 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/osccontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    15841 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/parametercontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6506 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/programcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     3056 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/sessioncontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    22973 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/sushi_info_types.py
+-rw-r--r--   0 max        (501) staff       (20)     6191 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/sushicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     2143 2023-04-13 14:13:40.000000 elkpy-1.1.1/src/elkpy/sushierrors.py
+-rw-r--r--   0 max        (501) staff       (20)     9701 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/sushiprocessor.py
+-rw-r--r--   0 max        (501) staff       (20)     3024 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/systemcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6641 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/timingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     7011 2023-03-30 13:19:14.000000 elkpy-1.1.1/src/elkpy/transportcontroller.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-04-14 14:09:56.864731 elkpy-1.1.1/src/elkpy.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      790 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)        9 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        6 2023-04-14 14:09:56.000000 elkpy-1.1.1/src/elkpy.egg-info/top_level.txt
```

### Comparing `elkpy-1.1.0/COPYING` & `elkpy-1.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/LICENSE` & `elkpy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/PKG-INFO` & `elkpy-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elkpy-1.1.0/README.md` & `elkpy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/pyproject.toml` & `elkpy-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elkpy"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Maxime Gendebien", email="max@elk.audio" },
   { name="Ruben Svensson", email="ruben@elk.audio" },
 ]
 description = "A basic controller for sushi using gRPC"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `elkpy-1.1.0/src/elkpy/audiographcontroller.py` & `elkpy-1.1.1/src/elkpy/audiographcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/audioroutingcontroller.py` & `elkpy-1.1.1/src/elkpy/audioroutingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/cvgatecontroller.py` & `elkpy-1.1.1/src/elkpy/cvgatecontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/grpc_gen.py` & `elkpy-1.1.1/src/elkpy/grpc_gen.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/keyboardcontroller.py` & `elkpy-1.1.1/src/elkpy/keyboardcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/midicontroller.py` & `elkpy-1.1.1/src/elkpy/midicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/notificationcontroller.py` & `elkpy-1.1.1/src/elkpy/notificationcontroller.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,30 +94,36 @@
         try:
             async with grpc.experimental.aio.insecure_channel(self.address) as channel:
                 stub = self._sushi_grpc.NotificationControllerStub(channel)
                 stream = stub.SubscribeToTransportChanges(self._sushi_proto.GenericVoidValue())
                 async for notification in stream:
                     # User logic here
                     if call_back and callable(call_back):
-                        call_back(notification)
+                        if asyncio.iscoroutinefunction(call_back):
+                            await call_back(notification)
+                        else:
+                            call_back(notification)
         except grpc.RpcError as e:
             sushierrors.grpc_error_handling(e)
         except AttributeError:
             raise TypeError(f"Parameter address = {self.address}. "
                             f"Should be a string containing the IP address and port to Sushi")
 
     async def process_timing_update_notifications(self, call_back=None):
         try:
             async with grpc.experimental.aio.insecure_channel(self.address) as channel:
                 stub = self._sushi_grpc.NotificationControllerStub(channel)
                 stream = stub.SubscribeToEngineCpuTimingUpdates(self._sushi_proto.GenericVoidValue())
                 async for notification in stream:
                     # User logic here
                     if call_back and callable(call_back):
-                        call_back(notification)
+                        if asyncio.iscoroutinefunction(call_back):
+                            await call_back(notification)
+                        else:
+                            call_back(notification)
                     else:
                         raise TypeError("No valid call-back function has been provided for Timing Update "
                                         "notification processing ")
         except grpc.RpcError as e:
             sushierrors.grpc_error_handling(e)
         except AttributeError:
             raise TypeError(f"Parameter address = {self.address}. "
@@ -127,15 +133,18 @@
         try:
             async with grpc.experimental.aio.insecure_channel(self.address) as channel:
                 stub = self._sushi_grpc.NotificationControllerStub(channel)
                 stream = stub.SubscribeToTrackChanges(self._sushi_proto.GenericVoidValue())
                 async for notification in stream:
                     # User logic here
                     if call_back and callable(call_back):
-                        call_back(notification)
+                        if asyncio.iscoroutinefunction(call_back):
+                            await call_back(notification)
+                        else:
+                            call_back(notification)
                     else:
                         raise TypeError("No valid call-back function has been provided for Track Change "
                                         "notification processing ")
         except grpc.RpcError as e:
             sushierrors.grpc_error_handling(e)
         except AttributeError:
             raise TypeError(f"Parameter address = {self.address}. "
@@ -145,15 +154,18 @@
         try:
             async with grpc.experimental.aio.insecure_channel(self.address) as channel:
                 stub = self._sushi_grpc.NotificationControllerStub(channel)
                 stream = stub.SubscribeToProcessorChanges(self._sushi_proto.GenericVoidValue())
                 async for notification in stream:
                     # User logic here
                     if call_back and callable(call_back):
-                        call_back(notification)
+                        if asyncio.iscoroutinefunction(call_back):
+                            await call_back(notification)
+                        else:
+                            call_back(notification)
                     else:
                         raise TypeError("No valid call-back function has been provided for Processor Change "
                                         "notification processing ")
         except grpc.RpcError as e:
             sushierrors.grpc_error_handling(e)
         except AttributeError:
             raise TypeError(f"Parameter address = {self.address}. "
@@ -171,15 +183,18 @@
         try:
             async with grpc.experimental.aio.insecure_channel(self.address) as channel:
                 stub = self._sushi_grpc.NotificationControllerStub(channel)
                 stream = stub.SubscribeToParameterUpdates(block_list)
                 async for notification in stream:
                     # User logic here
                     if call_back and callable(call_back):
-                        call_back(notification)
+                        if asyncio.iscoroutinefunction(call_back):
+                            await call_back(notification)
+                        else:
+                            call_back(notification)
                     else:
                         raise TypeError("No valid call-back function has been provided for Parameter Update "
                                         "notification processing ")
         except grpc.RpcError as e:
             sushierrors.grpc_error_handling(e)
         except AttributeError:
             raise TypeError(f"Parameter address = {self.address}. "
@@ -197,15 +212,18 @@
         try:
             async with grpc.experimental.aio.insecure_channel(self.address) as channel:
                 stub = self._sushi_grpc.NotificationControllerStub(channel)
                 stream = stub.SubscribeToPropertyUpdates(block_list)
                 async for notification in stream:
                     # User logic here
                     if call_back and callable(call_back):
-                        call_back(notification)
+                        if asyncio.iscoroutinefunction(call_back):
+                            await call_back(notification)
+                        else:
+                            call_back(notification)
                     else:
                         raise TypeError("No valid call-back function has been provided for Property Change "
                                         "notification processing ")
         except grpc.RpcError as e:
             sushierrors.grpc_error_handling(e)
         except AttributeError:
             raise TypeError(f"Parameter address = {self.address}. "
```

### Comparing `elkpy-1.1.0/src/elkpy/osccontroller.py` & `elkpy-1.1.1/src/elkpy/osccontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/parametercontroller.py` & `elkpy-1.1.1/src/elkpy/parametercontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/programcontroller.py` & `elkpy-1.1.1/src/elkpy/programcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/sessioncontroller.py` & `elkpy-1.1.1/src/elkpy/sessioncontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/sushi_info_types.py` & `elkpy-1.1.1/src/elkpy/sushi_info_types.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/sushicontroller.py` & `elkpy-1.1.1/src/elkpy/sushicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/sushierrors.py` & `elkpy-1.1.1/src/elkpy/sushierrors.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,46 +12,59 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License along with elkpy.  If
     not, see <http://www.gnu.org/licenses/>.
 """
 __license__ = "GPL-3.0"
 
+
 ############################
 # Error handling functions #
 ############################
 
 class SushiUnkownError(Exception):
     pass
 
+
 class SushiUnsupportedOperationError(Exception):
     pass
 
+
 class SushiNotFoundError(Exception):
     pass
 
+
 class SushiOutOfRangeError(Exception):
     pass
 
+
 class SushiInvalidArgumentError(Exception):
     pass
 
+
 class SushiInternalError(Exception):
     pass
 
-def grpc_error_handling(e, context_info = ''):
-    if (e.code().name == 'UNKNOWN'):
-        raise SushiUnkownError(e.details() , context_info) from e
-    elif (e.code().name == 'FAILED_PRECONDITION'):
-        raise SushiUnsupportedOperationError(e.details() , context_info) from e
-    elif (e.code().name == 'NOT_FOUND'):
-        raise SushiNotFoundError(e.details() , context_info) from e
-    elif (e.code().name == 'OUT_OF_RANGE'):
-        raise SushiOutOfRangeError(e.details() , context_info) from e
-    elif (e.code().name == 'INVALID_ARGUMENT'):
-        raise SushiInvalidArgumentError(e.details() , context_info) from e
-    elif (e.code().name == 'INTERNAL'):
-        raise SushiInternalError(e.details() , context_info) from e
+
+class SushiUnavailableError(Exception):
+    pass
+
+
+def grpc_error_handling(e, context_info=''):
+    if e.code().name == 'UNKNOWN':
+        raise SushiUnkownError(e.details(), context_info) from e
+    elif e.code().name == 'FAILED_PRECONDITION':
+        raise SushiUnsupportedOperationError(e.details(), context_info) from e
+    elif e.code().name == 'NOT_FOUND':
+        raise SushiNotFoundError(e.details(), context_info) from e
+    elif e.code().name == 'OUT_OF_RANGE':
+        raise SushiOutOfRangeError(e.details(), context_info) from e
+    elif e.code().name == 'INVALID_ARGUMENT':
+        raise SushiInvalidArgumentError(e.details(), context_info) from e
+    elif e.code().name == 'INTERNAL':
+        raise SushiInternalError(e.details(), context_info) from e
+    elif e.code().name == 'UNAVAILABLE':
+        raise SushiUnavailableError(e.details(), context_info) from e
     else:
         if context_info is not '':
             print(context_info)
         raise e
```

### Comparing `elkpy-1.1.0/src/elkpy/sushiprocessor.py` & `elkpy-1.1.1/src/elkpy/sushiprocessor.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/systemcontroller.py` & `elkpy-1.1.1/src/elkpy/systemcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/timingcontroller.py` & `elkpy-1.1.1/src/elkpy/timingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy/transportcontroller.py` & `elkpy-1.1.1/src/elkpy/transportcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.0/src/elkpy.egg-info/PKG-INFO` & `elkpy-1.1.1/src/elkpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.1.0
+Version: 1.1.1
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elkpy-1.1.0/src/elkpy.egg-info/SOURCES.txt` & `elkpy-1.1.1/src/elkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

