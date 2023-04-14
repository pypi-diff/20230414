# Comparing `tmp/butterneck-projen-0.0.6.tar.gz` & `tmp/butterneck-projen-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butterneck-projen-0.0.6.tar", last modified: Fri Apr 14 20:03:32 2023, max compression
+gzip compressed data, was "butterneck-projen-0.0.7.tar", last modified: Fri Apr 14 20:33:14 2023, max compression
```

## Comparing `butterneck-projen-0.0.6.tar` & `butterneck-projen-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/src/butterneck_projen/
--rw-r--r--   0 runner    (1001) docker     (123)   113875 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/src/butterneck_projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/src/butterneck_projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/src/butterneck_projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24227 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/src/butterneck_projen/_jsii/butterneck-projen@0.0.6.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:03:21.000000 butterneck-projen-0.0.6/src/butterneck_projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:03:32.767848 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 20:03:32.000000 butterneck-projen-0.0.6/src/butterneck_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.746700 butterneck-projen-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 20:33:14.746700 butterneck-projen-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:33:14.746700 butterneck-projen-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.742700 butterneck-projen-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.742700 butterneck-projen-0.0.7/src/butterneck_projen/
+-rw-r--r--   0 runner    (1001) docker     (123)   113875 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/src/butterneck_projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.742700 butterneck-projen-0.0.7/src/butterneck_projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/src/butterneck_projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24872 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/src/butterneck_projen/_jsii/butterneck-projen@0.0.7.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:33:02.000000 butterneck-projen-0.0.7/src/butterneck_projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:33:14.742700 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 20:33:14.000000 butterneck-projen-0.0.7/src/butterneck_projen.egg-info/top_level.txt
```

### Comparing `butterneck-projen-0.0.6/LICENSE` & `butterneck-projen-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `butterneck-projen-0.0.6/PKG-INFO` & `butterneck-projen-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterneck-projen
-Version: 0.0.6
+Version: 0.0.7
 Summary: butterneck-projen
 Home-page: https://github.com/butterneck/butterneck-projen.git
 Author: Filippo Pinton<pinton.filippo@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/butterneck/butterneck-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `butterneck-projen-0.0.6/setup.py` & `butterneck-projen-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "butterneck-projen",
-    "version": "0.0.6",
+    "version": "0.0.7",
     "description": "butterneck-projen",
     "license": "Apache-2.0",
     "url": "https://github.com/butterneck/butterneck-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "Filippo Pinton<pinton.filippo@protonmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "butterneck_projen",
         "butterneck_projen._jsii"
     ],
     "package_data": {
         "butterneck_projen._jsii": [
-            "butterneck-projen@0.0.6.jsii.tgz"
+            "butterneck-projen@0.0.7.jsii.tgz"
         ],
         "butterneck_projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `butterneck-projen-0.0.6/src/butterneck_projen/__init__.py` & `butterneck-projen-0.0.7/src/butterneck_projen/__init__.py`

 * *Files identical despite different names*

### Comparing `butterneck-projen-0.0.6/src/butterneck_projen.egg-info/PKG-INFO` & `butterneck-projen-0.0.7/src/butterneck_projen.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterneck-projen
-Version: 0.0.6
+Version: 0.0.7
 Summary: butterneck-projen
 Home-page: https://github.com/butterneck/butterneck-projen.git
 Author: Filippo Pinton<pinton.filippo@protonmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/butterneck/butterneck-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

