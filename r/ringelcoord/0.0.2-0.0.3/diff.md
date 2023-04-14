# Comparing `tmp/ringelcoord-0.0.2.tar.gz` & `tmp/ringelcoord-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringelcoord-0.0.2.tar", last modified: Fri Apr 14 17:58:50 2023, max compression
+gzip compressed data, was "ringelcoord-0.0.3.tar", last modified: Fri Apr 14 18:02:18 2023, max compression
```

## Comparing `ringelcoord-0.0.2.tar` & `ringelcoord-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-14 17:58:50.818269 ringelcoord-0.0.2/
--rw-r--r--   0 john      (1000) john      (1000)    35149 2023-04-14 17:30:42.000000 ringelcoord-0.0.2/LICENSE
--rw-r--r--   0 john      (1000) john      (1000)      405 2023-04-14 17:58:50.818269 ringelcoord-0.0.2/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)       17 2023-04-14 17:34:49.000000 ringelcoord-0.0.2/README.md
--rw-r--r--   0 john      (1000) john      (1000)      440 2023-04-14 17:58:46.000000 ringelcoord-0.0.2/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)       38 2023-04-14 17:58:50.818269 ringelcoord-0.0.2/setup.cfg
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-14 17:58:50.818269 ringelcoord-0.0.2/src/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-14 17:58:50.818269 ringelcoord-0.0.2/src/ringelcoord/
--rw-r--r--   0 john      (1000) john      (1000)     2224 2023-04-14 17:58:31.000000 ringelcoord-0.0.2/src/ringelcoord/__init__.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-14 17:58:50.818269 ringelcoord-0.0.2/src/ringelcoord.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)      405 2023-04-14 17:58:50.000000 ringelcoord-0.0.2/src/ringelcoord.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      254 2023-04-14 17:58:50.000000 ringelcoord-0.0.2/src/ringelcoord.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-14 17:58:50.000000 ringelcoord-0.0.2/src/ringelcoord.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)       17 2023-04-14 17:58:50.000000 ringelcoord-0.0.2/src/ringelcoord.egg-info/requires.txt
--rw-r--r--   0 john      (1000) john      (1000)       12 2023-04-14 17:58:50.000000 ringelcoord-0.0.2/src/ringelcoord.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-14 18:02:18.060819 ringelcoord-0.0.3/
+-rw-r--r--   0 john      (1000) john      (1000)    35149 2023-04-14 17:30:42.000000 ringelcoord-0.0.3/LICENSE
+-rw-r--r--   0 john      (1000) john      (1000)      405 2023-04-14 18:02:18.060819 ringelcoord-0.0.3/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)       17 2023-04-14 17:34:49.000000 ringelcoord-0.0.3/README.md
+-rw-r--r--   0 john      (1000) john      (1000)      440 2023-04-14 18:01:30.000000 ringelcoord-0.0.3/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)       38 2023-04-14 18:02:18.060819 ringelcoord-0.0.3/setup.cfg
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-14 18:02:18.060819 ringelcoord-0.0.3/src/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-14 18:02:18.060819 ringelcoord-0.0.3/src/ringelcoord/
+-rw-r--r--   0 john      (1000) john      (1000)     2225 2023-04-14 18:00:58.000000 ringelcoord-0.0.3/src/ringelcoord/__init__.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-14 18:02:18.060819 ringelcoord-0.0.3/src/ringelcoord.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)      405 2023-04-14 18:02:18.000000 ringelcoord-0.0.3/src/ringelcoord.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      254 2023-04-14 18:02:18.000000 ringelcoord-0.0.3/src/ringelcoord.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-14 18:02:18.000000 ringelcoord-0.0.3/src/ringelcoord.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)       17 2023-04-14 18:02:18.000000 ringelcoord-0.0.3/src/ringelcoord.egg-info/requires.txt
+-rw-r--r--   0 john      (1000) john      (1000)       12 2023-04-14 18:02:18.000000 ringelcoord-0.0.3/src/ringelcoord.egg-info/top_level.txt
```

### Comparing `ringelcoord-0.0.2/LICENSE` & `ringelcoord-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ringelcoord-0.0.2/src/ringelcoord/__init__.py` & `ringelcoord-0.0.3/src/ringelcoord/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             content, context = await self.msg_queue.get()
             if isinstance(context, Message):
                 await sock.send(f"CLIENT::NEW_MSG::{context.recipient}::<REPLY:{context.id}> {content}")
 
 
     
     async def __actual_run(self, token):
-        async with websockets.connect("wss://{self.url}") as socket:
+        async with websockets.connect(f"wss://{self.url}") as socket:
             asyncio.get_event_loop().create_task(self.send_msgs(socket))
             async for x in socket:
                 if x.startswith("SERVER::VERSION"):
                     _, _, ver = x.split("::", 2)
                     assert ver == "0.4", "update ringelcoord"
                     await socket.send("CLIENT::VERSION::0.4")
                 elif x.startswith("SERVER::REQUEST_LOGIN"):
```

