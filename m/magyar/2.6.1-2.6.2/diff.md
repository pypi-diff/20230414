# Comparing `tmp/magyar-2.6.1.tar.gz` & `tmp/magyar-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.6.1.tar", last modified: Thu Apr 13 20:01:22 2023, max compression
+gzip compressed data, was "magyar-2.6.2.tar", last modified: Fri Apr 14 15:16:18 2023, max compression
```

## Comparing `magyar-2.6.1.tar` & `magyar-2.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 20:01:22.172490 magyar-2.6.1/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-13 20:01:22.172490 magyar-2.6.1/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 19:21:03.000000 magyar-2.6.1/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-13 20:01:22.172490 magyar-2.6.1/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-13 20:01:22.000000 magyar-2.6.1/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      138 2023-04-13 20:01:22.000000 magyar-2.6.1/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 20:01:22.000000 magyar-2.6.1/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-13 20:01:22.000000 magyar-2.6.1/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-13 20:01:22.172490 magyar-2.6.1/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      972 2023-04-13 20:01:11.000000 magyar-2.6.1/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 15:16:18.249393 magyar-2.6.2/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-14 15:16:18.249393 magyar-2.6.2/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 19:21:03.000000 magyar-2.6.2/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 15:16:18.249393 magyar-2.6.2/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-14 15:16:18.000000 magyar-2.6.2/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      138 2023-04-14 15:16:18.000000 magyar-2.6.2/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 15:16:18.000000 magyar-2.6.2/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 15:16:18.000000 magyar-2.6.2/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-14 15:16:18.249393 magyar-2.6.2/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      972 2023-04-14 15:12:58.000000 magyar-2.6.2/setup.py
```

### Comparing `magyar-2.6.1/PKG-INFO` & `magyar-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.6.1
+Version: 2.6.2
 Summary: Magyar nevek listája
 Home-page: https://github.com/kobanya
 Author: Nagy Béla
 Author-email: nagy.bela.budapest@gmail.com
 License: MIT
 Keywords: magyar nevek
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `magyar-2.6.1/README.md` & `magyar-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `magyar-2.6.1/magyar.egg-info/PKG-INFO` & `magyar-2.6.2/magyar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.6.1
+Version: 2.6.2
 Summary: Magyar nevek listája
 Home-page: https://github.com/kobanya
 Author: Nagy Béla
 Author-email: nagy.bela.budapest@gmail.com
 License: MIT
 Keywords: magyar nevek
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `magyar-2.6.1/setup.py` & `magyar-2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='magyar',
-    version='2.6.1',
+    version='2.6.2',
     description='Magyar nevek listája',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kobanya',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

