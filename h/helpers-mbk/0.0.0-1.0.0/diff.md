# Comparing `tmp/helpers-mbk-0.0.0.tar.gz` & `tmp/helpers-mbk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helpers-mbk-0.0.0.tar", last modified: Fri Apr 14 20:16:14 2023, max compression
+gzip compressed data, was "helpers-mbk-1.0.0.tar", last modified: Fri Apr 14 20:29:45 2023, max compression
```

## Comparing `helpers-mbk-0.0.0.tar` & `helpers-mbk-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:16:14.754313 helpers-mbk-0.0.0/
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)     1084 2023-04-12 22:01:14.000000 helpers-mbk-0.0.0/LICENSE
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)        0 2023-04-12 16:27:20.000000 helpers-mbk-0.0.0/MANIFEST.in
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)     1905 2023-04-14 20:16:14.754313 helpers-mbk-0.0.0/PKG-INFO
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      116 2023-04-14 20:00:46.000000 helpers-mbk-0.0.0/README.md
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      838 2023-04-14 20:12:43.000000 helpers-mbk-0.0.0/pyproject.toml
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       38 2023-04-14 20:16:14.754313 helpers-mbk-0.0.0/setup.cfg
-drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:16:14.754313 helpers-mbk-0.0.0/src/
-drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:16:14.754313 helpers-mbk-0.0.0/src/helpers-mbk/
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)        0 2023-04-12 20:27:28.000000 helpers-mbk-0.0.0/src/helpers-mbk/__init__.py
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      224 2023-04-12 21:04:00.000000 helpers-mbk-0.0.0/src/helpers-mbk/__main__.py
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      509 2023-04-14 20:01:21.000000 helpers-mbk-0.0.0/src/helpers-mbk/helpers.py
-drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:16:14.754313 helpers-mbk-0.0.0/src/helpers_mbk.egg-info/
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)     1905 2023-04-14 20:16:14.000000 helpers-mbk-0.0.0/src/helpers_mbk.egg-info/PKG-INFO
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      396 2023-04-14 20:16:14.000000 helpers-mbk-0.0.0/src/helpers_mbk.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)        1 2023-04-14 20:16:14.000000 helpers-mbk-0.0.0/src/helpers_mbk.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       55 2023-04-14 20:16:14.000000 helpers-mbk-0.0.0/src/helpers_mbk.egg-info/entry_points.txt
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       42 2023-04-14 20:16:14.000000 helpers-mbk-0.0.0/src/helpers_mbk.egg-info/requires.txt
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       12 2023-04-14 20:16:14.000000 helpers-mbk-0.0.0/src/helpers_mbk.egg-info/top_level.txt
-drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:16:14.754313 helpers-mbk-0.0.0/tests/
--rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       70 2023-04-12 21:25:18.000000 helpers-mbk-0.0.0/tests/test_frequent_functions.py
+drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:29:45.043319 helpers-mbk-1.0.0/
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)     1084 2023-04-12 22:01:14.000000 helpers-mbk-1.0.0/LICENSE
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)        0 2023-04-12 16:27:20.000000 helpers-mbk-1.0.0/MANIFEST.in
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)     1906 2023-04-14 20:29:45.043319 helpers-mbk-1.0.0/PKG-INFO
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      116 2023-04-14 20:00:46.000000 helpers-mbk-1.0.0/README.md
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      839 2023-04-14 20:28:26.000000 helpers-mbk-1.0.0/pyproject.toml
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       38 2023-04-14 20:29:45.043319 helpers-mbk-1.0.0/setup.cfg
+drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:29:45.043319 helpers-mbk-1.0.0/src/
+drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:29:45.043319 helpers-mbk-1.0.0/src/helpers-mbk/
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)        0 2023-04-12 20:27:28.000000 helpers-mbk-1.0.0/src/helpers-mbk/__init__.py
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      224 2023-04-12 21:04:00.000000 helpers-mbk-1.0.0/src/helpers-mbk/__main__.py
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      509 2023-04-14 20:01:21.000000 helpers-mbk-1.0.0/src/helpers-mbk/helpers.py
+drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:29:45.043319 helpers-mbk-1.0.0/src/helpers_mbk.egg-info/
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)     1906 2023-04-14 20:29:45.000000 helpers-mbk-1.0.0/src/helpers_mbk.egg-info/PKG-INFO
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)      396 2023-04-14 20:29:45.000000 helpers-mbk-1.0.0/src/helpers_mbk.egg-info/SOURCES.txt
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)        1 2023-04-14 20:29:45.000000 helpers-mbk-1.0.0/src/helpers_mbk.egg-info/dependency_links.txt
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       55 2023-04-14 20:29:45.000000 helpers-mbk-1.0.0/src/helpers_mbk.egg-info/entry_points.txt
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       42 2023-04-14 20:29:45.000000 helpers-mbk-1.0.0/src/helpers_mbk.egg-info/requires.txt
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       12 2023-04-14 20:29:45.000000 helpers-mbk-1.0.0/src/helpers_mbk.egg-info/top_level.txt
+drwxrwxr-x   0 muhammed  (1000) muhammed  (1000)        0 2023-04-14 20:29:45.043319 helpers-mbk-1.0.0/tests/
+-rw-rw-r--   0 muhammed  (1000) muhammed  (1000)       70 2023-04-12 21:25:18.000000 helpers-mbk-1.0.0/tests/test_frequent_functions.py
```

### Comparing `helpers-mbk-0.0.0/LICENSE` & `helpers-mbk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helpers-mbk-0.0.0/PKG-INFO` & `helpers-mbk-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: helpers-mbk
-Version: 0.0.0
-Summary: Some function that Muhammed Buyukkinaci uses a lot
+Version: 1.0.0
+Summary: Some functions that Muhammed Buyukkinaci uses a lot
 Author-email: Muhammed Buyukkinaci <muhammedbuyukkinaci@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Muhammed Büyükkınacı]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `helpers-mbk-0.0.0/pyproject.toml` & `helpers-mbk-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "helpers-mbk"
-version = "0.0.0"
-description = "Some function that Muhammed Buyukkinaci uses a lot"
+version = "1.0.0"
+description = "Some functions that Muhammed Buyukkinaci uses a lot"
 readme = "README.md"
 authors = [{ name = "Muhammed Buyukkinaci", email = "muhammedbuyukkinaci@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `helpers-mbk-0.0.0/src/helpers_mbk.egg-info/PKG-INFO` & `helpers-mbk-1.0.0/src/helpers_mbk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: helpers-mbk
-Version: 0.0.0
-Summary: Some function that Muhammed Buyukkinaci uses a lot
+Version: 1.0.0
+Summary: Some functions that Muhammed Buyukkinaci uses a lot
 Author-email: Muhammed Buyukkinaci <muhammedbuyukkinaci@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Muhammed Büyükkınacı]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

