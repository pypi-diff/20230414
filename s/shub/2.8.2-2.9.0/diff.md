# Comparing `tmp/shub-2.8.2.tar.gz` & `tmp/shub-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shub-2.8.2.tar", last modified: Fri Jan 18 07:48:01 2019, max compression
+gzip compressed data, was "dist/shub-2.9.0.tar", last modified: Thu May 16 01:35:40 2019, max compression
```

## Comparing `shub-2.8.2.tar` & `shub-2.9.0.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 07:48:01.000000 shub-2.8.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      777 2019-01-18 07:46:25.000000 shub-2.8.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1648 2019-01-18 07:46:25.000000 shub-2.8.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 07:48:01.000000 shub-2.8.2/shub.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2019-01-18 07:48:01.000000 shub-2.8.2/shub.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-01-18 07:46:30.000000 shub-2.8.2/shub.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-01-18 07:48:01.000000 shub-2.8.2/shub.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2019-01-18 07:48:01.000000 shub-2.8.2/shub.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-01-18 07:48:01.000000 shub-2.8.2/shub.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2019-01-18 07:48:01.000000 shub-2.8.2/shub.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      772 2019-01-18 07:48:01.000000 shub-2.8.2/shub.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2019-01-18 07:48:01.000000 shub-2.8.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2019-01-18 07:48:01.000000 shub-2.8.2/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 07:48:01.000000 shub-2.8.2/shub/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2019-01-18 07:46:25.000000 shub-2.8.2/shub/bootstrap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1631 2019-01-18 07:46:25.000000 shub-2.8.2/shub/fetch_eggs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2019-01-18 07:46:25.000000 shub-2.8.2/shub/tool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2262 2019-01-18 07:46:25.000000 shub-2.8.2/shub/deploy_reqs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1493 2019-01-18 07:46:25.000000 shub-2.8.2/shub/log.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2877 2019-01-18 07:46:25.000000 shub-2.8.2/shub/migrate_eggs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3815 2019-01-18 07:46:25.000000 shub-2.8.2/shub/schedule.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3204 2019-01-18 07:46:25.000000 shub-2.8.2/shub/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      680 2019-01-18 07:46:25.000000 shub-2.8.2/shub/logout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2006 2019-01-18 07:46:25.000000 shub-2.8.2/shub/login.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      280 2019-01-18 07:46:25.000000 shub-2.8.2/shub/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      257 2019-01-18 07:46:25.000000 shub-2.8.2/shub/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2935 2019-01-18 07:46:25.000000 shub-2.8.2/shub/copy_eggs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21246 2019-01-18 07:46:25.000000 shub-2.8.2/shub/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2019-01-18 07:46:25.000000 shub-2.8.2/shub/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1346 2019-01-18 07:46:25.000000 shub-2.8.2/shub/requests.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-18 07:48:01.000000 shub-2.8.2/shub/image/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7058 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/push.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4894 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/build.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2559 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/upload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      417 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9218 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/deploy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6534 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/init.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9549 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      671 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/check.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6526 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5401 2019-01-18 07:46:25.000000 shub-2.8.2/shub/image/test.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7006 2019-01-18 07:46:25.000000 shub-2.8.2/shub/deploy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2019-01-18 07:46:25.000000 shub-2.8.2/shub/items.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28872 2019-01-18 07:46:25.000000 shub-2.8.2/shub/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1625 2019-01-18 07:46:25.000000 shub-2.8.2/shub/compat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4164 2019-01-18 07:46:25.000000 shub-2.8.2/shub/deploy_egg.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-16 01:35:40.000000 shub-2.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      777 2019-05-16 01:33:58.000000 shub-2.9.0/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1664 2019-05-16 01:33:58.000000 shub-2.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-16 01:35:40.000000 shub-2.9.0/shub.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2019-05-16 01:35:40.000000 shub-2.9.0/shub.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-16 01:34:04.000000 shub-2.9.0/shub.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       85 2019-05-16 01:35:40.000000 shub-2.9.0/shub.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2019-05-16 01:35:40.000000 shub-2.9.0/shub.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-16 01:35:40.000000 shub-2.9.0/shub.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2019-05-16 01:35:40.000000 shub-2.9.0/shub.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      825 2019-05-16 01:35:40.000000 shub-2.9.0/shub.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      132 2019-05-16 01:35:40.000000 shub-2.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1951 2019-05-16 01:35:40.000000 shub-2.9.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-16 01:35:40.000000 shub-2.9.0/shub/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2019-05-16 01:33:58.000000 shub-2.9.0/shub/bootstrap.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1631 2019-05-16 01:33:58.000000 shub-2.9.0/shub/fetch_eggs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2019-05-16 01:33:58.000000 shub-2.9.0/shub/tool.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2262 2019-05-16 01:33:58.000000 shub-2.9.0/shub/deploy_reqs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1493 2019-05-16 01:33:58.000000 shub-2.9.0/shub/log.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2877 2019-05-16 01:33:58.000000 shub-2.9.0/shub/migrate_eggs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3815 2019-05-16 01:33:58.000000 shub-2.9.0/shub/schedule.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3204 2019-05-16 01:33:58.000000 shub-2.9.0/shub/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      680 2019-05-16 01:33:58.000000 shub-2.9.0/shub/logout.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2006 2019-05-16 01:33:58.000000 shub-2.9.0/shub/login.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      280 2019-05-16 01:33:58.000000 shub-2.9.0/shub/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      257 2019-05-16 01:33:58.000000 shub-2.9.0/shub/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2935 2019-05-16 01:33:58.000000 shub-2.9.0/shub/copy_eggs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21246 2019-05-16 01:33:58.000000 shub-2.9.0/shub/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      151 2019-05-16 01:33:58.000000 shub-2.9.0/shub/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1346 2019-05-16 01:33:58.000000 shub-2.9.0/shub/requests.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-16 01:35:40.000000 shub-2.9.0/shub/image/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7058 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/push.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-16 01:35:40.000000 shub-2.9.0/shub/image/run/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2576 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/run/wrapper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5281 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/run/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4894 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/build.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2559 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/upload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9218 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/deploy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6534 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/init.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9818 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      671 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/check.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6526 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5401 2019-05-16 01:33:58.000000 shub-2.9.0/shub/image/test.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8334 2019-05-16 01:33:58.000000 shub-2.9.0/shub/deploy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2019-05-16 01:33:58.000000 shub-2.9.0/shub/items.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28976 2019-05-16 01:33:58.000000 shub-2.9.0/shub/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1625 2019-05-16 01:33:58.000000 shub-2.9.0/shub/compat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4164 2019-05-16 01:33:58.000000 shub-2.9.0/shub/deploy_egg.py
```

### Comparing `shub-2.8.2/README.rst` & `shub-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/setup.py` & `shub-2.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 with io.open(os.path.join(here, 'shub', '__init__.py'),
              mode='r', encoding='utf-8') as f:
     exec(f.read(), about)
 
 
 setup(
     name='shub',
-    version='2.8.2',
+    version='2.9.0',
     packages=find_packages(exclude=('tests', 'tests.*')),
     url=about['DOCS_LINK'],
     description='Scrapinghub Command Line Client',
     long_description=open('README.rst').read(),
     author='Scrapinghub',
     author_email='info@scrapinghub.com',
     maintainer='Scrapinghub',
@@ -34,14 +34,15 @@
         'pip',
         'PyYAML',
         'retrying',
         'requests',
         'scrapinghub>=2.0.3',
         'six>=1.7.0',
         'tqdm',
+        'toml',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
```

### Comparing `shub-2.8.2/shub.egg-info/PKG-INFO` & `shub-2.9.0/shub.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: shub
-Version: 2.8.2
+Version: 2.9.0
 Summary: Scrapinghub Command Line Client
 Home-page: https://shub.readthedocs.io/en/stable/
 Author: Scrapinghub
 Author-email: info@scrapinghub.com
 Maintainer: Scrapinghub
 Maintainer-email: info@scrapinghub.com
 License: BSD
```

### Comparing `shub-2.8.2/shub.egg-info/SOURCES.txt` & `shub-2.9.0/shub.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -34,8 +34,10 @@
 shub/image/check.py
 shub/image/deploy.py
 shub/image/init.py
 shub/image/list.py
 shub/image/push.py
 shub/image/test.py
 shub/image/upload.py
-shub/image/utils.py
+shub/image/utils.py
+shub/image/run/__init__.py
+shub/image/run/wrapper.py
```

### Comparing `shub-2.8.2/PKG-INFO` & `shub-2.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: shub
-Version: 2.8.2
+Version: 2.9.0
 Summary: Scrapinghub Command Line Client
 Home-page: https://shub.readthedocs.io/en/stable/
 Author: Scrapinghub
 Author-email: info@scrapinghub.com
 Maintainer: Scrapinghub
 Maintainer-email: info@scrapinghub.com
 License: BSD
```

### Comparing `shub-2.8.2/shub/bootstrap.py` & `shub-2.9.0/shub/bootstrap.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/fetch_eggs.py` & `shub-2.9.0/shub/fetch_eggs.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/tool.py` & `shub-2.9.0/shub/tool.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/deploy_reqs.py` & `shub-2.9.0/shub/deploy_reqs.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/log.py` & `shub-2.9.0/shub/log.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/migrate_eggs.py` & `shub-2.9.0/shub/migrate_eggs.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/schedule.py` & `shub-2.9.0/shub/schedule.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/exceptions.py` & `shub-2.9.0/shub/exceptions.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/logout.py` & `shub-2.9.0/shub/logout.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/login.py` & `shub-2.9.0/shub/login.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/copy_eggs.py` & `shub-2.9.0/shub/copy_eggs.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/config.py` & `shub-2.9.0/shub/config.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/requests.py` & `shub-2.9.0/shub/requests.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/image/push.py` & `shub-2.9.0/shub/image/push.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/image/build.py` & `shub-2.9.0/shub/image/build.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/image/upload.py` & `shub-2.9.0/shub/image/upload.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/image/deploy.py` & `shub-2.9.0/shub/image/deploy.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/image/init.py` & `shub-2.9.0/shub/image/init.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/image/utils.py` & `shub-2.9.0/shub/image/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import os
 import re
 import sys
+import shutil
+import tempfile
+import contextlib
 
 import click
 import yaml
 from tqdm import tqdm
 from six import binary_type
 
 from shub import config as shub_config
@@ -284,7 +287,17 @@
         file=sys.stdout,
         # helps to update bars on resizing terminal
         dynamic_ncols=True,
         # miniters improves progress on erratic updates caused by network
         miniters=1,
         **kwargs
     )
