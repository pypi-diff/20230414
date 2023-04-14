# Comparing `tmp/easy-events-2.8.2.tar.gz` & `tmp/easy-events-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-events-2.8.2.tar", last modified: Thu Apr  6 07:35:20 2023, max compression
+gzip compressed data, was "easy-events-2.9.0.tar", last modified: Fri Apr 14 08:48:42 2023, max compression
```

## Comparing `easy-events-2.8.2.tar` & `easy-events-2.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 07:35:20.728688 easy-events-2.8.2/
--rw-rw-rw-   0        0        0     1090 2023-03-11 04:58:56.000000 easy-events-2.8.2/LICENSE
--rw-rw-rw-   0        0        0     1962 2023-04-06 07:35:20.729704 easy-events-2.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     1358 2023-04-05 12:21:15.000000 easy-events-2.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 07:35:20.706700 easy-events-2.8.2/easy_events/
--rw-rw-rw-   0        0        0      359 2023-04-01 02:18:12.000000 easy-events-2.8.2/easy_events/__init__.py
--rw-rw-rw-   0        0        0     7122 2023-04-05 12:11:10.000000 easy-events-2.8.2/easy_events/async_events.py
--rw-rw-rw-   0        0        0     6825 2023-04-06 07:16:18.000000 easy-events-2.8.2/easy_events/events.py
--rw-rw-rw-   0        0        0     6180 2023-03-11 04:58:56.000000 easy-events-2.8.2/easy_events/objects.py
--rw-rw-rw-   0        0        0     5039 2023-04-06 07:33:41.000000 easy-events-2.8.2/easy_events/simple_events.py
-drwxrwxrwx   0        0        0        0 2023-04-06 07:35:20.724689 easy-events-2.8.2/easy_events.egg-info/
--rw-rw-rw-   0        0        0     1962 2023-04-06 07:35:20.000000 easy-events-2.8.2/easy_events.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-06 07:35:20.000000 easy-events-2.8.2/easy_events.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 07:35:20.000000 easy-events-2.8.2/easy_events.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-06 07:35:20.000000 easy-events-2.8.2/easy_events.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 07:35:20.733688 easy-events-2.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1157 2023-04-06 07:35:15.000000 easy-events-2.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:48:42.208683 easy-events-2.9.0/
+-rw-rw-rw-   0        0        0     1090 2023-03-11 04:58:56.000000 easy-events-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0     1962 2023-04-14 08:48:42.209681 easy-events-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1358 2023-04-05 12:21:15.000000 easy-events-2.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 08:48:42.180535 easy-events-2.9.0/easy_events/
+-rw-rw-rw-   0        0        0      359 2023-04-01 02:18:12.000000 easy-events-2.9.0/easy_events/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-04-13 21:43:59.000000 easy-events-2.9.0/easy_events/async_events.py
+-rw-rw-rw-   0        0        0     7003 2023-04-13 21:45:34.000000 easy-events-2.9.0/easy_events/events.py
+-rw-rw-rw-   0        0        0     6180 2023-03-11 04:58:56.000000 easy-events-2.9.0/easy_events/objects.py
+-rw-rw-rw-   0        0        0     5039 2023-04-07 20:31:08.000000 easy-events-2.9.0/easy_events/simple_events.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:48:42.202534 easy-events-2.9.0/easy_events.egg-info/
+-rw-rw-rw-   0        0        0     1962 2023-04-14 08:48:41.000000 easy-events-2.9.0/easy_events.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-04-14 08:48:41.000000 easy-events-2.9.0/easy_events.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:48:41.000000 easy-events-2.9.0/easy_events.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 08:48:41.000000 easy-events-2.9.0/easy_events.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 08:48:42.216683 easy-events-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1157 2023-04-14 08:48:35.000000 easy-events-2.9.0/setup.py
```

### Comparing `easy-events-2.8.2/LICENSE` & `easy-events-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-events-2.8.2/PKG-INFO` & `easy-events-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-events
-Version: 2.8.2
+Version: 2.9.0
 Summary: An universal wrapper (and useful tool) to make event / commands in python
 Home-page: https://github.com/ThePhoenix78/easy-events
 Download-URL: https://github.com/ThePhoenix78/easy-events/tarball/master
 Author: ThePhoenix78
 Author-email: thephoenix788@gmail.com
 License: MIT
 Keywords: wrapper,event,commands,command
