# Comparing `tmp/astrojs-aws.construct-0.0.5.tar.gz` & `tmp/astrojs-aws.construct-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrojs-aws.construct-0.0.5.tar", last modified: Fri Apr 14 08:41:57 2023, max compression
+gzip compressed data, was "astrojs-aws.construct-0.0.8.tar", last modified: Fri Apr 14 11:34:08 2023, max compression
```

## Comparing `astrojs-aws.construct-0.0.5.tar` & `astrojs-aws.construct-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 helbing    (501) staff       (20)        0 2023-04-14 08:41:57.374880 astrojs-aws.construct-0.0.5/
--rw-r--r--   0 helbing    (501) staff       (20)     1068 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/LICENSE
--rw-r--r--   0 helbing    (501) staff       (20)       23 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/MANIFEST.in
--rw-r--r--   0 helbing    (501) staff       (20)     2587 2023-04-14 08:41:57.374498 astrojs-aws.construct-0.0.5/PKG-INFO
--rw-r--r--   0 helbing    (501) staff       (20)     1712 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/README.md
--rw-r--r--   0 helbing    (501) staff       (20)      234 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/pyproject.toml
--rw-r--r--   0 helbing    (501) staff       (20)       38 2023-04-14 08:41:57.375022 astrojs-aws.construct-0.0.5/setup.cfg
--rw-r--r--   0 helbing    (501) staff       (20)     1878 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/setup.py
-drwxr-xr-x   0 helbing    (501) staff       (20)        0 2023-04-14 08:41:57.362165 astrojs-aws.construct-0.0.5/src/
-drwxr-xr-x   0 helbing    (501) staff       (20)        0 2023-04-14 08:41:57.362437 astrojs-aws.construct-0.0.5/src/astrojs_aws/
-drwxr-xr-x   0 helbing    (501) staff       (20)        0 2023-04-14 08:41:57.371147 astrojs-aws.construct-0.0.5/src/astrojs_aws/construct/
--rw-r--r--   0 helbing    (501) staff       (20)   144482 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws/construct/__init__.py
-drwxr-xr-x   0 helbing    (501) staff       (20)        0 2023-04-14 08:41:57.372952 astrojs-aws.construct-0.0.5/src/astrojs_aws/construct/_jsii/
--rw-r--r--   0 helbing    (501) staff       (20)      499 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws/construct/_jsii/__init__.py
--rw-r--r--   0 helbing    (501) staff       (20)    25722 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws/construct/_jsii/construct@0.0.5.jsii.tgz
--rw-r--r--   0 helbing    (501) staff       (20)        1 2023-04-14 08:41:44.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws/construct/py.typed
-drwxr-xr-x   0 helbing    (501) staff       (20)        0 2023-04-14 08:41:57.368796 astrojs-aws.construct-0.0.5/src/astrojs_aws.construct.egg-info/
--rw-r--r--   0 helbing    (501) staff       (20)     2587 2023-04-14 08:41:57.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws.construct.egg-info/PKG-INFO
--rw-r--r--   0 helbing    (501) staff       (20)      471 2023-04-14 08:41:57.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws.construct.egg-info/SOURCES.txt
--rw-r--r--   0 helbing    (501) staff       (20)        1 2023-04-14 08:41:57.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws.construct.egg-info/dependency_links.txt
--rw-r--r--   0 helbing    (501) staff       (20)      224 2023-04-14 08:41:57.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws.construct.egg-info/requires.txt
--rw-r--r--   0 helbing    (501) staff       (20)       12 2023-04-14 08:41:57.000000 astrojs-aws.construct-0.0.5/src/astrojs_aws.construct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.146971 astrojs-aws.construct-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.146971 astrojs-aws.construct-0.0.8/src/astrojs_aws/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/
+-rw-r--r--   0 runner    (1001) docker     (123)   144514 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25711 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/_jsii/construct@0.0.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:33:40.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 11:34:08.150971 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 11:34:08.000000 astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/top_level.txt
```

### Comparing `astrojs-aws.construct-0.0.5/LICENSE` & `astrojs-aws.construct-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `astrojs-aws.construct-0.0.5/PKG-INFO` & `astrojs-aws.construct-0.0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrojs-aws.construct
-Version: 0.0.5
+Version: 0.0.8
 Summary: The CDK Construct Library of Astro
 Home-page: https://astro-aws.org/
 Author: helbing
 License: MIT
 Project-URL: Source, https://github.com/helbing/astrojs-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -55,29 +55,29 @@
 ### Edge
 
 ![edge](https://raw.githubusercontent.com/helbing/astrojs-aws/main/docs/static/architecture/edge.png)
 
 ## Static Mode
 
 ```python
-site = astrojsaws.StaticAstroSite(self, "AstroSite",
-    static_dir="/path/to/dist"
-)
+const site = new astrojsaws.StaticAstroSite(this, "AstroSite", {
+  staticDir: "/path/to/dist",
+})
 ```
 
 ## Lambda Mode
 
 ```python
-site = astrojsaws.LambdaAstroSite(self, "AstroSite",
-    server_entry="/path/to/dist/server/entry.mjs",
-    static_dir="/path/to/dist/client"
-)
+const site = new astrojsaws.LambdaAstroSite(this, "AstroSite", {
+  serverEntry: "/path/to/dist/server/entry.mjs",
+  staticDir: "/path/to/dist/client",
+})
 ```
 
 ## Edge Mode
 
 ```python
-site = astrojsaws.EdgeAstroSite(self, "AstroSite",
-    server_entry="/path/to/dist/server/entry.mjs",
-    static_dir="/path/to/dist/client"
-)
+const site = new astrojsaws.EdgeAstroSite(this, "AstroSite", {
+  serverEntry: "/path/to/dist/server/entry.mjs",
+  staticDir: "/path/to/dist/client",
+})
 ```
```

