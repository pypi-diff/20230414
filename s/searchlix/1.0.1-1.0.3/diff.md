# Comparing `tmp/searchlix-1.0.1.tar.gz` & `tmp/searchlix-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\searchlix-1.0.1.tar", last modified: Fri Apr 14 20:09:47 2023, max compression
+gzip compressed data, was "dist\searchlix-1.0.3.tar", last modified: Fri Apr 14 20:34:41 2023, max compression
```

## Comparing `searchlix-1.0.1.tar` & `searchlix-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 20:09:47.000000 searchlix-1.0.1/
--rw-rw-rw-   0        0        0      310 2023-04-14 20:09:47.000000 searchlix-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      986 2023-04-14 20:09:39.000000 searchlix-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 20:09:47.000000 searchlix-1.0.1/searchlix/
--rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 searchlix-1.0.1/searchlix/__init__.py
--rw-rw-rw-   0        0        0     2682 2023-04-14 19:50:21.000000 searchlix-1.0.1/searchlix/searchlix.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:09:47.000000 searchlix-1.0.1/searchlix.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-14 20:09:47.000000 searchlix-1.0.1/searchlix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-14 20:09:47.000000 searchlix-1.0.1/searchlix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 20:09:47.000000 searchlix-1.0.1/searchlix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-14 20:09:47.000000 searchlix-1.0.1/searchlix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 20:09:47.000000 searchlix-1.0.1/searchlix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 20:09:47.000000 searchlix-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      441 2023-04-14 20:08:36.000000 searchlix-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:34:41.000000 searchlix-1.0.3/
+-rw-rw-rw-   0        0        0     1738 2023-04-14 20:34:41.000000 searchlix-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      986 2023-04-14 20:09:39.000000 searchlix-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix/
+-rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 searchlix-1.0.3/searchlix/__init__.py
+-rw-rw-rw-   0        0        0     2682 2023-04-14 19:50:21.000000 searchlix-1.0.3/searchlix/searchlix.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/
+-rw-rw-rw-   0        0        0     1738 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 20:34:41.000000 searchlix-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-04-14 20:33:56.000000 searchlix-1.0.3/setup.py
```

### Comparing `searchlix-1.0.1/README.md` & `searchlix-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `searchlix-1.0.1/searchlix/searchlix.py` & `searchlix-1.0.3/searchlix/searchlix.py`

 * *Files identical despite different names*

