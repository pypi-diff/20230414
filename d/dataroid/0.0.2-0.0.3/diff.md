# Comparing `tmp/dataroid-0.0.2.tar.gz` & `tmp/dataroid-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataroid-0.0.2.tar", last modified: Wed Apr 12 14:09:08 2023, max compression
+gzip compressed data, was "dataroid-0.0.3.tar", last modified: Fri Apr 14 09:07:06 2023, max compression
```

## Comparing `dataroid-0.0.2.tar` & `dataroid-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 14:09:08.263484 dataroid-0.0.2/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      581 2023-04-12 14:09:08.263484 dataroid-0.0.2/PKG-INFO
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 14:09:08.263484 dataroid-0.0.2/dataroid/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 14:03:59.000000 dataroid-0.0.2/dataroid/__init__.py
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1172 2023-04-12 13:02:55.000000 dataroid-0.0.2/dataroid/dataroid.py
-drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-12 14:09:08.263484 dataroid-0.0.2/dataroid.egg-info/
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      581 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/PKG-INFO
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      209 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/SOURCES.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        1 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/dependency_links.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       27 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/requires.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        9 2023-04-12 14:09:08.000000 dataroid-0.0.2/dataroid.egg-info/top_level.txt
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       38 2023-04-12 14:09:08.263484 dataroid-0.0.2/setup.cfg
--rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      791 2023-04-12 14:08:48.000000 dataroid-0.0.2/setup.py
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:07:06.803331 dataroid-0.0.3/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1832 2023-04-14 09:07:06.803331 dataroid-0.0.3/PKG-INFO
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:07:06.803331 dataroid-0.0.3/dataroid/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       22 2023-04-14 08:04:09.000000 dataroid-0.0.3/dataroid/__init__.py
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1167 2023-04-14 08:14:28.000000 dataroid-0.0.3/dataroid/dataroid.py
+drwxrwxr-x   0 burakegeli  (1000) burakegeli  (1000)        0 2023-04-14 09:07:06.803331 dataroid-0.0.3/dataroid.egg-info/
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)     1832 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/PKG-INFO
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      209 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/SOURCES.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        1 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/dependency_links.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       27 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/requires.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)        9 2023-04-14 09:07:06.000000 dataroid-0.0.3/dataroid.egg-info/top_level.txt
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)       38 2023-04-14 09:07:06.803331 dataroid-0.0.3/setup.cfg
+-rw-rw-r--   0 burakegeli  (1000) burakegeli  (1000)      994 2023-04-14 09:07:02.000000 dataroid-0.0.3/setup.py
```

### Comparing `dataroid-0.0.2/dataroid/dataroid.py` & `dataroid-0.0.3/dataroid/dataroid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 # In[1]:
 
 
-class Dataroid:    
+class Bot:    
     def __init__(self,data,sampling=False,**kwargs):
         '''
         Fit's a model by automaticaly identifying discrete and continuous columns.
         
         # Parameters:
         #     data (DataFrame):The data which will be used for training.
         #     sampling (Boolean):Sampling 1000 data points randomly.
```

