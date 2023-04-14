# Comparing `tmp/OpenGeode_Inspector-2.9.2-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_Inspector-3.0.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,8 @@
-Zip file size: 254898 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat   419840 b- defN 23-Feb-06 08:26 opengeode_inspector/OpenGeode-Inspector_inspector.dll
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Feb-06 08:25 opengeode_inspector/__init__.py
--rw-rw-rw-  2.0 fat      269 b- defN 23-Feb-06 08:25 opengeode_inspector/inspector.py
--rw-rw-rw-  2.0 fat   430592 b- defN 23-Feb-06 08:27 opengeode_inspector/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     5560 b- defN 23-Feb-06 08:27 OpenGeode_Inspector-2.9.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Feb-06 08:27 OpenGeode_Inspector-2.9.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Feb-06 08:27 OpenGeode_Inspector-2.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      765 b- defN 23-Feb-06 08:27 OpenGeode_Inspector-2.9.2.dist-info/RECORD
-8 files, 858294 bytes uncompressed, 253542 bytes compressed:  70.5%
+Zip file size: 3427 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Apr-14 08:29 opengeode_inspector/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-Apr-14 08:29 opengeode_inspector/inspector.py
+-rw-rw-rw-  2.0 fat     5480 b- defN 23-Apr-14 08:31 OpenGeode_Inspector-3.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-14 08:31 OpenGeode_Inspector-3.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-14 08:31 OpenGeode_Inspector-3.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      521 b- defN 23-Apr-14 08:31 OpenGeode_Inspector-3.0.0.dist-info/RECORD
+6 files, 6466 bytes uncompressed, 2471 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -1,25 +1,19 @@
-Filename: opengeode_inspector/OpenGeode-Inspector_inspector.dll
-Comment: 
-
 Filename: opengeode_inspector/__init__.py
 Comment: 
 
 Filename: opengeode_inspector/inspector.py
 Comment: 
 
-Filename: opengeode_inspector/opengeode_inspector_py_inspector.cp39-win_amd64.pyd
-Comment: 
-
-Filename: OpenGeode_Inspector-2.9.2.dist-info/METADATA
+Filename: OpenGeode_Inspector-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_Inspector-2.9.2.dist-info/WHEEL
+Filename: OpenGeode_Inspector-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_Inspector-2.9.2.dist-info/top_level.txt
+Filename: OpenGeode_Inspector-3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_Inspector-2.9.2.dist-info/RECORD
+Filename: OpenGeode_Inspector-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_inspector/__init__.py

```diff
@@ -1,21 +1,3 @@
-# Copyright (c) 2019 - 2023 Geode-solutions
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
+## Copyright (c) 2019 - 2023 Geode-solutions
 
 from .inspector import *
```

## opengeode_inspector/inspector.py

```diff
@@ -3,9 +3,9 @@
 #
 
 import opengeode
 import opengeode_io
 import opengeode_geosciences
 import opengeode_geosciencesio
 
-from .opengeode_inspector_py_inspector import *
-OpenGeodeInspectorInspector.initialize()
+from .bin.opengeode_inspector_py_inspector import *
+InspectorInspectorLibrary.initialize()
```

## Comparing `OpenGeode_Inspector-2.9.2.dist-info/METADATA` & `OpenGeode_Inspector-3.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: OpenGeode-Inspector
-Version: 2.9.2
+Version: 3.0.0
 Summary: Open source framework for inspecting the validity of geometric models
 Home-page: https://github.com/Geode-solutions/OpenGeode-Inspector
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
-Keywords: brep,inspecting,mesh,topology
 Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
-Requires-Dist: OpenGeode-core (==12.*,>=12.6.6)
-Requires-Dist: OpenGeode-IO (==5.*,>=5.23.1)
-Requires-Dist: OpenGeode-Geosciences (==5.*,>=5.7.6)
-Requires-Dist: OpenGeode-GeosciencesIO (==3.*,>=3.12.0)
+Requires-Dist: opengeode-core (==14.*,>=14.0.0)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.0)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.0.0)
+Requires-Dist: opengeode-io (==6.*,>=6.0.0)
 
 <h1 align="center">OpenGeode-Inspector<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenGeode module for inspecting meshes and models</h3>
 
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-ModuleTemplate/workflows/CI/badge.svg" alt="Build Status">
@@ -32,16 +30,16 @@
   <img src="https://img.shields.io/static/v1?label=Red%20Hat&logo=Red-Hat&logoColor=white&message=support&color=success" alt="Red Hat support">
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
   <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
   <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
