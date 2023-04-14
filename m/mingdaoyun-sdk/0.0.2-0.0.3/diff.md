# Comparing `tmp/mingdaoyun-sdk-0.0.2.tar.gz` & `tmp/mingdaoyun_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mingdaoyun-sdk-0.0.2.tar", last modified: Fri Apr 14 06:09:11 2023, max compression
+gzip compressed data, was "mingdaoyun_sdk-0.0.3.tar", last modified: Fri Apr 14 06:14:01 2023, max compression
```

## Comparing `mingdaoyun-sdk-0.0.2.tar` & `mingdaoyun_sdk-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/MingdaoOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/MingdaoYun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:09:11.000000 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 06:09:11.000000 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:09:11.000000 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 06:09:11.000000 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:14:01.335882 mingdaoyun_sdk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:14:01.335882 mingdaoyun_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:14:01.331882 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/MingdaoOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/MingdaoYun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:14:01.331882 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:14:01.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 06:14:01.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:14:01.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 06:14:01.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:14:01.335882 mingdaoyun_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/setup.py
```

### Comparing `mingdaoyun-sdk-0.0.2/PKG-INFO` & `mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mingdaoyun-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: 针对mingdaoyun的API封装的Python-SDK包
 Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
 Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/MingdaoOrg.py` & `mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/MingdaoOrg.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/MingdaoYun.py` & `mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/MingdaoYun.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/common.py` & `mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/common.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/PKG-INFO` & `mingdaoyun_sdk-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mingdaoyun-sdk
-Version: 0.0.2
+Name: mingdaoyun_sdk
+Version: 0.0.3
 Summary: 针对mingdaoyun的API封装的Python-SDK包
 Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
 Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mingdaoyun-sdk-0.0.2/setup.py` & `mingdaoyun_sdk-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
-    name="mingdaoyun-sdk",
+    name="mingdaoyun_sdk",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.0.2",
+    version="0.0.3",
     # 作者名
     author="Todd",
     # 作者邮箱
     author_email="ghostlitao@gmail.com",
     # 包的简介描述
     description="针对mingdaoyun的API封装的Python-SDK包",
     # 包的详细介绍(一般通过加载README.md)
```

