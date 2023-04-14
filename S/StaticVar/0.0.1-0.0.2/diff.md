# Comparing `tmp/StaticVar-0.0.1.tar.gz` & `tmp/StaticVar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StaticVar-0.0.1.tar", last modified: Fri Apr 14 04:37:07 2023, max compression
+gzip compressed data, was "StaticVar-0.0.2.tar", last modified: Fri Apr 14 04:42:00 2023, max compression
```

## Comparing `StaticVar-0.0.1.tar` & `StaticVar-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 04:37:07.612028 StaticVar-0.0.1/
--rw-rw-rw-   0        0        0      557 2023-04-14 04:37:07.611031 StaticVar-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-04-04 12:32:56.000000 StaticVar-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 04:37:07.584613 StaticVar-0.0.1/StaticVar/
--rw-rw-rw-   0        0        0     2084 2023-04-14 04:01:44.000000 StaticVar-0.0.1/StaticVar/StaticVar.py
--rw-rw-rw-   0        0        0       28 2023-04-14 04:01:52.000000 StaticVar-0.0.1/StaticVar/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 04:37:07.610077 StaticVar-0.0.1/StaticVar.egg-info/
--rw-rw-rw-   0        0        0      557 2023-04-14 04:37:07.000000 StaticVar-0.0.1/StaticVar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-14 04:37:07.000000 StaticVar-0.0.1/StaticVar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 04:37:07.000000 StaticVar-0.0.1/StaticVar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 04:37:07.000000 StaticVar-0.0.1/StaticVar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 04:37:07.000000 StaticVar-0.0.1/StaticVar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 04:37:07.612028 StaticVar-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-04-14 04:34:18.000000 StaticVar-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 04:42:00.928134 StaticVar-0.0.2/
+-rw-rw-rw-   0        0        0      508 2023-04-14 04:42:00.927097 StaticVar-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-04-04 12:32:56.000000 StaticVar-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 04:42:00.915128 StaticVar-0.0.2/StaticVar/
+-rw-rw-rw-   0        0        0     2084 2023-04-14 04:01:44.000000 StaticVar-0.0.2/StaticVar/StaticVar.py
+-rw-rw-rw-   0        0        0       28 2023-04-14 04:01:52.000000 StaticVar-0.0.2/StaticVar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 04:42:00.926046 StaticVar-0.0.2/StaticVar.egg-info/
+-rw-rw-rw-   0        0        0      508 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 04:42:00.000000 StaticVar-0.0.2/StaticVar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 04:42:00.928134 StaticVar-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      860 2023-04-14 04:41:45.000000 StaticVar-0.0.2/setup.py
```

### Comparing `StaticVar-0.0.1/README.md` & `StaticVar-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `StaticVar-0.0.1/StaticVar/StaticVar.py` & `StaticVar-0.0.2/StaticVar/StaticVar.py`

 * *Files identical despite different names*

### Comparing `StaticVar-0.0.1/setup.py` & `StaticVar-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Static variables for Python'
 LONG_DESCRIPTION = 'Static variables for Python like in C'
 
 setup(
         name="StaticVar", 
         version=VERSION,
         author="AbdelRahman Rahal",
@@ -14,13 +14,12 @@
         packages=find_packages(),
         install_requires=['varname'],
         
         keywords=['Static', 'Static Variables', 'StaticVar'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Developers",
-            "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3 :: Only",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

