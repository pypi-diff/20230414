# Comparing `tmp/codingame-1.4.1.tar.gz` & `tmp/codingame-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codingame-1.4.1.tar", last modified: Sat Feb 11 20:02:48 2023, max compression
+gzip compressed data, was "codingame-1.4.2.tar", last modified: Fri Apr 14 20:14:02 2023, max compression
```

## Comparing `codingame-1.4.1.tar` & `codingame-1.4.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:02:48.587972 codingame-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-11 20:02:38.000000 codingame-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-02-11 20:02:48.587972 codingame-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-02-11 20:02:38.000000 codingame-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:02:48.583972 codingame-1.4.1/codingame/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/clash_of_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:02:48.583972 codingame-1.4.1/codingame/client/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10594 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/client/async_.py
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/client/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/codingamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:02:48.587972 codingame-1.4.1/codingame/http/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/http/async_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/http/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/http/httperror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/http/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/leaderboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:02:48.587972 codingame-1.4.1/codingame/notification/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22294 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/notification/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/notification/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/notification/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:02:48.587972 codingame-1.4.1/codingame/types/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/types/clash_of_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/types/codingamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/types/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-02-11 20:02:38.000000 codingame-1.4.1/codingame/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 20:02:48.583972 codingame-1.4.1/codingame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-02-11 20:02:48.000000 codingame-1.4.1/codingame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-11 20:02:48.000000 codingame-1.4.1/codingame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 20:02:48.000000 codingame-1.4.1/codingame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-11 20:02:48.000000 codingame-1.4.1/codingame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-11 20:02:48.000000 codingame-1.4.1/codingame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-11 20:02:48.587972 codingame-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-02-11 20:02:38.000000 codingame-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:14:02.321656 codingame-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 20:13:53.000000 codingame-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-14 20:14:02.321656 codingame-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-14 20:13:53.000000 codingame-1.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:14:02.317656 codingame-1.4.2/codingame/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/clash_of_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:14:02.321656 codingame-1.4.2/codingame/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/client/async_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/client/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/codingamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:14:02.321656 codingame-1.4.2/codingame/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/http/async_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/http/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/http/httperror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/http/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/leaderboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:14:02.321656 codingame-1.4.2/codingame/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22294 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/notification/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/notification/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/notification/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:14:02.321656 codingame-1.4.2/codingame/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/types/clash_of_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/types/codingamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/types/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-14 20:13:53.000000 codingame-1.4.2/codingame/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:14:02.317656 codingame-1.4.2/codingame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-14 20:14:02.000000 codingame-1.4.2/codingame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-14 20:14:02.000000 codingame-1.4.2/codingame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:14:02.000000 codingame-1.4.2/codingame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 20:14:02.000000 codingame-1.4.2/codingame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 20:14:02.000000 codingame-1.4.2/codingame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-14 20:14:02.321656 codingame-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-14 20:13:53.000000 codingame-1.4.2/setup.py
```

### Comparing `codingame-1.4.1/LICENSE` & `codingame-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/PKG-INFO` & `codingame-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codingame
-Version: 1.4.1
+Version: 1.4.2
 Summary: Pythonic wrapper for the undocumented CodinGame API.
 Home-page: https://github.com/takos22/codingame
 Author: takos22
 Author-email: takos2210@gmail.com
 License: MIT
 Project-URL: Documentation, https://codingame.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/takos22/codingame/issues
```

### Comparing `codingame-1.4.1/README.rst` & `codingame-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/__init__.py` & `codingame-1.4.2/codingame/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 from typing import NamedTuple
 
 VersionInfo = NamedTuple(
     "VersionInfo", major=int, minor=int, micro=int, releaselevel=str, serial=int
 )
 
-version_info = VersionInfo(major=1, minor=4, micro=1, releaselevel="", serial=0)
+version_info = VersionInfo(major=1, minor=4, micro=2, releaselevel="", serial=0)
 
 __title__ = "codingame"
 __author__ = "takos22"
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 from .clash_of_code import ClashOfCode, Player
 from .client import Client
 from .codingamer import CodinGamer, PartialCodinGamer
 from .exceptions import (
     ChallengeNotFound,
     ClashOfCodeNotFound,
```

### Comparing `codingame-1.4.1/codingame/abc.py` & `codingame-1.4.2/codingame/abc.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/clash_of_code.py` & `codingame-1.4.2/codingame/clash_of_code.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/client/async_.py` & `codingame-1.4.2/codingame/client/async_.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                     "clash_of_code", f"No Clash of Code with handle {handle!r}"
                 ) from None
             raise  # pragma: no cover
         return ClashOfCode(self._state, data)
 
     async def get_pending_clash_of_code(self) -> typing.Optional[ClashOfCode]:
         data: list = await self._state.http.get_pending_clash_of_code()
