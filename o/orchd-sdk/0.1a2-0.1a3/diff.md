# Comparing `tmp/orchd-sdk-0.1a2.tar.gz` & `tmp/orchd-sdk-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchd-sdk-0.1a2.tar", last modified: Thu Feb 23 07:47:38 2023, max compression
+gzip compressed data, was "orchd-sdk-0.1a3.tar", last modified: Fri Apr 14 14:58:35 2023, max compression
```

## Comparing `orchd-sdk-0.1a2.tar` & `orchd-sdk-0.1a3.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 07:47:38.663349 orchd-sdk-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-02-23 07:47:38.663349 orchd-sdk-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-23 07:47:38.663349 orchd-sdk-0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2587 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 07:47:38.659349 orchd-sdk-0.1a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 07:47:38.663349 orchd-sdk-0.1a2/src/orchd_sdk/
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11267 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/logger.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1318 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)    12001 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    13919 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (122)     9414 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/reaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     6912 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/sensor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3436 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/sink.py
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-02-23 07:47:20.000000 orchd-sdk-0.1a2/src/orchd_sdk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-23 07:47:38.663349 orchd-sdk-0.1a2/src/orchd_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      690 2023-02-23 07:47:38.000000 orchd-sdk-0.1a2/src/orchd_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      563 2023-02-23 07:47:38.000000 orchd-sdk-0.1a2/src/orchd_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-23 07:47:38.000000 orchd-sdk-0.1a2/src/orchd_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-02-23 07:47:38.000000 orchd-sdk-0.1a2/src/orchd_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-02-23 07:47:38.000000 orchd-sdk-0.1a2/src/orchd_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-02-23 07:47:38.000000 orchd-sdk-0.1a2/src/orchd_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.389757 orchd-sdk-0.1a3/
+-rw-r--r--   0 mathias    (501) staff       (20)     1097 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/LICENSE.md
+-rw-r--r--   0 mathias    (501) staff       (20)      704 2023-04-14 14:58:35.389617 orchd-sdk-0.1a3/PKG-INFO
+-rw-r--r--   0 mathias    (501) staff       (20)     1256 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/README.md
+-rw-r--r--   0 mathias    (501) staff       (20)       38 2023-04-14 14:58:35.389804 orchd-sdk-0.1a3/setup.cfg
+-rw-r--r--   0 mathias    (501) staff       (20)     2587 2023-04-07 08:22:35.000000 orchd-sdk-0.1a3/setup.py
+drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.385676 orchd-sdk-0.1a3/src/
+drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.387824 orchd-sdk-0.1a3/src/orchd_sdk/
+-rw-r--r--   0 mathias    (501) staff       (20)       10 2023-04-14 13:36:21.000000 orchd-sdk-0.1a3/src/orchd_sdk/VERSION
+-rw-r--r--   0 mathias    (501) staff       (20)     1324 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/__init__.py
+drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.389430 orchd-sdk-0.1a3/src/orchd_sdk/api/
+-rw-r--r--   0 mathias    (501) staff       (20)     2463 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/__init__.py
+-rw-r--r--   0 mathias    (501) staff       (20)      575 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/events.py
+-rw-r--r--   0 mathias    (501) staff       (20)     2264 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/reactions.py
+-rw-r--r--   0 mathias    (501) staff       (20)     2298 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/sensors.py
+-rw-r--r--   0 mathias    (501) staff       (20)     1012 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/api/sinks.py
+-rw-r--r--   0 mathias    (501) staff       (20)    11267 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/cli.py
+-rw-r--r--   0 mathias    (501) staff       (20)     1550 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/common.py
+-rw-r--r--   0 mathias    (501) staff       (20)     2161 2023-04-07 08:34:34.000000 orchd-sdk-0.1a3/src/orchd_sdk/errors.py
+-rw-r--r--   0 mathias    (501) staff       (20)      869 2022-01-22 13:12:41.000000 orchd-sdk-0.1a3/src/orchd_sdk/logger.ini
+-rw-r--r--   0 mathias    (501) staff       (20)     1318 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/logging.py
+-rw-r--r--   0 mathias    (501) staff       (20)    12001 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/models.py
+-rw-r--r--   0 mathias    (501) staff       (20)    13919 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/project.py
+-rw-r--r--   0 mathias    (501) staff       (20)     9526 2023-04-14 13:34:59.000000 orchd-sdk-0.1a3/src/orchd_sdk/reaction.py
+-rw-r--r--   0 mathias    (501) staff       (20)     6912 2023-04-06 07:46:08.000000 orchd-sdk-0.1a3/src/orchd_sdk/sensor.py
+-rw-r--r--   0 mathias    (501) staff       (20)     3436 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/sink.py
+-rw-r--r--   0 mathias    (501) staff       (20)     2065 2022-04-17 19:06:31.000000 orchd-sdk-0.1a3/src/orchd_sdk/util.py
+drwxr-xr-x   0 mathias    (501) staff       (20)        0 2023-04-14 14:58:35.388805 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/
+-rw-r--r--   0 mathias    (501) staff       (20)      704 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mathias    (501) staff       (20)      587 2022-01-28 15:55:21.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/SOURCES 2.txt
+-rw-r--r--   0 mathias    (501) staff       (20)      783 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mathias    (501) staff       (20)        1 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mathias    (501) staff       (20)       49 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 mathias    (501) staff       (20)      112 2022-01-28 15:55:21.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/requires 2.txt
+-rw-r--r--   0 mathias    (501) staff       (20)      158 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/requires.txt
+-rw-r--r--   0 mathias    (501) staff       (20)       10 2023-04-14 14:58:35.000000 orchd-sdk-0.1a3/src/orchd_sdk.egg-info/top_level.txt
```

### Comparing `orchd-sdk-0.1a2/LICENSE.md` & `orchd-sdk-0.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/PKG-INFO` & `orchd-sdk-0.1a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: orchd-sdk
-Version: 0.1a2
+Version: 0.1a3
 Summary: SDK for Orchd Ecosystem Applications
 Home-page: http://orchd.io
 Author: Mathias Santos de Brito
 Author-email: mathias.brito@me.com
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: service resource orchestration edge cloud
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Distributed Computing
 Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE.md
