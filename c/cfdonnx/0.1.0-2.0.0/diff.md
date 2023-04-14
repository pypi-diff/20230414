# Comparing `tmp/cfdonnx-0.1.0.tar.gz` & `tmp/cfdonnx-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdonnx-0.1.0.tar", last modified: Fri Apr 14 11:46:15 2023, max compression
+gzip compressed data, was "cfdonnx-2.0.0.tar", last modified: Fri Apr 14 13:55:31 2023, max compression
```

## Comparing `cfdonnx-0.1.0.tar` & `cfdonnx-2.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 11:46:15.501229 cfdonnx-0.1.0/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-04-14 11:39:22.000000 cfdonnx-0.1.0/LICENSE.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2340 2023-04-14 11:46:15.501229 cfdonnx-0.1.0/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1903 2023-04-14 11:37:14.000000 cfdonnx-0.1.0/README.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-04-14 11:46:15.501229 cfdonnx-0.1.0/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      730 2023-04-14 11:46:02.000000 cfdonnx-0.1.0/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 11:46:15.497229 cfdonnx-0.1.0/src/
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 11:46:15.497229 cfdonnx-0.1.0/src/cfdonnx/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-04-06 08:52:13.000000 cfdonnx-0.1.0/src/cfdonnx/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     5536 2023-04-13 23:42:42.000000 cfdonnx-0.1.0/src/cfdonnx/__main__.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 11:46:15.501229 cfdonnx-0.1.0/src/cfdonnx/models/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-04-06 08:52:13.000000 cfdonnx-0.1.0/src/cfdonnx/models/__init__.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 11:46:15.501229 cfdonnx-0.1.0/src/cfdonnx/models/torch/
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1981 2023-04-06 09:08:43.000000 cfdonnx-0.1.0/src/cfdonnx/models/torch/AutoEncoder.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     1840 2023-04-06 09:08:33.000000 cfdonnx-0.1.0/src/cfdonnx/models/torch/AutoEncoderEx.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     5388 2023-04-13 22:55:57.000000 cfdonnx-0.1.0/src/cfdonnx/models/torch/MaxUnpool.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     4700 2023-04-06 09:12:55.000000 cfdonnx-0.1.0/src/cfdonnx/models/torch/UNetEx.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-04-06 08:52:13.000000 cfdonnx-0.1.0/src/cfdonnx/models/torch/__init__.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 11:46:15.497229 cfdonnx-0.1.0/src/cfdonnx.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2340 2023-04-14 11:46:15.000000 cfdonnx-0.1.0/src/cfdonnx.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      441 2023-04-14 11:46:15.000000 cfdonnx-0.1.0/src/cfdonnx.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-04-14 11:46:15.000000 cfdonnx-0.1.0/src/cfdonnx.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        8 2023-04-14 11:46:15.000000 cfdonnx-0.1.0/src/cfdonnx.egg-info/top_level.txt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 13:55:31.975653 cfdonnx-2.0.0/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1069 2023-04-14 11:39:22.000000 cfdonnx-2.0.0/LICENSE.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2340 2023-04-14 13:55:31.975653 cfdonnx-2.0.0/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1903 2023-04-14 11:37:14.000000 cfdonnx-2.0.0/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-04-14 13:55:31.975653 cfdonnx-2.0.0/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      840 2023-04-14 13:54:58.000000 cfdonnx-2.0.0/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 13:55:31.975653 cfdonnx-2.0.0/src/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 13:55:31.975653 cfdonnx-2.0.0/src/cfdonnx/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-04-06 08:52:13.000000 cfdonnx-2.0.0/src/cfdonnx/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     5536 2023-04-13 23:42:42.000000 cfdonnx-2.0.0/src/cfdonnx/__main__.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 13:55:31.975653 cfdonnx-2.0.0/src/cfdonnx/models/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-04-06 08:52:13.000000 cfdonnx-2.0.0/src/cfdonnx/models/__init__.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 13:55:31.975653 cfdonnx-2.0.0/src/cfdonnx/models/torch/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1981 2023-04-06 09:08:43.000000 cfdonnx-2.0.0/src/cfdonnx/models/torch/AutoEncoder.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     1840 2023-04-06 09:08:33.000000 cfdonnx-2.0.0/src/cfdonnx/models/torch/AutoEncoderEx.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     5388 2023-04-14 13:28:58.000000 cfdonnx-2.0.0/src/cfdonnx/models/torch/MaxUnpool.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     4700 2023-04-06 09:12:55.000000 cfdonnx-2.0.0/src/cfdonnx/models/torch/UNetEx.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-04-06 08:52:13.000000 cfdonnx-2.0.0/src/cfdonnx/models/torch/__init__.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-04-14 13:55:31.975653 cfdonnx-2.0.0/src/cfdonnx.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2340 2023-04-14 13:55:31.000000 cfdonnx-2.0.0/src/cfdonnx.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      475 2023-04-14 13:55:31.000000 cfdonnx-2.0.0/src/cfdonnx.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-04-14 13:55:31.000000 cfdonnx-2.0.0/src/cfdonnx.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       66 2023-04-14 13:55:31.000000 cfdonnx-2.0.0/src/cfdonnx.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        8 2023-04-14 13:55:31.000000 cfdonnx-2.0.0/src/cfdonnx.egg-info/top_level.txt
```

### Comparing `cfdonnx-0.1.0/LICENSE.txt` & `cfdonnx-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cfdonnx-0.1.0/PKG-INFO` & `cfdonnx-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdonnx
-Version: 0.1.0
+Version: 2.0.0
 Summary: Converting ML-CFD models to ONNX
 Home-page: https://github.com/simzero/cfdonnx
 Author: Carlos Pena Monferrer
 License: MIT
 Keywords: cfd ml onnx
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cfdonnx-0.1.0/README.md` & `cfdonnx-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cfdonnx-0.1.0/setup.py` & `cfdonnx-2.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='cfdonnx',
-    version='0.1.0',
+    version='2.0.0',
     description='Converting ML-CFD models to ONNX',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Carlos Pena Monferrer',
     keywords='cfd ml onnx',
     url='https://github.com/simzero/cfdonnx',
     packages=['cfdonnx', 'cfdonnx.models', 'cfdonnx.models.torch'],