```

### Comparing `easy-events-2.8.2/README.md` & `easy-events-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `easy-events-2.8.2/easy_events/async_events.py` & `easy-events-2.9.0/easy_events/async_events.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from inspect import getfullargspec
 from threading import Thread
 from asyncio import (
-    gather,
     wait_for,
     new_event_loop,
     iscoroutinefunction,
-    run_coroutine_threadsafe,
     AbstractEventLoop,
     TimeoutError,
     Future
 )
 import asyncio
 
 try:
@@ -144,15 +142,15 @@
                 return await com()
 
             if self.first_parameter_object:
                 return await com(data, **dico)
 
             return await com(**dico)
 
-    async def trigger(self, data, event_type: str = None, str_only: bool = None):
+    async def trigger(self, data, event_type: str = None, str_only: bool = None, thread: bool = False):
         none = type(None)
 
         if isinstance(str_only, none):
             str_only = self._str_only
 
         args = data
 
@@ -160,15 +158,19 @@
             pass
         elif not str(type(data)) == "<class 'easy_events.objects.Parameters'>":
             args = Parameters(data, self.prefix, str_only)
 
         event = self.grab_event(args._event, event_type)
 
         if isinstance(args._event, str) and event and args._called:
-            return await self.execute(event, args)
+            if thread:
+                loop = self.start_async_thread()
+                self.submit_async_thread(self.execute(event, args), loop)
+            else:
+                return await self.execute(event, args)
 
     def add_task(self, data, event_type: str = None, str_only: bool = None):
         none = type(None)
 
         if isinstance(str_only, none):
             str_only = self._str_only
 
@@ -200,14 +202,25 @@
             Thread(target=self._exec).start()
         else:
             self._exec()
 
     def _exec(self):
         asyncio.run(self.run_task())
 
+    def start_async_thread(self):
+        loop = asyncio.new_event_loop()
+        Thread(target=loop.run_forever).start()
+        return loop
+
+    def submit_async_thread(self, awaitable, loop):
+        return asyncio.run_coroutine_threadsafe(awaitable, loop)
+
+    def stop_async_thread(self, loop):
+        loop.call_soon_threadsafe(loop.stop)
+
     async def _thread(self):
         while self._run:
             await self.run_task()
             await asyncio.sleep(.1)
 
     def run(self):
         asyncio.run(self._thread())
@@ -215,34 +228,37 @@
 
 if __name__ == "__main__":
 
     client = AsyncEvents(first_parameter_object=False)
 
     @client.event()
     async def hello(*, world):
-        # await asyncio.sleep(1)
+        await asyncio.sleep(1)
         print(f"Hello {world}")
+
         return f"Hello {world}"
 
     def build_data(data):
         data.image = "png"
         data.file = "txt"
 
 
     data = Parameters("hello", client.prefix)
     build_data(data)
     data = client.add_task(data)
     # print(0, data)
 
-    data = client.add_task({"event": "hello", "parameters": {"world": "world", "lol": "data"}})
-    # print(1, data)
+    async def main():
+        data = await client.trigger({"event": "hello", "parameters": {"world": "world", "lol": "data"}}, thread=True)
+        # print(1, data)
 
-    data = client.add_task({"event": "hello", "parameters": ["world", "data"]})
-    # print(2, data)
+        data = await client.trigger({"event": "hello", "parameters": ["world", "data"]}, thread=True)
+        # print(2, data)
 
-    data = client.add_task(["hello", "world", "data"])
-    # print(3, data)
+        data = await client.trigger(["hello", "world", "data"])
+        # print(3, data)
 
-    data = client.add_task("hello world data4")
-    # print(4, data)
+        data = await client.trigger("hello world data4")
+        # print(4, data)
 
-    client.run_task_sync()
+    asyncio.run(main())
+    # client.run_task_sync()
```

### Comparing `easy-events-2.8.2/easy_events/events.py` & `easy-events-2.9.0/easy_events/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                 return com()
 
             if self.first_parameter_object:
                 return com(data, **dico)
 
             return com(**dico)
 
-    def trigger(self, data, event_type: str = None, str_only: bool = None):
+    def trigger(self, data, event_type: str = None, str_only: bool = None, thread: bool = False):
         none = type(None)
 
         if isinstance(str_only, none):
             str_only = self._str_only
 
         args = data
 
@@ -151,15 +151,19 @@
         elif not str(type(data)) == "<class 'easy_events.objects.Parameters'>":
             args = Parameters(data, self.prefix, str_only)
 
         event = self.grab_event(args._event, event_type)
 
         if isinstance(args._event, str) and event and args._called:
             try:
-                val = self.execute(event, args)
+                if thread:
+                    Thread(target=self.execute, args=[event, args]).start()
+                    return
+                else:
+                    val = self.execute(event, args)
             except Exception as e:
                 raise e
                 return f"{type(e)}: {e}"
 
             if isinstance(val, Parameters):
                 return val.transform()
```

### Comparing `easy-events-2.8.2/easy_events/objects.py` & `easy-events-2.9.0/easy_events/objects.py`

 * *Files identical despite different names*

### Comparing `easy-events-2.8.2/easy_events/simple_events.py` & `easy-events-2.9.0/easy_events/simple_events.py`

 * *Files identical despite different names*

### Comparing `easy-events-2.8.2/easy_events.egg-info/PKG-INFO` & `easy-events-2.9.0/easy_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-events
-Version: 2.8.2
+Version: 2.9.0
 Summary: An universal wrapper (and useful tool) to make event / commands in python
 Home-page: https://github.com/ThePhoenix78/easy-events
 Download-URL: https://github.com/ThePhoenix78/easy-events/tarball/master
 Author: ThePhoenix78
 Author-email: thephoenix788@gmail.com
 License: MIT
 Keywords: wrapper,event,commands,command
```

### Comparing `easy-events-2.8.2/setup.py` & `easy-events-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
 # long_description = "An universal wrapper (and useful tool) to make event / commands in python"
 
 setup(
     name='easy-events',
-    version="2.8.2",
+    version="2.9.0",
     url='https://github.com/ThePhoenix78/easy-events',
     download_url='https://github.com/ThePhoenix78/easy-events/tarball/master',
     license='MIT',
     author='ThePhoenix78',
     author_email='thephoenix788@gmail.com',
     description='An universal wrapper (and useful tool) to make event / commands in python',
     long_description=long_description,
```

