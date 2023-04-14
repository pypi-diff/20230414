# Comparing `tmp/sbxpy-0.3.7.2.tar.gz` & `tmp/sbxpy-0.3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sbxpy-0.3.7.2.tar", last modified: Thu Feb  9 02:22:23 2023, max compression
+gzip compressed data, was "sbxpy-0.3.7.3.tar", last modified: Fri Apr 14 15:24:05 2023, max compression
```

## Comparing `sbxpy-0.3.7.2.tar` & `sbxpy-0.3.7.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-02-09 02:22:23.385305 sbxpy-0.3.7.2/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1061 2021-02-22 17:46:21.000000 sbxpy-0.3.7.2/LICENSE
--rw-rw-r--   0 luis      (1000) luis      (1000)      554 2023-02-09 02:22:23.385305 sbxpy-0.3.7.2/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)      338 2021-02-22 17:46:21.000000 sbxpy-0.3.7.2/README.md
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-02-09 02:22:23.385305 sbxpy-0.3.7.2/sbxpy/
--rw-rw-r--   0 luis      (1000) luis      (1000)     3460 2022-01-05 17:10:46.000000 sbxpy-0.3.7.2/sbxpy/QueryBuilder.py
--rw-rw-r--   0 luis      (1000) luis      (1000)    30408 2023-02-09 02:18:58.000000 sbxpy-0.3.7.2/sbxpy/__init__.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2023-02-09 02:22:23.385305 sbxpy-0.3.7.2/sbxpy.egg-info/
--rw-rw-r--   0 luis      (1000) luis      (1000)      554 2023-02-09 02:22:23.000000 sbxpy-0.3.7.2/sbxpy.egg-info/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)      210 2023-02-09 02:22:23.000000 sbxpy-0.3.7.2/sbxpy.egg-info/SOURCES.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        1 2023-02-09 02:22:23.000000 sbxpy-0.3.7.2/sbxpy.egg-info/dependency_links.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)       15 2023-02-09 02:22:23.000000 sbxpy-0.3.7.2/sbxpy.egg-info/requires.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        6 2023-02-09 02:22:23.000000 sbxpy-0.3.7.2/sbxpy.egg-info/top_level.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)       38 2023-02-09 02:22:23.385305 sbxpy-0.3.7.2/setup.cfg
--rw-rw-r--   0 luis      (1000) luis      (1000)      791 2023-02-09 02:19:40.000000 sbxpy-0.3.7.2/setup.py
+drwxr-xr-x   0 martinzuleta   (501) staff       (20)        0 2023-04-14 15:24:05.549284 sbxpy-0.3.7.3/
+-rw-r--r--   0 martinzuleta   (501) staff       (20)     1061 2023-04-14 14:56:05.000000 sbxpy-0.3.7.3/LICENSE
+-rw-r--r--   0 martinzuleta   (501) staff       (20)      529 2023-04-14 15:24:05.549063 sbxpy-0.3.7.3/PKG-INFO
+-rw-r--r--   0 martinzuleta   (501) staff       (20)      338 2023-04-14 14:56:05.000000 sbxpy-0.3.7.3/README.md
+drwxr-xr-x   0 martinzuleta   (501) staff       (20)        0 2023-04-14 15:24:05.547930 sbxpy-0.3.7.3/sbxpy/
+-rw-r--r--   0 martinzuleta   (501) staff       (20)     3460 2023-04-14 14:56:05.000000 sbxpy-0.3.7.3/sbxpy/QueryBuilder.py
+-rw-r--r--   0 martinzuleta   (501) staff       (20)    30408 2023-04-14 14:56:05.000000 sbxpy-0.3.7.3/sbxpy/__init__.py
+drwxr-xr-x   0 martinzuleta   (501) staff       (20)        0 2023-04-14 15:24:05.548848 sbxpy-0.3.7.3/sbxpy.egg-info/
+-rw-r--r--   0 martinzuleta   (501) staff       (20)      529 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/PKG-INFO
+-rw-r--r--   0 martinzuleta   (501) staff       (20)      210 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/SOURCES.txt
+-rw-r--r--   0 martinzuleta   (501) staff       (20)        1 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/dependency_links.txt
+-rw-r--r--   0 martinzuleta   (501) staff       (20)       15 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/requires.txt
+-rw-r--r--   0 martinzuleta   (501) staff       (20)        6 2023-04-14 15:24:05.000000 sbxpy-0.3.7.3/sbxpy.egg-info/top_level.txt
+-rw-r--r--   0 martinzuleta   (501) staff       (20)       38 2023-04-14 15:24:05.549324 sbxpy-0.3.7.3/setup.cfg
+-rw-r--r--   0 martinzuleta   (501) staff       (20)      791 2023-04-14 15:23:34.000000 sbxpy-0.3.7.3/setup.py
```

### Comparing `sbxpy-0.3.7.2/LICENSE` & `sbxpy-0.3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sbxpy-0.3.7.2/sbxpy/QueryBuilder.py` & `sbxpy-0.3.7.3/sbxpy/QueryBuilder.py`

 * *Files identical despite different names*

### Comparing `sbxpy-0.3.7.2/sbxpy/__init__.py` & `sbxpy-0.3.7.3/sbxpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sbxpy-0.3.7.2/setup.py` & `sbxpy-0.3.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sbxpy",
-    version="0.3.7.2",
+    version="0.3.7.3",
     author="Luis Guzmán",
     author_email="lgguzman890414@gmail.com",
     description="This is the module  create all request used to communicate with SbxCloud",
     long_description="This is the module  create all request used to communicate with SbxCloud",
     long_description_content_type="text/markdown",
     url="https://github.com/sbxcloud/sbxcloudpython",
     packages=setuptools.find_packages(),
```

