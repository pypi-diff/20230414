# Comparing `tmp/jadelogs-0.8.tar.gz` & `tmp/jadelogs-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jadelogs-0.8.tar", last modified: Thu Feb 23 07:02:21 2023, max compression
+gzip compressed data, was "jadelogs-0.9.tar", last modified: Fri Feb 24 14:23:35 2023, max compression
```

## Comparing `jadelogs-0.8.tar` & `jadelogs-0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-23 07:02:21.469755 jadelogs-0.8/
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)      585 2023-02-23 07:02:21.469755 jadelogs-0.8/MANIFEST
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)      732 2023-02-23 07:02:21.469755 jadelogs-0.8/PKG-INFO
-drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-23 07:02:21.469755 jadelogs-0.8/jadelogs/
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)       56 2023-02-12 16:27:37.280811 jadelogs-0.8/jadelogs/__init__.py
-drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-23 07:02:21.469755 jadelogs-0.8/jadelogs/common/
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-12 17:08:38.095044 jadelogs-0.8/jadelogs/common/__init__.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)      978 2023-02-23 06:59:47.476305 jadelogs-0.8/jadelogs/common/config.py
-drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-23 07:02:21.469755 jadelogs-0.8/jadelogs/datamodels/
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-12 06:47:45.224514 jadelogs-0.8/jadelogs/datamodels/__init__.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1422 2023-02-12 18:14:07.715185 jadelogs-0.8/jadelogs/datamodels/batch_datamodel.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1615 2023-02-22 15:17:28.201125 jadelogs-0.8/jadelogs/datamodels/datapoint_model.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     2891 2023-02-22 15:27:36.240253 jadelogs-0.8/jadelogs/datamodels/epoch_datamodel.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     2192 2023-02-12 19:50:04.487180 jadelogs-0.8/jadelogs/datamodels/experiment_datamodel.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1438 2023-02-12 17:47:05.326897 jadelogs-0.8/jadelogs/datamodels/jade_log_datamodel.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1069 2023-02-12 19:39:57.105672 jadelogs-0.8/jadelogs/datamodels/log_datamodel.py
-drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-23 07:02:21.469755 jadelogs-0.8/jadelogs/file_manager/
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-12 06:30:38.241882 jadelogs-0.8/jadelogs/file_manager/__init__.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     2061 2023-02-22 11:34:44.559795 jadelogs-0.8/jadelogs/file_manager/file_manager.py
-drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-23 07:02:21.469755 jadelogs-0.8/jadelogs/jade_logger/
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-12 06:39:24.695460 jadelogs-0.8/jadelogs/jade_logger/__init__.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     3497 2023-02-22 15:29:40.395271 jadelogs-0.8/jadelogs/jade_logger/jade_logger.py
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        6 2023-02-12 16:26:21.797731 jadelogs-0.8/jadelogs/requirements.txt
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)       62 2023-02-11 21:16:34.580740 jadelogs-0.8/setup.cfg
--rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1625 2023-02-23 07:02:11.229928 jadelogs-0.8/setup.py
+drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-24 14:23:35.592872 jadelogs-0.9/
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)      585 2023-02-24 14:23:35.592872 jadelogs-0.9/MANIFEST
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)      732 2023-02-24 14:23:35.592872 jadelogs-0.9/PKG-INFO
+drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-24 14:23:35.592872 jadelogs-0.9/jadelogs/
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)       56 2023-02-12 16:27:37.280811 jadelogs-0.9/jadelogs/__init__.py
+drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-24 14:23:35.592872 jadelogs-0.9/jadelogs/common/
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-12 17:08:38.095044 jadelogs-0.9/jadelogs/common/__init__.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)      978 2023-02-24 06:20:07.643275 jadelogs-0.9/jadelogs/common/config.py
+drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-24 14:23:35.592872 jadelogs-0.9/jadelogs/datamodels/
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-12 06:47:45.224514 jadelogs-0.9/jadelogs/datamodels/__init__.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1422 2023-02-12 18:14:07.715185 jadelogs-0.9/jadelogs/datamodels/batch_datamodel.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1615 2023-02-24 06:20:07.643275 jadelogs-0.9/jadelogs/datamodels/datapoint_model.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     2891 2023-02-24 06:20:07.643275 jadelogs-0.9/jadelogs/datamodels/epoch_datamodel.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     2192 2023-02-12 19:50:04.487180 jadelogs-0.9/jadelogs/datamodels/experiment_datamodel.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1438 2023-02-12 17:47:05.326897 jadelogs-0.9/jadelogs/datamodels/jade_log_datamodel.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1069 2023-02-12 19:39:57.105672 jadelogs-0.9/jadelogs/datamodels/log_datamodel.py
+drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-24 14:23:35.592872 jadelogs-0.9/jadelogs/file_manager/
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-12 06:30:38.241882 jadelogs-0.9/jadelogs/file_manager/__init__.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     2218 2023-02-24 06:28:35.027385 jadelogs-0.9/jadelogs/file_manager/file_manager.py
+drwxrwxr-x   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-24 14:23:35.592872 jadelogs-0.9/jadelogs/jade_logger/
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        0 2023-02-12 06:39:24.695460 jadelogs-0.9/jadelogs/jade_logger/__init__.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     3579 2023-02-24 06:20:07.643275 jadelogs-0.9/jadelogs/jade_logger/jade_logger.py
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)        6 2023-02-12 16:26:21.797731 jadelogs-0.9/jadelogs/requirements.txt
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)       62 2023-02-11 21:16:34.580740 jadelogs-0.9/setup.cfg
+-rw-rw-r--   0 lalady6977  (1001) lalady6977  (1001)     1625 2023-02-24 14:23:29.764933 jadelogs-0.9/setup.py
```

### Comparing `jadelogs-0.8/MANIFEST` & `jadelogs-0.9/MANIFEST`

 * *Files identical despite different names*

### Comparing `jadelogs-0.8/PKG-INFO` & `jadelogs-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: jadelogs
-Version: 0.8
+Version: 0.9
 Summary: Package to log and track progress of machine learning programs run on the Jade supercomputer
 Home-page: https://github.com/vedmathai/jade-logs
 Author: Ved Mathai
 Author-email: vedu29@gmail.com
 License: MIT
 Description: UNKNOWN
 Keywords: jade,supercomputer,logs