### Comparing `astrojs-aws.construct-0.0.5/README.md` & `astrojs-aws.construct-0.0.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -31,29 +31,29 @@
 ### Edge
 
 ![edge](https://raw.githubusercontent.com/helbing/astrojs-aws/main/docs/static/architecture/edge.png)
 
 ## Static Mode
 
 ```python
-site = astrojsaws.StaticAstroSite(self, "AstroSite",
-    static_dir="/path/to/dist"
-)
+const site = new astrojsaws.StaticAstroSite(this, "AstroSite", {
+  staticDir: "/path/to/dist",
+})
 ```
 
 ## Lambda Mode
 
 ```python
-site = astrojsaws.LambdaAstroSite(self, "AstroSite",
-    server_entry="/path/to/dist/server/entry.mjs",
-    static_dir="/path/to/dist/client"
-)
+const site = new astrojsaws.LambdaAstroSite(this, "AstroSite", {
+  serverEntry: "/path/to/dist/server/entry.mjs",
+  staticDir: "/path/to/dist/client",
+})
 ```
 
 ## Edge Mode
 
 ```python
-site = astrojsaws.EdgeAstroSite(self, "AstroSite",
-    server_entry="/path/to/dist/server/entry.mjs",
-    static_dir="/path/to/dist/client"
-)
+const site = new astrojsaws.EdgeAstroSite(this, "AstroSite", {
+  serverEntry: "/path/to/dist/server/entry.mjs",
+  staticDir: "/path/to/dist/client",
+})
 ```
```

### Comparing `astrojs-aws.construct-0.0.5/setup.py` & `astrojs-aws.construct-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "astrojs-aws.construct",
-    "version": "0.0.5",
+    "version": "0.0.8",
     "description": "The CDK Construct Library of Astro",
     "license": "MIT",
     "url": "https://astro-aws.org/",
     "long_description_content_type": "text/markdown",
     "author": "helbing",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "astrojs_aws.construct",
         "astrojs_aws.construct._jsii"
     ],
     "package_data": {
         "astrojs_aws.construct._jsii": [
-            "construct@0.0.5.jsii.tgz"
+            "construct@0.0.8.jsii.tgz"
         ],
         "astrojs_aws.construct": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `astrojs-aws.construct-0.0.5/src/astrojs_aws/construct/__init__.py` & `astrojs-aws.construct-0.0.8/src/astrojs_aws/construct/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,35 +32,35 @@
 ### Edge
 
 ![edge](https://raw.githubusercontent.com/helbing/astrojs-aws/main/docs/static/architecture/edge.png)
 
 ## Static Mode
 
 ```python
-site = astrojsaws.StaticAstroSite(self, "AstroSite",
-    static_dir="/path/to/dist"
-)
+const site = new astrojsaws.StaticAstroSite(this, "AstroSite", {
+  staticDir: "/path/to/dist",
+})
 ```
 
 ## Lambda Mode
 
 ```python
-site = astrojsaws.LambdaAstroSite(self, "AstroSite",
-    server_entry="/path/to/dist/server/entry.mjs",
-    static_dir="/path/to/dist/client"
-)
+const site = new astrojsaws.LambdaAstroSite(this, "AstroSite", {
+  serverEntry: "/path/to/dist/server/entry.mjs",
+  staticDir: "/path/to/dist/client",
+})
 ```
 
 ## Edge Mode
 
 ```python
-site = astrojsaws.EdgeAstroSite(self, "AstroSite",
-    server_entry="/path/to/dist/server/entry.mjs",
-    static_dir="/path/to/dist/client"
-)
+const site = new astrojsaws.EdgeAstroSite(this, "AstroSite", {
+  serverEntry: "/path/to/dist/server/entry.mjs",
+  staticDir: "/path/to/dist/client",
+})
 ```
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
```

### Comparing `astrojs-aws.construct-0.0.5/src/astrojs_aws.construct.egg-info/PKG-INFO` & `astrojs-aws.construct-0.0.8/src/astrojs_aws.construct.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrojs-aws.construct
-Version: 0.0.5
+Version: 0.0.8
 Summary: The CDK Construct Library of Astro
 Home-page: https://astro-aws.org/
 Author: helbing
 License: MIT
 Project-URL: Source, https://github.com/helbing/astrojs-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -55,29 +55,29 @@
 ### Edge
 
 ![edge](https://raw.githubusercontent.com/helbing/astrojs-aws/main/docs/static/architecture/edge.png)
 
 ## Static Mode
 
 ```python
-site = astrojsaws.StaticAstroSite(self, "AstroSite",
-    static_dir="/path/to/dist"
-)
+const site = new astrojsaws.StaticAstroSite(this, "AstroSite", {
+  staticDir: "/path/to/dist",
+})
 ```
 
 ## Lambda Mode
 
 ```python
-site = astrojsaws.LambdaAstroSite(self, "AstroSite",
-    server_entry="/path/to/dist/server/entry.mjs",
-    static_dir="/path/to/dist/client"
-)
+const site = new astrojsaws.LambdaAstroSite(this, "AstroSite", {
+  serverEntry: "/path/to/dist/server/entry.mjs",
+  staticDir: "/path/to/dist/client",
+})
 ```
 
 ## Edge Mode
 
 ```python
-site = astrojsaws.EdgeAstroSite(self, "AstroSite",
-    server_entry="/path/to/dist/server/entry.mjs",
-    static_dir="/path/to/dist/client"
-)
+const site = new astrojsaws.EdgeAstroSite(this, "AstroSite", {
+  serverEntry: "/path/to/dist/server/entry.mjs",
+  staticDir: "/path/to/dist/client",
+})
 ```
```

