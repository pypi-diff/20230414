# Comparing `tmp/cryptographylibs-1.0.0.tar.gz` & `tmp/cryptographylibs-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographylibs-1.0.0.tar", last modified: Wed Apr 12 20:25:58 2023, max compression
+gzip compressed data, was "cryptographylibs-2.0.0.tar", last modified: Fri Apr 14 17:37:03 2023, max compression
```

## Comparing `cryptographylibs-1.0.0.tar` & `cryptographylibs-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:25:58.881766 cryptographylibs-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-12 20:25:58.881766 cryptographylibs-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:25:58.881766 cryptographylibs-1.0.0/cryptographylibs/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 20:25:58.000000 cryptographylibs-1.0.0/cryptographylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:25:58.881766 cryptographylibs-1.0.0/cryptographylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-12 20:25:58.000000 cryptographylibs-1.0.0/cryptographylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-12 20:25:58.000000 cryptographylibs-1.0.0/cryptographylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:25:58.000000 cryptographylibs-1.0.0/cryptographylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-12 20:25:58.000000 cryptographylibs-1.0.0/cryptographylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 20:25:58.881766 cryptographylibs-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      537 2023-04-12 20:25:57.000000 cryptographylibs-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:37:03.111402 cryptographylibs-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      453 2023-04-14 17:37:03.111402 cryptographylibs-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:37:03.111402 cryptographylibs-2.0.0/cryptographylibs/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-14 17:37:02.000000 cryptographylibs-2.0.0/cryptographylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 17:37:03.111402 cryptographylibs-2.0.0/cryptographylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      453 2023-04-14 17:37:03.000000 cryptographylibs-2.0.0/cryptographylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-14 17:37:03.000000 cryptographylibs-2.0.0/cryptographylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 17:37:03.000000 cryptographylibs-2.0.0/cryptographylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-14 17:37:03.000000 cryptographylibs-2.0.0/cryptographylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 17:37:03.111402 cryptographylibs-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      666 2023-04-14 17:37:01.000000 cryptographylibs-2.0.0/setup.py
```

### Comparing `cryptographylibs-1.0.0/setup.py` & `cryptographylibs-2.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '2.0.0'
+DESCRIPTION = "A Very complex coded PYthon package to handle and crypt strings in Python3"
+LONG_DESCRIPTION = "A Very complex coded PYthon package to handle and crypt strings in Python3"
 
 # Setting up
 setup(
     name="cryptographylibs",
     version=VERSION,
-    author="NHJonas",
+    author="knwnLegend",
     author_email="nick.faltermeier@gmx.de",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
```

