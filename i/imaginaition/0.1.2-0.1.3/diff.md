# Comparing `tmp/imaginaition-0.1.2.tar.gz` & `tmp/imaginaition-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaginaition-0.1.2.tar", last modified: Fri Apr 14 05:47:10 2023, max compression
+gzip compressed data, was "imaginaition-0.1.3.tar", last modified: Fri Apr 14 05:58:30 2023, max compression
```

## Comparing `imaginaition-0.1.2.tar` & `imaginaition-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 joeltan    (501) staff       (20)        0 2023-04-14 05:47:10.704743 imaginaition-0.1.2/
--rw-r--r--   0 joeltan    (501) staff       (20)    16724 2023-04-14 03:32:49.000000 imaginaition-0.1.2/LICENSE
--rw-r--r--   0 joeltan    (501) staff       (20)      371 2023-04-14 05:47:10.704598 imaginaition-0.1.2/PKG-INFO
--rw-r--r--   0 joeltan    (501) staff       (20)      130 2023-04-14 04:22:18.000000 imaginaition-0.1.2/README.md
--rw-r--r--   0 joeltan    (501) staff       (20)      449 2023-04-14 05:45:15.000000 imaginaition-0.1.2/pyproject.toml
--rw-r--r--   0 joeltan    (501) staff       (20)       38 2023-04-14 05:47:10.704788 imaginaition-0.1.2/setup.cfg
-drwxr-xr-x   0 joeltan    (501) staff       (20)        0 2023-04-14 05:47:10.701832 imaginaition-0.1.2/src/
-drwxr-xr-x   0 joeltan    (501) staff       (20)        0 2023-04-14 05:47:10.703527 imaginaition-0.1.2/src/imaginaition/
--rw-r--r--   0 joeltan    (501) staff       (20)       61 2023-04-14 05:35:28.000000 imaginaition-0.1.2/src/imaginaition/__init__.py
--rw-r--r--   0 joeltan    (501) staff       (20)      584 2023-04-14 05:34:17.000000 imaginaition-0.1.2/src/imaginaition/__main__.py
--rw-r--r--   0 joeltan    (501) staff       (20)     1074 2023-04-14 03:56:35.000000 imaginaition-0.1.2/src/imaginaition/cut.py
--rw-r--r--   0 joeltan    (501) staff       (20)      980 2023-04-14 03:56:26.000000 imaginaition-0.1.2/src/imaginaition/help.py
--rw-r--r--   0 joeltan    (501) staff       (20)      615 2023-04-14 02:02:20.000000 imaginaition-0.1.2/src/imaginaition/imaginaition_logging.py
--rw-r--r--   0 joeltan    (501) staff       (20)        0 2023-04-14 01:57:27.000000 imaginaition-0.1.2/src/imaginaition/imagine.py
-drwxr-xr-x   0 joeltan    (501) staff       (20)        0 2023-04-14 05:47:10.704381 imaginaition-0.1.2/src/imaginaition.egg-info/
--rw-r--r--   0 joeltan    (501) staff       (20)      371 2023-04-14 05:47:10.000000 imaginaition-0.1.2/src/imaginaition.egg-info/PKG-INFO
--rw-r--r--   0 joeltan    (501) staff       (20)      450 2023-04-14 05:47:10.000000 imaginaition-0.1.2/src/imaginaition.egg-info/SOURCES.txt
--rw-r--r--   0 joeltan    (501) staff       (20)        1 2023-04-14 05:47:10.000000 imaginaition-0.1.2/src/imaginaition.egg-info/dependency_links.txt
--rw-r--r--   0 joeltan    (501) staff       (20)       51 2023-04-14 05:47:10.000000 imaginaition-0.1.2/src/imaginaition.egg-info/entry_points.txt
--rw-r--r--   0 joeltan    (501) staff       (20)       21 2023-04-14 05:47:10.000000 imaginaition-0.1.2/src/imaginaition.egg-info/requires.txt
--rw-r--r--   0 joeltan    (501) staff       (20)       13 2023-04-14 05:47:10.000000 imaginaition-0.1.2/src/imaginaition.egg-info/top_level.txt
+drwxr-xr-x   0 joeltan    (501) staff       (20)        0 2023-04-14 05:58:30.020040 imaginaition-0.1.3/
+-rw-r--r--   0 joeltan    (501) staff       (20)    35148 2023-04-14 05:55:25.000000 imaginaition-0.1.3/LICENSE.md
+-rw-r--r--   0 joeltan    (501) staff       (20)    40899 2023-04-14 05:58:30.019896 imaginaition-0.1.3/PKG-INFO
+-rw-r--r--   0 joeltan    (501) staff       (20)      130 2023-04-14 04:22:18.000000 imaginaition-0.1.3/README.md
+-rw-r--r--   0 joeltan    (501) staff       (20)      452 2023-04-14 05:58:05.000000 imaginaition-0.1.3/pyproject.toml
+-rw-r--r--   0 joeltan    (501) staff       (20)       38 2023-04-14 05:58:30.020080 imaginaition-0.1.3/setup.cfg
+drwxr-xr-x   0 joeltan    (501) staff       (20)        0 2023-04-14 05:58:30.017621 imaginaition-0.1.3/src/
+drwxr-xr-x   0 joeltan    (501) staff       (20)        0 2023-04-14 05:58:30.018797 imaginaition-0.1.3/src/imaginaition/
+-rw-r--r--   0 joeltan    (501) staff       (20)       61 2023-04-14 05:35:28.000000 imaginaition-0.1.3/src/imaginaition/__init__.py
+-rw-r--r--   0 joeltan    (501) staff       (20)      584 2023-04-14 05:34:17.000000 imaginaition-0.1.3/src/imaginaition/__main__.py
+-rw-r--r--   0 joeltan    (501) staff       (20)     1074 2023-04-14 03:56:35.000000 imaginaition-0.1.3/src/imaginaition/cut.py
+-rw-r--r--   0 joeltan    (501) staff       (20)      980 2023-04-14 03:56:26.000000 imaginaition-0.1.3/src/imaginaition/help.py
+-rw-r--r--   0 joeltan    (501) staff       (20)      615 2023-04-14 02:02:20.000000 imaginaition-0.1.3/src/imaginaition/imaginaition_logging.py
+-rw-r--r--   0 joeltan    (501) staff       (20)        0 2023-04-14 01:57:27.000000 imaginaition-0.1.3/src/imaginaition/imagine.py
+drwxr-xr-x   0 joeltan    (501) staff       (20)        0 2023-04-14 05:58:30.019659 imaginaition-0.1.3/src/imaginaition.egg-info/
+-rw-r--r--   0 joeltan    (501) staff       (20)    40899 2023-04-14 05:58:30.000000 imaginaition-0.1.3/src/imaginaition.egg-info/PKG-INFO
+-rw-r--r--   0 joeltan    (501) staff       (20)      453 2023-04-14 05:58:30.000000 imaginaition-0.1.3/src/imaginaition.egg-info/SOURCES.txt
+-rw-r--r--   0 joeltan    (501) staff       (20)        1 2023-04-14 05:58:30.000000 imaginaition-0.1.3/src/imaginaition.egg-info/dependency_links.txt
+-rw-r--r--   0 joeltan    (501) staff       (20)       51 2023-04-14 05:58:30.000000 imaginaition-0.1.3/src/imaginaition.egg-info/entry_points.txt
+-rw-r--r--   0 joeltan    (501) staff       (20)       21 2023-04-14 05:58:30.000000 imaginaition-0.1.3/src/imaginaition.egg-info/requires.txt
+-rw-r--r--   0 joeltan    (501) staff       (20)       13 2023-04-14 05:58:30.000000 imaginaition-0.1.3/src/imaginaition.egg-info/top_level.txt
```

### Comparing `imaginaition-0.1.2/src/imaginaition/__main__.py` & `imaginaition-0.1.3/src/imaginaition/__main__.py`

 * *Files identical despite different names*

### Comparing `imaginaition-0.1.2/src/imaginaition/cut.py` & `imaginaition-0.1.3/src/imaginaition/cut.py`

 * *Files identical despite different names*

### Comparing `imaginaition-0.1.2/src/imaginaition/help.py` & `imaginaition-0.1.3/src/imaginaition/help.py`

 * *Files identical despite different names*

### Comparing `imaginaition-0.1.2/src/imaginaition/imaginaition_logging.py` & `imaginaition-0.1.3/src/imaginaition/imaginaition_logging.py`

 * *Files identical despite different names*

