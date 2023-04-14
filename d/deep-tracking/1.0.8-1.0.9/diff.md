# Comparing `tmp/deep_tracking-1.0.8.tar.gz` & `tmp/deep_tracking-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_tracking-1.0.8.tar", last modified: Tue Apr 11 23:50:49 2023, max compression
+gzip compressed data, was "deep_tracking-1.0.9.tar", last modified: Fri Apr 14 00:57:13 2023, max compression
```

## Comparing `deep_tracking-1.0.8.tar` & `deep_tracking-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:50:49.454373 deep_tracking-1.0.8/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 19:33:15.000000 deep_tracking-1.0.8/LICENSE.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 23:50:49.454373 deep_tracking-1.0.8/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      429 2023-04-04 11:20:37.000000 deep_tracking-1.0.8/README.md
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:50:49.450373 deep_tracking-1.0.8/deep_tracking/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       34 2023-04-11 20:24:32.000000 deep_tracking-1.0.8/deep_tracking/__init__.py
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)    10283 2023-04-11 23:50:32.000000 deep_tracking-1.0.8/deep_tracking/deep_tracking.py
-drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-11 23:50:49.454373 deep_tracking-1.0.8/deep_tracking.egg-info/
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/PKG-INFO
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      271 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/SOURCES.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/dependency_links.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/requires.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-11 23:50:49.000000 deep_tracking-1.0.8/deep_tracking.egg-info/top_level.txt
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-11 23:50:49.454373 deep_tracking-1.0.8/setup.cfg
--rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      773 2023-04-11 23:50:39.000000 deep_tracking-1.0.8/setup.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-14 00:57:13.335496 deep_tracking-1.0.9/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)     1085 2023-04-11 19:33:15.000000 deep_tracking-1.0.9/LICENSE.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-14 00:57:13.335496 deep_tracking-1.0.9/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      429 2023-04-04 11:20:37.000000 deep_tracking-1.0.9/README.md
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-14 00:57:13.331496 deep_tracking-1.0.9/deep_tracking/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       34 2023-04-11 20:24:32.000000 deep_tracking-1.0.9/deep_tracking/__init__.py
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)    10495 2023-04-13 18:52:38.000000 deep_tracking-1.0.9/deep_tracking/deep_tracking.py
+drwxrwxr-x   0 biazotogabriel  (1000) biazotogabriel  (1000)        0 2023-04-14 00:57:13.335496 deep_tracking-1.0.9/deep_tracking.egg-info/
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      594 2023-04-14 00:57:13.000000 deep_tracking-1.0.9/deep_tracking.egg-info/PKG-INFO
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      271 2023-04-14 00:57:13.000000 deep_tracking-1.0.9/deep_tracking.egg-info/SOURCES.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)        1 2023-04-14 00:57:13.000000 deep_tracking-1.0.9/deep_tracking.egg-info/dependency_links.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-14 00:57:13.000000 deep_tracking-1.0.9/deep_tracking.egg-info/requires.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       14 2023-04-14 00:57:13.000000 deep_tracking-1.0.9/deep_tracking.egg-info/top_level.txt
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)       38 2023-04-14 00:57:13.335496 deep_tracking-1.0.9/setup.cfg
+-rw-rw-r--   0 biazotogabriel  (1000) biazotogabriel  (1000)      773 2023-04-14 00:56:04.000000 deep_tracking-1.0.9/setup.py
```

### Comparing `deep_tracking-1.0.8/LICENSE.txt` & `deep_tracking-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deep_tracking-1.0.8/PKG-INFO` & `deep_tracking-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep_tracking
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library to track the development of data science works using the DE&P method
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep de&p data science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deep_tracking-1.0.8/deep_tracking/deep_tracking.py` & `deep_tracking-1.0.9/deep_tracking/deep_tracking.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,19 @@
         #print(last_consolidated_order, order)
         self.rolback(last_consolidated_order)
         process = self.__processes.pop(order)
         self.__processes.insert(new_order, process)
         return None   
     
     def run(self, data, processes):
-        for process in processes:
-            order = self.get_process_order(process[0], process[1])
-            data = self.__processes[order].run(data)
+        for process_id in processes:
+            order = self.get_process_order(process_id[0], process_id[1])
+            process = self.__processes[order]
+            data = process.run(data)
+            print(f'[{process.scope}/{process.action}] - {process.description}')
         return data
     
     def save(self, file_name):
         if os.path.exists(f'{file_name}.trk'):
             answer = input('There is already another tracker saved with this name. Do you want to continue? [Y to continue]')
             if answer != 'Y':
                 return None
@@ -191,17 +193,20 @@
             if actions is not None:
                 if process.action not in actions:
                     continue
             processes.append((process.scope, process.action))
         return processes
     
     def get_backup(self, backup, method='=='):
-        backup_id = self.get_backup_id(backup, method)
+        if isinstance(backup, int):
+            backup_id = backup
+        else:
+            backup_id = self.get_backup_id(backup, method)
         if backup_id is not None:
-            return self.__backups[backup_id]
+            return self.__backups[backup_id].copy()
         return None
     
     def get_backup_id(self, backup, method='=='):
         if isinstance(backup, tuple):
             scope = backup[0]
             action = backup[1]
             order = self.get_process_order(scope, action)
```

### Comparing `deep_tracking-1.0.8/deep_tracking.egg-info/PKG-INFO` & `deep_tracking-1.0.9/deep_tracking.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-tracking
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library to track the development of data science works using the DE&P method
 Home-page: https://github.com/biazotogabriel/deep_tracking
 Author: Gabriel Nuernberg Biazoto
 Author-email: biazotogabriel@gmail.com
 License: MIT
 Keywords: deep de&p data science
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deep_tracking-1.0.8/setup.py` & `deep_tracking-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='deep_tracking',
-    version='1.0.8',
+    version='1.0.9',
     description='Library to track the development of data science works using the DE&P method',
     long_description = 'Library to track the development of data science works using the DE&P method',
     author='Gabriel Nuernberg Biazoto',
     author_email='biazotogabriel@gmail.com',
     url='https://github.com/biazotogabriel/deep_tracking',
     packages=['deep_tracking'],
     license = 'MIT',
```

