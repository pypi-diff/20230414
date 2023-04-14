# Comparing `tmp/Tom Toolbox-0.0.1.tar.gz` & `tmp/Tom-Toolbox-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tom Toolbox-0.0.1.tar", last modified: Tue Apr 11 20:05:36 2023, max compression
+gzip compressed data, was "Tom-Toolbox-0.0.1.post1.tar", last modified: Fri Apr 14 08:03:49 2023, max compression
```

## Comparing `Tom Toolbox-0.0.1.tar` & `Tom-Toolbox-0.0.1.post1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-11 20:05:36.762020 Tom Toolbox-0.0.1/
--rw-r--r--   0 angel     (1000) users      (984)      420 2023-04-11 20:05:36.762020 Tom Toolbox-0.0.1/PKG-INFO
--rw-r--r--   0 angel     (1000) users      (984)       51 2023-04-11 20:03:25.000000 Tom Toolbox-0.0.1/README.md
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-11 20:05:36.762020 Tom Toolbox-0.0.1/Tom_Toolbox.egg-info/
--rw-r--r--   0 angel     (1000) users      (984)      420 2023-04-11 20:05:36.000000 Tom Toolbox-0.0.1/Tom_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 angel     (1000) users      (984)      236 2023-04-11 20:05:36.000000 Tom Toolbox-0.0.1/Tom_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 angel     (1000) users      (984)        1 2023-04-11 20:05:36.000000 Tom Toolbox-0.0.1/Tom_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 angel     (1000) users      (984)        8 2023-04-11 20:05:36.000000 Tom Toolbox-0.0.1/Tom_Toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-11 20:05:36.762020 Tom Toolbox-0.0.1/Toolbox/
--rw-r--r--   0 angel     (1000) users      (984)        0 2023-04-11 19:44:44.000000 Tom Toolbox-0.0.1/Toolbox/__init__.py
--rw-r--r--   0 angel     (1000) users      (984)     1531 2023-04-11 05:03:34.000000 Tom Toolbox-0.0.1/Toolbox/ansi_colors.py
--rw-r--r--   0 angel     (1000) users      (984)     8186 2023-04-11 19:47:55.000000 Tom Toolbox-0.0.1/Toolbox/pacman.py
--rw-r--r--   0 angel     (1000) users      (984)     1380 2023-04-11 19:16:56.000000 Tom Toolbox-0.0.1/Toolbox/tools.py
--rw-r--r--   0 angel     (1000) users      (984)       38 2023-04-11 20:05:36.762020 Tom Toolbox-0.0.1/setup.cfg
--rw-r--r--   0 angel     (1000) users      (984)      626 2023-04-11 20:05:21.000000 Tom Toolbox-0.0.1/setup.py
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:03:49.807345 Tom-Toolbox-0.0.1.post1/
+-rw-r--r--   0 angel     (1000) users      (984)      599 2023-04-14 08:03:49.807345 Tom-Toolbox-0.0.1.post1/PKG-INFO
+-rw-r--r--   0 angel     (1000) users      (984)      225 2023-04-14 07:51:15.000000 Tom-Toolbox-0.0.1.post1/README.md
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:03:49.805344 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/
+-rw-r--r--   0 angel     (1000) users      (984)      599 2023-04-14 08:03:49.000000 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 angel     (1000) users      (984)      246 2023-04-14 08:03:49.000000 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 angel     (1000) users      (984)        1 2023-04-14 08:03:49.000000 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 angel     (1000) users      (984)        8 2023-04-14 08:03:49.000000 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:03:49.807345 Tom-Toolbox-0.0.1.post1/Toolbox/
+-rw-r--r--   0 angel     (1000) users      (984)        0 2023-04-11 19:44:44.000000 Tom-Toolbox-0.0.1.post1/Toolbox/__init__.py
+-rw-r--r--   0 angel     (1000) users      (984)     1531 2023-04-11 05:03:34.000000 Tom-Toolbox-0.0.1.post1/Toolbox/ansi_colors.py
+-rw-r--r--   0 angel     (1000) users      (984)     8186 2023-04-11 19:47:55.000000 Tom-Toolbox-0.0.1.post1/Toolbox/pacman.py
+-rw-r--r--   0 angel     (1000) users      (984)     1380 2023-04-11 19:16:56.000000 Tom-Toolbox-0.0.1.post1/Toolbox/tools.py
+-rw-r--r--   0 angel     (1000) users      (984)      138 2023-04-14 08:03:49.807345 Tom-Toolbox-0.0.1.post1/setup.cfg
+-rw-r--r--   0 angel     (1000) users      (984)      568 2023-04-14 07:56:58.000000 Tom-Toolbox-0.0.1.post1/setup.py
```

### Comparing `Tom Toolbox-0.0.1/Toolbox/ansi_colors.py` & `Tom-Toolbox-0.0.1.post1/Toolbox/ansi_colors.py`

 * *Files identical despite different names*

### Comparing `Tom Toolbox-0.0.1/Toolbox/pacman.py` & `Tom-Toolbox-0.0.1.post1/Toolbox/pacman.py`

 * *Files identical despite different names*

### Comparing `Tom Toolbox-0.0.1/Toolbox/tools.py` & `Tom-Toolbox-0.0.1.post1/Toolbox/tools.py`

 * *Files identical despite different names*

### Comparing `Tom Toolbox-0.0.1/setup.py` & `Tom-Toolbox-0.0.1.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import setuptools
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
 setuptools.setup(
-    name="Tom Toolbox",
-    version="0.0.1",
+    name="Tom-Toolbox",
+    version="0.0.1-1",
     author="Tom5521",
     description="A collection of utilities for python 3.10 and above",
-    long_description=long_description,
+    long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Tom5521/Toolbox",
     packages=setuptools.find_packages(exclude=["test.py", ".gitignore"]),
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-)
+)
```