+
+UNKNOWN
+
```

### Comparing `orchd-sdk-0.1a2/README.md` & `orchd-sdk-0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/setup.py` & `orchd-sdk-0.1a3/setup.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/__init__.py` & `orchd-sdk-0.1a3/src/orchd_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/cli.py` & `orchd-sdk-0.1a3/src/orchd_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/common.py` & `orchd-sdk-0.1a3/src/orchd_sdk/common.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/errors.py` & `orchd-sdk-0.1a3/src/orchd_sdk/errors.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Software.
 #
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
 # WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
+
 class InvalidInputError(Exception):
     """
     Invalid input given.
     """
 
 
 class ReactorError(Exception):
@@ -30,7 +31,31 @@
 
 class ReactionError(Exception):
     """ Raised on Reaction Management and Operation errors."""
 
 
 class ReactionHandlerError(Exception):
     """ Raised by ReactionHandler implementations."""
+
+
+class InvalidRequestError(Exception):
+    """ Raised when the request is invalid."""
+
+
+class NotFoundError(Exception):
+    """ Raised when the resource is not found."""
+
+
+class ServerError(Exception):
+    """ Raised when the server is not available."""
+
+
+def handle_http_errors(response):
+    if response.status == 404:
+        raise NotFoundError()
+    elif response.status == 400 or response.status == 422:
+        raise InvalidRequestError()
+    elif response.status == 500:
+        raise ServerError()
+    elif response.status > 400:
+        raise Exception(response.status, response.reason)
+    return response
```

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/logger.ini` & `orchd-sdk-0.1a3/src/orchd_sdk/logger.ini`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/logging.py` & `orchd-sdk-0.1a3/src/orchd_sdk/logging.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/models.py` & `orchd-sdk-0.1a3/src/orchd_sdk/models.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/project.py` & `orchd-sdk-0.1a3/src/orchd_sdk/project.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/reaction.py` & `orchd-sdk-0.1a3/src/orchd_sdk/reaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import sys
 import uuid
 
 from abc import abstractmethod, ABC
 from asyncio import AbstractEventLoop
 from typing import Any, Dict, List, Union, Tuple
 
