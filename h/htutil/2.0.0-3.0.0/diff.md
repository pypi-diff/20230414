# Comparing `tmp/htutil-2.0.0.tar.gz` & `tmp/htutil-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/htutil/htutil/dist/.tmp-v36eypkt/htutil-2.0.0.tar", last modified: Fri Mar 17 07:41:03 2023, max compression
+gzip compressed data, was "/home/runner/work/htutil/htutil/dist/.tmp-wctbzqvj/htutil-3.0.0.tar", last modified: Fri Apr 14 02:07:07 2023, max compression
```

## Comparing `htutil-2.0.0.tar` & `htutil-3.0.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-17 07:41:03.000000 htutil-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)    35129 2023-03-17 07:40:54.000000 htutil-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2817 2023-03-17 07:41:03.000000 htutil-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2401 2023-03-17 07:40:54.000000 htutil-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-17 07:41:03.000000 htutil-2.0.0/htutil/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-17 07:40:54.000000 htutil-2.0.0/htutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1044 2023-03-17 07:40:54.000000 htutil-2.0.0/htutil/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)      596 2023-03-17 07:40:54.000000 htutil-2.0.0/htutil/counter.py
--rw-r--r--   0 runner    (1001) docker     (116)     3314 2023-03-17 07:40:54.000000 htutil-2.0.0/htutil/file.py
--rw-r--r--   0 runner    (1001) docker     (116)     1718 2023-03-17 07:40:54.000000 htutil-2.0.0/htutil/log.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-17 07:41:03.000000 htutil-2.0.0/htutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2817 2023-03-17 07:41:03.000000 htutil-2.0.0/htutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      228 2023-03-17 07:41:03.000000 htutil-2.0.0/htutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-17 07:41:03.000000 htutil-2.0.0/htutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2023-03-17 07:41:03.000000 htutil-2.0.0/htutil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-17 07:41:03.000000 htutil-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      623 2023-03-17 07:40:54.000000 htutil-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:07:07.000000 htutil-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35129 2023-04-14 02:06:57.000000 htutil-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-14 02:07:07.000000 htutil-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-14 02:06:57.000000 htutil-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 02:06:57.000000 htutil-3.0.0/htutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-14 02:06:57.000000 htutil-3.0.0/htutil/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-14 02:06:57.000000 htutil-3.0.0/htutil/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-14 02:06:57.000000 htutil-3.0.0/htutil/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 02:07:07.000000 htutil-3.0.0/htutil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 02:07:07.000000 htutil-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-14 02:06:57.000000 htutil-3.0.0/setup.py
```

### Comparing `htutil-2.0.0/LICENSE` & `htutil-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htutil-2.0.0/README.md` & `htutil-3.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: htutil
+Version: 3.0.0
+Summary: HaoTian's Python Util
+Home-page: https://github.com/117503445/htutil
+Author: 117503445
+Author-email: t117503445@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # htutil
 
 HaoTian's Python Util
 
 ![version](https://img.shields.io/pypi/v/htutil)
 ![downloads](https://img.shields.io/pypi/dm/htutil)
 ![format](https://img.shields.io/pypi/format/htutil)
@@ -39,74 +52,14 @@
     # hello\nworld in 1.txt
     append_lines('1.txt',['\npython'])
     # hello\nworld\npython in 1.txt
     s = read_lines('1.txt')
     print(s)  # ['hello', 'world', 'python']
 ```
 
-### Log
-
-```python
-from htutil import log
-from htutil.log import p
-```
-
-A powerful logger, support var name output.
-
-```python
-a = 3
-p(a)
-p(a-1)
-
-b = bob()
-p(b.a)
-```
-
-The output is
-
-```txt
-a = 3;2020-12-19 16:43:49;/Users/t117503445/Project/htutil/htutil/log.py:55
-a-1 = 2;2020-12-19 16:43:49;/Users/t117503445/Project/htutil/htutil/log.py:56
-b.a = 3;2020-12-19 16:43:49;/Users/t117503445/Project/htutil/htutil/log.py:58
-```
-
-You could change the output format.
-
-```python
-config(format = '${var_name} = ${value} ### ${time} ### ${file_name}:${line_number}')
-p(a)
-```
-
-then the output is
-
-```txt
-a = 3 ### 2020-12-19 16:46:56 ### /Users/t117503445/Project/htutil/htutil/log.py:60
-```
-
-The default format is ${var_name} = ${value};${time};${file_name}:${line_number}
-
-If you want to save the log output to file, you could use callback.
-
-```python
-def callback_example(string: str):
-    file.append_text('1.log',string)
-
-register_p_callback(callback_example)
-a = 3
-p(a)
-```
-
-lambda is also a good choice.
-
-```python
-register_p_callback(lambda string:file.append_text('1.log',string))
-a = 3
-p(a)
-```
-
 ### cache
 
 cache def result by pickle file.
 
 ```python
 from htutil import cache
 @cache.file_cache
```

### Comparing `htutil-2.0.0/htutil/cache.py` & `htutil-3.0.0/htutil/cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-'''
-Author: HaoTian Qi
-Date: 2021-02-18 13:40:42
-Description: function result cache
-LastEditTime: 2021-02-18 13:58:34
-LastEditors: HaoTian Qi
-FilePath: \htutil\htutil\cache.py
-'''
 import time
 import pickle as pkl
 from pathlib import Path
 import inspect
 
 
 def file_cache(function):
```

### Comparing `htutil-2.0.0/htutil/file.py` & `htutil-3.0.0/htutil/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-'''
-Author: HaoTian Qi
-Date: 2020-12-19 15:12:53
-Description: file IO warpper
-LastEditTime: 2022-10-15 10:06:36
-LastEditors: HaoTian Qi
-FilePath: \htutil\htutil\file.py
-'''
-
 import os
 import pickle as pkl
 import json
 
 
 def read_text(path: str) -> str:
     with open(path, 'r', encoding='utf-8', errors='ignore') as f:
```

### Comparing `htutil-2.0.0/setup.py` & `htutil-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="htutil",
-    version="2.0.0",
+    version="3.0.0",
     author="117503445",
     author_email="t117503445@gmail.com",
     description="HaoTian's Python Util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/117503445/htutil",
     packages=setuptools.find_packages(),
```

