# Comparing `tmp/tools_hjh-2.5.3.tar.gz` & `tmp/tools_hjh-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.5.3.tar", last modified: Thu Apr 13 09:32:15 2023, max compression
+gzip compressed data, was "dist\tools_hjh-2.5.4.tar", last modified: Fri Apr 14 11:41:59 2023, max compression
```

## Comparing `tools_hjh-2.5.3.tar` & `tools_hjh-2.5.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.3/LICENSE
--rw-rw-rw-   0        0        0      207 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0      417 2023-04-13 09:32:02.000000 tools_hjh-2.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/tools_hjh/
--rw-rw-rw-   0        0        0     2834 2023-03-31 11:20:27.000000 tools_hjh-2.5.3/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     9420 2023-04-13 09:26:36.000000 tools_hjh-2.5.3/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.3/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.3/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.3/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.3/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    32863 2023-04-13 09:27:34.000000 tools_hjh-2.5.3/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.5.3/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.3/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     6599 2023-03-10 15:33:54.000000 tools_hjh-2.5.3/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.3/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 09:32:15.000000 tools_hjh-2.5.3/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      453 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 09:32:13.000000 tools_hjh-2.5.3/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.5.4/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      417 2023-04-14 11:41:47.000000 tools_hjh-2.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/tools_hjh/
+-rw-rw-rw-   0        0        0     2834 2023-03-31 11:20:27.000000 tools_hjh-2.5.4/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     9420 2023-04-13 09:26:36.000000 tools_hjh-2.5.4/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     3797 2022-12-27 09:28:14.000000 tools_hjh-2.5.4/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3888 2022-12-29 03:35:54.000000 tools_hjh-2.5.4/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.5.4/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.5.4/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    33359 2023-04-14 11:39:10.000000 tools_hjh-2.5.4/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.5.4/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     2092 2023-01-13 02:50:42.000000 tools_hjh-2.5.4/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     6599 2023-03-10 15:33:54.000000 tools_hjh-2.5.4/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      485 2023-01-13 02:20:59.000000 tools_hjh-2.5.4/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:41:59.000000 tools_hjh-2.5.4/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      453 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 11:41:57.000000 tools_hjh-2.5.4/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.5.3/tools_hjh/Chrome.py` & `tools_hjh-2.5.4/tools_hjh/Chrome.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.3/tools_hjh/DBConn.py` & `tools_hjh-2.5.4/tools_hjh/DBConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.3/tools_hjh/HTTPRequest.py` & `tools_hjh-2.5.4/tools_hjh/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.3/tools_hjh/HTTPTools.py` & `tools_hjh-2.5.4/tools_hjh/HTTPTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.3/tools_hjh/Log.py` & `tools_hjh-2.5.4/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.3/tools_hjh/MemoryDB.py` & `tools_hjh-2.5.4/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.3/tools_hjh/OracleTools.py` & `tools_hjh-2.5.4/tools_hjh/OracleTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,21 +411,40 @@
                 port = tns_s.split('PORT=')[idx].split(')')[0]
                 tnss[tns_name.lower()] = (host, port, service_name.lower(), sid.lower())
         return tnss
 
     @staticmethod     
     def analysis_ogg_status(host_conn):
         """ 进入主机全部找到的ggsci，执行info all 返回结果 """
+        
+        class QueryResults2:
+
+            def __init__(self, cols=(), rows=[]):
+                self.cols = cols
+                self.rows = rows
+        
+            def get_cols(self):
+                return self.cols
+        
+            def get_rows(self):
+                return self.rows
+            
+            def set_cols(self, cols):
+                self.cols = cols
+                
+            def set_rows(self, rows):
+                self.rows = rows
+
         query_time = locattime()
         host = host_conn.host
         username = host_conn.username
         
         # 进程状态 
         # 查询时间 ogg所在主机HOST ggsci所在路径 进程类型 进程状态 进程名称 lag_at_chkpt time_since_chkpt
-        ogg_status = QueryResults()
+        ogg_status = QueryResults2()
         ogg_status.get_rows().clear()
         ogg_status.set_cols(('query_time', 'host', 'ggsci_path', 'type', 'status', 'name', 'lag_at_chkpt', 'time_since_chkpt'))
         
         # 解析进程状态 
         cmd = 'locate *ggsci'
         paths = host_conn.exec_command(cmd)
         for path in paths.split('\n'):
```

### Comparing `tools_hjh-2.5.3/tools_hjh/SSHConn.py` & `tools_hjh-2.5.4/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.3/tools_hjh/ThreadPool.py` & `tools_hjh-2.5.4/tools_hjh/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.5.3/tools_hjh/Tools.py` & `tools_hjh-2.5.4/tools_hjh/Tools.py`

 * *Files identical despite different names*

