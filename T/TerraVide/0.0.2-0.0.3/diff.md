# Comparing `tmp/TerraVide-0.0.2.tar.gz` & `tmp/TerraVide-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TerraVide-0.0.2.tar", last modified: Thu Apr 13 22:44:38 2023, max compression
+gzip compressed data, was "dist/TerraVide-0.0.3.tar", last modified: Thu Apr 13 23:30:36 2023, max compression
```

## Comparing `TerraVide-0.0.2.tar` & `TerraVide-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,16 @@
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 22:44:38.823810 TerraVide-0.0.2/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.0.2/LICENSE.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1152 2023-04-13 22:44:38.823618 TerraVide-0.0.2/PKG-INFO
-drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 22:44:38.823378 TerraVide-0.0.2/TerraVide.egg-info/
--rw-r--r--   0 sarangpramode   (501) staff       (20)     1152 2023-04-13 22:44:38.000000 TerraVide-0.0.2/TerraVide.egg-info/PKG-INFO
--rw-r--r--   0 sarangpramode   (501) staff       (20)      152 2023-04-13 22:44:38.000000 TerraVide-0.0.2/TerraVide.egg-info/SOURCES.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-13 22:44:38.000000 TerraVide-0.0.2/TerraVide.egg-info/dependency_links.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)        5 2023-04-13 22:44:38.000000 TerraVide-0.0.2/TerraVide.egg-info/top_level.txt
--rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-13 22:44:38.823855 TerraVide-0.0.2/setup.cfg
--rw-r--r--   0 sarangpramode   (501) staff       (20)     2547 2023-04-13 22:43:57.000000 TerraVide-0.0.2/setup.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:30:36.000000 TerraVide-0.0.3/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1305 2023-04-13 23:30:36.000000 TerraVide-0.0.3/PKG-INFO
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:30:36.000000 TerraVide-0.0.3/terravide/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:14:29.000000 TerraVide-0.0.3/terravide/__init__.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:30:36.000000 TerraVide-0.0.3/terravide/src/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        0 2023-04-13 20:29:35.000000 TerraVide-0.0.3/terravide/src/__init__.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     4188 2023-04-13 23:30:19.000000 TerraVide-0.0.3/terravide/src/dataset.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1823 2023-04-13 21:59:13.000000 TerraVide-0.0.3/terravide/src/info.py
+drwxr-xr-x   0 sarangpramode   (501) staff       (20)        0 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1305 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/PKG-INFO
+-rw-r--r--   0 sarangpramode   (501) staff       (20)      247 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/SOURCES.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       15 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/top_level.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)        1 2023-04-13 23:30:36.000000 TerraVide-0.0.3/TerraVide.egg-info/dependency_links.txt
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     2547 2023-04-13 23:30:31.000000 TerraVide-0.0.3/setup.py
+-rw-r--r--   0 sarangpramode   (501) staff       (20)       38 2023-04-13 23:30:36.000000 TerraVide-0.0.3/setup.cfg
+-rw-r--r--   0 sarangpramode   (501) staff       (20)     1079 2023-04-13 21:41:11.000000 TerraVide-0.0.3/LICENSE.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `TerraVide-0.0.2/LICENSE.txt` & `TerraVide-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TerraVide-0.0.2/PKG-INFO` & `TerraVide-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: TerraVide
-Version: 0.0.2
+Version: 0.0.3
 Summary: An open source python package to process and simulate large urban environments mapped with LiDAR data
+Home-page: UNKNOWN
 Author: Sarang Pramode
+License: UNKNOWN
+Description: # TerraVide
+        
+        TerraVide is an open source python package to process large urban environments mapped with LiDAR(Light Detection and Ranging) data.
+        
+        It offers the ability to enrich raw lidar data and extract individual tree canopies from raw point clouds. Additionally it offers a suite of modules to simulate and analyze the classified enviroment and quantify shade impacts through interactive visualiztions
+        
+        TerraVide aims to facilitate large-scale forest management and make more robust and generic tree extraction methods with equitable tree planting decisions. The package is designed to be scalable and can handle large datasets with minimal computational overhead.
+        
+        # License
+        
+        TerraVide is released under the MIT license.
+        
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# TerraVide
-
-TerraVide is an open source python package to process large urban environments mapped with LiDAR(Light Detection and Ranging) data.
-
-It offers the ability to enrich raw lidar data and extract individual tree canopies from raw point clouds. Additionally it offers a suite of modules to simulate and analyze the classified enviroment and quantify shade impacts through interactive visualiztions
-
-TerraVide aims to facilitate large-scale forest management and make more robust and generic tree extraction methods with equitable tree planting decisions. The package is designed to be scalable and can handle large datasets with minimal computational overhead.
-
-# License
-
-TerraVide is released under the MIT license.
-
-
-
```

### Comparing `TerraVide-0.0.2/TerraVide.egg-info/PKG-INFO` & `TerraVide-0.0.3/TerraVide.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: TerraVide
-Version: 0.0.2
+Version: 0.0.3
 Summary: An open source python package to process and simulate large urban environments mapped with LiDAR data
+Home-page: UNKNOWN
 Author: Sarang Pramode
+License: UNKNOWN
+Description: # TerraVide
+        
+        TerraVide is an open source python package to process large urban environments mapped with LiDAR(Light Detection and Ranging) data.
+        
+        It offers the ability to enrich raw lidar data and extract individual tree canopies from raw point clouds. Additionally it offers a suite of modules to simulate and analyze the classified enviroment and quantify shade impacts through interactive visualiztions
+        
+        TerraVide aims to facilitate large-scale forest management and make more robust and generic tree extraction methods with equitable tree planting decisions. The package is designed to be scalable and can handle large datasets with minimal computational overhead.
+        
+        # License
+        
+        TerraVide is released under the MIT license.
+        
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# TerraVide
-
-TerraVide is an open source python package to process large urban environments mapped with LiDAR(Light Detection and Ranging) data.
-
-It offers the ability to enrich raw lidar data and extract individual tree canopies from raw point clouds. Additionally it offers a suite of modules to simulate and analyze the classified enviroment and quantify shade impacts through interactive visualiztions
-
-TerraVide aims to facilitate large-scale forest management and make more robust and generic tree extraction methods with equitable tree planting decisions. The package is designed to be scalable and can handle large datasets with minimal computational overhead.
-
-# License
-
-TerraVide is released under the MIT license.
-
-
-
```

### Comparing `TerraVide-0.0.2/setup.py` & `TerraVide-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TerraVide",                     # This is the name of the package
-    version="0.0.2",                        #release version
+    version="0.0.3",                        #release version
     author="Sarang Pramode",                     # Full name of the author
     description="An open source python package to process and simulate large urban environments mapped with LiDAR data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

