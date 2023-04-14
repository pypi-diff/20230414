# Comparing `tmp/streaming-logs-1.0.8.tar.gz` & `tmp/streaming-logs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streaming-logs-1.0.8.tar", last modified: Mon Nov 28 17:06:05 2022, max compression
+gzip compressed data, was "streaming-logs-1.0.9.tar", last modified: Fri Apr 14 16:10:28 2023, max compression
```

## Comparing `streaming-logs-1.0.8.tar` & `streaming-logs-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anibal     (502) staff       (20)        0 2022-11-28 17:06:05.492915 streaming-logs-1.0.8/
--rw-r--r--   0 anibal     (502) staff       (20)    16725 2022-05-10 15:39:24.000000 streaming-logs-1.0.8/LICENSE
--rw-r--r--   0 anibal     (502) staff       (20)       29 2022-09-28 22:59:24.000000 streaming-logs-1.0.8/MANIFEST.in
--rw-r--r--   0 anibal     (502) staff       (20)      570 2022-11-28 17:06:05.492728 streaming-logs-1.0.8/PKG-INFO
--rw-r--r--   0 anibal     (502) staff       (20)       38 2022-11-28 17:06:05.492960 streaming-logs-1.0.8/setup.cfg
--rw-r--r--   0 anibal     (502) staff       (20)     1553 2022-09-28 23:03:47.000000 streaming-logs-1.0.8/setup.py
-drwxr-xr-x   0 anibal     (502) staff       (20)        0 2022-11-28 17:06:05.486216 streaming-logs-1.0.8/streaming_logs.egg-info/
--rw-r--r--   0 anibal     (502) staff       (20)      570 2022-11-28 17:06:05.000000 streaming-logs-1.0.8/streaming_logs.egg-info/PKG-INFO
--rw-r--r--   0 anibal     (502) staff       (20)      407 2022-11-28 17:06:05.000000 streaming-logs-1.0.8/streaming_logs.egg-info/SOURCES.txt
--rw-r--r--   0 anibal     (502) staff       (20)        1 2022-11-28 17:06:05.000000 streaming-logs-1.0.8/streaming_logs.egg-info/dependency_links.txt
--rw-r--r--   0 anibal     (502) staff       (20)        9 2022-11-28 17:06:05.000000 streaming-logs-1.0.8/streaming_logs.egg-info/requires.txt
--rw-r--r--   0 anibal     (502) staff       (20)       14 2022-11-28 17:06:05.000000 streaming-logs-1.0.8/streaming_logs.egg-info/top_level.txt
-drwxr-xr-x   0 anibal     (502) staff       (20)        0 2022-11-28 17:06:05.492174 streaming-logs-1.0.8/streaminglogs/
--rw-r--r--   0 anibal     (502) staff       (20)      246 2022-11-28 17:05:31.000000 streaming-logs-1.0.8/streaminglogs/__init__.py
--rw-r--r--   0 anibal     (502) staff       (20)      791 2022-11-15 23:47:32.000000 streaming-logs-1.0.8/streaminglogs/activitylog.py
--rw-r--r--   0 anibal     (502) staff       (20)     1124 2022-11-15 23:47:37.000000 streaming-logs-1.0.8/streaminglogs/exceptionlog.py
--rw-r--r--   0 anibal     (502) staff       (20)      557 2022-09-28 23:04:30.000000 streaming-logs-1.0.8/streaminglogs/genericlog.py
--rw-r--r--   0 anibal     (502) staff       (20)     5376 2022-11-28 17:05:03.000000 streaming-logs-1.0.8/streaminglogs/logginghandler.py
--rw-r--r--   0 anibal     (502) staff       (20)      267 2022-11-20 11:48:47.000000 streaming-logs-1.0.8/streaminglogs/streaminglogsservicecontext.py
+drwxr-xr-x   0 anibal     (502) staff       (20)        0 2023-04-14 16:10:28.184318 streaming-logs-1.0.9/
+-rw-r--r--   0 anibal     (502) staff       (20)    16725 2022-05-10 15:39:24.000000 streaming-logs-1.0.9/LICENSE
+-rw-r--r--   0 anibal     (502) staff       (20)       29 2022-09-28 22:59:24.000000 streaming-logs-1.0.9/MANIFEST.in
+-rw-r--r--   0 anibal     (502) staff       (20)      570 2023-04-14 16:10:28.184142 streaming-logs-1.0.9/PKG-INFO
+-rw-r--r--   0 anibal     (502) staff       (20)       38 2023-04-14 16:10:28.184362 streaming-logs-1.0.9/setup.cfg
+-rw-r--r--   0 anibal     (502) staff       (20)     1553 2022-09-28 23:03:47.000000 streaming-logs-1.0.9/setup.py
+drwxr-xr-x   0 anibal     (502) staff       (20)        0 2023-04-14 16:10:28.181255 streaming-logs-1.0.9/streaming_logs.egg-info/
+-rw-r--r--   0 anibal     (502) staff       (20)      570 2023-04-14 16:10:28.000000 streaming-logs-1.0.9/streaming_logs.egg-info/PKG-INFO
+-rw-r--r--   0 anibal     (502) staff       (20)      407 2023-04-14 16:10:28.000000 streaming-logs-1.0.9/streaming_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 anibal     (502) staff       (20)        1 2023-04-14 16:10:28.000000 streaming-logs-1.0.9/streaming_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 anibal     (502) staff       (20)        9 2023-04-14 16:10:28.000000 streaming-logs-1.0.9/streaming_logs.egg-info/requires.txt
+-rw-r--r--   0 anibal     (502) staff       (20)       14 2023-04-14 16:10:28.000000 streaming-logs-1.0.9/streaming_logs.egg-info/top_level.txt
+drwxr-xr-x   0 anibal     (502) staff       (20)        0 2023-04-14 16:10:28.183791 streaming-logs-1.0.9/streaminglogs/
+-rw-r--r--   0 anibal     (502) staff       (20)      246 2023-04-14 16:10:04.000000 streaming-logs-1.0.9/streaminglogs/__init__.py
+-rw-r--r--   0 anibal     (502) staff       (20)      791 2022-11-15 23:47:32.000000 streaming-logs-1.0.9/streaminglogs/activitylog.py
+-rw-r--r--   0 anibal     (502) staff       (20)     1124 2022-11-15 23:47:37.000000 streaming-logs-1.0.9/streaminglogs/exceptionlog.py
+-rw-r--r--   0 anibal     (502) staff       (20)      557 2022-09-28 23:04:30.000000 streaming-logs-1.0.9/streaminglogs/genericlog.py
+-rw-r--r--   0 anibal     (502) staff       (20)     5804 2023-04-14 16:09:45.000000 streaming-logs-1.0.9/streaminglogs/logginghandler.py
+-rw-r--r--   0 anibal     (502) staff       (20)      267 2022-11-20 11:48:47.000000 streaming-logs-1.0.9/streaminglogs/streaminglogsservicecontext.py
```

### Comparing `streaming-logs-1.0.8/LICENSE` & `streaming-logs-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `streaming-logs-1.0.8/PKG-INFO` & `streaming-logs-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming-logs
-Version: 1.0.8
+Version: 1.0.9
 Summary: Streaming Logs SDK 4 Python.
 Home-page: https://location-world@dev.azure.com/location-world/Research%20and%20Development/_git/streaming-logs.py
 Author: Location World
 Author-email: info@location-world.com
 License: MPL-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `streaming-logs-1.0.8/setup.py` & `streaming-logs-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `streaming-logs-1.0.8/streaming_logs.egg-info/PKG-INFO` & `streaming-logs-1.0.9/streaming_logs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streaming-logs
-Version: 1.0.8
+Version: 1.0.9
 Summary: Streaming Logs SDK 4 Python.
 Home-page: https://location-world@dev.azure.com/location-world/Research%20and%20Development/_git/streaming-logs.py
 Author: Location World
 Author-email: info@location-world.com
 License: MPL-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `streaming-logs-1.0.8/streaminglogs/activitylog.py` & `streaming-logs-1.0.9/streaminglogs/activitylog.py`

 * *Files identical despite different names*

### Comparing `streaming-logs-1.0.8/streaminglogs/exceptionlog.py` & `streaming-logs-1.0.9/streaminglogs/exceptionlog.py`

 * *Files identical despite different names*

### Comparing `streaming-logs-1.0.8/streaminglogs/genericlog.py` & `streaming-logs-1.0.9/streaminglogs/genericlog.py`

 * *Files identical despite different names*

### Comparing `streaming-logs-1.0.8/streaminglogs/logginghandler.py` & `streaming-logs-1.0.9/streaminglogs/logginghandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,43 @@
 class LoggingHandler:
 
     __context: StreamingLogsServiceContext
     __is_debug: bool
     __origin: str
     __ip_address: str
 
