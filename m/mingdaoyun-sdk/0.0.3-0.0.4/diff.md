# Comparing `tmp/mingdaoyun_sdk-0.0.3.tar.gz` & `tmp/mingdaoyun_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mingdaoyun_sdk-0.0.3.tar", last modified: Fri Apr 14 06:14:01 2023, max compression
+gzip compressed data, was "mingdaoyun_sdk-0.0.4.tar", last modified: Fri Apr 14 06:25:44 2023, max compression
```

## Comparing `mingdaoyun_sdk-0.0.3.tar` & `mingdaoyun_sdk-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:14:01.335882 mingdaoyun_sdk-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:14:01.335882 mingdaoyun_sdk-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:14:01.331882 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/MingdaoOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/MingdaoYun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:14:01.331882 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:14:01.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 06:14:01.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:14:01.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 06:14:01.000000 mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:14:01.335882 mingdaoyun_sdk-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-14 06:13:44.000000 mingdaoyun_sdk-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:25:44.014514 mingdaoyun_sdk-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:25:44.014514 mingdaoyun_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 06:25:34.000000 mingdaoyun_sdk-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:25:44.010514 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-14 06:25:34.000000 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk/MingdaoOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-04-14 06:25:34.000000 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk/MingdaoYun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:25:34.000000 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-14 06:25:34.000000 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:25:44.014514 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:25:44.000000 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 06:25:44.000000 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:25:44.000000 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 06:25:44.000000 mingdaoyun_sdk-0.0.4/mingdaoyun_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:25:44.014514 mingdaoyun_sdk-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-14 06:25:34.000000 mingdaoyun_sdk-0.0.4/setup.py
```

### Comparing `mingdaoyun_sdk-0.0.3/PKG-INFO` & `mingdaoyun_sdk-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mingdaoyun_sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: 针对mingdaoyun的API封装的Python-SDK包
 Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
 Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/MingdaoOrg.py` & `mingdaoyun_sdk-0.0.4/mingdaoyun_sdk/MingdaoOrg.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @Version 1.0
 @Description 明道云组织结构帮助类
 """
 import hashlib
 import base64
 import time
 
-from common import http
+from mingdaoyun_sdk.common import http
 
 
 class MingdaoOrg:
     appKey = ""
     secretKey = ""
     host = ""
     projectId = ""
```

### Comparing `mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/MingdaoYun.py` & `mingdaoyun_sdk-0.0.4/mingdaoyun_sdk/MingdaoYun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 """
 @Author Todd
 @Version 1.0
 @Description 明道云API封装类
 """
-from common import http
+from mingdaoyun_sdk.common import http
 
 
 class MingdaoYun:
     appKey = ""
     sign = ""
     host = ""
```

### Comparing `mingdaoyun_sdk-0.0.3/mingdaoyun_sdk/common.py` & `mingdaoyun_sdk-0.0.4/mingdaoyun_sdk/common.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun_sdk-0.0.3/mingdaoyun_sdk.egg-info/PKG-INFO` & `mingdaoyun_sdk-0.0.4/mingdaoyun_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mingdaoyun-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: 针对mingdaoyun的API封装的Python-SDK包
 Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
 Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mingdaoyun_sdk-0.0.3/setup.py` & `mingdaoyun_sdk-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="mingdaoyun_sdk",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.0.3",
+    version="0.0.4",
     # 作者名
     author="Todd",
     # 作者邮箱
     author_email="ghostlitao@gmail.com",
     # 包的简介描述
     description="针对mingdaoyun的API封装的Python-SDK包",
     # 包的详细介绍(一般通过加载README.md)
```

