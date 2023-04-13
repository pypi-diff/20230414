# Comparing `tmp/risset-2.4.0.tar.gz` & `tmp/risset-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risset-2.4.0.tar", last modified: Wed Apr 12 23:58:15 2023, max compression
+gzip compressed data, was "risset-2.4.1.tar", last modified: Thu Apr 13 23:01:23 2023, max compression
```

## Comparing `risset-2.4.0.tar` & `risset-2.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 23:58:15.449814 risset-2.4.0/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 23:58:15.449814 risset-2.4.0/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     8076 2022-02-17 11:13:13.000000 risset-2.4.0/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-12 23:58:15.448814 risset-2.4.0/risset.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     8391 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       40 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-12 23:58:15.000000 risset-2.4.0/risset.egg-info/top_level.txt
--rwxrwxr-x   0 em        (1000) em        (1000)   107887 2023-04-12 23:58:06.000000 risset-2.4.0/risset.py
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-12 23:58:15.449814 risset-2.4.0/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-12 12:16:30.000000 risset-2.4.0/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-13 23:01:23.052319 risset-2.4.1/
+-rw-rw-r--   0 em        (1000) em        (1000)     5627 2023-04-13 23:01:23.052319 risset-2.4.1/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     5349 2023-04-13 00:18:38.000000 risset-2.4.1/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-13 23:01:23.051319 risset-2.4.1/risset.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     5627 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      210 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       39 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       26 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        7 2023-04-13 23:01:23.000000 risset-2.4.1/risset.egg-info/top_level.txt
+-rwxrwxr-x   0 em        (1000) em        (1000)   107887 2023-04-13 23:01:14.000000 risset-2.4.1/risset.py
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-13 23:01:23.052319 risset-2.4.1/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)      897 2023-04-12 12:16:30.000000 risset-2.4.1/setup.py
```

### Comparing `risset-2.4.0/risset.py` & `risset-2.4.1/risset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 from __future__ import annotations
 
-__version__ = "2.4.0"
+__version__ = "2.4.1"
 
 import sys
 
 if (sys.version_info.major, sys.version_info.minor) < (3, 8):
     print("Python 3.8 or higher is needed", file=sys.stderr)
     sys.exit(-1)
```

### Comparing `risset-2.4.0/setup.py` & `risset-2.4.1/setup.py`

 * *Files identical despite different names*