-        if len(data) == 0:
+        if not data:
             return None  # pragma: no cover
         return ClashOfCode(self._state, data[0])  # pragma: no cover
 
     # --------------------------------------------------------------------------
     # Language IDs
 
     async def get_language_ids(self) -> typing.List[str]:
@@ -270,15 +270,18 @@
         try:
             data = await self._state.http.get_challenge_leaderboard(
                 challenge_id,
                 group,
                 self.codingamer.public_handle if self.logged_in else "",
             )
         except HTTPError as error:
-            if error.data["id"] == 702:
+            if (
+                error.data.get("id") == 702
+                or error.data.get("code") == "NOT_FOUND"
+            ):  # see issue #26
                 raise NotFound.from_type(
                     "challenge", f"No Challenge named {challenge_id!r}"
                 ) from None
             raise  # pragma: no cover
 
         return ChallengeLeaderboard(self._state, challenge_id, group, data)
```

### Comparing `codingame-1.4.1/codingame/client/base.py` & `codingame-1.4.2/codingame/client/base.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/client/client.py` & `codingame-1.4.2/codingame/client/client.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/client/sync.py` & `codingame-1.4.2/codingame/client/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                     "clash_of_code", f"No Clash of Code with handle {handle!r}"
                 ) from None
             raise  # pragma: no cover
         return ClashOfCode(self._state, data)
 
     def get_pending_clash_of_code(self) -> typing.Optional[ClashOfCode]:
         data: list = self._state.http.get_pending_clash_of_code()
-        if len(data) == 0:
+        if not data:
             return None  # pragma: no cover
         return ClashOfCode(self._state, data[0])  # pragma: no cover
 
     # --------------------------------------------------------------------------
     # Language IDs
 
     def get_language_ids(self) -> typing.List[str]:
@@ -261,15 +261,18 @@
         try:
             data = self._state.http.get_challenge_leaderboard(
                 challenge_id,
                 group,
                 self.codingamer.public_handle if self.logged_in else "",
             )
         except HTTPError as error:
-            if error.data["id"] == 702:
+            if (
+                error.data.get("id") == 702
+                or error.data.get("code") == "NOT_FOUND"
+            ):  # see issue #26
                 raise NotFound.from_type(
                     "challenge", f"No Challenge named {challenge_id!r}"
                 ) from None
             raise  # pragma: no cover
 
         return ChallengeLeaderboard(self._state, challenge_id, group, data)
```

### Comparing `codingame-1.4.1/codingame/codingamer.py` & `codingame-1.4.2/codingame/codingamer.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/exceptions.py` & `codingame-1.4.2/codingame/exceptions.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/http/async_.py` & `codingame-1.4.2/codingame/http/async_.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,18 @@
     @property
     def is_async(self):
         return True
 
     async def close(self):
         await self.__session.close()
 
-    async def request(self, service: str, func: str, parameters: list = []):
+    async def request(
+        self, service: str, func: str, parameters: typing.Optional[list] = None
+    ):
+        parameters = parameters or []
         url = self.API_URL + service + "/" + func
         async with self.__session.post(url, json=parameters) as response:
             data = await response.json()
             try:
                 response.raise_for_status()
             except aiohttp.ClientResponseError as error:
                 raise HTTPError.from_aiohttp(error, data) from None
```

### Comparing `codingame-1.4.1/codingame/http/base.py` & `codingame-1.4.2/codingame/http/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 
 if typing.TYPE_CHECKING:
     from ..state import ConnectionState
 
 __all__ = ("BaseHTTPClient",)
 
 
