# Comparing `tmp/joonmyung-1.4.1.tar.gz` & `tmp/joonmyung-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/joonmyung-1.4.1.tar", last modified: Thu Apr  6 18:28:15 2023, max compression
+gzip compressed data, was "dist/joonmyung-1.4.2.tar", last modified: Fri Apr 14 13:09:58 2023, max compression
```

## Comparing `joonmyung-1.4.1.tar` & `joonmyung-1.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-06 18:28:15.000000 joonmyung-1.4.1/
--rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-04-06 18:28:15.000000 joonmyung-1.4.1/PKG-INFO
--rw-r--r--   0 joonmyung   (501) staff       (20)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.1/README.md
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-06 18:28:15.000000 joonmyung-1.4.1/joonmyung/
--rw-r--r--   0 joonmyung   (501) staff       (20)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.1/joonmyung/__init__.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.1/joonmyung/app.py
--rw-r--r--   0 joonmyung   (501) staff       (20)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.1/joonmyung/data.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    13286 2023-03-06 13:16:50.000000 joonmyung-1.4.1/joonmyung/draw.py
--rw-r--r--   0 joonmyung   (501) staff       (20)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.1/joonmyung/dummy.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.1/joonmyung/file.py
--rw-r--r--   0 joonmyung   (501) staff       (20)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.1/joonmyung/gradcam.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     5375 2023-04-06 18:13:55.000000 joonmyung-1.4.1/joonmyung/log.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-06 18:28:15.000000 joonmyung-1.4.1/joonmyung/meta_data/
--rw-r--r--   0 joonmyung   (501) staff       (20)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.1/joonmyung/meta_data/__init__.py
--rw-r--r--   0 joonmyung   (501) staff       (20)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.1/joonmyung/meta_data/label.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     2277 2023-03-01 06:32:47.000000 joonmyung-1.4.1/joonmyung/meta_data/utils.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     6030 2023-03-04 10:44:55.000000 joonmyung-1.4.1/joonmyung/metric.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     3214 2023-03-30 15:51:49.000000 joonmyung-1.4.1/joonmyung/script.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.1/joonmyung/status.py
--rw-r--r--   0 joonmyung   (501) staff       (20)     3949 2023-04-06 17:51:01.000000 joonmyung-1.4.1/joonmyung/utils.py
-drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-06 18:28:15.000000 joonmyung-1.4.1/joonmyung.egg-info/
--rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-04-06 18:28:14.000000 joonmyung-1.4.1/joonmyung.egg-info/PKG-INFO
--rw-r--r--   0 joonmyung   (501) staff       (20)      501 2023-04-06 18:28:14.000000 joonmyung-1.4.1/joonmyung.egg-info/SOURCES.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-04-06 18:28:14.000000 joonmyung-1.4.1/joonmyung.egg-info/dependency_links.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-03-08 20:12:53.000000 joonmyung-1.4.1/joonmyung.egg-info/not-zip-safe
--rw-r--r--   0 joonmyung   (501) staff       (20)       10 2023-04-06 18:28:14.000000 joonmyung-1.4.1/joonmyung.egg-info/top_level.txt
--rw-r--r--   0 joonmyung   (501) staff       (20)       38 2023-04-06 18:28:15.000000 joonmyung-1.4.1/setup.cfg
--rw-r--r--   0 joonmyung   (501) staff       (20)      781 2023-04-06 18:14:56.000000 joonmyung-1.4.1/setup.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-14 13:09:58.000000 joonmyung-1.4.2/
+-rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-04-14 13:09:58.000000 joonmyung-1.4.2/PKG-INFO
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1138 2023-04-06 18:15:10.000000 joonmyung-1.4.2/README.md
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-14 13:09:58.000000 joonmyung-1.4.2/joonmyung/
+-rw-r--r--   0 joonmyung   (501) staff       (20)       15 2023-02-22 17:22:56.000000 joonmyung-1.4.2/joonmyung/__init__.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     6700 2023-04-03 12:26:27.000000 joonmyung-1.4.2/joonmyung/app.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)      695 2023-02-24 17:07:52.000000 joonmyung-1.4.2/joonmyung/data.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)    13219 2023-04-14 13:09:54.000000 joonmyung-1.4.2/joonmyung/draw.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)       29 2023-04-03 12:26:27.000000 joonmyung-1.4.2/joonmyung/dummy.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     2755 2023-02-22 17:22:56.000000 joonmyung-1.4.2/joonmyung/file.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)      920 2023-02-22 17:22:56.000000 joonmyung-1.4.2/joonmyung/gradcam.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     5375 2023-04-06 18:13:55.000000 joonmyung-1.4.2/joonmyung/log.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-14 13:09:58.000000 joonmyung-1.4.2/joonmyung/meta_data/
+-rw-r--r--   0 joonmyung   (501) staff       (20)       41 2023-03-01 06:51:46.000000 joonmyung-1.4.2/joonmyung/meta_data/__init__.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)    45491 2023-02-22 17:22:56.000000 joonmyung-1.4.2/joonmyung/meta_data/label.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     2277 2023-03-01 06:32:47.000000 joonmyung-1.4.2/joonmyung/meta_data/utils.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     6030 2023-03-04 10:44:55.000000 joonmyung-1.4.2/joonmyung/metric.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     3214 2023-03-30 15:51:49.000000 joonmyung-1.4.2/joonmyung/script.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     1487 2023-03-01 13:25:20.000000 joonmyung-1.4.2/joonmyung/status.py
+-rw-r--r--   0 joonmyung   (501) staff       (20)     3949 2023-04-06 17:51:01.000000 joonmyung-1.4.2/joonmyung/utils.py
+drwxr-xr-x   0 joonmyung   (501) staff       (20)        0 2023-04-14 13:09:58.000000 joonmyung-1.4.2/joonmyung.egg-info/
+-rw-r--r--   0 joonmyung   (501) staff       (20)      241 2023-04-14 13:09:58.000000 joonmyung-1.4.2/joonmyung.egg-info/PKG-INFO
+-rw-r--r--   0 joonmyung   (501) staff       (20)      501 2023-04-14 13:09:58.000000 joonmyung-1.4.2/joonmyung.egg-info/SOURCES.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-04-14 13:09:58.000000 joonmyung-1.4.2/joonmyung.egg-info/dependency_links.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)        1 2023-03-08 20:12:53.000000 joonmyung-1.4.2/joonmyung.egg-info/not-zip-safe
+-rw-r--r--   0 joonmyung   (501) staff       (20)       10 2023-04-14 13:09:58.000000 joonmyung-1.4.2/joonmyung.egg-info/top_level.txt
+-rw-r--r--   0 joonmyung   (501) staff       (20)       38 2023-04-14 13:09:58.000000 joonmyung-1.4.2/setup.cfg
+-rw-r--r--   0 joonmyung   (501) staff       (20)      781 2023-04-14 13:09:54.000000 joonmyung-1.4.2/setup.py
```

### Comparing `joonmyung-1.4.1/README.md` & `joonmyung-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/app.py` & `joonmyung-1.4.2/joonmyung/app.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/data.py` & `joonmyung-1.4.2/joonmyung/data.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/draw.py` & `joonmyung-1.4.2/joonmyung/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,16 +164,14 @@
         attentions = attentions.mean(axis=2) #
     elif head_fusion == "max":
         attentions = attentions.max(axis=2)[0]
     elif head_fusion == "min":
         attentions = attentions.min(axis=2)[0]
     elif head_fusion == "median":
         attentions = attentions.median(axis=2)[0]
