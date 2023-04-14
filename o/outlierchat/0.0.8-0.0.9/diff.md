# Comparing `tmp/outlierchat-0.0.8.tar.gz` & `tmp/outlierchat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outlierchat-0.0.8.tar", last modified: Thu Mar  9 18:41:59 2023, max compression
+gzip compressed data, was "outlierchat-0.0.9.tar", last modified: Thu Mar  9 18:53:53 2023, max compression
```

## Comparing `outlierchat-0.0.8.tar` & `outlierchat-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.622473 outlierchat-0.0.8/
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     2598 2023-03-09 18:41:59.622473 outlierchat-0.0.8/PKG-INFO
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     1874 2023-02-26 03:12:35.000000 outlierchat-0.0.8/README.md
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)       38 2023-03-09 18:41:59.622473 outlierchat-0.0.8/setup.cfg
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)      804 2023-03-09 18:41:47.000000 outlierchat-0.0.8/setup.py
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.602473 outlierchat-0.0.8/src/
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.606473 outlierchat-0.0.8/src/outlier/
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)      210 2023-03-09 18:38:18.000000 outlierchat-0.0.8/src/outlier/__init__.py
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.606473 outlierchat-0.0.8/src/outlier/biz/
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:37:07.000000 outlierchat-0.0.8/src/outlier/biz/__init__.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     2077 2023-03-09 03:54:12.000000 outlierchat-0.0.8/src/outlier/biz/beans.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)    11202 2023-03-09 12:55:38.000000 outlierchat-0.0.8/src/outlier/biz/bizservice.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     5162 2023-03-09 18:22:33.000000 outlierchat-0.0.8/src/outlier/client.py
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.610473 outlierchat-0.0.8/src/outlier/encryption/
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:38:24.000000 outlierchat-0.0.8/src/outlier/encryption/__init__.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     2614 2023-03-09 12:36:29.000000 outlierchat-0.0.8/src/outlier/encryption/protocol.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     4063 2023-03-09 12:34:20.000000 outlierchat-0.0.8/src/outlier/encryption/sessionservice.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     5740 2023-03-09 18:22:20.000000 outlierchat-0.0.8/src/outlier/server.py
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.614473 outlierchat-0.0.8/src/outlier/tools/
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:38:26.000000 outlierchat-0.0.8/src/outlier/tools/__init__.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)       90 2023-03-08 15:10:22.000000 outlierchat-0.0.8/src/outlier/tools/aux.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     1082 2023-03-09 08:55:15.000000 outlierchat-0.0.8/src/outlier/tools/decorators.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     3016 2023-03-09 08:56:01.000000 outlierchat-0.0.8/src/outlier/tools/threadpool.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     1258 2023-03-09 08:55:08.000000 outlierchat-0.0.8/src/outlier/tools/utils.py
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.614473 outlierchat-0.0.8/src/outlier/transmission/
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:38:28.000000 outlierchat-0.0.8/src/outlier/transmission/__init__.py
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     7775 2023-03-09 12:56:26.000000 outlierchat-0.0.8/src/outlier/transmission/tcpservice.py
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.618473 outlierchat-0.0.8/src/outlierchat.egg-info/
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     2598 2023-03-09 18:41:59.000000 outlierchat-0.0.8/src/outlierchat.egg-info/PKG-INFO
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)      682 2023-03-09 18:41:59.000000 outlierchat-0.0.8/src/outlierchat.egg-info/SOURCES.txt
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        1 2023-03-09 18:41:59.000000 outlierchat-0.0.8/src/outlierchat.egg-info/dependency_links.txt
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        8 2023-03-09 18:41:59.000000 outlierchat-0.0.8/src/outlierchat.egg-info/top_level.txt
-drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:41:59.622473 outlierchat-0.0.8/test/
--rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     1107 2023-03-08 15:10:22.000000 outlierchat-0.0.8/test/test_threadpool.py
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.811234 outlierchat-0.0.9/
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     2598 2023-03-09 18:53:53.811234 outlierchat-0.0.9/PKG-INFO
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     1874 2023-02-26 03:12:35.000000 outlierchat-0.0.9/README.md
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)       38 2023-03-09 18:53:53.811234 outlierchat-0.0.9/setup.cfg
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)      799 2023-03-09 18:53:09.000000 outlierchat-0.0.9/setup.py
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.795234 outlierchat-0.0.9/src/
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.799234 outlierchat-0.0.9/src/outlier/
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)      210 2023-03-09 18:38:18.000000 outlierchat-0.0.9/src/outlier/__init__.py
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.803234 outlierchat-0.0.9/src/outlier/biz/
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:37:07.000000 outlierchat-0.0.9/src/outlier/biz/__init__.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     2077 2023-03-09 03:54:12.000000 outlierchat-0.0.9/src/outlier/biz/beans.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)    11206 2023-03-09 18:43:33.000000 outlierchat-0.0.9/src/outlier/biz/bizservice.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     5157 2023-03-09 18:47:49.000000 outlierchat-0.0.9/src/outlier/client.py
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.803234 outlierchat-0.0.9/src/outlier/encryption/
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:38:24.000000 outlierchat-0.0.9/src/outlier/encryption/__init__.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     2614 2023-03-09 12:36:29.000000 outlierchat-0.0.9/src/outlier/encryption/protocol.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     4069 2023-03-09 18:44:00.000000 outlierchat-0.0.9/src/outlier/encryption/sessionservice.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     5740 2023-03-09 18:47:27.000000 outlierchat-0.0.9/src/outlier/server.py
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.807234 outlierchat-0.0.9/src/outlier/tools/
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:38:26.000000 outlierchat-0.0.9/src/outlier/tools/__init__.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)       90 2023-03-08 15:10:22.000000 outlierchat-0.0.9/src/outlier/tools/aux.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     1082 2023-03-09 08:55:15.000000 outlierchat-0.0.9/src/outlier/tools/decorators.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     3016 2023-03-09 08:56:01.000000 outlierchat-0.0.9/src/outlier/tools/threadpool.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     1258 2023-03-09 08:55:08.000000 outlierchat-0.0.9/src/outlier/tools/utils.py
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.807234 outlierchat-0.0.9/src/outlier/transmission/
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:38:28.000000 outlierchat-0.0.9/src/outlier/transmission/__init__.py
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     7783 2023-03-09 18:47:15.000000 outlierchat-0.0.9/src/outlier/transmission/tcpservice.py
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.811234 outlierchat-0.0.9/src/outlierchat.egg-info/
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     2598 2023-03-09 18:53:53.000000 outlierchat-0.0.9/src/outlierchat.egg-info/PKG-INFO
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)      682 2023-03-09 18:53:53.000000 outlierchat-0.0.9/src/outlierchat.egg-info/SOURCES.txt
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        1 2023-03-09 18:53:53.000000 outlierchat-0.0.9/src/outlierchat.egg-info/dependency_links.txt
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)        8 2023-03-09 18:53:53.000000 outlierchat-0.0.9/src/outlierchat.egg-info/top_level.txt
+drwxrwxr-x   0 phoenix   (1002) phoenix   (1002)        0 2023-03-09 18:53:53.811234 outlierchat-0.0.9/test/
+-rw-rw-r--   0 phoenix   (1002) phoenix   (1002)     1107 2023-03-08 15:10:22.000000 outlierchat-0.0.9/test/test_threadpool.py
```

### Comparing `outlierchat-0.0.8/PKG-INFO` & `outlierchat-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outlierchat
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple server to build a secret channel for chat.
 Home-page: UNKNOWN
 Author: Thetis
 Author-email: 736396627@qq.com
 License: UNKNOWN
 Description: <!--
          * @Date: 2023-01-07 22:59:34