+DEFAULT_FILTER = {
+    "active": False,
+    "keyword": "",
+    "column": "",
+    "filter": "",
+}
+
+
 class BaseHTTPClient(ABC):
     BASE_URL = "https://www.codingame.com"
     API_URL = BASE_URL + "/services/"
     STATIC_URL = "https://static.codingame.com"
 
     headers: dict = {
         "User-Agent": (
@@ -35,15 +43,17 @@
         ...  # pragma: no cover
 
     @abstractmethod
     def close(self):
         ...  # pragma: no cover
 
     @abstractmethod
-    def request(self, service: str, func: str, parameters: list = []):
+    def request(
+        self, service: str, func: str, parameters: typing.Optional[list] = None
+    ):
         ...  # pragma: no cover
 
     @abstractmethod
     def set_cookie(
         self,
         name: str,
         value: typing.Optional[str] = None,
@@ -146,55 +156,43 @@
 
     def get_global_leaderboard(
         self,
         page: int,
         type: str,
         group: str,
         handle: str = "",
-        filter: dict = {
-            "active": False,
-            "keyword": "",
-            "column": "",
-            "filter": "",
-        },
+        filter: typing.Optional[dict] = None,
     ):
+        filter = filter or DEFAULT_FILTER
         return self.request(
             "Leaderboards",
             "getGlobalLeaderboard",
             [page, type, filter, handle, True, group],
         )
 
     def get_challenge_leaderboard(
         self,
         challenge_id: str,
         group: str,
         handle: str = "",
-        filter: dict = {
-            "active": False,
-            "keyword": "",
-            "column": "",
-            "filter": "",
-        },
+        filter: typing.Optional[dict] = None,
     ):
+        filter = filter or DEFAULT_FILTER
         return self.request(
             "Leaderboards",
             "getFilteredChallengeLeaderboard",
             [challenge_id, handle, group, filter],
         )
 
     def get_puzzle_leaderboard(
         self,
         puzzle_id: str,
         group: str,
         handle: str = "",
-        filter: dict = {
-            "active": False,
-            "keyword": "",
-            "column": "",
-            "filter": "",
-        },
+        filter: typing.Optional[dict] = None,
     ):
+        filter = filter or DEFAULT_FILTER
         return self.request(
             "Leaderboards",
             "getFilteredPuzzleLeaderboard",
             [puzzle_id, handle, group, filter],
         )
```

### Comparing `codingame-1.4.1/codingame/http/httperror.py` & `codingame-1.4.2/codingame/http/httperror.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/http/sync.py` & `codingame-1.4.2/codingame/http/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,18 @@
     @property
     def is_async(self) -> bool:
         return False
 
     def close(self):
         self.__session.close()
 
-    def request(self, service: str, func: str, parameters: list = []):
+    def request(
+        self, service: str, func: str, parameters: typing.Optional[list] = None
+    ):
+        parameters = parameters or []
         url = self.API_URL + service + "/" + func
         with self.__session.post(
             url, json=parameters, headers=self.headers
         ) as response:
             data = response.json()
             try:
                 response.raise_for_status()
```

### Comparing `codingame-1.4.1/codingame/leaderboard.py` & `codingame-1.4.2/codingame/leaderboard.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/notification/__init__.py` & `codingame-1.4.2/codingame/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/notification/data.py` & `codingame-1.4.2/codingame/notification/data.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/notification/enums.py` & `codingame-1.4.2/codingame/notification/enums.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/notification/notification.py` & `codingame-1.4.2/codingame/notification/notification.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/state.py` & `codingame-1.4.2/codingame/state.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/types/clash_of_code.py` & `codingame-1.4.2/codingame/types/clash_of_code.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/types/codingamer.py` & `codingame-1.4.2/codingame/types/codingamer.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/types/notification.py` & `codingame-1.4.2/codingame/types/notification.py`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/codingame/utils.py` & `codingame-1.4.2/codingame/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,19 @@
         "OPTIM",
         "CODEGOLF",
     ]:
         raise ValueError(
             "type argument must be one of: GENERAL, CONTESTS, "
             f"BOT_PROGRAMMING, OPTIM, CODEGOLF. Got: {type}"
         )
+
     return type
 
 
-def validate_leaderboard_group(group: str, logged_in: bool) -> bool:
+def validate_leaderboard_group(group: str, logged_in: bool) -> str:
     """Validates that the leaderboard group is one of ``"global"``,
     ``"country"``, ``"company"``, ``"school"`` or ``"following"`` and that the
     user is logged in except for ``"global"``.
 
     Parameters
     ----------
         type : :class:`str`
@@ -88,14 +89,16 @@
             "group argument must be one of: global, country, company, "
             f"school, following. Got: {group}"
         )
 
     if group in ["country", "company", "school", "following"] and not logged_in:
         raise LoginRequired()
 
+    return group
+
 
 DT_FORMAT_1 = "%b %d, %Y %I:%M:%S %p"
 DT_FORMAT_2 = "%b %d, %Y, %I:%M:%S %p"  # see issue #23
 
 
 def to_datetime(data: typing.Optional[typing.Union[int, str]]) -> datetime:
     if isinstance(data, int):
```

### Comparing `codingame-1.4.1/codingame.egg-info/PKG-INFO` & `codingame-1.4.2/codingame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codingame
-Version: 1.4.1
+Version: 1.4.2
 Summary: Pythonic wrapper for the undocumented CodinGame API.
 Home-page: https://github.com/takos22/codingame
 Author: takos22
 Author-email: takos2210@gmail.com
 License: MIT
 Project-URL: Documentation, https://codingame.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/takos22/codingame/issues
```

### Comparing `codingame-1.4.1/codingame.egg-info/SOURCES.txt` & `codingame-1.4.2/codingame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/setup.cfg` & `codingame-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `codingame-1.4.1/setup.py` & `codingame-1.4.2/setup.py`

 * *Files identical despite different names*

