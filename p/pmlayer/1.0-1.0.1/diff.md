# Comparing `tmp/pmlayer-1.0.tar.gz` & `tmp/pmlayer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmlayer-1.0.tar", last modified: Fri Feb 17 10:44:20 2023, max compression
+gzip compressed data, was "pmlayer-1.0.1.tar", last modified: Fri Apr 14 08:50:36 2023, max compression
```

## Comparing `pmlayer-1.0.tar` & `pmlayer-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-02-17 10:44:20.334005 pmlayer-1.0/
--rw-rw-rw-   0        0        0    11558 2022-10-12 13:47:20.000000 pmlayer-1.0/LICENSE
--rw-rw-rw-   0        0        0     1314 2023-02-17 10:44:20.332012 pmlayer-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-02-17 08:41:03.000000 pmlayer-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-17 10:44:20.274663 pmlayer-1.0/pmlayer/
--rw-rw-rw-   0        0        0        0 2023-02-01 07:17:16.000000 pmlayer-1.0/pmlayer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-17 10:44:20.316095 pmlayer-1.0/pmlayer/common/
--rw-rw-rw-   0        0        0        0 2023-02-01 07:17:16.000000 pmlayer-1.0/pmlayer/common/__init__.py
--rw-rw-rw-   0        0        0      706 2022-12-13 03:30:05.000000 pmlayer-1.0/pmlayer/common/util.py
-drwxrwxrwx   0        0        0        0 2023-02-17 10:44:20.325029 pmlayer-1.0/pmlayer/torch/
--rw-rw-rw-   0        0        0        0 2023-02-01 07:17:16.000000 pmlayer-1.0/pmlayer/torch/__init__.py
--rw-rw-rw-   0        0        0    12487 2022-12-12 04:36:00.000000 pmlayer-1.0/pmlayer/torch/hierarchical_lattice_layer.py
-drwxrwxrwx   0        0        0        0 2023-02-17 10:44:20.329026 pmlayer-1.0/pmlayer/torch/layers/
--rw-rw-rw-   0        0        0      178 2022-12-13 03:28:15.000000 pmlayer-1.0/pmlayer/torch/layers/__init__.py
--rw-rw-rw-   0        0        0     2721 2022-12-13 02:58:04.000000 pmlayer-1.0/pmlayer/torch/linear_layer.py
--rw-rw-rw-   0        0        0     1464 2022-12-13 02:58:33.000000 pmlayer-1.0/pmlayer/torch/mlp.py
--rw-rw-rw-   0        0        0     5081 2022-12-12 04:36:00.000000 pmlayer-1.0/pmlayer/torch/piecewise_linear_layer.py
-drwxrwxrwx   0        0        0        0 2023-02-17 10:44:20.311145 pmlayer-1.0/pmlayer.egg-info/
--rw-rw-rw-   0        0        0     1314 2023-02-17 10:44:20.000000 pmlayer-1.0/pmlayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-02-17 10:44:20.000000 pmlayer-1.0/pmlayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-17 10:44:20.000000 pmlayer-1.0/pmlayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-02-17 10:44:20.000000 pmlayer-1.0/pmlayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-17 10:44:20.000000 pmlayer-1.0/pmlayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-17 10:44:20.334005 pmlayer-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1494 2023-02-17 10:42:22.000000 pmlayer-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:50:36.049859 pmlayer-1.0.1/
+-rw-rw-rw-   0        0        0    11579 2023-04-14 08:29:58.000000 pmlayer-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1504 2023-04-14 08:50:36.048861 pmlayer-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2023-04-14 08:45:13.000000 pmlayer-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 08:50:35.941483 pmlayer-1.0.1/pmlayer/
+-rw-rw-rw-   0        0        0        0 2023-02-01 07:17:16.000000 pmlayer-1.0.1/pmlayer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:50:35.985453 pmlayer-1.0.1/pmlayer/common/
+-rw-rw-rw-   0        0        0        0 2023-02-01 07:17:16.000000 pmlayer-1.0.1/pmlayer/common/__init__.py
+-rw-rw-rw-   0        0        0      706 2022-12-13 03:30:05.000000 pmlayer-1.0.1/pmlayer/common/util.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:50:36.042364 pmlayer-1.0.1/pmlayer/torch/
+-rw-rw-rw-   0        0        0        0 2023-02-01 07:17:16.000000 pmlayer-1.0.1/pmlayer/torch/__init__.py
+-rw-rw-rw-   0        0        0    12487 2023-04-14 06:03:06.000000 pmlayer-1.0.1/pmlayer/torch/hierarchical_lattice_layer.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:50:36.045866 pmlayer-1.0.1/pmlayer/torch/layers/
+-rw-rw-rw-   0        0        0      178 2022-12-13 03:28:15.000000 pmlayer-1.0.1/pmlayer/torch/layers/__init__.py
+-rw-rw-rw-   0        0        0     2721 2022-12-13 02:58:04.000000 pmlayer-1.0.1/pmlayer/torch/linear_layer.py
+-rw-rw-rw-   0        0        0     1464 2022-12-13 02:58:33.000000 pmlayer-1.0.1/pmlayer/torch/mlp.py
+-rw-rw-rw-   0        0        0     5081 2022-12-12 04:36:00.000000 pmlayer-1.0.1/pmlayer/torch/piecewise_linear_layer.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:50:35.981460 pmlayer-1.0.1/pmlayer.egg-info/
+-rw-rw-rw-   0        0        0     1504 2023-04-14 08:50:35.000000 pmlayer-1.0.1/pmlayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-04-14 08:50:35.000000 pmlayer-1.0.1/pmlayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:50:35.000000 pmlayer-1.0.1/pmlayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-14 08:50:35.000000 pmlayer-1.0.1/pmlayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 08:50:35.000000 pmlayer-1.0.1/pmlayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 08:50:36.050856 pmlayer-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1496 2023-04-14 08:48:20.000000 pmlayer-1.0.1/setup.py
```

### Comparing `pmlayer-1.0/LICENSE` & `pmlayer-1.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2022-2023 International Business Machines Corporation
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `pmlayer-1.0/pmlayer/common/util.py` & `pmlayer-1.0.1/pmlayer/common/util.py`

 * *Files identical despite different names*