```

### Comparing `outlierchat-0.0.8/README.md` & `outlierchat-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `outlierchat-0.0.8/src/outlier/biz/beans.py` & `outlierchat-0.0.9/src/outlier/biz/beans.py`

 * *Files identical despite different names*

### Comparing `outlierchat-0.0.8/src/outlier/biz/bizservice.py` & `outlierchat-0.0.9/src/outlier/biz/bizservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Date: 2023-03-08 23:10:22
 LastEditors: ThetisEliza wxf199601@gmail.com
-LastEditTime: 2023-03-09 20:55:38
+LastEditTime: 2023-03-10 02:43:33
 FilePath: /outlier/src/outlier/biz/bizservice.py
 
 This is the key layer for bussniness implementation. We use server 
 as the `stem` update way, client follows. we use some way to add the biz
 respond function automatically and we use some way to make the client can
 easily correspoing to it.
 For exmaple,
@@ -43,16 +43,16 @@
 import logging
 import re
 import signal
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Callable, Dict, List
 
-from encryption.sessionservice import Package, Session, SessionService
-from transmission.tcpservice import Ops
+from ..encryption.sessionservice import Package, Session, SessionService
+from ..transmission.tcpservice import Ops
 
 
 class State(Enum):
     IDLE = -1
     Hall = 0
     Room = 1
     Cfrm = 2
