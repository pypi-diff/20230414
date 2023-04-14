# Comparing `tmp/flojoy-0.2.2.dev6.tar.gz` & `tmp/flojoy-0.2.2.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flojoy-0.2.2.dev6.tar", last modified: Fri Apr 14 15:28:06 2023, max compression
+gzip compressed data, was "flojoy-0.2.2.dev7.tar", last modified: Fri Apr 14 16:11:39 2023, max compression
```

## Comparing `flojoy-0.2.2.dev6.tar` & `flojoy-0.2.2.dev7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-14 15:28:06.356133 flojoy-0.2.2.dev6/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1062 2022-10-05 16:22:32.000000 flojoy-0.2.2.dev6/LICENSE.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-14 15:28:06.356133 flojoy-0.2.2.dev6/PKG-INFO
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       31 2022-10-05 16:21:51.000000 flojoy-0.2.2.dev6/README.md
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-14 15:28:06.356133 flojoy-0.2.2.dev6/flojoy/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      188 2023-04-03 20:53:50.000000 flojoy-0.2.2.dev6/flojoy/__init__.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      209 2023-04-04 16:27:03.000000 flojoy-0.2.2.dev6/flojoy/flojoy_instruction.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    19695 2023-04-13 22:54:52.000000 flojoy-0.2.2.dev6/flojoy/flojoy_python.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2132 2023-04-13 22:49:50.000000 flojoy-0.2.2.dev6/flojoy/job_result_builder.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1725 2023-04-13 22:53:14.000000 flojoy-0.2.2.dev6/flojoy/job_result_utils.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1287 2023-04-14 15:24:45.000000 flojoy-0.2.2.dev6/flojoy/plotly_utils.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6070 2023-02-20 19:12:45.000000 flojoy-0.2.2.dev6/flojoy/utils.py
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-14 15:28:06.356133 flojoy-0.2.2.dev6/flojoy.egg-info/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-14 15:28:06.000000 flojoy-0.2.2.dev6/flojoy.egg-info/PKG-INFO
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-04-14 15:28:06.000000 flojoy-0.2.2.dev6/flojoy.egg-info/SOURCES.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-04-14 15:28:06.000000 flojoy-0.2.2.dev6/flojoy.egg-info/dependency_links.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-04-14 15:28:06.000000 flojoy-0.2.2.dev6/flojoy.egg-info/requires.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-04-14 15:28:06.000000 flojoy-0.2.2.dev6/flojoy.egg-info/top_level.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-04-14 15:28:06.356133 flojoy-0.2.2.dev6/setup.cfg
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      956 2023-04-14 15:27:34.000000 flojoy-0.2.2.dev6/setup.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-14 16:11:39.886619 flojoy-0.2.2.dev7/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1062 2022-10-05 16:22:32.000000 flojoy-0.2.2.dev7/LICENSE.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-14 16:11:39.886619 flojoy-0.2.2.dev7/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       31 2022-10-05 16:21:51.000000 flojoy-0.2.2.dev7/README.md
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-14 16:11:39.886619 flojoy-0.2.2.dev7/flojoy/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      188 2023-04-03 20:53:50.000000 flojoy-0.2.2.dev7/flojoy/__init__.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      209 2023-04-04 16:27:03.000000 flojoy-0.2.2.dev7/flojoy/flojoy_instruction.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    19695 2023-04-13 22:54:52.000000 flojoy-0.2.2.dev7/flojoy/flojoy_python.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2132 2023-04-13 22:49:50.000000 flojoy-0.2.2.dev7/flojoy/job_result_builder.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1725 2023-04-13 22:53:14.000000 flojoy-0.2.2.dev7/flojoy/job_result_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1311 2023-04-14 16:09:21.000000 flojoy-0.2.2.dev7/flojoy/plotly_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6070 2023-02-20 19:12:45.000000 flojoy-0.2.2.dev7/flojoy/utils.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-14 16:11:39.886619 flojoy-0.2.2.dev7/flojoy.egg-info/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-14 16:11:39.000000 flojoy-0.2.2.dev7/flojoy.egg-info/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-04-14 16:11:39.000000 flojoy-0.2.2.dev7/flojoy.egg-info/SOURCES.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-04-14 16:11:39.000000 flojoy-0.2.2.dev7/flojoy.egg-info/dependency_links.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-04-14 16:11:39.000000 flojoy-0.2.2.dev7/flojoy.egg-info/requires.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-04-14 16:11:39.000000 flojoy-0.2.2.dev7/flojoy.egg-info/top_level.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-04-14 16:11:39.886619 flojoy-0.2.2.dev7/setup.cfg
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      956 2023-04-14 16:11:13.000000 flojoy-0.2.2.dev7/setup.py
```

### Comparing `flojoy-0.2.2.dev6/LICENSE.txt` & `flojoy-0.2.2.dev7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev6/PKG-INFO` & `flojoy-0.2.2.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.2.2.dev6
+Version: 0.2.2.dev7
 Summary: Python client library for Flojoy.
 Home-page: https://github.com/flojoy-io/flojoy-python
 Author: flojoy
 Author-email: jack.parmer@proton.me
 License: MIT
 Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
 Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
```

### Comparing `flojoy-0.2.2.dev6/flojoy/flojoy_python.py` & `flojoy-0.2.2.dev7/flojoy/flojoy_python.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev6/flojoy/job_result_builder.py` & `flojoy-0.2.2.dev7/flojoy/job_result_builder.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev6/flojoy/job_result_utils.py` & `flojoy-0.2.2.dev7/flojoy/job_result_utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev6/flojoy/plotly_utils.py` & `flojoy-0.2.2.dev7/flojoy/plotly_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             if value.a is None:
                 img_combined = np.stack((value.r, value.g, value.b), axis=2)
             else:
                 img_combined = np.stack(
                     (value.r, value.g, value.b, value.a), axis=2)
             fig = px.imshow(img=img_combined)
         case 'ordered_pair':
-            if len(value.x) != len(value.y):
+            if value.x is not None and len(value.x) != len(value.y):
                 value.x = np.arange(0, len(value.y), 1)
             fig = px.line(x=value.x, y=value.y)
         case 'ordered_triple':
             fig = px.scatter_3d(x=value.x, y=value.y, z=value.z)
         case 'scalar':
             fig = px.histogram(x=value.c)
         case 'grayscale' | 'matrix' | 'dataframe':
```

### Comparing `flojoy-0.2.2.dev6/flojoy/utils.py` & `flojoy-0.2.2.dev7/flojoy/utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev6/flojoy.egg-info/PKG-INFO` & `flojoy-0.2.2.dev7/flojoy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.2.2.dev6
+Version: 0.2.2.dev7
 Summary: Python client library for Flojoy.
 Home-page: https://github.com/flojoy-io/flojoy-python
 Author: flojoy
 Author-email: jack.parmer@proton.me
 License: MIT
 Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
 Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
```

### Comparing `flojoy-0.2.2.dev6/setup.py` & `flojoy-0.2.2.dev7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name='flojoy',
     packages=['flojoy'],
-    version='0.2.2.dev6',
+    version='0.2.2.dev7',
     license='MIT',
     description='Python client library for Flojoy.',
     author='flojoy',
     author_email='jack.parmer@proton.me',
     url='https://github.com/flojoy-io/flojoy-python',
     download_url='https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip',
     keywords=['data-acquisition', 'lab-automation', 'low-code', 'python', 'scheduler', 'topic'],
```

