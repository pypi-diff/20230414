# Comparing `tmp/raphtory-0.0.8-cp39-none-win_amd64.whl.zip` & `tmp/raphtory-0.0.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2037667 bytes, number of entries: 7
--rw-r--r--  4.6 unx     8659 b- defN 23-Apr-09 22:32 raphtory-0.0.8.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Apr-09 22:32 raphtory-0.0.8.dist-info/WHEEL
--rw-r--r--  4.6 unx     2005 b- defN 23-Apr-09 22:32 raphtory/nullmodels.py
--rw-r--r--  4.6 unx     7447 b- defN 23-Apr-09 22:32 raphtory/vis.py
--rw-r--r--  4.6 unx      311 b- defN 23-Apr-09 22:32 raphtory/__init__.py
--rwxr-xr-x  4.6 unx  5526528 b- defN 23-Apr-09 22:32 raphtory/raphtory.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      532 b- defN 23-Apr-09 22:32 raphtory-0.0.8.dist-info/RECORD
-7 files, 5545578 bytes uncompressed, 2036739 bytes compressed:  63.3%
+Zip file size: 2052474 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     8906 b- defN 23-Apr-14 13:05 raphtory-0.0.9.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Apr-14 13:05 raphtory-0.0.9.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2005 b- defN 23-Apr-14 13:05 raphtory/nullmodels.py
+-rw-r--r--  4.6 unx     7447 b- defN 23-Apr-14 13:05 raphtory/vis.py
+-rw-r--r--  4.6 unx      311 b- defN 23-Apr-14 13:05 raphtory/__init__.py
+-rwxr-xr-x  4.6 unx  5557760 b- defN 23-Apr-14 13:05 raphtory/raphtory.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      532 b- defN 23-Apr-14 13:05 raphtory-0.0.9.dist-info/RECORD
+7 files, 5577057 bytes uncompressed, 2051546 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: raphtory-0.0.8.dist-info/METADATA
+Filename: raphtory-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: raphtory-0.0.8.dist-info/WHEEL
+Filename: raphtory-0.0.9.dist-info/WHEEL
 Comment: 
 
 Filename: raphtory/nullmodels.py
 Comment: 
 
 Filename: raphtory/vis.py
 Comment: 
 
 Filename: raphtory/__init__.py
 Comment: 
 
 Filename: raphtory/raphtory.cp39-win_amd64.pyd
 Comment: 
 
-Filename: raphtory-0.0.8.dist-info/RECORD
+Filename: raphtory-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `raphtory-0.0.8.dist-info/METADATA` & `raphtory-0.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: raphtory
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy >= 1.21.2
-Requires-Dist: matplotlib >= 3.4.3
 Requires-Dist: pandas >= 1.3.3
-Requires-Dist: networkx >= 2.6.3
-Requires-Dist: scipy >= 1.10.1
+Requires-Dist: pyvis >= 0.3.2; extra == 'vis'
+Requires-Dist: networkx >= 2.6.3; extra == 'vis'
+Requires-Dist: matplotlib >= 3.4.3; extra == 'vis'
+Requires-Dist: seaborn >= 0.11.2; extra == 'vis'
+Provides-Extra: vis
 Summary: Python package for DocBrown, a temporal graph library
 Keywords: graph,temporal-graph,temporal
 Home-Page: https://github.com/Raphtory/docbrown/
 Author: Pometry
 License: AGPL-3.0-only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -27,14 +28,15 @@
 <p align="center">
 <a href="https://github.com/Raphtory/docbrown/actions/workflows/build.yml/badge.svg">
 <img alt="Test and Build" src="https://github.com/Raphtory/docbrown/actions/workflows/build.yml/badge.svg" />
 </a>
 <a href="https://github.com/Raphtory/docbrown/issues">
 <img alt="Issues" src="https://img.shields.io/github/issues/Raphtory/docbrown?color=brightgreen" />
 </a>
+<a href="https://codecov.io/gh/Raphtory/docbrown" >  <img src="https://codecov.io/gh/Raphtory/docbrown/branch/main/graph/badge.svg?token=tfJxUiqVzh"/>  </a>
 </p>
 <p align="center">
 <a href="https://www.raphtory.com">🌍 Website </a>
 &nbsp
 <a href="https://docbrown.readthedocs.io">📖 Docs</a>
 &nbsp
 <a href="https://www.pometry.com"><img src="https://user-images.githubusercontent.com/6665739/202438989-2859f8b8-30fb-4402-820a-563049e1fdb3.png" height="20" align="center"/> Pometry</a> 
@@ -183,8 +185,10 @@
 <a href="https://github.com/raphtory/docbrown/graphs/contributors"><img src="https://contrib.rocks/image?repo=raphtory/docbrown"/></a>
 
 Since Doc Brown is still a prototype, we are open to any contributions. If you find any issues or would like to work on some issues yourself, visit the [issues](https://github.com/Raphtory/docbrown/issues) page. Join our [Slack](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA) if you're having any issues or would like to find out more about how you can get stuck in with Raphtory.
 
 # License  
 
 Raphtory is licensed under the terms of the Apache License (check out our LICENSE file).
+
+
```

### html2text {}

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 2.1 Name: raphtory Version: 0.0.8 Classifier: Programming
+Metadata-Version: 2.1 Name: raphtory Version: 0.0.9 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy >= 1.21.2 Requires-Dist: matplotlib >= 3.4.3 Requires-
-Dist: pandas >= 1.3.3 Requires-Dist: networkx >= 2.6.3 Requires-Dist: scipy >=
-1.10.1 Summary: Python package for DocBrown, a temporal graph library Keywords:
-graph,temporal-graph,temporal Home-Page: https://github.com/Raphtory/docbrown/
-Author: Pometry License: AGPL-3.0-only Requires-Python: >=3.7 Description-
-Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Source
-Code, https://github.com/Raphtory/docbrown/
+Requires-Dist: pandas >= 1.3.3 Requires-Dist: pyvis >= 0.3.2; extra == 'vis'
+Requires-Dist: networkx >= 2.6.3; extra == 'vis' Requires-Dist: matplotlib >=
+3.4.3; extra == 'vis' Requires-Dist: seaborn >= 0.11.2; extra == 'vis'
+Provides-Extra: vis Summary: Python package for DocBrown, a temporal graph
+library Keywords: graph,temporal-graph,temporal Home-Page: https://github.com/
+Raphtory/docbrown/ Author: Pometry License: AGPL-3.0-only Requires-Python:
+>=3.7 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/Raphtory/docbrown/
                                   [Raphtory]
 
-                           [Test_and_Build] [Issues]
+[Test_and_Build] [Issues] [https://codecov.io/gh/Raphtory/docbrown/branch/main/
+                       graph/badge.svg?token=tfJxUiqVzh]
 ð_Website   ð_Docs   [https://user-images.githubusercontent.com/6665739/
 202438989-2859f8b8-30fb-4402-820a-563049e1fdb3.png]_Pometry   ð_Report_a_Bug
    [https://user-images.githubusercontent.com/6665739/154071628-a55fb5f9-6994-
                     4dcf-be03-401afc7d9ee0.png]_Join_Slack
 
 # What is Doc Brown? ð¥¼ Doc Brown is the Rust prototype for the next version
 of [Raphtory](https://github.com/Raphtory/Raphtory), rethinking several aspects
```

