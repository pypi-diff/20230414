# Comparing `tmp/robit-0.3.0.tar.gz` & `tmp/robit-0.3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robit-0.3.0.tar", last modified: Fri Apr 14 15:04:03 2023, max compression
+gzip compressed data, was "robit-0.3.0.1.tar", last modified: Fri Apr 14 21:38:35 2023, max compression
```

## Comparing `robit-0.3.0.tar` & `robit-0.3.0.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.690367 robit-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 15:03:53.000000 robit-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 15:03:53.000000 robit-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-14 15:04:03.690367 robit-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-14 15:03:53.000000 robit-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 15:03:53.000000 robit-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.682366 robit-0.3.0/robit/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-14 15:03:53.000000 robit-0.3.0/robit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.686366 robit-0.3.0/robit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/health.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/name.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/web_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-14 15:03:53.000000 robit-0.3.0/robit/core/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.686366 robit-0.3.0/robit/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/alpine.js
--rw-r--r--   0 runner    (1001) docker     (123)   194855 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)    80448 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/core.js
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/index.css
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/worker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 15:03:53.000000 robit-0.3.0/robit/html/worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.690367 robit-0.3.0/robit/job/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 15:03:53.000000 robit-0.3.0/robit/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-14 15:03:53.000000 robit-0.3.0/robit/job/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-14 15:03:53.000000 robit-0.3.0/robit/job/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.690367 robit-0.3.0/robit/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:53.000000 robit-0.3.0/robit/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-14 15:03:53.000000 robit-0.3.0/robit/monitor/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-14 15:03:53.000000 robit-0.3.0/robit/monitor/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.690367 robit-0.3.0/robit/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:53.000000 robit-0.3.0/robit/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-14 15:03:53.000000 robit-0.3.0/robit/test/test_cron.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 15:03:53.000000 robit-0.3.0/robit/test/test_robit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.690367 robit-0.3.0/robit/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:03:53.000000 robit-0.3.0/robit/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-14 15:03:53.000000 robit-0.3.0/robit/worker/web_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-14 15:03:53.000000 robit-0.3.0/robit/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:04:03.682366 robit-0.3.0/robit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-14 15:04:03.000000 robit-0.3.0/robit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-14 15:04:03.000000 robit-0.3.0/robit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:04:03.000000 robit-0.3.0/robit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 15:04:03.000000 robit-0.3.0/robit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-14 15:04:03.690367 robit-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 15:03:53.000000 robit-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-14 21:38:26.000000 robit-0.3.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 21:38:26.000000 robit-0.3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-14 21:38:35.766015 robit-0.3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-14 21:38:26.000000 robit-0.3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 21:38:26.000000 robit-0.3.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.762015 robit-0.3.0.1/robit/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/web_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/core/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/alpine.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194855 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)    80448 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/core.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15672 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/worker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/html/worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/job/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/job/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/monitor/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/monitor/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/test/test_cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/test/test_robit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.766015 robit-0.3.0.1/robit/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/worker/web_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-14 21:38:26.000000 robit-0.3.0.1/robit/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:38:35.762015 robit-0.3.0.1/robit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-14 21:38:35.000000 robit-0.3.0.1/robit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-14 21:38:35.000000 robit-0.3.0.1/robit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:38:35.000000 robit-0.3.0.1/robit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 21:38:35.000000 robit-0.3.0.1/robit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-14 21:38:35.766015 robit-0.3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 21:38:26.000000 robit-0.3.0.1/setup.py
```

### Comparing `robit-0.3.0/LICENSE.txt` & `robit-0.3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/PKG-INFO` & `robit-0.3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robit
-Version: 0.3.0
+Version: 0.3.0.1
 Summary: Service Worker Framework
 Home-page: https://github.com/stratusadv/robit
 Author: Nathan Johnson
 Author-email: nathanj@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robit-0.3.0/README.md` & `robit-0.3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/core/alert.py` & `robit-0.3.0.1/robit/core/alert.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/core/clock.py` & `robit-0.3.0.1/robit/core/clock.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime, timedelta
 
