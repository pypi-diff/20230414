# Comparing `tmp/sball-0.9.2.tar.gz` & `tmp/sball-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sball-0.9.2.tar", last modified: Fri Apr 14 13:32:28 2023, max compression
+gzip compressed data, was "sball-0.9.3.tar", last modified: Fri Apr 14 13:49:59 2023, max compression
```

## Comparing `sball-0.9.2.tar` & `sball-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:32:28.274572 sball-0.9.2/
--rw-rw-rw-   0        0        0      401 2023-04-14 13:32:28.274572 sball-0.9.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 13:32:28.268574 sball-0.9.2/sball.egg-info/
--rw-rw-rw-   0        0        0      401 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 13:32:28.275575 sball-0.9.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 13:32:28.272571 sball-0.9.2/src/
--rw-rw-rw-   0        0        0       14 2023-04-14 12:15:27.000000 sball-0.9.2/src/__init__.py
--rw-rw-rw-   0        0        0     4957 2023-04-14 13:31:43.000000 sball-0.9.2/src/sball.py
--rw-rw-rw-   0        0        0      659 2023-04-14 13:31:48.000000 sball-0.9.2/src/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:49:59.622388 sball-0.9.3/
+-rw-rw-rw-   0        0        0      401 2023-04-14 13:49:59.621387 sball-0.9.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 13:49:59.613387 sball-0.9.3/sball.egg-info/
+-rw-rw-rw-   0        0        0      401 2023-04-14 13:49:59.000000 sball-0.9.3/sball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-04-14 13:49:59.000000 sball-0.9.3/sball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:49:59.000000 sball-0.9.3/sball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-14 13:49:59.000000 sball-0.9.3/sball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-04-14 13:49:59.000000 sball-0.9.3/sball.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:49:59.622388 sball-0.9.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:49:59.616388 sball-0.9.3/src/
+-rw-rw-rw-   0        0        0        0 2023-04-14 13:48:01.000000 sball-0.9.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:49:59.619386 sball-0.9.3/src/sball/
+-rw-rw-rw-   0        0        0       14 2023-04-14 12:15:27.000000 sball-0.9.3/src/sball/__init__.py
+-rw-rw-rw-   0        0        0     4957 2023-04-14 13:31:43.000000 sball-0.9.3/src/sball/sball.py
+-rw-rw-rw-   0        0        0      655 2023-04-14 13:49:35.000000 sball-0.9.3/src/setup.py
```

### Comparing `sball-0.9.2/src/sball.py` & `sball-0.9.3/src/sball/sball.py`

 * *Files identical despite different names*

### Comparing `sball-0.9.2/src/setup.py` & `sball-0.9.3/src/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="sball",
-    version="0.9.2",
+    version="0.9.3",
     author="michael_a_wilson",
     author_email="michael.a.wilson@yale.edu",
     description=(
         "sball.py: a script to submit job arrays from individual "
         "scripts using Yale CRC's dSQ."
     ),
     url="https://github.com/mawilson1234/sball",
@@ -14,11 +14,11 @@
     classifiers=(
         "Programming Language :: Python",
         "Development Status :: 4 - Beta",
         "Operating System :: OS Independent",
     ),
     entry_points={
         "console_scripts": [
-            "sball=src.sball:sbatch_all"
+            "sball=sball:sbatch_all"
         ]
     }
 )
```