@@ -17,9 +17,13 @@
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
+        "torch==2.0.0",
+        "torchvision==0.15.1",
+        "onnx==1.13.1",
+        "onnxruntime==1.14.1",
     ],
 )
```

### Comparing `cfdonnx-0.1.0/src/cfdonnx/__main__.py` & `cfdonnx-2.0.0/src/cfdonnx/__main__.py`

 * *Files identical despite different names*

### Comparing `cfdonnx-0.1.0/src/cfdonnx/models/torch/AutoEncoder.py` & `cfdonnx-2.0.0/src/cfdonnx/models/torch/AutoEncoder.py`

 * *Files identical despite different names*

### Comparing `cfdonnx-0.1.0/src/cfdonnx/models/torch/AutoEncoderEx.py` & `cfdonnx-2.0.0/src/cfdonnx/models/torch/AutoEncoderEx.py`

 * *Files identical despite different names*

### Comparing `cfdonnx-0.1.0/src/cfdonnx/models/torch/MaxUnpool.py` & `cfdonnx-2.0.0/src/cfdonnx/models/torch/MaxUnpool.py`

 * *Files identical despite different names*

### Comparing `cfdonnx-0.1.0/src/cfdonnx/models/torch/UNetEx.py` & `cfdonnx-2.0.0/src/cfdonnx/models/torch/UNetEx.py`

 * *Files identical despite different names*

### Comparing `cfdonnx-0.1.0/src/cfdonnx.egg-info/PKG-INFO` & `cfdonnx-2.0.0/src/cfdonnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdonnx
-Version: 0.1.0
+Version: 2.0.0
 Summary: Converting ML-CFD models to ONNX
 Home-page: https://github.com/simzero/cfdonnx
 Author: Carlos Pena Monferrer
 License: MIT
 Keywords: cfd ml onnx
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

