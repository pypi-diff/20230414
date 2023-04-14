# Comparing `tmp/OpenGeode_GeosciencesIO-3.9.2-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_GeosciencesIO-4.0.0-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,13 @@
-Zip file size: 215971 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat   387072 b- defN 22-Aug-03 08:18 opengeode_geosciencesio/OpenGeode-GeosciencesIO_geosciences.dll
--rw-rw-rw-  2.0 fat     1256 b- defN 22-Aug-03 08:17 opengeode_geosciencesio/__init__.py
--rw-rw-rw-  2.0 fat   110080 b- defN 22-Aug-03 08:18 opengeode_geosciencesio/opengeode_geosciencesio_py_geosciences.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3297 b- defN 22-Aug-03 08:18 OpenGeode_GeosciencesIO-3.9.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 22-Aug-03 08:18 OpenGeode_GeosciencesIO-3.9.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 22-Aug-03 08:18 OpenGeode_GeosciencesIO-3.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      717 b- defN 22-Aug-03 08:18 OpenGeode_GeosciencesIO-3.9.2.dist-info/RECORD
-7 files, 502546 bytes uncompressed, 214675 bytes compressed:  57.3%
+Zip file size: 416477 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       87 b- defN 23-Apr-14 07:14 opengeode_geosciencesio/__init__.py
+-rw-r--r--  2.0 unx     1211 b- defN 23-Apr-14 07:14 opengeode_geosciencesio/mesh.py
+-rw-r--r--  2.0 unx     1242 b- defN 23-Apr-14 07:14 opengeode_geosciencesio/model.py
+-rwxr-xr-x  2.0 unx   223608 b- defN 23-Apr-14 07:15 opengeode_geosciencesio/lib64/libOpenGeode-GeosciencesIO_mesh.so
+-rwxr-xr-x  2.0 unx   646568 b- defN 23-Apr-14 07:15 opengeode_geosciencesio/lib64/libOpenGeode-GeosciencesIO_model.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-Apr-14 07:15 opengeode_geosciencesio/lib64/opengeode_geosciencesio_py_mesh.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   122232 b- defN 23-Apr-14 07:15 opengeode_geosciencesio/lib64/opengeode_geosciencesio_py_model.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     3241 b- defN 23-Apr-14 07:15 OpenGeode_GeosciencesIO-4.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      103 b- defN 23-Apr-14 07:15 OpenGeode_GeosciencesIO-4.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Apr-14 07:15 OpenGeode_GeosciencesIO-4.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1180 b- defN 23-Apr-14 07:15 OpenGeode_GeosciencesIO-4.0.0.dist-info/RECORD
+11 files, 1121728 bytes uncompressed, 414411 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -1,22 +1,34 @@
-Filename: opengeode_geosciencesio/OpenGeode-GeosciencesIO_geosciences.dll
+Filename: opengeode_geosciencesio/__init__.py
 Comment: 
 
-Filename: opengeode_geosciencesio/__init__.py
+Filename: opengeode_geosciencesio/mesh.py
+Comment: 
+
+Filename: opengeode_geosciencesio/model.py
+Comment: 
+
+Filename: opengeode_geosciencesio/lib64/libOpenGeode-GeosciencesIO_mesh.so
+Comment: 
+
+Filename: opengeode_geosciencesio/lib64/libOpenGeode-GeosciencesIO_model.so
+Comment: 
+
+Filename: opengeode_geosciencesio/lib64/opengeode_geosciencesio_py_mesh.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: opengeode_geosciencesio/opengeode_geosciencesio_py_geosciences.cp39-win_amd64.pyd
+Filename: opengeode_geosciencesio/lib64/opengeode_geosciencesio_py_model.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-3.9.2.dist-info/METADATA
+Filename: OpenGeode_GeosciencesIO-4.0.0.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-3.9.2.dist-info/WHEEL
+Filename: OpenGeode_GeosciencesIO-4.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-3.9.2.dist-info/top_level.txt
+Filename: OpenGeode_GeosciencesIO-4.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-3.9.2.dist-info/RECORD
+Filename: OpenGeode_GeosciencesIO-4.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciencesio/__init__.py

```diff
@@ -1,25 +1,4 @@
-# Copyright (c) 2019 - 2022 Geode-solutions
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
-
-import opengeode
-import opengeode_geosciences
-
-from .opengeode_geosciencesio_py_geosciences import *
-initialize_geosciences_io()
+## Copyright (c) 2019 - 2023 Geode-solutions
+
+from .mesh import *
+from .model import *
```

