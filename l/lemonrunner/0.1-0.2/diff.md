# Comparing `tmp/lemonrunner-0.1.linux-x86_64.tar.gz` & `tmp/lemonrunner-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemonrunner-0.1.linux-x86_64.tar", last modified: Fri Apr 14 16:12:19 2023, max compression
+gzip compressed data, was "lemonrunner-0.2.tar", last modified: Fri Apr 14 16:14:41 2023, max compression
```

## Comparing `lemonrunner-0.1.linux-x86_64.tar` & `lemonrunner-0.2.tar`

### file list

```diff
@@ -1,23 +1,17 @@
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.397640 ./
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.397640 ./usr/
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.397640 ./usr/local/
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.397640 ./usr/local/lib/
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.397640 ./usr/local/lib/python3.10/
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/lemonrunner/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)       48 2023-04-14 16:05:34.000000 ./usr/local/lib/python3.10/dist-packages/lemonrunner/__init__.py
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/lemonrunner/__pycache__/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      215 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/lemonrunner/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     3930 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/lemonrunner/__pycache__/lemonrunner.cpython-310.pyc
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     3606 2023-04-14 16:05:54.000000 ./usr/local/lib/python3.10/dist-packages/lemonrunner/lemonrunner.py
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/lemonrunner-0.1.egg-info/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     1367 2023-04-14 16:12:19.361640 ./usr/local/lib/python3.10/dist-packages/lemonrunner-0.1.egg-info/PKG-INFO
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      260 2023-04-14 16:12:19.361640 ./usr/local/lib/python3.10/dist-packages/lemonrunner-0.1.egg-info/SOURCES.txt
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)        1 2023-04-14 16:12:19.361640 ./usr/local/lib/python3.10/dist-packages/lemonrunner-0.1.egg-info/dependency_links.txt
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)       18 2023-04-14 16:12:19.361640 ./usr/local/lib/python3.10/dist-packages/lemonrunner-0.1.egg-info/top_level.txt
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/tests/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 11:43:06.000000 ./usr/local/lib/python3.10/dist-packages/tests/__init__.py
-drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/tests/__pycache__/
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      150 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/tests/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      941 2023-04-14 16:12:19.401640 ./usr/local/lib/python3.10/dist-packages/tests/__pycache__/test_definitely.cpython-310.pyc
--rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      542 2023-04-14 16:06:28.000000 ./usr/local/lib/python3.10/dist-packages/tests/test_definitely.py
+drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:14:41.494033 lemonrunner-0.2/
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     1071 2023-04-14 15:50:11.000000 lemonrunner-0.2/LICENSE
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     1365 2023-04-14 16:14:41.494033 lemonrunner-0.2/PKG-INFO
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      975 2023-04-14 16:14:04.000000 lemonrunner-0.2/README.md
+drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:14:41.494033 lemonrunner-0.2/lemonrunner/
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)       48 2023-04-14 16:05:34.000000 lemonrunner-0.2/lemonrunner/__init__.py
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     3606 2023-04-14 16:05:54.000000 lemonrunner-0.2/lemonrunner/lemonrunner.py
+drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:14:41.494033 lemonrunner-0.2/lemonrunner.egg-info/
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)     1365 2023-04-14 16:14:41.000000 lemonrunner-0.2/lemonrunner.egg-info/PKG-INFO
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      260 2023-04-14 16:14:41.000000 lemonrunner-0.2/lemonrunner.egg-info/SOURCES.txt
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)        1 2023-04-14 16:14:41.000000 lemonrunner-0.2/lemonrunner.egg-info/dependency_links.txt
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)       18 2023-04-14 16:14:41.000000 lemonrunner-0.2/lemonrunner.egg-info/top_level.txt
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)       38 2023-04-14 16:14:41.494033 lemonrunner-0.2/setup.cfg
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      705 2023-04-14 16:13:45.000000 lemonrunner-0.2/setup.py
+drwxrwxr-x   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 16:14:41.494033 lemonrunner-0.2/tests/
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)        0 2023-04-14 11:43:06.000000 lemonrunner-0.2/tests/__init__.py
+-rw-rw-r--   0 sveinrou  (1000) sveinrou  (1000)      542 2023-04-14 16:06:28.000000 lemonrunner-0.2/tests/test_definitely.py
```

### Comparing `./usr/local/lib/python3.10/dist-packages/lemonrunner/lemonrunner.py` & `lemonrunner-0.2/lemonrunner/lemonrunner.py`

 * *Files identical despite different names*

### Comparing `./usr/local/lib/python3.10/dist-packages/lemonrunner-0.1.egg-info/PKG-INFO` & `lemonrunner-0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonrunner
-Version: 0.1
+Version: 0.2
 Summary: UNKNOWN
 Home-page: https://github.com/sveinrou/definitively
 Author: sveinrou
 Author-email: sveinrou@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -13,21 +13,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lemonrunner
 
 Run this forever and stream the results.
 
-The entry point is the Definitively-class, which exposes the run-method. Run
+The entry point is the Lemonrunner-class, which exposes the run-method. Run
 takes an id, a function, and optional key-word arguments for args, kwargs,
 timeout, times and interval.
 
 Any function passed to run will be run either forever, or N times, if the times arument is given. Returns, yielded values or exceptions are all retrieved from the monitor-method.
 
-The monitor function of the Definitively-class is a generator which yields each message from each function as they come in.
+The monitor function of the Lemonrunner-class is a generator which yields each message from each function as they come in.
 
 ## Example
 
 ```python3
 from time import sleep
 
 from lemonrunner import Lemonrunner
```

### Comparing `./usr/local/lib/python3.10/dist-packages/tests/test_definitely.py` & `lemonrunner-0.2/tests/test_definitely.py`

 * *Files identical despite different names*

