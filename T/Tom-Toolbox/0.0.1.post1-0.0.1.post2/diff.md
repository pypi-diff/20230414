# Comparing `tmp/Tom-Toolbox-0.0.1.post1.tar.gz` & `tmp/Tom-Toolbox-0.0.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tom-Toolbox-0.0.1.post1.tar", last modified: Fri Apr 14 08:03:49 2023, max compression
+gzip compressed data, was "Tom-Toolbox-0.0.1.post2.tar", last modified: Fri Apr 14 08:52:18 2023, max compression
```

## Comparing `Tom-Toolbox-0.0.1.post1.tar` & `Tom-Toolbox-0.0.1.post2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:03:49.807345 Tom-Toolbox-0.0.1.post1/
--rw-r--r--   0 angel     (1000) users      (984)      599 2023-04-14 08:03:49.807345 Tom-Toolbox-0.0.1.post1/PKG-INFO
--rw-r--r--   0 angel     (1000) users      (984)      225 2023-04-14 07:51:15.000000 Tom-Toolbox-0.0.1.post1/README.md
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:03:49.805344 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/
--rw-r--r--   0 angel     (1000) users      (984)      599 2023-04-14 08:03:49.000000 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/PKG-INFO
--rw-r--r--   0 angel     (1000) users      (984)      246 2023-04-14 08:03:49.000000 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 angel     (1000) users      (984)        1 2023-04-14 08:03:49.000000 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 angel     (1000) users      (984)        8 2023-04-14 08:03:49.000000 Tom-Toolbox-0.0.1.post1/Tom_Toolbox.egg-info/top_level.txt
-drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:03:49.807345 Tom-Toolbox-0.0.1.post1/Toolbox/
--rw-r--r--   0 angel     (1000) users      (984)        0 2023-04-11 19:44:44.000000 Tom-Toolbox-0.0.1.post1/Toolbox/__init__.py
--rw-r--r--   0 angel     (1000) users      (984)     1531 2023-04-11 05:03:34.000000 Tom-Toolbox-0.0.1.post1/Toolbox/ansi_colors.py
--rw-r--r--   0 angel     (1000) users      (984)     8186 2023-04-11 19:47:55.000000 Tom-Toolbox-0.0.1.post1/Toolbox/pacman.py
--rw-r--r--   0 angel     (1000) users      (984)     1380 2023-04-11 19:16:56.000000 Tom-Toolbox-0.0.1.post1/Toolbox/tools.py
--rw-r--r--   0 angel     (1000) users      (984)      138 2023-04-14 08:03:49.807345 Tom-Toolbox-0.0.1.post1/setup.cfg
--rw-r--r--   0 angel     (1000) users      (984)      568 2023-04-14 07:56:58.000000 Tom-Toolbox-0.0.1.post1/setup.py
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:52:18.235666 Tom-Toolbox-0.0.1.post2/
+-rw-r--r--   0 angel     (1000) users      (984)     6378 2023-04-14 08:52:18.235666 Tom-Toolbox-0.0.1.post2/PKG-INFO
+-rw-r--r--   0 angel     (1000) users      (984)     6003 2023-04-14 08:48:31.000000 Tom-Toolbox-0.0.1.post2/README.md
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:52:18.233666 Tom-Toolbox-0.0.1.post2/Tom_Toolbox.egg-info/
+-rw-r--r--   0 angel     (1000) users      (984)     6378 2023-04-14 08:52:18.000000 Tom-Toolbox-0.0.1.post2/Tom_Toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 angel     (1000) users      (984)      246 2023-04-14 08:52:18.000000 Tom-Toolbox-0.0.1.post2/Tom_Toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 angel     (1000) users      (984)        1 2023-04-14 08:52:18.000000 Tom-Toolbox-0.0.1.post2/Tom_Toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 angel     (1000) users      (984)        8 2023-04-14 08:52:18.000000 Tom-Toolbox-0.0.1.post2/Tom_Toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 angel     (1000) users      (984)        0 2023-04-14 08:52:18.235666 Tom-Toolbox-0.0.1.post2/Toolbox/
+-rw-r--r--   0 angel     (1000) users      (984)        0 2023-04-11 19:44:44.000000 Tom-Toolbox-0.0.1.post2/Toolbox/__init__.py
+-rw-r--r--   0 angel     (1000) users      (984)     1531 2023-04-14 08:23:58.000000 Tom-Toolbox-0.0.1.post2/Toolbox/ansi_colors.py
+-rw-r--r--   0 angel     (1000) users      (984)     8186 2023-04-11 19:47:55.000000 Tom-Toolbox-0.0.1.post2/Toolbox/pacman.py
+-rw-r--r--   0 angel     (1000) users      (984)     1380 2023-04-11 19:16:56.000000 Tom-Toolbox-0.0.1.post2/Toolbox/tools.py
+-rw-r--r--   0 angel     (1000) users      (984)      138 2023-04-14 08:52:18.235666 Tom-Toolbox-0.0.1.post2/setup.cfg
+-rw-r--r--   0 angel     (1000) users      (984)      568 2023-04-14 08:51:29.000000 Tom-Toolbox-0.0.1.post2/setup.py
```

### Comparing `Tom-Toolbox-0.0.1.post1/Toolbox/ansi_colors.py` & `Tom-Toolbox-0.0.1.post2/Toolbox/ansi_colors.py`

 * *Files identical despite different names*

### Comparing `Tom-Toolbox-0.0.1.post1/Toolbox/pacman.py` & `Tom-Toolbox-0.0.1.post2/Toolbox/pacman.py`

 * *Files identical despite different names*

### Comparing `Tom-Toolbox-0.0.1.post1/Toolbox/tools.py` & `Tom-Toolbox-0.0.1.post2/Toolbox/tools.py`

 * *Files identical despite different names*

### Comparing `Tom-Toolbox-0.0.1.post1/setup.py` & `Tom-Toolbox-0.0.1.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(
     name="Tom-Toolbox",
-    version="0.0.1-1",
+    version="0.0.1-2",
     author="Tom5521",
     description="A collection of utilities for python 3.10 and above",
-    long_description=open('README.md').read(),
+    long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Tom5521/Toolbox",
     packages=setuptools.find_packages(exclude=["test.py", ".gitignore"]),
     classifiers=[
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

