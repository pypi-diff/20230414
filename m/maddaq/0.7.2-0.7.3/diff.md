# Comparing `tmp/maddaq-0.7.2.tar.gz` & `tmp/maddaq-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maddaq-0.7.2.tar", last modified: Thu Apr 13 19:59:55 2023, max compression
+gzip compressed data, was "maddaq-0.7.3.tar", last modified: Fri Apr 14 16:23:32 2023, max compression
```

## Comparing `maddaq-0.7.2.tar` & `maddaq-0.7.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 19:59:55.037039 maddaq-0.7.2/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-13 19:59:55.036725 maddaq-0.7.2/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.2/README.md
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 19:59:55.031521 maddaq-0.7.2/maddaq/
--rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.2/maddaq/GTimer.py
--rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.2/maddaq/MadDAQData.py
--rw-r--r--   0 lacasta    (503) staff       (20)    13786 2023-04-04 16:03:13.000000 maddaq-0.7.2/maddaq/MadDAQModule.py
--rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.2/maddaq/Progress.py
--rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.2/maddaq/ScanManager.py
--rw-r--r--   0 lacasta    (503) staff       (20)      486 2023-04-13 19:59:41.000000 maddaq-0.7.2/maddaq/__init__.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 19:59:55.036329 maddaq-0.7.2/maddaq/cmmds/
--rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.2/maddaq/cmmds/__init__.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.2/maddaq/cmmds/analyze_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.2/maddaq/cmmds/file_info.py
--rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.2/maddaq/cmmds/fit_utils.py
--rw-r--r--   0 lacasta    (503) staff       (20)     5783 2023-04-13 16:47:46.000000 maddaq-0.7.2/maddaq/cmmds/getSpectrum.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.2/maddaq/cmmds/read_data.py
--rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.2/maddaq/cmmds/show_data.py
-drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-13 19:59:55.033870 maddaq-0.7.2/maddaq.egg-info/
--rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-13 19:59:55.000000 maddaq-0.7.2/maddaq.egg-info/PKG-INFO
--rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-13 19:59:55.000000 maddaq-0.7.2/maddaq.egg-info/SOURCES.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-13 19:59:55.000000 maddaq-0.7.2/maddaq.egg-info/dependency_links.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-13 19:59:55.000000 maddaq-0.7.2/maddaq.egg-info/entry_points.txt
--rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-13 19:59:55.000000 maddaq-0.7.2/maddaq.egg-info/requires.txt
--rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-13 19:59:55.000000 maddaq-0.7.2/maddaq.egg-info/top_level.txt
--rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-13 19:54:51.000000 maddaq-0.7.2/pyproject.toml
--rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-13 19:59:55.037114 maddaq-0.7.2/setup.cfg
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-14 16:23:32.489770 maddaq-0.7.3/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-14 16:23:32.489497 maddaq-0.7.3/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)     4553 2023-04-13 15:28:31.000000 maddaq-0.7.3/README.md
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-14 16:23:32.483177 maddaq-0.7.3/maddaq/
+-rw-r--r--   0 lacasta    (503) staff       (20)      998 2019-09-19 07:26:57.000000 maddaq-0.7.3/maddaq/GTimer.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     7547 2022-10-13 08:37:37.000000 maddaq-0.7.3/maddaq/MadDAQData.py
+-rw-r--r--   0 lacasta    (503) staff       (20)    14238 2023-04-14 16:21:00.000000 maddaq-0.7.3/maddaq/MadDAQModule.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     2336 2022-01-12 19:26:43.000000 maddaq-0.7.3/maddaq/Progress.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     4037 2022-10-01 17:07:05.000000 maddaq-0.7.3/maddaq/ScanManager.py
+-rw-r--r--   0 lacasta    (503) staff       (20)      485 2023-04-14 16:15:11.000000 maddaq-0.7.3/maddaq/__init__.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-14 16:23:32.488980 maddaq-0.7.3/maddaq/cmmds/
+-rw-r--r--   0 lacasta    (503) staff       (20)        0 2023-04-13 16:51:33.000000 maddaq-0.7.3/maddaq/cmmds/__init__.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     5865 2023-04-13 19:53:59.000000 maddaq-0.7.3/maddaq/cmmds/analyze_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)      586 2023-04-13 16:17:24.000000 maddaq-0.7.3/maddaq/cmmds/file_info.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     8197 2022-10-01 17:15:09.000000 maddaq-0.7.3/maddaq/cmmds/fit_utils.py
+-rw-r--r--   0 lacasta    (503) staff       (20)     5783 2023-04-13 16:47:46.000000 maddaq-0.7.3/maddaq/cmmds/getSpectrum.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     1887 2023-04-13 16:16:23.000000 maddaq-0.7.3/maddaq/cmmds/read_data.py
+-rwxr-xr-x   0 lacasta    (503) staff       (20)     6111 2023-04-13 16:13:35.000000 maddaq-0.7.3/maddaq/cmmds/show_data.py
+drwxr-xr-x   0 lacasta    (503) staff       (20)        0 2023-04-14 16:23:32.485847 maddaq-0.7.3/maddaq.egg-info/
+-rw-r--r--   0 lacasta    (503) staff       (20)     4987 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/PKG-INFO
+-rw-r--r--   0 lacasta    (503) staff       (20)      513 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/SOURCES.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        1 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/dependency_links.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      144 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/entry_points.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)       71 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/requires.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)        7 2023-04-14 16:23:32.000000 maddaq-0.7.3/maddaq.egg-info/top_level.txt
+-rw-r--r--   0 lacasta    (503) staff       (20)      810 2023-04-14 16:15:11.000000 maddaq-0.7.3/pyproject.toml
+-rw-r--r--   0 lacasta    (503) staff       (20)       38 2023-04-14 16:23:32.489847 maddaq-0.7.3/setup.cfg
```

### Comparing `maddaq-0.7.2/PKG-INFO` & `maddaq-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.2
+Version: 0.7.3
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.2/README.md` & `maddaq-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/GTimer.py` & `maddaq-0.7.3/maddaq/GTimer.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/MadDAQData.py` & `maddaq-0.7.3/maddaq/MadDAQData.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/MadDAQModule.py` & `maddaq-0.7.3/maddaq/MadDAQModule.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,25 +261,39 @@
             cmmd = np.mean(data[1:])
             data -= cmmd
         else:
             cmmd = 0.0
 
         out = []
         if evt.romode == MadDAQModule.SPARSE_ADJ and self.do_cluster:
-            sn = data/self.noise[indx]
+            vsn = data/self.noise[indx]
             E = 0.0
             X = 0.0
             nstrip = 0
-            for val, sn, indx in zip(data, sn, self.adjacents):
-                if sn > 5.0:
+            i = 0
+            while i < len(data):
+                if i == 0:
+                    val = data[i]
                     E += val
-                    X += indx*val
+                    X += self.adjacents[i]*val
                     nstrip += val
+                    i += 1
                 else:
-                    break
+                    ngood = 0
+                    for j in (i, i+1):
+                        if vsn[j] > 5.0:
+                            val = data[j]
+                            E += val
+                            X += self.adjacents[j]*val
+                            nstrip += val
+                            ngood += 1
+
+                    i += 2
+                    if ngood == 0:
+                        break
 
             if nstrip > 0:
                 X /= nstrip
                 out.append((evt.chan+X, E))
 
         else:
             out.append((evt.chan, data[0]))
```

### Comparing `maddaq-0.7.2/maddaq/Progress.py` & `maddaq-0.7.3/maddaq/Progress.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/ScanManager.py` & `maddaq-0.7.3/maddaq/ScanManager.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/cmmds/analyze_data.py` & `maddaq-0.7.3/maddaq/cmmds/analyze_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/cmmds/file_info.py` & `maddaq-0.7.3/maddaq/cmmds/file_info.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/cmmds/fit_utils.py` & `maddaq-0.7.3/maddaq/cmmds/fit_utils.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/cmmds/getSpectrum.py` & `maddaq-0.7.3/maddaq/cmmds/getSpectrum.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/cmmds/read_data.py` & `maddaq-0.7.3/maddaq/cmmds/read_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq/cmmds/show_data.py` & `maddaq-0.7.3/maddaq/cmmds/show_data.py`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/maddaq.egg-info/PKG-INFO` & `maddaq-0.7.3/maddaq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maddaq
-Version: 0.7.2
+Version: 0.7.3
 Summary: A collection of python scripts to access maddaq data.
 Author-email: Carlos Lacasta <carlos.lacasta@alibavasystems.com>
 Project-URL: Homepage, https://igit.ific.uv.es
 Project-URL: Bug Tracker, https://igit.ific.uv.es
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `maddaq-0.7.2/maddaq.egg-info/SOURCES.txt` & `maddaq-0.7.3/maddaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maddaq-0.7.2/pyproject.toml` & `maddaq-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maddaq"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
   { name="Carlos Lacasta", email="carlos.lacasta@alibavasystems.com" },
 ]
 description = "A collection of python scripts to access maddaq data."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

