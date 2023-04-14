# Comparing `tmp/baidufanyiformind-0.0.1.tar.gz` & `tmp/baidufanyiformind-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baidufanyiformind-0.0.1.tar", last modified: Fri Apr 14 13:42:37 2023, max compression
+gzip compressed data, was "baidufanyiformind-0.0.2.tar", last modified: Fri Apr 14 14:01:15 2023, max compression
```

## Comparing `baidufanyiformind-0.0.1.tar` & `baidufanyiformind-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:37.461382 baidufanyiformind-0.0.1/
--rw-rw-rw-   0        0        0      561 2023-04-14 13:42:37.461382 baidufanyiformind-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      133 2023-04-14 13:32:19.000000 baidufanyiformind-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:37.451272 baidufanyiformind-0.0.1/baidufanyiformind/
--rw-rw-rw-   0        0        0     2734 2023-04-14 13:40:36.000000 baidufanyiformind-0.0.1/baidufanyiformind/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:42:37.459382 baidufanyiformind-0.0.1/baidufanyiformind.egg-info/
--rw-rw-rw-   0        0        0      561 2023-04-14 13:42:37.000000 baidufanyiformind-0.0.1/baidufanyiformind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-14 13:42:37.000000 baidufanyiformind-0.0.1/baidufanyiformind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:42:37.000000 baidufanyiformind-0.0.1/baidufanyiformind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 13:42:37.000000 baidufanyiformind-0.0.1/baidufanyiformind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-14 13:42:37.000000 baidufanyiformind-0.0.1/baidufanyiformind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 13:42:37.462384 baidufanyiformind-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-04-14 13:31:09.000000 baidufanyiformind-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:01:15.623413 baidufanyiformind-0.0.2/
+-rw-rw-rw-   0        0        0      561 2023-04-14 14:01:15.623413 baidufanyiformind-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2023-04-14 13:32:19.000000 baidufanyiformind-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 14:01:15.615415 baidufanyiformind-0.0.2/baidufanyiformind/
+-rw-rw-rw-   0        0        0     2738 2023-04-14 14:00:38.000000 baidufanyiformind-0.0.2/baidufanyiformind/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:01:15.622414 baidufanyiformind-0.0.2/baidufanyiformind.egg-info/
+-rw-rw-rw-   0        0        0      561 2023-04-14 14:01:15.000000 baidufanyiformind-0.0.2/baidufanyiformind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-04-14 14:01:15.000000 baidufanyiformind-0.0.2/baidufanyiformind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:01:15.000000 baidufanyiformind-0.0.2/baidufanyiformind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-14 14:01:15.000000 baidufanyiformind-0.0.2/baidufanyiformind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:01:15.624416 baidufanyiformind-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-04-14 14:00:18.000000 baidufanyiformind-0.0.2/setup.py
```

### Comparing `baidufanyiformind-0.0.1/PKG-INFO` & `baidufanyiformind-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidufanyiformind
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for baidufanyi
 Home-page: https://gitee.com/liliang9693/baidufanyiformind
 Author: liliang
 Author-email: liang.li@dfrobot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `baidufanyiformind-0.0.1/baidufanyiformind/__init__.py` & `baidufanyiformind-0.0.2/baidufanyiformind/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #-*- coding: utf-8 -*-
 
+name = "baidufanyiformind"
+
+__all__ = ['_errcodeswitch','setAccount','baiduFanyi']
+
+__version__ = '0.0.2'
+
 import requests
 import hashlib
 import random
 
-name = "baidufanyiformind"
-
-__all__ = ['_errcodeswitch','setAccount','baiduFanyi']
 
-__version__ = '0.0.1'
 
 _baidufanyi_appid=''
 _baidufanyi_sec=''
 
 def _errcodeswitch(code=0):
     if code == '52000':
         return '成功'
```

### Comparing `baidufanyiformind-0.0.1/baidufanyiformind.egg-info/PKG-INFO` & `baidufanyiformind-0.0.2/baidufanyiformind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidufanyiformind
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for baidufanyi
 Home-page: https://gitee.com/liliang9693/baidufanyiformind
 Author: liliang
 Author-email: liang.li@dfrobot.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `baidufanyiformind-0.0.1/setup.py` & `baidufanyiformind-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="baidufanyiformind",
-    version="0.0.1",
+    version="0.0.2",
     author="liliang",
     author_email="liang.li@dfrobot.com",
     description="A package for baidufanyi",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/liliang9693/baidufanyiformind",
     packages=setuptools.find_packages(),
-    install_requires=['hashlib'],
+    install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.4',
 )
```