+from reactivex import Observable
 from reactivex.observer import Observer
 from reactivex.subject import Subject
 
 from orchd_sdk.common import import_class
 from orchd_sdk.errors import SinkError, ReactionHandlerError, ReactionError
 from orchd_sdk.models import Event, ReactionTemplate, SinkTemplate, ReactionInfo
 from orchd_sdk.sink import AbstractSink, DummySink
@@ -65,15 +66,16 @@
 
 class ReactionHandler(ABC):
     """
     A Reaction handler for a event.
     """
 
     @abstractmethod
-    def handle(self, event: Event, reaction: ReactionTemplate) -> None:
+    def handle(self, event: Observable[Event], reaction: ReactionTemplate) \
+            -> Observable[Event]:
         """
         Code to be executed as an reaction to an event.
 
         :param event: The event that triggered the action.
         :param reaction: The reaction object.
         """
 
@@ -250,14 +252,15 @@
         super().__init__(custom_template or DummyReaction.template)
 
 
 class DummyReactionHandler(ReactionHandler):
     """
     A Dummy ReactionHandler that is used in system tests.
     """
-    def handle(self, event: Event, reaction: ReactionTemplate) -> Any:
+    def handle(self, event: Observable[Event], reaction: ReactionTemplate) \
+            -> Observable[Event]:
         logger.info(f'DummyReactionHandler.handle Called')
         return event
 
 
 global_reactions_event_bus = ReactionsEventBus()
 """System wide ReactionEventBus"""
```

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/sensor.py` & `orchd-sdk-0.1a3/src/orchd_sdk/sensor.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/sink.py` & `orchd-sdk-0.1a3/src/orchd_sdk/sink.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk/util.py` & `orchd-sdk-0.1a3/src/orchd_sdk/util.py`

 * *Files identical despite different names*

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk.egg-info/PKG-INFO` & `orchd-sdk-0.1a3/src/orchd_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: orchd-sdk
-Version: 0.1a2
+Version: 0.1a3
 Summary: SDK for Orchd Ecosystem Applications
 Home-page: http://orchd.io
 Author: Mathias Santos de Brito
 Author-email: mathias.brito@me.com
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: service resource orchestration edge cloud
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Distributed Computing
 Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE.md
+
+UNKNOWN
+
```

### Comparing `orchd-sdk-0.1a2/src/orchd_sdk.egg-info/SOURCES.txt` & `orchd-sdk-0.1a3/src/orchd_sdk.egg-info/SOURCES 2.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-LICENSE.md
 README.md
 setup.py
 src/orchd_sdk/VERSION
 src/orchd_sdk/__init__.py
 src/orchd_sdk/cli.py
 src/orchd_sdk/common.py
 src/orchd_sdk/errors.py
 src/orchd_sdk/logger.ini
 src/orchd_sdk/logging.py
 src/orchd_sdk/models.py
 src/orchd_sdk/project.py
 src/orchd_sdk/reaction.py
+src/orchd_sdk/reaction.schema.json
 src/orchd_sdk/sensor.py
 src/orchd_sdk/sink.py
 src/orchd_sdk/util.py
 src/orchd_sdk.egg-info/PKG-INFO
 src/orchd_sdk.egg-info/SOURCES.txt
 src/orchd_sdk.egg-info/dependency_links.txt
 src/orchd_sdk.egg-info/entry_points.txt
```