-  <a href="https://slackin-opengeode.herokuapp.com">
-    <img src="https://slackin-opengeode.herokuapp.com/badge.svg" alt="Slack invite">
+  <a href="https://opengeode-slack-invite.herokuapp.com">
+    <img src="https://opengeode-slack-invite.herokuapp.com/badge.svg" alt="Slack invite">
   </a>
   <a href="https://doi.org/10.5281/zenodo.3610370">
     <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3610370.svg" alt="DOI">
   </a>
 
 ---
 
@@ -102,15 +100,15 @@
  * BRep:
    * Validity of the topology
    * Checks on each component mesh: all the previous mesh checks depending on the component mesh type
    * Checks on the validity of the unique vertices (linking to vertices, colocation of unique vertices points, un-colocation of points with same unique vertices)
    * Intersection of the component mesh surfaces between each other
 
 ## Questions
-For questions and support please use the official [slack](https://slackin-opengeode.herokuapp.com) and go to the channel #inspector. The issue list of this repo is exclusively for bug reports and feature requests. 
+For questions and support please use the official [slack](https://opengeode-slack-invite.herokuapp.com) and go to the channel #inspector. The issue list of this repo is exclusively for bug reports and feature requests. 
 
 
 ## License
 
 [MIT](https://opensource.org/licenses/MIT)
 
 Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,16 +1,15 @@
-Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 2.9.2 Summary: Open
+Metadata-Version: 2.1 Name: OpenGeode-Inspector Version: 3.0.0 Summary: Open
 source framework for inspecting the validity of geometric models Home-page:
 https://github.com/Geode-solutions/OpenGeode-Inspector Author: Geode-solutions
-Author-email: contact@geode-solutions.com License: MIT Keywords:
-brep,inspecting,mesh,topology Platform: UNKNOWN Classifier: License :: OSI
-Approved :: MIT License Description-Content-Type: text/markdown Requires-Dist:
-OpenGeode-core (==12.*,>=12.6.6) Requires-Dist: OpenGeode-IO (==5.*,>=5.23.1)
-Requires-Dist: OpenGeode-Geosciences (==5.*,>=5.7.6) Requires-Dist: OpenGeode-
-GeosciencesIO (==3.*,>=3.12.0)
+Author-email: contact@geode-solutions.com License: MIT Platform: UNKNOWN
+Description-Content-Type: text/markdown Requires-Dist: opengeode-core
+(==14.*,>=14.0.0) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.0)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.0.0) Requires-Dist:
+opengeode-io (==6.*,>=6.0.0)
               ****** OpenGeode-Inspectorby Geode-solutions ******
           **** OpenGeode module for inspecting meshes and models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
       [Language] [License] [Semantic-release] [Slack_invite] [DOI] --- ##
  Introduction OpenGeode-Inspector is a module of [OpenGeode] providing ways of
  inspecting your meshes and models and verifying their validity. [OpenGeode]:
@@ -43,12 +42,12 @@
  vertices, colocation of unique vertices points, un-colocation of points with
   same unique vertices) * Intersection of the component mesh surfaces between
 each other * BRep: * Validity of the topology * Checks on each component mesh:
  all the previous mesh checks depending on the component mesh type * Checks on
 the validity of the unique vertices (linking to vertices, colocation of unique
      vertices points, un-colocation of points with same unique vertices) *
 Intersection of the component mesh surfaces between each other ## Questions For
-    questions and support please use the official [slack](https://slackin-
- opengeode.herokuapp.com) and go to the channel #inspector. The issue list of
-this repo is exclusively for bug reports and feature requests. ## License [MIT]
+questions and support please use the official [slack](https://opengeode-slack-
+invite.herokuapp.com) and go to the channel #inspector. The issue list of this
+  repo is exclusively for bug reports and feature requests. ## License [MIT]
     (https://opensource.org/licenses/MIT) Copyright (c) 2019 - 2023, Geode-
                                   solutions
```

