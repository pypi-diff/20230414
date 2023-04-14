# Comparing `tmp/pathaia-0.2.2.tar.gz` & `tmp/pathaia-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PathAIA/PathAIA/dist/.tmp-sybdqe43/pathaia-0.2.2.tar", last modified: Tue Apr 11 08:21:38 2023, max compression
+gzip compressed data, was "/home/runner/work/PathAIA/PathAIA/dist/.tmp-od1_efp2/pathaia-0.2.3.tar", last modified: Fri Apr 14 12:13:54 2023, max compression
```

## Comparing `pathaia-0.2.2.tar` & `pathaia-0.2.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-11 08:21:27.000000 pathaia-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-04-11 08:21:38.000000 pathaia-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5167 2023-04-11 08:21:27.000000 pathaia-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    21320 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/functional_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      158 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/datasets/object_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/graphs/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11849 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/clustering.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    15868 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/functional_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/kruskal.py
--rw-r--r--   0 runner    (1001) docker     (122)    17649 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/object_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/graphs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/patches/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     5683 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    28403 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/functional_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     6622 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/object_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/slide_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/patches/visu.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/semantic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/semantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/semantic/functional_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia/util/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (122)    11170 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/images.py
--rw-r--r--   0 runner    (1001) docker     (122)    12227 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/management.py
--rw-r--r--   0 runner    (1001) docker     (122)     6166 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-04-11 08:21:27.000000 pathaia-0.2.2/pathaia/util/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 08:21:37.000000 pathaia-0.2.2/pathaia.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-11 08:21:38.000000 pathaia-0.2.2/pathaia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 08:21:38.000000 pathaia-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-04-11 08:21:27.000000 pathaia-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:38.000000 pathaia-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-11 08:21:27.000000 pathaia-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18276 2023-04-11 08:21:27.000000 pathaia-0.2.2/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-04-11 08:21:27.000000 pathaia-0.2.2/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-14 12:13:42.000000 pathaia-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-04-14 12:13:54.000000 pathaia-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5167 2023-04-14 12:13:42.000000 pathaia-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3752 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/datasets/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1259 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/datasets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21320 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/datasets/functional_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      158 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/datasets/object_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia/graphs/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11849 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/graphs/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/graphs/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15868 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/graphs/functional_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3236 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/graphs/kruskal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17649 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/graphs/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/graphs/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      397 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/patches/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/patches/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5683 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/patches/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28403 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/patches/functional_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6622 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/patches/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4216 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/patches/slide_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/patches/visu.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia/semantic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/semantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5059 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/semantic/functional_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia/util/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11170 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/util/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/util/images.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12227 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/util/management.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6166 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/util/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7336 2023-04-14 12:13:42.000000 pathaia-0.2.3/pathaia/util/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-14 12:13:54.000000 pathaia-0.2.3/pathaia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-14 12:13:54.000000 pathaia-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-04-14 12:13:42.000000 pathaia-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:54.000000 pathaia-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 12:13:42.000000 pathaia-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18276 2023-04-14 12:13:42.000000 pathaia-0.2.3/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-04-14 12:13:42.000000 pathaia-0.2.3/tests/helpers.py
```

### Comparing `pathaia-0.2.2/LICENSE` & `pathaia-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/PKG-INFO` & `pathaia-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathaia
-Version: 0.2.2
+Version: 0.2.3
 Summary: procedures for wsi analysis
 Author: Arnaud Abreu
 Author-email: arnaud.abreu.p@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pathaia Version: 0.2.2 Summary: procedures for wsi