+    __ipynb_unhandled_exceptions_additional_info: str
+
     @classmethod
     def __init__(cls,
                  context: StreamingLogsServiceContext,
                  is_debug,
-                 enable_ipynb_unhandled_exceptions_tracing=False):
+                 enable_ipynb_unhandled_exceptions_tracing=False,
+                 ipynb_unhandled_exceptions_additional_info=None):
         cls.__context = context
         cls.__is_debug = is_debug
         cls.__origin = cls.__context.origin + '.debug' if cls.__is_debug else cls.__context.origin
         cls.__ip_address = cls.__get_ip()
         if enable_ipynb_unhandled_exceptions_tracing:
+            cls.__ipynb_unhandled_exceptions_additional_info = ipynb_unhandled_exceptions_additional_info
             get_ipython().set_custom_exc((Exception,), cls.trace_unhandled_exception)
 
     @classmethod
     def trace_unhandled_exception(cls, shell, etype, evalue, tb, tb_offset=None):
         shell.showtraceback((etype, evalue, tb), tb_offset=tb_offset)
 
         itb = AutoFormattedTB(mode='Plain', tb_offset=1)
         stb = itb.structured_traceback(etype, evalue, tb)
         sstb = itb.stb2text(stb)
 
-        cls.trace_exception(evalue, sstb)
+        if cls.__ipynb_unhandled_exceptions_additional_info is None:
+            cls.trace_exception(evalue, sstb)
+            return
+
+        cls.trace_exception(evalue, sstb, additional_info=cls.__ipynb_unhandled_exceptions_additional_info)
 
     @classmethod
     def trace_activity(cls, message: str, tags=None, additional_info=None, console_only: bool = False):
 
         if cls.__is_debug:
             print(message)
```