### Comparing `pmlayer-1.0/pmlayer/torch/hierarchical_lattice_layer.py` & `pmlayer-1.0.1/pmlayer/torch/hierarchical_lattice_layer.py`

 * *Files identical despite different names*

### Comparing `pmlayer-1.0/pmlayer/torch/linear_layer.py` & `pmlayer-1.0.1/pmlayer/torch/linear_layer.py`

 * *Files identical despite different names*

### Comparing `pmlayer-1.0/pmlayer/torch/mlp.py` & `pmlayer-1.0.1/pmlayer/torch/mlp.py`

 * *Files identical despite different names*

### Comparing `pmlayer-1.0/pmlayer/torch/piecewise_linear_layer.py` & `pmlayer-1.0.1/pmlayer/torch/piecewise_linear_layer.py`

 * *Files identical despite different names*

### Comparing `pmlayer-1.0/setup.py` & `pmlayer-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 DESCRIPTION = 'pmlayer: partially monotone layer'
 NAME = 'pmlayer'
 AUTHOR = 'Hiroki Yanagisawa'
 AUTHOR_EMAIL = 'yanagis@jp.ibm.com'
 URL = 'https://github.com/IBM/pmlayer'
 LICENSE = 'Apache 2.0'
 DOWNLOAD_URL = 'https://github.com/IBM/pmlayer'
-VERSION = '1.0'
+VERSION = '1.0.1'
 PYTHON_REQUIRES = ">=3.6"
 
 INSTALL_REQUIRES = [
     'torch>=1.5',
     'numpy>=0.1',
 ]
```