+
+
+@contextlib.contextmanager
+def make_temp_directory(cleanup=True, **kwargs):
+    temp_dir = tempfile.mkdtemp(**kwargs)
+    try:
+        yield temp_dir
+    finally:
+        if cleanup:
+            shutil.rmtree(temp_dir)
```

### Comparing `shub-2.8.2/shub/image/check.py` & `shub-2.9.0/shub/image/check.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/image/list.py` & `shub-2.9.0/shub/image/list.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/image/test.py` & `shub-2.9.0/shub/image/test.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/deploy.py` & `shub-2.9.0/shub/deploy.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import glob
 import shutil
 import tempfile
 import json
 from six.moves.urllib.parse import urljoin
 
 import click
+import toml
 # Not used in code but needed in runtime, don't remove!
 import setuptools
 _1 = setuptools  # NOQA
 try:
     # Only available in setuptools >= 24.0.0
     import setuptools.msvc
 except ImportError:
@@ -146,16 +147,20 @@
     if stack:
         data['stack'] = stack
 
     try:
         files = [('eggs', open(path, 'rb')) for path in expanded_eggs]
         if _is_pipfile(requirements_file):
             requirements_file = _get_pipfile_requirements()
+        elif _is_poetry(requirements_file):
+            requirements_file = _get_poetry_requirements()
+        elif requirements_file:
+            requirements_file = open(requirements_file, 'rb')
         if requirements_file:
