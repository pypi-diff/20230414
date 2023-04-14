# Comparing `tmp/alma-cdk.cross-region-parameter-0.0.13.tar.gz` & `tmp/alma-cdk.cross-region-parameter-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alma-cdk.cross-region-parameter-0.0.13.tar", last modified: Tue Nov  8 10:38:27 2022, max compression
+gzip compressed data, was "alma-cdk.cross-region-parameter-0.0.14.tar", last modified: Fri Apr 14 08:08:32 2023, max compression
```

## Comparing `alma-cdk.cross-region-parameter-0.0.13.tar` & `alma-cdk.cross-region-parameter-0.0.14.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:38:27.141346 alma-cdk.cross-region-parameter-0.0.13/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-11-08 10:38:27.141346 alma-cdk.cross-region-parameter-0.0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-08 10:38:27.141346 alma-cdk.cross-region-parameter-0.0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:38:27.129346 alma-cdk.cross-region-parameter-0.0.13/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:38:27.129346 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:38:27.129346 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk/cross_region_parameter/
--rw-r--r--   0 runner    (1001) docker     (121)    22901 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk/cross_region_parameter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:38:27.129346 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk/cross_region_parameter/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk/cross_region_parameter/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121) 10201680 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk/cross_region_parameter/_jsii/cross-region-parameter@0.0.13.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 10:38:15.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk/cross_region_parameter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 10:38:27.129346 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk.cross_region_parameter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2244 2022-11-08 10:38:26.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk.cross_region_parameter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-11-08 10:38:27.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk.cross_region_parameter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 10:38:26.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk.cross_region_parameter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-08 10:38:26.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk.cross_region_parameter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-08 10:38:27.000000 alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk.cross_region_parameter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:08:32.478240 alma-cdk.cross-region-parameter-0.0.14/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-14 08:08:32.478240 alma-cdk.cross-region-parameter-0.0.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:08:32.478240 alma-cdk.cross-region-parameter-0.0.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:08:32.466240 alma-cdk.cross-region-parameter-0.0.14/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:08:32.466240 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:08:32.470240 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk/cross_region_parameter/
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk/cross_region_parameter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:08:32.470240 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk/cross_region_parameter/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk/cross_region_parameter/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 10201686 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk/cross_region_parameter/_jsii/cross-region-parameter@0.0.14.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:08:18.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk/cross_region_parameter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:08:32.470240 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk.cross_region_parameter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-14 08:08:31.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk.cross_region_parameter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-14 08:08:32.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk.cross_region_parameter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:08:31.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk.cross_region_parameter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 08:08:32.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk.cross_region_parameter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 08:08:32.000000 alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk.cross_region_parameter.egg-info/top_level.txt
```

### Comparing `alma-cdk.cross-region-parameter-0.0.13/LICENSE` & `alma-cdk.cross-region-parameter-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `alma-cdk.cross-region-parameter-0.0.13/PKG-INFO` & `alma-cdk.cross-region-parameter-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alma-cdk.cross-region-parameter
-Version: 0.0.13
+Version: 0.0.14
 Summary: Store AWS SSM Parameter Store Parameters into another AWS Region with AWS CDK
 Home-page: https://github.com/alma-cdk/cross-region-parameter.git
 Author: Alma Media<opensource@almamedia.dev>
 License: Apache-2.0
 Project-URL: Source, https://github.com/alma-cdk/cross-region-parameter.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `alma-cdk.cross-region-parameter-0.0.13/README.md` & `alma-cdk.cross-region-parameter-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `alma-cdk.cross-region-parameter-0.0.13/setup.py` & `alma-cdk.cross-region-parameter-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "alma-cdk.cross-region-parameter",
-    "version": "0.0.13",
+    "version": "0.0.14",
     "description": "Store AWS SSM Parameter Store Parameters into another AWS Region with AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/alma-cdk/cross-region-parameter.git",
     "long_description_content_type": "text/markdown",
     "author": "Alma Media<opensource@almamedia.dev>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "alma_cdk.cross_region_parameter",
         "alma_cdk.cross_region_parameter._jsii"
     ],
     "package_data": {
         "alma_cdk.cross_region_parameter._jsii": [
-            "cross-region-parameter@0.0.13.jsii.tgz"
+            "cross-region-parameter@0.0.14.jsii.tgz"
         ],
         "alma_cdk.cross_region_parameter": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk/cross_region_parameter/__init__.py` & `alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk/cross_region_parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk.cross_region_parameter.egg-info/PKG-INFO` & `alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk.cross_region_parameter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alma-cdk.cross-region-parameter
-Version: 0.0.13
+Version: 0.0.14
 Summary: Store AWS SSM Parameter Store Parameters into another AWS Region with AWS CDK
 Home-page: https://github.com/alma-cdk/cross-region-parameter.git
 Author: Alma Media<opensource@almamedia.dev>
 License: Apache-2.0
 Project-URL: Source, https://github.com/alma-cdk/cross-region-parameter.git
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `alma-cdk.cross-region-parameter-0.0.13/src/alma_cdk.cross_region_parameter.egg-info/SOURCES.txt` & `alma-cdk.cross-region-parameter-0.0.14/src/alma_cdk.cross_region_parameter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/alma_cdk.cross_region_parameter.egg-info/SOURCES.txt
 src/alma_cdk.cross_region_parameter.egg-info/dependency_links.txt
 src/alma_cdk.cross_region_parameter.egg-info/requires.txt
 src/alma_cdk.cross_region_parameter.egg-info/top_level.txt
 src/alma_cdk/cross_region_parameter/__init__.py
 src/alma_cdk/cross_region_parameter/py.typed
 src/alma_cdk/cross_region_parameter/_jsii/__init__.py
-src/alma_cdk/cross_region_parameter/_jsii/cross-region-parameter@0.0.13.jsii.tgz
+src/alma_cdk/cross_region_parameter/_jsii/cross-region-parameter@0.0.14.jsii.tgz
```