```

### Comparing `jadelogs-0.8/jadelogs/common/config.py` & `jadelogs-0.9/jadelogs/common/config.py`

 * *Files identical despite different names*

### Comparing `jadelogs-0.8/jadelogs/datamodels/batch_datamodel.py` & `jadelogs-0.9/jadelogs/datamodels/batch_datamodel.py`

 * *Files identical despite different names*

### Comparing `jadelogs-0.8/jadelogs/datamodels/datapoint_model.py` & `jadelogs-0.9/jadelogs/datamodels/datapoint_model.py`

 * *Files identical despite different names*

### Comparing `jadelogs-0.8/jadelogs/datamodels/epoch_datamodel.py` & `jadelogs-0.9/jadelogs/datamodels/epoch_datamodel.py`

 * *Files identical despite different names*

### Comparing `jadelogs-0.8/jadelogs/datamodels/experiment_datamodel.py` & `jadelogs-0.9/jadelogs/datamodels/experiment_datamodel.py`

 * *Files identical despite different names*

### Comparing `jadelogs-0.8/jadelogs/datamodels/jade_log_datamodel.py` & `jadelogs-0.9/jadelogs/datamodels/jade_log_datamodel.py`

 * *Files identical despite different names*

### Comparing `jadelogs-0.8/jadelogs/datamodels/log_datamodel.py` & `jadelogs-0.9/jadelogs/datamodels/log_datamodel.py`

 * *Files identical despite different names*

### Comparing `jadelogs-0.8/jadelogs/file_manager/file_manager.py` & `jadelogs-0.9/jadelogs/file_manager/file_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import shutil
 
 from jadelogs.common.config import Config
 from jadelogs.datamodels.jade_log_datamodel import JadeLogDatamodel
 
 
 class FileManager:
 
@@ -41,19 +42,21 @@
         folderpath = os.path.join(self.project_folder(), 'logs', request_id)
         if not os.path.exists(folderpath):
             os.makedirs(folderpath)
         return folderpath
 
     def write_jade_log(self, jade_log):
         folderpath = self.logs_folderpath()
-        if os.path.exists(folderpath) is False:
-            os.makedirs(folderpath)
-        filepath = os.path.join(folderpath, 'log.json')
+        inner_folderpath = os.path.join(folderpath, 'logs')
+        if os.path.exists(inner_folderpath) is False:
+            os.makedirs(inner_folderpath)
+        filepath = os.path.join(inner_folderpath, 'log.json')
         with open(filepath, 'wt') as f:
             json.dump(jade_log.to_dict(), f)
+        shutil.make_archive(folderpath, 'zip', inner_folderpath)
 
     def read_log_file(self):
         folderpath = self.logs_folderpath()
         filepath = os.path.join(folderpath, 'log.json')
         with open(filepath, 'rt') as f:
             jade_log = JadeLogDatamodel.from_dict(json.load(f))
         return jade_log
```

### Comparing `jadelogs-0.8/jadelogs/jade_logger/jade_logger.py` & `jadelogs-0.9/jadelogs/jade_logger/jade_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     def end_experiment(self):
         self.save_snapshot()
         self.reset()
 
     def save_snapshot(self):
         self.file_manager.write_jade_log(self._jade_log)
 
+    def from_snapshot(self, val):
+        return JadeLogDatamodel.from_dict(val)
+
     def global_log(self, message, level=5):
         log = LogDatamodel.create(message, level)
         self._jade_log.add_global_log(log)
         self.save_snapshot()
 
     def log(self, message, level=5):
         experiment = self._jade_log.current_experiment()
```

### Comparing `jadelogs-0.8/setup.py` & `jadelogs-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 setup(
     name = 'jadelogs',         # How you named your package folder (MyLib)
     packages=['jadelogs'],
     package_data={
         'jadelogs': ['*','*/*','*/*/*']
     },   # Chose the same as "name"
-    version = '0.8',      # Start with a small number and increase it with every change you make
+    version = '0.9',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Package to log and track progress of machine learning programs run on the Jade supercomputer',   # Give a short description about your library
     author = 'Ved Mathai',                   # Type in your name
     author_email = 'vedu29@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/vedmathai/jade-logs',   # Provide either the link to your github or to your website
     keywords = ['jade', 'supercomputer', 'logs'],   # Keywords that define your package best
     install_requires=[],
```

