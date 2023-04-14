# Comparing `tmp/cryptographylibary-1.0.0.tar.gz` & `tmp/cryptographylibary-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographylibary-1.0.0.tar", last modified: Wed Apr 12 20:26:43 2023, max compression
+gzip compressed data, was "cryptographylibary-2.0.0.tar", last modified: Fri Apr 14 18:33:58 2023, max compression
```

## Comparing `cryptographylibary-1.0.0.tar` & `cryptographylibary-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:26:43.513422 cryptographylibary-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-12 20:26:43.513422 cryptographylibary-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:26:43.509422 cryptographylibary-1.0.0/cryptographylibary/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 20:26:43.000000 cryptographylibary-1.0.0/cryptographylibary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:26:43.509422 cryptographylibary-1.0.0/cryptographylibary.egg-info/
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-12 20:26:43.000000 cryptographylibary-1.0.0/cryptographylibary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-12 20:26:43.000000 cryptographylibary-1.0.0/cryptographylibary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:26:43.000000 cryptographylibary-1.0.0/cryptographylibary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-12 20:26:43.000000 cryptographylibary-1.0.0/cryptographylibary.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 20:26:43.513422 cryptographylibary-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      539 2023-04-12 20:26:42.000000 cryptographylibary-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 18:33:58.943876 cryptographylibary-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-14 18:33:58.943876 cryptographylibary-2.0.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 18:33:58.939876 cryptographylibary-2.0.0/cryptographylibary/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-14 18:33:58.000000 cryptographylibary-2.0.0/cryptographylibary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 18:33:58.943876 cryptographylibary-2.0.0/cryptographylibary.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      395 2023-04-14 18:33:58.000000 cryptographylibary-2.0.0/cryptographylibary.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-14 18:33:58.000000 cryptographylibary-2.0.0/cryptographylibary.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 18:33:58.000000 cryptographylibary-2.0.0/cryptographylibary.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-14 18:33:58.000000 cryptographylibary-2.0.0/cryptographylibary.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 18:33:58.943876 cryptographylibary-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      608 2023-04-14 18:33:57.000000 cryptographylibary-2.0.0/setup.py
```

### Comparing `cryptographylibary-1.0.0/setup.py` & `cryptographylibary-2.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '2.0.0'
+DESCRIPTION = "PYthon packge to handle crypting in Python3."
+LONG_DESCRIPTION = "PYthon packge to handle crypting in Python3."
 
 # Setting up
 setup(
     name="cryptographylibary",
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

