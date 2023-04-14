# Comparing `tmp/pythesyncer-23.4.14.19.tar.gz` & `tmp/pythesyncer-23.4.14.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythesyncer-23.4.14.19.tar", last modified: Fri Apr 14 11:59:11 2023, max compression
+gzip compressed data, was "dist/pythesyncer-23.4.14.20.tar", last modified: Fri Apr 14 12:25:41 2023, max compression
```

## Comparing `pythesyncer-23.4.14.19.tar` & `pythesyncer-23.4.14.20.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 11:59:11.007259 pythesyncer-23.4.14.19/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      434 2023-04-14 11:59:11.007259 pythesyncer-23.4.14.19/PKG-INFO
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       76 2023-04-14 11:29:59.000000 pythesyncer-23.4.14.19/README.md
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 11:59:11.003258 pythesyncer-23.4.14.19/pythesyncer/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2692 2023-04-14 11:58:27.000000 pythesyncer-23.4.14.19/pythesyncer/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1241 2023-04-14 11:47:39.000000 pythesyncer-23.4.14.19/pythesyncer/auth.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 11:59:11.007259 pythesyncer-23.4.14.19/pythesyncer.egg-info/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      434 2023-04-14 11:59:10.000000 pythesyncer-23.4.14.19/pythesyncer.egg-info/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      274 2023-04-14 11:59:10.000000 pythesyncer-23.4.14.19/pythesyncer.egg-info/SOURCES.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-04-14 11:59:10.000000 pythesyncer-23.4.14.19/pythesyncer.egg-info/dependency_links.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       55 2023-04-14 11:59:10.000000 pythesyncer-23.4.14.19/pythesyncer.egg-info/entry_points.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       20 2023-04-14 11:59:10.000000 pythesyncer-23.4.14.19/pythesyncer.egg-info/requires.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       12 2023-04-14 11:59:10.000000 pythesyncer-23.4.14.19/pythesyncer.egg-info/top_level.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-04-14 11:59:11.007259 pythesyncer-23.4.14.19/setup.cfg
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      864 2023-04-14 11:58:13.000000 pythesyncer-23.4.14.19/setup.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      434 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/PKG-INFO
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)       76 2023-04-14 11:29:59.000000 pythesyncer-23.4.14.20/README.md
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/pythesyncer/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2618 2023-04-14 12:20:57.000000 pythesyncer-23.4.14.20/pythesyncer/__init__.py
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1241 2023-04-14 11:47:39.000000 pythesyncer-23.4.14.20/pythesyncer/auth.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/pythesyncer.egg-info/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      434 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/PKG-INFO
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      274 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       55 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/entry_points.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       20 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/requires.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       12 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/top_level.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/setup.cfg
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      864 2023-04-14 11:58:13.000000 pythesyncer-23.4.14.20/setup.py
```

### Comparing `pythesyncer-23.4.14.19/pythesyncer/__init__.py` & `pythesyncer-23.4.14.20/pythesyncer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,33 +5,31 @@
 import threading
 from enum import Enum
 
 import boto3
 import codefast as cf
 import fire
 from boto3.s3.transfer import TransferConfig
-from codefast.asyncio import async_render
+from codefast.asyncio import asyncformer
 from rich import print
 
 from .auth import auth
 
 # —--------------------------------------------
 
 
-
 class ProgressPercentage(object):
 
     def __init__(self, filename):
         self._filename = filename
         self._size = float(os.path.getsize(filename))
         self._seen_so_far = 0
         self._lock = threading.Lock()
 
     def __call__(self, bytes_amount):
-        # To simplify, assume this is hooked up to a single filename
         with self._lock:
             self._seen_so_far += bytes_amount
             percentage = (self._seen_so_far / self._size) * 100
             sys.stdout.write(
                 "\r%s  %s / %s  (%.2f%%)" %
                 (self._filename, self._seen_so_far, self._size, percentage))
             sys.stdout.flush()
@@ -64,29 +62,29 @@
     elif action == Action.down:
         await sync_down(obj)
 
 
 async def sync_up(obj):
     if os.path.isfile(obj):
         cf.info('Uploading file: {}'.format(obj))
-        await async_render(upload_file, obj)
+        await asyncformer(upload_file, obj)
 
     elif os.path.isdir(obj):
         cf.info('Uploading dir: {}'.format(obj))
         os.system(
             '7z a -t7z -m0=lzma2 -mx=9 -mfb=64 -md=32m -ms=on archive.7z {}'.
             format(obj))
-        await async_render(upload_file, 'archive.7z')
+        await asyncformer(upload_file, 'archive.7z')
         os.remove('archive.7z')
         cf.info("Upload done: {}".format(obj))
 
 
 async def sync_down(obj):
     remote_file = os.path.join(auth.host_api, obj)
-    await async_render(cf.net.download, remote_file, obj)
+    await asyncformer(cf.net.download, remote_file, obj)
 
 
 def entry(action: str, obj: str):
     if action not in [a.value for a in Action]:
         print('Action must be one of {}'.format([a.value for a in Action]))
         return
     action = Action(action)
```

### Comparing `pythesyncer-23.4.14.19/pythesyncer/auth.py` & `pythesyncer-23.4.14.20/pythesyncer/auth.py`

 * *Files identical despite different names*

### Comparing `pythesyncer-23.4.14.19/setup.py` & `pythesyncer-23.4.14.20/setup.py`

 * *Files identical despite different names*

