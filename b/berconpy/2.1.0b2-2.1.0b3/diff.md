# Comparing `tmp/berconpy-2.1.0b2.tar.gz` & `tmp/berconpy-2.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berconpy-2.1.0b2.tar", last modified: Thu Mar 30 00:16:29 2023, max compression
+gzip compressed data, was "berconpy-2.1.0b3.tar", last modified: Mon Apr  3 17:44:23 2023, max compression
```

## Comparing `berconpy-2.1.0b2.tar` & `berconpy-2.1.0b3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 00:16:29.037119 berconpy-2.1.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-30 00:16:29.037119 berconpy-2.1.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 00:16:29.037119 berconpy-2.1.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 00:16:29.029119 berconpy-2.1.0b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 00:16:29.033119 berconpy-2.1.0b2/src/berconpy/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 00:16:29.033119 berconpy-2.1.0b2/src/berconpy/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/asyncio/ban.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/asyncio/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/asyncio/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19715 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/asyncio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/asyncio/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/ban.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 00:16:29.033119 berconpy-2.1.0b2/src/berconpy/ext/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 00:16:29.037119 berconpy-2.1.0b2/src/berconpy/ext/arma/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/ext/arma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/ext/arma/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 00:16:29.037119 berconpy-2.1.0b2/src/berconpy/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/protocol/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/protocol/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/protocol/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/protocol/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/protocol/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/protocol/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-30 00:16:13.000000 berconpy-2.1.0b2/src/berconpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 00:16:29.033119 berconpy-2.1.0b2/src/berconpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-30 00:16:29.000000 berconpy-2.1.0b2/src/berconpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-30 00:16:29.000000 berconpy-2.1.0b2/src/berconpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 00:16:29.000000 berconpy-2.1.0b2/src/berconpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-30 00:16:29.000000 berconpy-2.1.0b2/src/berconpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-30 00:16:29.000000 berconpy-2.1.0b2/src/berconpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:44:23.672112 berconpy-2.1.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-03 17:44:23.672112 berconpy-2.1.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 17:44:23.672112 berconpy-2.1.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:44:23.668112 berconpy-2.1.0b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:44:23.668112 berconpy-2.1.0b3/src/berconpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:44:23.672112 berconpy-2.1.0b3/src/berconpy/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/asyncio/ban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/asyncio/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/asyncio/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/asyncio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/asyncio/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/ban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:44:23.668112 berconpy-2.1.0b3/src/berconpy/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:44:23.672112 berconpy-2.1.0b3/src/berconpy/ext/arma/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/ext/arma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/ext/arma/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:44:23.672112 berconpy-2.1.0b3/src/berconpy/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/protocol/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/protocol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/protocol/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/protocol/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15511 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/protocol/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/protocol/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-03 17:44:09.000000 berconpy-2.1.0b3/src/berconpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 17:44:23.672112 berconpy-2.1.0b3/src/berconpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-03 17:44:23.000000 berconpy-2.1.0b3/src/berconpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-03 17:44:23.000000 berconpy-2.1.0b3/src/berconpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 17:44:23.000000 berconpy-2.1.0b3/src/berconpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-03 17:44:23.000000 berconpy-2.1.0b3/src/berconpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-03 17:44:23.000000 berconpy-2.1.0b3/src/berconpy.egg-info/top_level.txt
```

### Comparing `berconpy-2.1.0b2/LICENSE` & `berconpy-2.1.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/PKG-INFO` & `berconpy-2.1.0b3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berconpy
-Version: 2.1.0b2
+Version: 2.1.0b3
 Summary: An async wrapper for the BattlEye RCON protocol
 Author: thegamecracks
 License: MIT
 Project-URL: Homepage, https://github.com/thegamecracks/berconpy
 Project-URL: Documentation, http://berconpy.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/thegamecracks/berconpy/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `berconpy-2.1.0b2/README.md` & `berconpy-2.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/pyproject.toml` & `berconpy-2.1.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/__init__.py` & `berconpy-2.1.0b3/src/berconpy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     ServerAuthEvent,
     ServerCommandEvent,
     ServerEvent,
     ServerMessageEvent,
     ServerState,
 )
 
