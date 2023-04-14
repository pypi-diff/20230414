# Comparing `tmp/piplibcrypter-1.0.0.tar.gz` & `tmp/piplibcrypter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piplibcrypter-1.0.0.tar", last modified: Wed Apr 12 20:27:33 2023, max compression
+gzip compressed data, was "piplibcrypter-1.1.0.tar", last modified: Fri Apr 14 20:09:05 2023, max compression
```

## Comparing `piplibcrypter-1.0.0.tar` & `piplibcrypter-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:27:33.245031 piplibcrypter-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      321 2023-04-12 20:27:33.245031 piplibcrypter-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:27:33.241031 piplibcrypter-1.0.0/piplibcrypter/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 20:27:32.000000 piplibcrypter-1.0.0/piplibcrypter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 20:27:33.245031 piplibcrypter-1.0.0/piplibcrypter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      321 2023-04-12 20:27:33.000000 piplibcrypter-1.0.0/piplibcrypter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      182 2023-04-12 20:27:33.000000 piplibcrypter-1.0.0/piplibcrypter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 20:27:33.000000 piplibcrypter-1.0.0/piplibcrypter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-12 20:27:33.000000 piplibcrypter-1.0.0/piplibcrypter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 20:27:33.245031 piplibcrypter-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      534 2023-04-12 20:27:32.000000 piplibcrypter-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 20:09:05.056707 piplibcrypter-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-14 20:09:05.056707 piplibcrypter-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 20:09:05.056707 piplibcrypter-1.1.0/piplibcrypter/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-14 20:09:04.000000 piplibcrypter-1.1.0/piplibcrypter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 20:09:05.056707 piplibcrypter-1.1.0/piplibcrypter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-04-14 20:09:04.000000 piplibcrypter-1.1.0/piplibcrypter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      182 2023-04-14 20:09:05.000000 piplibcrypter-1.1.0/piplibcrypter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 20:09:04.000000 piplibcrypter-1.1.0/piplibcrypter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-14 20:09:04.000000 piplibcrypter-1.1.0/piplibcrypter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 20:09:05.056707 piplibcrypter-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      576 2023-04-14 20:09:04.000000 piplibcrypter-1.1.0/setup.py
```

### Comparing `piplibcrypter-1.0.0/setup.py` & `piplibcrypter-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
-DESCRIPTION = "Hello World"
-LONG_DESCRIPTION = "Hello World"
+VERSION = '1.1.0'
+DESCRIPTION = "Package that helps with crypting"
+LONG_DESCRIPTION = "Package that helps with crypting"
 
 # Setting up
 setup(
     name="piplibcrypter",
     version=VERSION,
     author="NHJonas",
     author_email="nick.faltermeier@gmx.de",
```