-            files.append(('requirements', open(requirements_file, 'rb')))
+            files.append(('requirements', requirements_file))
     except IOError as e:
         raise ShubException("%s %s" % (e.strerror, e.filename))
     files.append(('egg', open(eggpath, 'rb')))
     url = _url(endpoint, 'scrapyd/addversion.json')
     click.echo('Deploying to Scrapy Cloud project "%s"' % project)
     return make_deploy_request(url, data, files, auth, verbose, keep_log)
 
@@ -180,15 +185,51 @@
         if 'hash' in v:
             del v['hash']
         if 'hashes' in v:
             del v['hashes']
         # Scrapy Cloud also doesn't support editable packages
         if 'editable' in v:
             del v['editable']
-    return convert_deps_to_pip(deps)
+    return open(convert_deps_to_pip(deps), 'rb')
+
+
+def _is_poetry(name):
+    if name != 'pyproject.toml':
+        return False
+    data = toml.load(name)
+    return 'poetry' in (data.get('tool') or {})
+
+
+def _get_poetry_requirements():
+    try:
+        data = toml.load('poetry.lock')
+    except IOError:
+        raise ShubException('Please make sure the poetry lock file is present')
+    # Adapted from poetry 1.0.0a2 poetry/utils/exporter.py
+    lines = []
+    for package in data['package']:
+        source = package.get('source') or {}
+        source_type = source.get('type')
+        if source_type == 'git':
+            line = 'git+{}@{}#egg={}'.format(
+                source['url'], source['reference'], package['name']
+            )
+        elif source_type in ['directory', 'file']:
+            line = ''
+            line += source['url']
+        else:
+            line = '{}=={}'.format(package['name'], package['version'])
+
+            if source_type == 'legacy' and source['url']:
+                line += ' \\\n'
+                line += '    --index-url {}'.format(source['url'])
+
+        line += '\n'
+        lines.append(line)
+    return ''.join(lines)
 
 
 def _build_egg():
     if not inside_project():
         raise NotFoundException("No Scrapy project found in this location.")
     create_default_setup_py()
     d = tempfile.mkdtemp(prefix="shub-deploy-")