-__version__ = "2.1.0b2"
+__version__ = "2.1.0b3"
```

### Comparing `berconpy-2.1.0b2/src/berconpy/asyncio/ban.py` & `berconpy-2.1.0b3/src/berconpy/asyncio/ban.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/asyncio/cache.py` & `berconpy-2.1.0b3/src/berconpy/asyncio/cache.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/asyncio/client.py` & `berconpy-2.1.0b3/src/berconpy/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/asyncio/dispatch.py` & `berconpy-2.1.0b3/src/berconpy/asyncio/dispatch.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/asyncio/io.py` & `berconpy-2.1.0b3/src/berconpy/asyncio/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,18 +442,17 @@
                 self._reset_protocol()
                 self._is_logged_in = loop.create_future()
                 continue
 
             elapsed_time = time.monotonic() - self._last_command
             if elapsed_time > self.config.keep_alive_interval:
                 log.debug("sending keep alive packet")
-                asyncio.create_task(
-                    self._send_keep_alive(),
-                    name="berconpy-keep-alive",
-                )
+                # NOTE: may result in "Task destroyed but it is pending!"
+                #       TaskGroup would be a good idea here
+                keep_alive_task = self._begin_keep_alive()
 
             try:
                 coro = self._close_event.wait()
                 await asyncio.wait_for(coro, timeout=self.config.run_interval)
             except asyncio.TimeoutError:
                 pass
 
@@ -505,15 +504,27 @@
 
                 # exponential backoff
                 self.disconnect()
                 await asyncio.sleep(2 ** (i % 11))
 
         return False
 
-    async def _send_keep_alive(self):
+    def _begin_keep_alive(self) -> asyncio.Task[None]:
+        def done_callback(task: asyncio.Task):
+            if not isinstance(task.exception(), RCONCommandError):
+                task.result()  # unexpected error
+
+        task = asyncio.create_task(
+            self._send_keep_alive(),
+            name="berconpy-keep-alive",
+        )
+        task.add_done_callback(done_callback)
+        return task
+
+    async def _send_keep_alive(self) -> None:
         assert self.client is not None
 
         if time.monotonic() - self._last_players > self.config.players_interval:
             # Instead of an empty message, ask for players so we can
             # periodically update the client's cache
             self._last_players = time.monotonic()
             response = await self.send_command("players")
```

### Comparing `berconpy-2.1.0b2/src/berconpy/asyncio/player.py` & `berconpy-2.1.0b3/src/berconpy/asyncio/player.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/ban.py` & `berconpy-2.1.0b3/src/berconpy/ban.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/cache.py` & `berconpy-2.1.0b3/src/berconpy/cache.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/client.py` & `berconpy-2.1.0b3/src/berconpy/client.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/dispatch.py` & `berconpy-2.1.0b3/src/berconpy/dispatch.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/ext/arma/client.py` & `berconpy-2.1.0b3/src/berconpy/ext/arma/client.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/parser.py` & `berconpy-2.1.0b3/src/berconpy/parser.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/player.py` & `berconpy-2.1.0b3/src/berconpy/player.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/protocol/__init__.py` & `berconpy-2.1.0b3/src/berconpy/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/protocol/base.py` & `berconpy-2.1.0b3/src/berconpy/protocol/base.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/protocol/check.py` & `berconpy-2.1.0b3/src/berconpy/protocol/check.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/protocol/client.py` & `berconpy-2.1.0b3/src/berconpy/protocol/client.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/protocol/errors.py` & `berconpy-2.1.0b3/src/berconpy/protocol/errors.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/protocol/events.py` & `berconpy-2.1.0b3/src/berconpy/protocol/events.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/protocol/packet.py` & `berconpy-2.1.0b3/src/berconpy/protocol/packet.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/protocol/server.py` & `berconpy-2.1.0b3/src/berconpy/protocol/server.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy/utils.py` & `berconpy-2.1.0b3/src/berconpy/utils.py`

 * *Files identical despite different names*

### Comparing `berconpy-2.1.0b2/src/berconpy.egg-info/PKG-INFO` & `berconpy-2.1.0b3/src/berconpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berconpy
-Version: 2.1.0b2
+Version: 2.1.0b3
 Summary: An async wrapper for the BattlEye RCON protocol
 Author: thegamecracks
 License: MIT
 Project-URL: Homepage, https://github.com/thegamecracks/berconpy
 Project-URL: Documentation, http://berconpy.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/thegamecracks/berconpy/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `berconpy-2.1.0b2/src/berconpy.egg-info/SOURCES.txt` & `berconpy-2.1.0b3/src/berconpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

