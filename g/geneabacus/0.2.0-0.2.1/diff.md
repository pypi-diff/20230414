# Comparing `tmp/geneabacus-0.2.0.tar.gz` & `tmp/geneabacus-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneabacus-0.2.0.tar", last modified: Mon Oct 24 20:38:16 2022, max compression
+gzip compressed data, was "geneabacus-0.2.1.tar", last modified: Fri Apr 14 20:12:16 2023, max compression
```

## Comparing `geneabacus-0.2.0.tar` & `geneabacus-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2022-10-24 20:38:16.537586 geneabacus-0.2.0/
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)       17 2022-10-24 20:18:10.000000 geneabacus-0.2.0/.gitignore
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)    16726 2022-10-24 20:18:10.000000 geneabacus-0.2.0/LICENSE
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1449 2022-10-24 20:38:16.537586 geneabacus-0.2.0/PKG-INFO
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1138 2022-10-24 20:28:09.000000 geneabacus-0.2.0/README.md
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)      131 2022-10-24 20:35:35.000000 geneabacus-0.2.0/pyproject.toml
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)      465 2022-10-24 20:38:16.537586 geneabacus-0.2.0/setup.cfg
-drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2022-10-24 20:38:16.537586 geneabacus-0.2.0/src/
-drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2022-10-24 20:38:16.537586 geneabacus-0.2.0/src/geneabacus/
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)        0 2022-10-24 20:18:10.000000 geneabacus-0.2.0/src/geneabacus/__init__.py
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)     4772 2022-10-24 20:18:10.000000 geneabacus-0.2.0/src/geneabacus/profileio.py
-drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2022-10-24 20:38:16.537586 geneabacus-0.2.0/src/geneabacus.egg-info/
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1449 2022-10-24 20:38:16.000000 geneabacus-0.2.0/src/geneabacus.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)      297 2022-10-24 20:38:16.000000 geneabacus-0.2.0/src/geneabacus.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)        1 2022-10-24 20:38:16.000000 geneabacus-0.2.0/src/geneabacus.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)       10 2022-10-24 20:38:16.000000 geneabacus-0.2.0/src/geneabacus.egg-info/requires.txt
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)       11 2022-10-24 20:38:16.000000 geneabacus-0.2.0/src/geneabacus.egg-info/top_level.txt
+drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2023-04-14 20:12:16.443937 geneabacus-0.2.1/
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)       17 2022-10-24 20:18:10.000000 geneabacus-0.2.1/.gitignore
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)    16726 2022-10-24 20:18:10.000000 geneabacus-0.2.1/LICENSE
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1448 2023-04-14 20:12:16.443937 geneabacus-0.2.1/PKG-INFO
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1137 2023-03-09 17:37:32.000000 geneabacus-0.2.1/README.md
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)      131 2022-10-24 20:35:35.000000 geneabacus-0.2.1/pyproject.toml
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)      465 2023-04-14 20:12:16.443937 geneabacus-0.2.1/setup.cfg
+drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2023-04-14 20:12:16.440604 geneabacus-0.2.1/src/
+drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2023-04-14 20:12:16.440604 geneabacus-0.2.1/src/geneabacus/
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)        0 2022-10-24 20:18:10.000000 geneabacus-0.2.1/src/geneabacus/__init__.py
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)     4907 2023-04-13 22:24:08.000000 geneabacus-0.2.1/src/geneabacus/profileio.py
+drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2023-04-14 20:12:16.443937 geneabacus-0.2.1/src/geneabacus.egg-info/
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1448 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)      297 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)        1 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)       10 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/requires.txt
+-rw-r--r--   0 charles   (1000) giraldezlab  (1200)       11 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/top_level.txt
```

### Comparing `geneabacus-0.2.0/LICENSE` & `geneabacus-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneabacus-0.2.0/PKG-INFO` & `geneabacus-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneabacus
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python IO functions for GeneAbacus
 Home-page: https://git.sr.ht/~vejnar/GeneAbacus-python
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,8 +41,8 @@
 array([0., 0., 21., ..., 0., 3., 0.], dtype=float32)
 ```
 
 ## License
 
 *GeneAbacus* is distributed under the Mozilla Public License Version 2.0 (see /LICENSE).
 
-Copyright (C) 2015-2022 Charles E. Vejnar
+Copyright © 2015-2023 Charles E. Vejnar
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geneabacus-0.2.0/README.md` & `geneabacus-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 array([0., 0., 21., ..., 0., 3., 0.], dtype=float32)
 ```
 
 ## License
 
 *GeneAbacus* is distributed under the Mozilla Public License Version 2.0 (see /LICENSE).
 