```

### Comparing `shub-2.8.2/shub/items.py` & `shub-2.9.0/shub/items.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/utils.py` & `shub-2.9.0/shub/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from six.moves.configparser import SafeConfigParser
 from distutils.spawn import find_executable
 from distutils.version import LooseVersion, StrictVersion
 from glob import glob
 from importlib import import_module
 from tempfile import NamedTemporaryFile, TemporaryFile
 from six.moves.urllib.parse import urljoin
+from six import string_types
 
 import click
 import pip
 import requests
 import yaml
 
 # https://github.com/scrapinghub/shub/pull/309#pullrequestreview-113977920
@@ -111,15 +112,19 @@
 
 
 def _check_deploy_files_size(files):
     """Ensure that request's files total size is less than current limit."""
     ctx = click.get_current_context(silent=True)
     if not isinstance(files, list) or ctx and ctx.params.get('ignore-size'):
         return
-    files_size = sum(os.fstat(fp.fileno()).st_size for (fname, fp) in files)
+    files_size = sum(
+        len(fp) if isinstance(fp, string_types)
+        else os.fstat(fp.fileno()).st_size
+        for (fname, fp) in files
+    )
     if files_size > REQUEST_FILES_SIZE_LIMIT:
         raise DeployRequestTooLargeException
 
 
 def write_and_echo_logs(keep_log, last_logs, rsp, verbose):
     """It will write logs to temporal file and echo if verbose is True."""
     with NamedTemporaryFile(prefix='shub_deploy_', suffix='.log',
```

### Comparing `shub-2.8.2/shub/compat.py` & `shub-2.9.0/shub/compat.py`

 * *Files identical despite different names*

### Comparing `shub-2.8.2/shub/deploy_egg.py` & `shub-2.9.0/shub/deploy_egg.py`

 * *Files identical despite different names*

