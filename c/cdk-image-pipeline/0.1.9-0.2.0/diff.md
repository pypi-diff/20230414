# Comparing `tmp/cdk-image-pipeline-0.1.9.tar.gz` & `tmp/cdk-image-pipeline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-image-pipeline-0.1.9.tar", last modified: Fri Aug 19 19:22:49 2022, max compression
+gzip compressed data, was "cdk-image-pipeline-0.2.0.tar", last modified: Fri Apr 14 00:37:49 2023, max compression
```

## Comparing `cdk-image-pipeline-0.1.9.tar` & `cdk-image-pipeline-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:22:49.211671 cdk-image-pipeline-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8820 2022-08-19 19:22:49.211671 cdk-image-pipeline-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7861 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-19 19:22:49.211671 cdk-image-pipeline-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:22:49.207671 cdk-image-pipeline-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:22:49.207671 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)    23821 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:22:49.211671 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline/_jsii/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22409 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.1.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 19:22:37.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 19:22:49.211671 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8820 2022-08-19 19:22:48.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-08-19 19:22:49.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 19:22:48.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-19 19:22:49.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-19 19:22:49.000000 cdk-image-pipeline-0.1.9/src/cdk_image_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    35524 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26390 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/_jsii/cdk-image-pipeline@0.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:37:37.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:37:49.056272 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 00:37:49.000000 cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/top_level.txt
```

### Comparing `cdk-image-pipeline-0.1.9/LICENSE` & `cdk-image-pipeline-0.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 Amazon.com, Inc. or its affiliates. All Rights Reserved.
+Copyright 2023 Amazon.com, Inc. or its affiliates. All Rights Reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so.
```

### Comparing `cdk-image-pipeline-0.1.9/PKG-INFO` & `cdk-image-pipeline-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.1.9
+Version: 0.2.0
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -267,9 +267,7 @@
 
 ## Additional API notes
 
 ---
 
 
 [API Reference](API.md)
-
-
```

### Comparing `cdk-image-pipeline-0.1.9/README.md` & `cdk-image-pipeline-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-image-pipeline-0.1.9/setup.py` & `cdk-image-pipeline-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-image-pipeline",
-    "version": "0.1.9",
+    "version": "0.2.0",
     "description": "Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK",
     "license": "MIT-0",
     "url": "https://github.com/aws-samples/cdk-image-pipeline.git",
     "long_description_content_type": "text/markdown",
     "author": "Cameron Magee<magcamer@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_image_pipeline",
         "cdk_image_pipeline._jsii"
     ],
     "package_data": {
         "cdk_image_pipeline._jsii": [
-            "cdk-image-pipeline@0.1.9.jsii.tgz"
+            "cdk-image-pipeline@0.2.0.jsii.tgz"
         ],
         "cdk_image_pipeline": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.38.1, <3.0.0",
-        "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.65.0, <2.0.0",
+        "aws-cdk-lib>=2.73.0, <3.0.0",
+        "constructs>=10.1.215, <11.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-image-pipeline-0.1.9/src/cdk_image_pipeline.egg-info/PKG-INFO` & `cdk-image-pipeline-0.2.0/src/cdk_image_pipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-image-pipeline
-Version: 0.1.9
+Version: 0.2.0
 Summary: Quickly deploy a complete EC2 Image Builder Image Pipeline using CDK
 Home-page: https://github.com/aws-samples/cdk-image-pipeline.git
 Author: Cameron Magee<magcamer@amazon.com>
 License: MIT-0
 Project-URL: Source, https://github.com/aws-samples/cdk-image-pipeline.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -267,9 +267,7 @@
 
 ## Additional API notes
 
 ---
 
 
 [API Reference](API.md)
-
-
```