```

### Comparing `outlierchat-0.0.8/src/outlier/client.py` & `outlierchat-0.0.9/src/outlier/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
 import time
 from argparse import ArgumentParser
 from typing import List
 
 from .biz.beans import ChatMessage
 from .biz.bizservice import BizRequest, ClientBizService, State, bizclnt
-from .biz.server import Server
 from .encryption.sessionservice import ConnectSessService, SessionService
 from .transmission.tcpservice import TcpConnectService
 
 from .tools.utils import initlogger
-
+from .server import Server
 
 class Client(ClientBizService):
     def __init__(self, sessservice: SessionService, **kwargs) -> None:
         super().__init__(sessservice, **kwargs)
         
         self.chatblock = False
         self.buffer: List[ChatMessage] = list()
```

### Comparing `outlierchat-0.0.8/src/outlier/encryption/protocol.py` & `outlierchat-0.0.9/src/outlier/encryption/protocol.py`

 * *Files identical despite different names*

### Comparing `outlierchat-0.0.8/src/outlier/encryption/sessionservice.py` & `outlierchat-0.0.9/src/outlier/encryption/sessionservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 '''
 Date: 2023-03-08 23:10:22
 LastEditors: ThetisEliza wxf199601@gmail.com
-LastEditTime: 2023-03-09 20:34:20
+LastEditTime: 2023-03-10 02:43:49
 FilePath: /outlier/src/outlier/encryption/sessionservice.py
 
 This module is to encrypt and decrypt tcp byteflow and provide better interfaces for business layer
 '''
 import logging
 from dataclasses import dataclass, field
-from typing import List, Set, Dict, Any
-from transmission.tcpservice import TcpService, Connection, Ops
+from typing import Any, Dict, List, Set
+
+from ..tools.decorators import singleton
+from ..transmission.tcpservice import Connection, Ops, TcpService
 from .protocol import Package
-from tools.decorators import singleton
+
 
 @dataclass
 class Session:
     """Encapsuled connection and organize it with group
     """
     conn:   Connection = None
     group:  int       = -1
```

### Comparing `outlierchat-0.0.8/src/outlier/server.py` & `outlierchat-0.0.9/src/outlier/server.py`

 * *Files identical despite different names*

### Comparing `outlierchat-0.0.8/src/outlier/tools/decorators.py` & `outlierchat-0.0.9/src/outlier/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `outlierchat-0.0.8/src/outlier/tools/threadpool.py` & `outlierchat-0.0.9/src/outlier/tools/threadpool.py`

 * *Files identical despite different names*

### Comparing `outlierchat-0.0.8/src/outlier/tools/utils.py` & `outlierchat-0.0.9/src/outlier/tools/utils.py`

 * *Files identical despite different names*

### Comparing `outlierchat-0.0.8/src/outlier/transmission/tcpservice.py` & `outlierchat-0.0.9/src/outlier/transmission/tcpservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 '''
 Date: 2023-03-08 23:10:22
 LastEditors: ThetisEliza wxf199601@gmail.com
-LastEditTime: 2023-03-09 20:56:15
+LastEditTime: 2023-03-10 02:47:10
 FilePath: /outlier/src/outlier/transmission/tcpservice.py
 
 This module is to provide stable and reliable layer communication as tcp protocol
 '''
 
-import socket
-import select
 import logging
+import select
+import socket
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Callable, Any, Dict
-from tools.threadpool import ThreadPool
-from tools.decorators import onexit, singleton
-from tools.aux import Ops
+from typing import Any, Callable, Dict
+
+from ..tools.aux import Ops
+from ..tools.decorators import onexit, singleton
+from ..tools.threadpool import ThreadPool
+
 
 @dataclass
 class Connection:
     sock: socket.socket
     addr: Any
     last: float
```

### Comparing `outlierchat-0.0.8/src/outlierchat.egg-info/PKG-INFO` & `outlierchat-0.0.9/src/outlierchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outlierchat
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple server to build a secret channel for chat.
 Home-page: UNKNOWN
 Author: Thetis
 Author-email: 736396627@qq.com
 License: UNKNOWN
 Description: <!--
          * @Date: 2023-01-07 22:59:34
```

### Comparing `outlierchat-0.0.8/src/outlierchat.egg-info/SOURCES.txt` & `outlierchat-0.0.9/src/outlierchat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `outlierchat-0.0.8/test/test_threadpool.py` & `outlierchat-0.0.9/test/test_threadpool.py`

 * *Files identical despite different names*