+Metadata-Version: 2.1 Name: pathaia Version: 0.2.3 Summary: procedures for wsi
 analysis Author: Arnaud Abreu Author-email: arnaud.abreu.p@gmail.com
 Description-Content-Type: text/markdown License-File: LICENSE
           # PathAIA **Simple digital pathology analysis tools.** ---
      Basic_Usage â¢ Advanced_features â¢ Docs â¢ Community â¢ License
    [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pathaia)]
  (https://pypi.org/project/pathaia/) [![PyPI Status](https://badge.fury.io/py/
    pathaia.svg)](https://badge.fury.io/py/pathaia) [![PyPI Status](https://
```

### Comparing `pathaia-0.2.2/README.md` & `pathaia-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/datasets/data.py` & `pathaia-0.2.3/pathaia/datasets/data.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/datasets/errors.py` & `pathaia-0.2.3/pathaia/datasets/errors.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/datasets/functional_api.py` & `pathaia-0.2.3/pathaia/datasets/functional_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/graphs/clustering.py` & `pathaia-0.2.3/pathaia/graphs/clustering.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/graphs/errors.py` & `pathaia-0.2.3/pathaia/graphs/errors.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/graphs/functional_api.py` & `pathaia-0.2.3/pathaia/graphs/functional_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/graphs/kruskal.py` & `pathaia-0.2.3/pathaia/graphs/kruskal.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/graphs/object_api.py` & `pathaia-0.2.3/pathaia/graphs/object_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/graphs/types.py` & `pathaia-0.2.3/pathaia/graphs/types.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/patches/errors.py` & `pathaia-0.2.3/pathaia/patches/errors.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/patches/filters.py` & `pathaia-0.2.3/pathaia/patches/filters.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/patches/functional_api.py` & `pathaia-0.2.3/pathaia/patches/functional_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/patches/object_api.py` & `pathaia-0.2.3/pathaia/patches/object_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/patches/slide_filters.py` & `pathaia-0.2.3/pathaia/patches/slide_filters.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/patches/visu.py` & `pathaia-0.2.3/pathaia/patches/visu.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/semantic/functional_api.py` & `pathaia-0.2.3/pathaia/semantic/functional_api.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/util/convert.py` & `pathaia-0.2.3/pathaia/util/convert.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/util/images.py` & `pathaia-0.2.3/pathaia/util/images.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/util/management.py` & `pathaia-0.2.3/pathaia/util/management.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/util/paths.py` & `pathaia-0.2.3/pathaia/util/paths.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia/util/types.py` & `pathaia-0.2.3/pathaia/util/types.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/pathaia.egg-info/PKG-INFO` & `pathaia-0.2.3/pathaia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathaia
-Version: 0.2.2
+Version: 0.2.3
 Summary: procedures for wsi analysis
 Author: Arnaud Abreu
 Author-email: arnaud.abreu.p@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pathaia Version: 0.2.2 Summary: procedures for wsi
+Metadata-Version: 2.1 Name: pathaia Version: 0.2.3 Summary: procedures for wsi
 analysis Author: Arnaud Abreu Author-email: arnaud.abreu.p@gmail.com
 Description-Content-Type: text/markdown License-File: LICENSE
           # PathAIA **Simple digital pathology analysis tools.** ---
      Basic_Usage â¢ Advanced_features â¢ Docs â¢ Community â¢ License
    [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pathaia)]
  (https://pypi.org/project/pathaia/) [![PyPI Status](https://badge.fury.io/py/
    pathaia.svg)](https://badge.fury.io/py/pathaia) [![PyPI Status](https://
```

### Comparing `pathaia-0.2.2/pathaia.egg-info/SOURCES.txt` & `pathaia-0.2.3/pathaia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/setup.py` & `pathaia-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="pathaia",
-    version="0.2.2",
+    version="0.2.3",
     description="procedures for wsi analysis",
     author="Arnaud Abreu",
     author_email="arnaud.abreu.p@gmail.com",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
         "fastcore>=1,<2",
         "numpy>=1,<2",
         "tqdm>=4,<5",
-        "openslide-python>=3,<4",
+        "openslide-python>=1.1,<1.2",
         "opencv-python>=4,<5",
         "scikit-image>=0.19,<1",
         "matplotlib>=3,<4",
         "nptyping>=2,<3",
         "pandas>=1,<2",
         "dataclasses",
         "sortedcontainers>=2,<3",
```

### Comparing `pathaia-0.2.2/tests/data.py` & `pathaia-0.2.3/tests/data.py`

 * *Files identical despite different names*

### Comparing `pathaia-0.2.2/tests/helpers.py` & `pathaia-0.2.3/tests/helpers.py`

 * *Files identical despite different names*

