# Comparing `tmp/sherbystats-0.0.5.tar.gz` & `tmp/sherbystats-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherbystats-0.0.5.tar", last modified: Mon Mar 27 15:13:29 2023, max compression
+gzip compressed data, was "sherbystats-0.0.6.tar", last modified: Fri Apr 14 13:32:14 2023, max compression
```

## Comparing `sherbystats-0.0.5.tar` & `sherbystats-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-03-27 15:13:29.448999 sherbystats-0.0.5/
--rw-r--r--   0 ryangosselin   (501) staff       (20)      511 2023-03-27 15:13:29.448668 sherbystats-0.0.5/PKG-INFO
--rw-r--r--   0 ryangosselin   (501) staff       (20)       38 2023-03-27 15:13:29.449139 sherbystats-0.0.5/setup.cfg
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      663 2023-03-27 15:12:38.000000 sherbystats-0.0.5/setup.py
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-03-27 15:13:29.445748 sherbystats-0.0.5/sherbystats/
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      138 2023-03-20 18:15:45.000000 sherbystats-0.0.5/sherbystats/__init__.py
--rwxr-xr-x   0 ryangosselin   (501) staff       (20)     4755 2022-12-02 18:57:23.000000 sherbystats-0.0.5/sherbystats/anova.py
--rw-r--r--   0 ryangosselin   (501) staff       (20)    12256 2022-11-28 21:45:55.000000 sherbystats-0.0.5/sherbystats/doe.py
--rwxr-xr-x   0 ryangosselin   (501) staff       (20)      993 2022-11-28 21:46:07.000000 sherbystats-0.0.5/sherbystats/mlr.py
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      700 2022-11-28 21:46:48.000000 sherbystats-0.0.5/sherbystats/xlsread.py
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-03-27 15:13:29.447962 sherbystats-0.0.5/sherbystats.egg-info/
--rw-r--r--   0 ryangosselin   (501) staff       (20)      511 2023-03-27 15:13:29.000000 sherbystats-0.0.5/sherbystats.egg-info/PKG-INFO
--rw-r--r--   0 ryangosselin   (501) staff       (20)      254 2023-03-27 15:13:29.000000 sherbystats-0.0.5/sherbystats.egg-info/SOURCES.txt
--rw-r--r--   0 ryangosselin   (501) staff       (20)        1 2023-03-27 15:13:29.000000 sherbystats-0.0.5/sherbystats.egg-info/dependency_links.txt
--rw-r--r--   0 ryangosselin   (501) staff       (20)       12 2023-03-27 15:13:29.000000 sherbystats-0.0.5/sherbystats.egg-info/top_level.txt
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-14 13:32:14.764653 sherbystats-0.0.6/
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-04-14 13:32:14.764260 sherbystats-0.0.6/PKG-INFO
+-rw-r--r--   0 ryangosselin   (501) staff       (20)       38 2023-04-14 13:32:14.764832 sherbystats-0.0.6/setup.cfg
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      663 2023-04-14 13:28:30.000000 sherbystats-0.0.6/setup.py
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-14 13:32:14.760538 sherbystats-0.0.6/sherbystats/
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      173 2023-04-14 13:30:30.000000 sherbystats-0.0.6/sherbystats/__init__.py
+-rwxr-xr-x   0 ryangosselin   (501) staff       (20)     4755 2022-12-02 18:57:23.000000 sherbystats-0.0.6/sherbystats/anova.py
+-rw-r--r--   0 ryangosselin   (501) staff       (20)    12256 2022-11-28 21:45:55.000000 sherbystats-0.0.6/sherbystats/doe.py
+-rwxr-xr-x   0 ryangosselin   (501) staff       (20)      993 2022-11-28 21:46:07.000000 sherbystats-0.0.6/sherbystats/mlr.py
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)     1839 2023-04-14 13:29:38.000000 sherbystats-0.0.6/sherbystats/normplot.py
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      700 2022-11-28 21:46:48.000000 sherbystats-0.0.6/sherbystats/xlsread.py
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-14 13:32:14.763620 sherbystats-0.0.6/sherbystats.egg-info/
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-04-14 13:32:14.000000 sherbystats-0.0.6/sherbystats.egg-info/PKG-INFO
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      278 2023-04-14 13:32:14.000000 sherbystats-0.0.6/sherbystats.egg-info/SOURCES.txt
+-rw-r--r--   0 ryangosselin   (501) staff       (20)        1 2023-04-14 13:32:14.000000 sherbystats-0.0.6/sherbystats.egg-info/dependency_links.txt
+-rw-r--r--   0 ryangosselin   (501) staff       (20)       12 2023-04-14 13:32:14.000000 sherbystats-0.0.6/sherbystats.egg-info/top_level.txt
```

### Comparing `sherbystats-0.0.5/setup.py` & `sherbystats-0.0.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import setuptools
 
 
 setuptools.setup(
     name="sherbystats",
-    version="0.0.5",
+    version="0.0.6",
     author="Ryan Gosselin",
     author_email="ryan.gosselin@usherbrooke.ca",
     url="https://www.usherbrooke.ca/gchimiquebiotech/departement/professeurs/ryan-gosselin/",
     packages=["sherbystats"],
     description="Ryan @ UdeS",
     long_description="Python for GCB140 and GCH711:\
     \n\
-    \nfct_anova\
-    \nfct_doe\
-    \nfct_mlr\
-    \nfct_xlsread",
+    \nanova\
+    \ndoe\
+    \nmlr\
+    \nnormplot\
+    \nxlsread",
     long_description_content_type="text/markdown",
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ),
 )
```

### Comparing `sherbystats-0.0.5/sherbystats/anova.py` & `sherbystats-0.0.6/sherbystats/anova.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.5/sherbystats/doe.py` & `sherbystats-0.0.6/sherbystats/doe.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.5/sherbystats/mlr.py` & `sherbystats-0.0.6/sherbystats/mlr.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.5/sherbystats/xlsread.py` & `sherbystats-0.0.6/sherbystats/xlsread.py`

 * *Files identical despite different names*

