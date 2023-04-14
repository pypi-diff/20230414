# Comparing `tmp/margsoft-0.0.8.tar.gz` & `tmp/margsoft-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "margsoft-0.0.8.tar", last modified: Mon Dec 19 10:55:23 2022, max compression
+gzip compressed data, was "margsoft-0.0.9.tar", last modified: Mon Dec 19 11:49:56 2022, max compression
```

## Comparing `margsoft-0.0.8.tar` & `margsoft-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 10:55:23.806654 margsoft-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-19 10:55:02.000000 margsoft-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      744 2022-12-19 10:55:23.806654 margsoft-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-19 10:55:02.000000 margsoft-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-19 10:55:02.000000 margsoft-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 10:55:23.806654 margsoft-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2022-12-19 10:55:02.000000 margsoft-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 10:55:23.802654 margsoft-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 10:55:23.802654 margsoft-0.0.8/src/margsoft/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 10:55:02.000000 margsoft-0.0.8/src/margsoft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2022-12-19 10:55:02.000000 margsoft-0.0.8/src/margsoft/mineral.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 10:55:23.802654 margsoft-0.0.8/src/margsoft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2022-12-19 10:55:23.000000 margsoft-0.0.8/src/margsoft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-19 10:55:23.000000 margsoft-0.0.8/src/margsoft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 10:55:23.000000 margsoft-0.0.8/src/margsoft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-19 10:55:23.000000 margsoft-0.0.8/src/margsoft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-19 10:55:23.000000 margsoft-0.0.8/src/margsoft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 11:49:56.546992 margsoft-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-19 11:49:37.000000 margsoft-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2022-12-19 11:49:56.546992 margsoft-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-19 11:49:37.000000 margsoft-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-19 11:49:37.000000 margsoft-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 11:49:56.546992 margsoft-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2022-12-19 11:49:37.000000 margsoft-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 11:49:56.542992 margsoft-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 11:49:56.542992 margsoft-0.0.9/src/margsoft/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 11:49:37.000000 margsoft-0.0.9/src/margsoft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2022-12-19 11:49:37.000000 margsoft-0.0.9/src/margsoft/mineral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 11:49:56.546992 margsoft-0.0.9/src/margsoft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2022-12-19 11:49:56.000000 margsoft-0.0.9/src/margsoft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2022-12-19 11:49:56.000000 margsoft-0.0.9/src/margsoft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 11:49:56.000000 margsoft-0.0.9/src/margsoft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-19 11:49:56.000000 margsoft-0.0.9/src/margsoft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-19 11:49:56.000000 margsoft-0.0.9/src/margsoft.egg-info/top_level.txt
```

### Comparing `margsoft-0.0.8/LICENSE` & `margsoft-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `margsoft-0.0.8/PKG-INFO` & `margsoft-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margsoft
-Version: 0.0.8
+Version: 0.0.9
 Summary: data collection package
 Home-page: https://github.com/Codebugged-Research/datacollection
 Author: Codebugged-Research
 Author-email: thecodebugged@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `margsoft-0.0.8/setup.py` & `margsoft-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 REPO_NAME = "datacollection"
 AUTHOR_USER_NAME = "Codebugged-Research"
 SRC_REPO = "src"
 
 
 setuptools.setup(
     name="margsoft",
-    version="0.0.8",
+    version="0.0.9",
     author=AUTHOR_USER_NAME,
     description="data collection package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     author_email="thecodebugged@gmail.com",
     package_dir={'': "src"},
```

### Comparing `margsoft-0.0.8/src/margsoft/mineral.py` & `margsoft-0.0.9/src/margsoft/mineral.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import cv2
 import time
 import numpy as np
 import os
 import pathlib
 from datetime import datetime
 import sys
-CONFIDENCE_THRESHOLD = 0.25
+CONFIDENCE_THRESHOLD = 0.7
 NMS_THRESHOLD = 0.1
 def collectdataset(rtsp,names_file,weight_file,cfg_file,path,dir_n):
     print("inside the function")
     cap = cv2.VideoCapture(rtsp, cv2.CAP_FFMPEG)
     prevTime = 0
     # width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
     # height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
-    cv2.namedWindow("output", cv2.WINDOW_NORMAL)    
+    #cv2.namedWindow("output", cv2.WINDOW_NORMAL)    
     class_names = []
     with open(names_file, "r") as f:
         class_names = [cname.strip() for cname in f.readlines()]
 
         
     # frame_width = int(cap.get(3))
     # frame_height = int(cap.get(4))
@@ -31,15 +31,16 @@
     try:
         while cap.isOpened(): 
             ret, frame = cap.read()
             frame=cv2.resize(frame, (720, 720))
             frame = np.array(frame)
             classes, scores, boxes = model.detect(frame, CONFIDENCE_THRESHOLD, NMS_THRESHOLD)
             for (classid, score, box) in zip(classes, scores, boxes):
-                if(class_names[classid]!="other"):
+                if(class_names[classid] not in ["other"]):
+                    print(class_names[classid],score)
                     print("found!!!")
                     curr_datetime = datetime.utcnow().strftime('%Y%m%d%H%M%S%f')
                     f_name = path+dir_n+"/"+str(curr_datetime)+".jpg"
                     cv2.imwrite(f_name, frame)
                     print(f_name)
     except KeyboardInterrupt:
         print("Bye")
```

### Comparing `margsoft-0.0.8/src/margsoft.egg-info/PKG-INFO` & `margsoft-0.0.9/src/margsoft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: margsoft
-Version: 0.0.8
+Version: 0.0.9
 Summary: data collection package
 Home-page: https://github.com/Codebugged-Research/datacollection
 Author: Codebugged-Research
 Author-email: thecodebugged@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