-CREATED_DATE_FORMAT = '%b %d, %Y %I:%M:%S %p'
+CREATED_DATE_FORMAT = '%b %d, %Y at %I:%M:%S %p'
 
 
 class Clock:
     def __init__(
             self,
             utc_offset: int = 0,
     ):
```

### Comparing `robit-0.3.0/robit/core/cron.py` & `robit-0.3.0.1/robit/core/cron.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,26 @@
             value: str,
             utc_offset: int = 0,
     ):
         self.value = value
         self.utc_offset = utc_offset
 
         cron_segment_list = self.value.split(' ')
-
         if 5 > len(cron_segment_list) > 6:
             value_error = f'Cron string {self.value} is not the correct length.\n'
             value_error += f'Should be 5 elements in a string "* * * * *"]\n'
             value_error += f'or 6 elements in a string if your working with seconds "* * * * * *"'
             raise ValueError(value_error)
 
-        cron_segment = 0
-        self.second = None
-
         if len(cron_segment_list) == 6:
-            self.second = SecondCronValue(cron_segment_list[cron_segment])
+            self.second = SecondCronValue(cron_segment_list[0])
             cron_segment = 1
+        else:
+            cron_segment = 0
+            self.second = SecondCronValue('00')
 
         self.minute = MinuteCronValue(cron_segment_list[cron_segment])
         self.hour = HourCronValue(cron_segment_list[cron_segment + 1])
         self.day_of_month = DayOfMonthCronValue(cron_segment_list[cron_segment + 2])
         self.month = MonthCronValue(cron_segment_list[cron_segment + 3])
         self.day_of_week = DayOfWeekCronValue(cron_segment_list[cron_segment + 4])
 
@@ -66,17 +65,15 @@
     def next_run_datetime_verbose(self):
         return self.next_datetime.strftime(CREATED_DATE_FORMAT)
 
     def set_next_datetime(self):
         ndt = datetime.utcnow().replace(microsecond=0) + timedelta(hours=self.utc_offset)
         now = datetime.utcnow().replace(microsecond=0) + timedelta(hours=self.utc_offset)
 
-        if self.second is not None:
-            ndt = self.second.get_next_date_time(ndt, now)
-
+        ndt = self.second.get_next_date_time(ndt, now)
         ndt = self.minute.get_next_date_time(ndt, now, second=self.second)
         ndt = self.hour.get_next_date_time(ndt, now, minute=self.minute)
         ndt = self.day_of_month.get_next_date_time(ndt, now, hour=self.hour)
         ndt = self.month.get_next_date_time(ndt, now, day_of_month=self.day_of_month)
         ndt = self.day_of_week.get_next_date_time(ndt, now)
 
         self.next_datetime = ndt
@@ -130,16 +127,17 @@
 class SecondCronValue(CronValue):
     def get_next_date_time(self, ndt: datetime, now: datetime, **kwargs) -> datetime:
         if self.function == 'every':
             ndt += timedelta(seconds=1)
         elif self.function == 'specific':
             ndt = ndt.replace(second=self.specific)
 
-            if now.minute >= ndt.minute:
+            if now.second >= self.specific:
                 ndt += timedelta(minutes=1)
+
         elif self.function == 'step':
             count_step_list = [0]
             count = self.step
             while count < 60:
                 count_step_list.append(count)
                 count += self.step
 
@@ -153,29 +151,22 @@
 
         return ndt
 
 
 class MinuteCronValue(CronValue):
     def get_next_date_time(self, ndt: datetime, now: datetime, **kwargs) -> datetime:
         if self.function == 'every':
-            if kwargs['second'] is not None:
-                pass
-            else:
-                ndt += timedelta(minutes=1)
-
+            pass
         elif self.function == 'specific':
             ndt = ndt.replace(minute=self.specific)
+            # if kwargs['second'].function == 'specific':
+            #     if now.second >= ndt.second:
+            #         ndt += timedelta(minutes=1)
 
