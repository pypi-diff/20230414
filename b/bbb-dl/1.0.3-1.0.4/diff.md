# Comparing `tmp/bbb-dl-1.0.3.tar.gz` & `tmp/bbb-dl-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbb-dl-1.0.3.tar", last modified: Thu Apr 13 20:16:43 2023, max compression
+gzip compressed data, was "bbb-dl-1.0.4.tar", last modified: Fri Apr 14 08:50:51 2023, max compression
```

## Comparing `bbb-dl-1.0.3.tar` & `bbb-dl-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:16:43.527043 bbb-dl-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-13 20:16:43.527043 bbb-dl-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:16:43.523043 bbb-dl-1.0.3/bbb_dl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/browser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/ffmpeg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58606 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    22273 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/bbb_dl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:16:43.527043 bbb-dl-1.0.3/bbb_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 20:16:43.000000 bbb-dl-1.0.3/bbb_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 20:16:43.527043 bbb-dl-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-13 20:16:29.000000 bbb-dl-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/bbb_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11835 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/ffmpeg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58606 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22273 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/bbb_dl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/bbb_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 08:50:51.000000 bbb-dl-1.0.4/bbb_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 08:50:51.880468 bbb-dl-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-14 08:50:42.000000 bbb-dl-1.0.4/setup.py
```

### Comparing `bbb-dl-1.0.3/LICENSE` & `bbb-dl-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.3/PKG-INFO` & `bbb-dl-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-dl
-Version: 1.0.3
+Version: 1.0.4
 Summary: Big Blue Button Downloader that downloads a BBB lesson as MP4 video
 Home-page: https://github.com/C0D3D3V/bbb-dl
 Author: C0D3D3V
 License: GPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bbb-dl-1.0.3/README.md` & `bbb-dl-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.3/bbb_dl/batch.py` & `bbb-dl-1.0.4/bbb_dl/batch.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.3/bbb_dl/browser.py` & `bbb-dl-1.0.4/bbb_dl/browser.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.3/bbb_dl/ffmpeg.py` & `bbb-dl-1.0.4/bbb_dl/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.3/bbb_dl/main.py` & `bbb-dl-1.0.4/bbb_dl/main.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.3/bbb_dl/utils.py` & `bbb-dl-1.0.4/bbb_dl/utils.py`

 * *Files identical despite different names*

### Comparing `bbb-dl-1.0.3/bbb_dl.egg-info/PKG-INFO` & `bbb-dl-1.0.4/bbb_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbb-dl
-Version: 1.0.3
+Version: 1.0.4
 Summary: Big Blue Button Downloader that downloads a BBB lesson as MP4 video
 Home-page: https://github.com/C0D3D3V/bbb-dl
 Author: C0D3D3V
 License: GPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bbb-dl-1.0.3/setup.py` & `bbb-dl-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from os import path
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 # Get the version from bbb_dl/version.py without importing the package
 exec(compile(open('bbb_dl/version.py', encoding="utf-8").read(), 'bbb_dl/version.py', 'exec'))
 
 
 def readme():
     this_directory = path.abspath(path.dirname(__file__))
@@ -29,17 +30,18 @@
             'bbb-dl-browser = bbb_dl.browser:main',
         ],
     },
     python_requires='>=3.7',
     install_requires=[
         'aiofiles>=22.1.0',
         'aiohttp>=3.8.3',
+        'colorama>=0.4.6',
         'playwright>=1.29.0',
+        'PySide6>=6.5.0',
         'python-ffmpeg>=1.0.16',
-        'colorama>=0.4.6',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Education',
```