-Copyright (C) 2015-2022 Charles E. Vejnar
+Copyright © 2015-2023 Charles E. Vejnar
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geneabacus-0.2.0/src/geneabacus/profileio.py` & `geneabacus-0.2.1/src/geneabacus/profileio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 #
-# Copyright (C) 2015-2022 Charles E. Vejnar
+# Copyright © 2015 Charles E. Vejnar
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://www.mozilla.org/MPL/2.0/.
 #
 
 import json
@@ -20,30 +20,33 @@
 
 def parse_feat_line(line):
     cells = line.rstrip().split('\t')
     return [cells[0], int(cells[1])]
 
 def pfopen(filename, path_features=None, fon_name='transcript_stable_id', fon_coords='exons', features=[], rw=False):
     assert os.path.exists(filename), f'{filename} not found'
-    assert os.path.exists(path_features), f'{path_features} not found'
     # Open file
     if filename.endswith('.bin'):
         f = open(filename, 'rb')
     elif filename.endswith('.bin.lz4'):
         f = lz4.frame.open(filename, 'rb')
     else:
         raise ValueError('Invalid format')
     # Open feature file
-    if path_features.endswith('.fon1.json'):
-        features = [[ft[fon_name], get_flength(ft[fon_coords])] for ft in json.load(open(path_features, 'rt'))['features']]
-    elif path_features.endswith('.tab'):
-        with open(path_features, 'rt') as ftab:
-            features = [parse_feat_line(l) for l in ftab]
-    else:
-        raise ValueError(f'Unknown format: {path_features}')
+    if path_features is not None:
+        assert os.path.exists(path_features), f'{path_features} not found'
+        if path_features.endswith('.fon1.json'):
+            features = [[ft[fon_name], get_flength(ft[fon_coords])] for ft in json.load(open(path_features, 'rt'))['features']]
+        elif path_features.endswith('.tab'):
+            with open(path_features, 'rt') as ftab:
+                features = [parse_feat_line(l) for l in ftab]
+        else:
+            raise ValueError(f'Unknown format: {path_features}')
+    elif len(features) == 0:
+        raise ValueError('No input features')
     # Read version
     detected_version = np.frombuffer(f.read(1), dtype='uint8')[0]
     assert detected_version in [3], f'Unknown version: {detected_version}'
     # Read Length
     full_length = np.frombuffer(f.read(4), dtype='uint32')[0]
     # Read checksum
     detected_csum = np.frombuffer(f.read(4), dtype='uint32')[0]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geneabacus-0.2.0/src/geneabacus.egg-info/PKG-INFO` & `geneabacus-0.2.1/src/geneabacus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneabacus
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python IO functions for GeneAbacus
 Home-page: https://git.sr.ht/~vejnar/GeneAbacus-python
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -41,8 +41,8 @@
 array([0., 0., 21., ..., 0., 3., 0.], dtype=float32)
 ```
 
 ## License
 
 *GeneAbacus* is distributed under the Mozilla Public License Version 2.0 (see /LICENSE).
 
-Copyright (C) 2015-2022 Charles E. Vejnar
+Copyright © 2015-2023 Charles E. Vejnar
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