-            if kwargs['second'] is not None:
-                if ndt.minute == self.specific:
-                    if kwargs['second'].function == 'specific':
-                        if now.second >= ndt.second:
-                            ndt += timedelta(hours=1)
-
-            if now.minute > ndt.minute:
+            if now.minute >= self.specific:
                 ndt += timedelta(hours=1)
 
         elif self.function == 'step':
             count_step_list = [0]
             count = self.step
             while count < 60:
                 count_step_list.append(count)
@@ -196,20 +187,20 @@
     def get_next_date_time(self, ndt: datetime, now: datetime, **kwargs) -> datetime:
         if self.function == 'every':
             pass
 
         if self.function == 'specific':
             ndt = ndt.replace(hour=self.specific)
 
-            if ndt.hour == self.specific:
-                if kwargs['minute'].function == 'specific':
-                    if now.minute >= ndt.minute:
-                        ndt += timedelta(days=1)
+            # if ndt.hour == self.specific:
+            #     if kwargs['minute'].function == 'specific':
+            #         if now.minute >= ndt.minute:
+            #             ndt += timedelta(days=1)
 
-            if ndt.hour > self.specific:
+            if now.hour >= self.specific:
                 ndt += timedelta(days=1)
 
         elif self.function == 'step':
             count_step_list = [0]
             count = self.step
             while count < 24:
                 count_step_list.append(count)
@@ -241,15 +232,15 @@
 
             if ndt.day == self.specific:
 
                 if kwargs['hour'].function == 'specific':
                     if now.hour >= ndt.hour:
                         ndt = ndt.replace(month=next_month)
 
-            if ndt.day > self.specific:
+            if now.day > self.specific:
                 ndt = ndt.replace(month=next_month)
 
         return ndt
 
 
 class MonthCronValue(CronValue):
     def get_next_date_time(self, ndt: datetime, now: datetime, **kwargs) -> datetime:
```

### Comparing `robit-0.3.0/robit/core/health.py` & `robit-0.3.0.1/robit/core/health.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/core/log.py` & `robit-0.3.0.1/robit/core/log.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/core/status.py` & `robit-0.3.0.1/robit/core/status.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/core/timer.py` & `robit-0.3.0.1/robit/core/timer.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/core/web_server.py` & `robit-0.3.0.1/robit/core/web_server.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/alpine.js` & `robit-0.3.0.1/robit/html/alpine.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/bootstrap.css` & `robit-0.3.0.1/robit/html/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/bootstrap.js` & `robit-0.3.0.1/robit/html/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/icon.png` & `robit-0.3.0.1/robit/html/icon.png`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/index.css` & `robit-0.3.0.1/robit/html/index.css`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/monitor.html` & `robit-0.3.0.1/robit/html/monitor.html`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/monitor.js` & `robit-0.3.0.1/robit/html/monitor.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/worker.html` & `robit-0.3.0.1/robit/html/worker.html`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/html/worker.js` & `robit-0.3.0.1/robit/html/worker.js`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/job/group.py` & `robit-0.3.0.1/robit/job/group.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/job/job.py` & `robit-0.3.0.1/robit/job/job.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/monitor/monitor.py` & `robit-0.3.0.1/robit/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/monitor/web_server.py` & `robit-0.3.0.1/robit/monitor/web_server.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/worker/web_server.py` & `robit-0.3.0.1/robit/worker/web_server.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit/worker/worker.py` & `robit-0.3.0.1/robit/worker/worker.py`

 * *Files identical despite different names*

### Comparing `robit-0.3.0/robit.egg-info/PKG-INFO` & `robit-0.3.0.1/robit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robit
-Version: 0.3.0
+Version: 0.3.0.1
 Summary: Service Worker Framework
 Home-page: https://github.com/stratusadv/robit
 Author: Nathan Johnson
 Author-email: nathanj@stratusadv.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robit-0.3.0/robit.egg-info/SOURCES.txt` & `robit-0.3.0.1/robit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

