# Comparing `tmp/Geode_MyModule-1.2.0-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_MyModule-2.0.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,8 @@
-Zip file size: 1057546 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat  2037760 b- defN 23-Mar-06 13:37 geode_mymodule/Geode-MyModule_mylib.dll
--rw-rw-rw-  2.0 fat       97 b- defN 23-Mar-06 13:37 geode_mymodule/__init__.py
--rw-rw-rw-  2.0 fat   126464 b- defN 23-Mar-06 13:37 geode_mymodule/geode_mymodule_py_mylib.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      194 b- defN 23-Mar-06 13:37 geode_mymodule/mylib.py
--rw-rw-rw-  2.0 fat     2096 b- defN 23-Mar-06 13:37 Geode_MyModule-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Mar-06 13:37 Geode_MyModule-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Mar-06 13:37 Geode_MyModule-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      702 b- defN 23-Mar-06 13:37 Geode_MyModule-1.2.0.dist-info/RECORD
-8 files, 2167428 bytes uncompressed, 1056314 bytes compressed:  51.3%
+Zip file size: 2259 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       70 b- defN 23-Apr-14 11:09 geode_mymodule/__init__.py
+-rw-rw-rw-  2.0 fat      195 b- defN 23-Apr-14 11:09 geode_mymodule/mylib.py
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-Apr-14 11:10 Geode_MyModule-2.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-14 11:10 Geode_MyModule-2.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Apr-14 11:10 Geode_MyModule-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      487 b- defN 23-Apr-14 11:10 Geode_MyModule-2.0.0.dist-info/RECORD
+6 files, 2957 bytes uncompressed, 1371 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -1,25 +1,19 @@
-Filename: geode_mymodule/Geode-MyModule_mylib.dll
-Comment: 
-
 Filename: geode_mymodule/__init__.py
 Comment: 
 
-Filename: geode_mymodule/geode_mymodule_py_mylib.cp39-win_amd64.pyd
-Comment: 
-
 Filename: geode_mymodule/mylib.py
 Comment: 
 
-Filename: Geode_MyModule-1.2.0.dist-info/METADATA
+Filename: Geode_MyModule-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: Geode_MyModule-1.2.0.dist-info/WHEEL
+Filename: Geode_MyModule-2.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_MyModule-1.2.0.dist-info/top_level.txt
+Filename: Geode_MyModule-2.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_MyModule-1.2.0.dist-info/RECORD
+Filename: Geode_MyModule-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_mymodule/__init__.py

```diff
@@ -1,5 +1,3 @@
-#
-# Copyright (c) 2019 - 2022 Geode-solutions. All rights reserved.
-#
+## Copyright (c) 2019 - 2023 Geode-solutions
 
 from .mylib import *
```

## geode_mymodule/mylib.py

```diff
@@ -1,9 +1,9 @@
 #
 # Copyright (c) 2019 - 2022 Geode-solutions. All rights reserved.
 #
 
 import opengeode
-from geode_common import core
+import geode_common
 
-from .geode_mymodule_py_mylib import *
-MyModuleMyLib.initialize()
+from .bin.geode_mymodule_py_mylib import *
+MyModuleMyLibLibrary.initialize()
```

## Comparing `Geode_MyModule-1.2.0.dist-info/METADATA` & `Geode_MyModule-2.0.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Geode-MyModule
-Version: 1.2.0
+Version: 2.0.0
 Summary: Template for creating your own OpenGeode private module
-Home-page: https://github.com/Geode-solutions/Geode-ModuleTemplate
+Home-page: https://github.com/Geode-solutions/Geode-MyModule
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: OpenGeode-core (==13.*,>=13.0.0)
-Requires-Dist: Geode-Common (==23.*,>=23.2.0)
+Requires-Dist: geode-common (==25.*,>=25.0.0)
+Requires-Dist: opengeode-core (==14.*,>=14.0.0)
 
 <h1 align="center">Geode-ModuleTemplate_private<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Template for creating your own OpenGeode private module</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-ModuleTemplate_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-MyModule Version: 1.2.0 Summary: Template for
+Metadata-Version: 2.1 Name: Geode-MyModule Version: 2.0.0 Summary: Template for
 creating your own OpenGeode private module Home-page: https://github.com/Geode-
-solutions/Geode-ModuleTemplate Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: OpenGeode-core (==13.*,>=13.0.0)
-Requires-Dist: Geode-Common (==23.*,>=23.2.0)
+solutions/Geode-MyModule Author: Geode-solutions Author-email: contact@geode-
+solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
+text/markdown Requires-Dist: geode-common (==25.*,>=25.0.0) Requires-Dist:
+opengeode-core (==14.*,>=14.0.0)
          ****** Geode-ModuleTemplate_privateby Geode-solutions ******
        **** Template for creating your own OpenGeode private module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2022, Geode-solutions
```