## Comparing `OpenGeode_GeosciencesIO-3.9.2.dist-info/METADATA` & `OpenGeode_GeosciencesIO-4.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: OpenGeode-GeosciencesIO
-Version: 3.9.2
+Version: 4.0.0
 Summary: Input/Output formats for OpenGeode-Geosciences
 Home-page: https://github.com/Geode-solutions/OpenGeode-GeosciencesIO
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
-Requires-Dist: OpenGeode-core (==11.*,>=11.0.1)
-Requires-Dist: OpenGeode-Geosciences (==5.*,>=5.5.0)
+Requires-Dist: opengeode-core (==14.*,>=14.0.0)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.0)
 
 <h1 align="center">OpenGeode-GeosciencesIO<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Input/Output formats for OpenGeode-Geosciences</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/workflows/CD/badge.svg" alt="Deploy Status">
@@ -29,16 +27,16 @@
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
 </p>
 
 ---
@@ -54,21 +52,19 @@
 To check out our live documentation, visit [docs.geode-solutions.com](https://docs.geode-solutions.com).
 
 Installing OpenGeode-GeosciencesIO is done:
  * either, by compiling the C++ source.
  * or, by using pip command ```pip install OpenGeode-GeosciencesIO``` and add ```import opengeode_geosciencesio``` in your Python script.
 
 ## Questions
-For questions and support please use the official [slack](https://slackin-opengeode.herokuapp.com) and go to the channel #geosciences_io. The issue list of this repo is exclusively for bug reports and feature requests. 
+For questions and support please use the official [slack](https://opengeode-slack-invite.herokuapp.com) and go to the channel #geosciences_io. The issue list of this repo is exclusively for bug reports and feature requests. 
 
 ## Changelog
 
 Detailed changes for each release are documented in the [release notes](https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/releases).
 
 
 ## License
 
 [MIT](https://opensource.org/licenses/MIT)
 
-Copyright (c) 2019 - 2022, Geode-solutions
-
-
+Copyright (c) 2019 - 2023, Geode-solutions
```

### html2text {}

```diff
@@ -1,26 +1,25 @@
-Metadata-Version: 2.1 Name: OpenGeode-GeosciencesIO Version: 3.9.2 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-GeosciencesIO Version: 4.0.0 Summary:
 Input/Output formats for OpenGeode-Geosciences Home-page: https://github.com/
 Geode-solutions/OpenGeode-GeosciencesIO Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: MIT Platform: UNKNOWN Classifier: License
-:: OSI Approved :: MIT License Description-Content-Type: text/markdown
-Requires-Dist: OpenGeode-core (==11.*,>=11.0.1) Requires-Dist: OpenGeode-
-Geosciences (==5.*,>=5.5.0)
+contact@geode-solutions.com License: MIT Description-Content-Type: text/
+markdown Requires-Dist: opengeode-core (==14.*,>=14.0.0) Requires-Dist:
+opengeode-geosciences (==7.*,>=7.0.0)
             ****** OpenGeode-GeosciencesIOby Geode-solutions ******
            **** Input/Output formats for OpenGeode-Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-GeosciencesIO provides input and output formats
 for [OpenGeode-Geosciences] objects. [OpenGeode-Geosciences]: https://
 github.com/Geode-solutions/OpenGeode-Geosciences ## Documentation To check out
 our live documentation, visit [docs.geode-solutions.com](https://docs.geode-
 solutions.com). Installing OpenGeode-GeosciencesIO is done: * either, by
 compiling the C++ source. * or, by using pip command ```pip install OpenGeode-
 GeosciencesIO``` and add ```import opengeode_geosciencesio``` in your Python
 script. ## Questions For questions and support please use the official [slack]
-(https://slackin-opengeode.herokuapp.com) and go to the channel
+(https://opengeode-slack-invite.herokuapp.com) and go to the channel
 #geosciences_io. The issue list of this repo is exclusively for bug reports and
 feature requests. ## Changelog Detailed changes for each release are documented
 in the [release notes](https://github.com/Geode-solutions/OpenGeode-
 GeosciencesIO/releases). ## License [MIT](https://opensource.org/licenses/MIT)
-Copyright (c) 2019 - 2022, Geode-solutions
+Copyright (c) 2019 - 2023, Geode-solutions
```