-    else:
-        raise "Attention head fusion type Not supported"
 
     if bs is not None:
         attentions = attentions[:, bs]
 
     _, B, _, T = attentions.shape
     H = W = int(T ** 0.5)
     if starts is not None:
```

### Comparing `joonmyung-1.4.1/joonmyung/file.py` & `joonmyung-1.4.2/joonmyung/file.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/gradcam.py` & `joonmyung-1.4.2/joonmyung/gradcam.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/log.py` & `joonmyung-1.4.2/joonmyung/log.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/meta_data/label.py` & `joonmyung-1.4.2/joonmyung/meta_data/label.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/meta_data/utils.py` & `joonmyung-1.4.2/joonmyung/meta_data/utils.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/metric.py` & `joonmyung-1.4.2/joonmyung/metric.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/script.py` & `joonmyung-1.4.2/joonmyung/script.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/status.py` & `joonmyung-1.4.2/joonmyung/status.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/joonmyung/utils.py` & `joonmyung-1.4.2/joonmyung/utils.py`

 * *Files identical despite different names*

### Comparing `joonmyung-1.4.1/setup.py` & `joonmyung-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import find_packages
 setuptools.setup(
     name="joonmyung",
-    version="1.4.1",
+    version="1.4.2",
     author="JoonMyung Choi",
     author_email="pizard@korea.ac.kr",
     description="JoonMyung's Library",
     url="https://github.com/pizard/JoonMyung.git",
     license="MIT",
     packages=find_packages(exclude=["playground",
                                     "playground.*",
```

