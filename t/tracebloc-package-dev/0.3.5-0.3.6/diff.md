# Comparing `tmp/tracebloc_package-dev-0.3.5.tar.gz` & `tmp/tracebloc_package-dev-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.3.5.tar", last modified: Fri Mar 31 04:32:30 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.3.6.tar", last modified: Fri Apr 14 07:24:26 2023, max compression
```

## Comparing `tracebloc_package-dev-0.3.5.tar` & `tracebloc_package-dev-0.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-03-31 04:32:30.869815 tracebloc_package-dev-0.3.5/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.3.5/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-03-31 04:32:30.869915 tracebloc_package-dev-0.3.5/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.3.5/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-03-31 04:32:30.870240 tracebloc_package-dev-0.3.5/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      859 2023-03-31 04:31:52.000000 tracebloc_package-dev-0.3.5/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-03-31 04:32:30.868289 tracebloc_package-dev-0.3.5/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.3.5/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5697 2023-03-20 10:56:57.000000 tracebloc_package-dev-0.3.5/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    16788 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.5/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    53146 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.5/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.3.5/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)     7029 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.5/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10062 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.5/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     3832 2023-03-20 08:05:24.000000 tracebloc_package-dev-0.3.5/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.3.5/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-03-31 04:32:30.869655 tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-03-31 04:32:30.000000 tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-03-31 04:32:30.000000 tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-03-31 04:32:30.000000 tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-03-31 04:32:30.000000 tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)       73 2023-03-31 04:32:30.000000 tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-03-31 04:32:30.000000 tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-04-14 07:24:26.918223 tracebloc_package-dev-0.3.6/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.3.6/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-04-14 07:24:26.918519 tracebloc_package-dev-0.3.6/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.3.6/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-04-14 07:24:26.919491 tracebloc_package-dev-0.3.6/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      859 2023-04-14 07:23:43.000000 tracebloc_package-dev-0.3.6/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-04-14 07:24:26.916744 tracebloc_package-dev-0.3.6/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-03-15 10:59:39.000000 tracebloc_package-dev-0.3.6/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5697 2023-03-20 10:56:57.000000 tracebloc_package-dev-0.3.6/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    16788 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.6/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    53195 2023-04-14 07:22:52.000000 tracebloc_package-dev-0.3.6/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.3.6/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7029 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.6/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10062 2023-03-31 04:30:11.000000 tracebloc_package-dev-0.3.6/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3832 2023-03-20 08:05:24.000000 tracebloc_package-dev-0.3.6/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3203 2022-06-09 05:22:24.000000 tracebloc_package-dev-0.3.6/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-04-14 07:24:26.918048 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)       73 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-04-14 07:24:26.000000 tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.3.5/LICENSE.txt` & `tracebloc_package-dev-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.5/PKG-INFO` & `tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tracebloc_package-dev
-Version: 0.3.5
+Name: tracebloc-package-dev
+Version: 0.3.6
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.3.5/setup.py` & `tracebloc_package-dev-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.3.5",
+    version="0.3.6",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.3.6/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.3.6/tracebloc_package/functional_test.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.3.6/tracebloc_package/linkModelDataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,16 +386,18 @@
         # get images count for selected edge
         images = int(self.__total_images[edge_min])
         batch = images // 3
         if 8 < batch < 16:
             return 8
         elif 16 < batch < 32:
             return 16
-        if 32 < batch < 64:
+        elif 32 < batch < 64:
             return 32
+        elif batch > 64:
+            return 64
         else:
             return batch
 
     def batchSize(self, batchSize: int):
         """
         Integer or None. Number of samples per gradient update. If unspecified, batch_size will default to 32.
         example: trainingObject.batchSize(16)
```

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package/messages.py` & `tracebloc_package-dev-0.3.6/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package/upload.py` & `tracebloc_package-dev-0.3.6/tracebloc_package/upload.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package/user.py` & `tracebloc_package-dev-0.3.6/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package/utils.py` & `tracebloc_package-dev-0.3.6/tracebloc_package/utils.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package/weights.py` & `tracebloc_package-dev-0.3.6/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tracebloc-package-dev
-Version: 0.3.5
+Name: tracebloc_package-dev
+Version: 0.3.6
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.3.5/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.3.6/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

