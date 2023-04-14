# Comparing `tmp/sball-0.9.0.tar.gz` & `tmp/sball-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sball-0.9.0.tar", last modified: Fri Apr 14 13:02:22 2023, max compression
+gzip compressed data, was "sball-0.9.1.tar", last modified: Fri Apr 14 13:14:44 2023, max compression
```

## Comparing `sball-0.9.0.tar` & `sball-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:02:22.536260 sball-0.9.0/
--rw-rw-rw-   0        0        0      409 2023-04-14 13:02:22.535260 sball-0.9.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 13:02:22.521259 sball-0.9.0/sball/
--rw-rw-rw-   0        0        0       14 2023-04-14 12:15:27.000000 sball-0.9.0/sball/__init__.py
--rw-rw-rw-   0        0        0     4957 2023-04-14 12:48:14.000000 sball-0.9.0/sball/sball.py
--rw-rw-rw-   0        0        0      656 2023-04-14 12:48:59.000000 sball-0.9.0/sball/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:02:22.534258 sball-0.9.0/sball.egg-info/
--rw-rw-rw-   0        0        0      409 2023-04-14 13:02:22.000000 sball-0.9.0/sball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-04-14 13:02:22.000000 sball-0.9.0/sball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:02:22.000000 sball-0.9.0/sball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-14 13:02:22.000000 sball-0.9.0/sball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 13:02:22.000000 sball-0.9.0/sball.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 13:02:22.536260 sball-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:14:44.901799 sball-0.9.1/
+-rw-rw-rw-   0        0        0      401 2023-04-14 13:14:44.900798 sball-0.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 13:14:44.894800 sball-0.9.1/sball.egg-info/
+-rw-rw-rw-   0        0        0      401 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:14:44.901799 sball-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:14:44.898800 sball-0.9.1/src/
+-rw-rw-rw-   0        0        0       14 2023-04-14 12:15:27.000000 sball-0.9.1/src/__init__.py
+-rw-rw-rw-   0        0        0     4957 2023-04-14 12:48:14.000000 sball-0.9.1/src/sball.py
+-rw-rw-rw-   0        0        0      659 2023-04-14 13:11:12.000000 sball-0.9.1/src/setup.py
```

### Comparing `sball-0.9.0/sball/sball.py` & `sball-0.9.1/src/sball.py`

 * *Files identical despite different names*

### Comparing `sball-0.9.0/sball/setup.py` & `sball-0.9.1/src/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 setuptools.setup(
     name="sball",
-    version="0.9.0",
+    version="0.9.1",
     author="michael_a_wilson",
     author_email="michael.a.wilson@yale.edu",
     description=(
-        "sball.py: a script to submit job arrays from individual ",
+        "sball.py: a script to submit job arrays from individual "
         "scripts using Yale CRC's dSQ."
     ),
     url="https://github.com/mawilson1234/sball",
     packages=setuptools.find_packages(),
     classifiers=(
         "Programming Language :: Python",
         "Development Status :: 4 - Beta",
         "Operating System :: OS Independent",
     ),
     entry_points={
         "console_scripts": [
-            "sball=sball:sbatch_all"
+            "sball=src.sball:sbatch_all"
         ]
     }
 )
```

