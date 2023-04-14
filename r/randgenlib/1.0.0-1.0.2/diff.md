# Comparing `tmp/randgenlib-1.0.0.tar.gz` & `tmp/randgenlib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randgenlib-1.0.0.tar", last modified: Mon Apr 10 16:06:59 2023, max compression
+gzip compressed data, was "randgenlib-1.0.2.tar", last modified: Fri Apr 14 21:50:17 2023, max compression
```

## Comparing `randgenlib-1.0.0.tar` & `randgenlib-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 16:06:59.442845 randgenlib-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-10 16:06:59.442845 randgenlib-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 16:06:59.442845 randgenlib-1.0.0/randgenlib/
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-10 16:06:59.000000 randgenlib-1.0.0/randgenlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 16:06:59.442845 randgenlib-1.0.0/randgenlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-10 16:06:59.000000 randgenlib-1.0.0/randgenlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-10 16:06:59.000000 randgenlib-1.0.0/randgenlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 16:06:59.000000 randgenlib-1.0.0/randgenlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-10 16:06:59.000000 randgenlib-1.0.0/randgenlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-10 16:06:59.442845 randgenlib-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      568 2023-04-10 16:06:58.000000 randgenlib-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:50:17.749609 randgenlib-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-14 21:50:17.749609 randgenlib-1.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:50:17.749609 randgenlib-1.0.2/randgenlib/
+-rw-r--r--   0 root         (0) root         (0)    82161 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:50:17.749609 randgenlib-1.0.2/randgenlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 21:50:17.749609 randgenlib-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-04-14 21:50:16.000000 randgenlib-1.0.2/setup.py
```

### Comparing `randgenlib-1.0.0/setup.py` & `randgenlib-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Simple Hello World! Script."
-LONG_DESCRIPTION = "Simple Hello World! Script."
+VERSION = '1.0.2'
+DESCRIPTION = "Random generates strings."
+LONG_DESCRIPTION = "Random generates strings."
 
 # Setting up
 setup(
     name="randgenlib",
     version=VERSION,
-    author="TOS follower",
+    author="GigaAlex",
     author_email="nick.faltermeier@gmx.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
```

