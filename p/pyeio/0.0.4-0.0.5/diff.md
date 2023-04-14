# Comparing `tmp/pyeio-0.0.4.tar.gz` & `tmp/pyeio-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeio-0.0.4.tar", last modified: Thu Mar  9 02:46:32 2023, max compression
+gzip compressed data, was "pyeio-0.0.5.tar", last modified: Fri Apr 14 16:11:29 2023, max compression
```

## Comparing `pyeio-0.0.4.tar` & `pyeio-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 harttraveller   (501) staff       (20)        0 2023-03-09 02:46:32.312957 pyeio-0.0.4/
--rw-r--r--   0 harttraveller   (501) staff       (20)     1078 2023-01-17 03:16:42.000000 pyeio-0.0.4/LICENSE
--rw-r--r--   0 harttraveller   (501) staff       (20)     1220 2023-03-09 02:46:32.312839 pyeio-0.0.4/PKG-INFO
--rw-r--r--   0 harttraveller   (501) staff       (20)      959 2023-03-09 02:45:49.000000 pyeio-0.0.4/README.md
-drwxr-xr-x   0 harttraveller   (501) staff       (20)        0 2023-03-09 02:46:32.311964 pyeio-0.0.4/pyeio/
--rw-r--r--   0 harttraveller   (501) staff       (20)       45 2023-01-17 05:49:05.000000 pyeio-0.0.4/pyeio/__init__.py
--rw-r--r--   0 harttraveller   (501) staff       (20)     4195 2023-01-17 07:58:15.000000 pyeio-0.0.4/pyeio/builder.py
--rw-r--r--   0 harttraveller   (501) staff       (20)     1389 2023-01-17 03:41:05.000000 pyeio-0.0.4/pyeio/director.py
-drwxr-xr-x   0 harttraveller   (501) staff       (20)        0 2023-03-09 02:46:32.312570 pyeio-0.0.4/pyeio.egg-info/
--rw-r--r--   0 harttraveller   (501) staff       (20)     1220 2023-03-09 02:46:32.000000 pyeio-0.0.4/pyeio.egg-info/PKG-INFO
--rw-r--r--   0 harttraveller   (501) staff       (20)      242 2023-03-09 02:46:32.000000 pyeio-0.0.4/pyeio.egg-info/SOURCES.txt
--rw-r--r--   0 harttraveller   (501) staff       (20)        1 2023-03-09 02:46:32.000000 pyeio-0.0.4/pyeio.egg-info/dependency_links.txt
--rw-r--r--   0 harttraveller   (501) staff       (20)        8 2023-03-09 02:46:32.000000 pyeio-0.0.4/pyeio.egg-info/requires.txt
--rw-r--r--   0 harttraveller   (501) staff       (20)        6 2023-03-09 02:46:32.000000 pyeio-0.0.4/pyeio.egg-info/top_level.txt
--rw-r--r--   0 harttraveller   (501) staff       (20)       38 2023-03-09 02:46:32.312996 pyeio-0.0.4/setup.cfg
--rw-r--r--   0 harttraveller   (501) staff       (20)      507 2023-03-09 02:46:25.000000 pyeio-0.0.4/setup.py
-drwxr-xr-x   0 harttraveller   (501) staff       (20)        0 2023-03-09 02:46:32.312701 pyeio-0.0.4/tests/
--rw-r--r--   0 harttraveller   (501) staff       (20)        0 2023-01-16 22:05:40.000000 pyeio-0.0.4/tests/test_json.py
+drwxr-xr-x   0 harttraveller   (501) staff       (20)        0 2023-04-14 16:11:29.953584 pyeio-0.0.5/
+-rw-r--r--   0 harttraveller   (501) staff       (20)     1071 2023-04-14 15:37:51.000000 pyeio-0.0.5/LICENSE
+-rw-r--r--   0 harttraveller   (501) staff       (20)     1557 2023-04-14 16:11:29.953463 pyeio-0.0.5/PKG-INFO
+-rw-r--r--   0 harttraveller   (501) staff       (20)     1296 2023-04-14 15:51:46.000000 pyeio-0.0.5/README.md
+drwxr-xr-x   0 harttraveller   (501) staff       (20)        0 2023-04-14 16:11:29.952168 pyeio-0.0.5/pyeio/
+-rw-r--r--   0 harttraveller   (501) staff       (20)       41 2023-03-16 18:39:58.000000 pyeio-0.0.5/pyeio/__init__.py
+-rw-r--r--   0 harttraveller   (501) staff       (20)     2799 2023-04-14 16:10:34.000000 pyeio-0.0.5/pyeio/core.py
+-rw-r--r--   0 harttraveller   (501) staff       (20)     1423 2023-04-14 16:08:32.000000 pyeio-0.0.5/pyeio/form.py
+-rw-r--r--   0 harttraveller   (501) staff       (20)      517 2023-03-16 18:18:01.000000 pyeio-0.0.5/pyeio/utils.py
+drwxr-xr-x   0 harttraveller   (501) staff       (20)        0 2023-04-14 16:11:29.952834 pyeio-0.0.5/pyeio.egg-info/
+-rw-r--r--   0 harttraveller   (501) staff       (20)     1557 2023-04-14 16:11:29.000000 pyeio-0.0.5/pyeio.egg-info/PKG-INFO
+-rw-r--r--   0 harttraveller   (501) staff       (20)      307 2023-04-14 16:11:29.000000 pyeio-0.0.5/pyeio.egg-info/SOURCES.txt
+-rw-r--r--   0 harttraveller   (501) staff       (20)        1 2023-04-14 16:11:29.000000 pyeio-0.0.5/pyeio.egg-info/dependency_links.txt
+-rw-r--r--   0 harttraveller   (501) staff       (20)       20 2023-04-14 16:11:29.000000 pyeio-0.0.5/pyeio.egg-info/requires.txt
+-rw-r--r--   0 harttraveller   (501) staff       (20)        6 2023-04-14 16:11:29.000000 pyeio-0.0.5/pyeio.egg-info/top_level.txt
+-rw-r--r--   0 harttraveller   (501) staff       (20)       38 2023-04-14 16:11:29.953627 pyeio-0.0.5/setup.cfg
+-rw-r--r--   0 harttraveller   (501) staff       (20)      525 2023-04-14 16:11:17.000000 pyeio-0.0.5/setup.py
+drwxr-xr-x   0 harttraveller   (501) staff       (20)        0 2023-04-14 16:11:29.953300 pyeio-0.0.5/tests/
+-rw-r--r--   0 harttraveller   (501) staff       (20)        0 2023-04-14 15:14:23.000000 pyeio-0.0.5/tests/test_csv.py
+-rw-r--r--   0 harttraveller   (501) staff       (20)        0 2023-01-16 22:05:40.000000 pyeio-0.0.5/tests/test_json.py
+-rw-r--r--   0 harttraveller   (501) staff       (20)        0 2023-04-14 15:19:26.000000 pyeio-0.0.5/tests/test_jsonl.py
+-rw-r--r--   0 harttraveller   (501) staff       (20)        0 2023-04-14 15:12:43.000000 pyeio-0.0.5/tests/test_toml.py
```

### Comparing `pyeio-0.0.4/LICENSE` & `pyeio-0.0.5/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Cephalon Intelligence
+Copyright (c) 2023 Hart Traveller
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

