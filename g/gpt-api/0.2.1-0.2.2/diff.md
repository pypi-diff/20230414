# Comparing `tmp/gpt-api-0.2.1.tar.gz` & `tmp/gpt-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-api-0.2.1.tar", last modified: Fri Apr 14 09:17:15 2023, max compression
+gzip compressed data, was "gpt-api-0.2.2.tar", last modified: Fri Apr 14 10:19:31 2023, max compression
```

## Comparing `gpt-api-0.2.1.tar` & `gpt-api-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 09:17:15.782808 gpt-api-0.2.1/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 09:17:15.782120 gpt-api-0.2.1/PKG-INFO
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 09:17:15.779531 gpt-api-0.2.1/api/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.2.1/api/__init__.py
--rw-r--r--   0 yuanchangjun   (501) staff       (20)     3924 2023-04-14 09:16:21.000000 gpt-api-0.2.1/api/gpt.py
-drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 09:17:15.781610 gpt-api-0.2.1/gpt_api.egg-info/
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/PKG-INFO
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/SOURCES.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/dependency_links.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/requires.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-14 09:17:15.000000 gpt-api-0.2.1/gpt_api.egg-info/top_level.txt
--rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-14 09:17:15.782977 gpt-api-0.2.1/setup.cfg
--rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.2.1/setup.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 10:19:31.538896 gpt-api-0.2.2/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 10:19:31.538510 gpt-api-0.2.2/PKG-INFO
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 10:19:31.534353 gpt-api-0.2.2/api/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        0 2023-04-13 02:23:04.000000 gpt-api-0.2.2/api/__init__.py
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)     3924 2023-04-14 09:16:21.000000 gpt-api-0.2.2/api/gpt.py
+drwxr-xr-x   0 yuanchangjun   (501) staff       (20)        0 2023-04-14 10:19:31.537814 gpt-api-0.2.2/gpt_api.egg-info/
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      356 2023-04-14 10:19:31.000000 gpt-api-0.2.2/gpt_api.egg-info/PKG-INFO
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      189 2023-04-14 10:19:31.000000 gpt-api-0.2.2/gpt_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        1 2023-04-14 10:19:31.000000 gpt-api-0.2.2/gpt_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        7 2023-04-14 10:19:31.000000 gpt-api-0.2.2/gpt_api.egg-info/requires.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)        4 2023-04-14 10:19:31.000000 gpt-api-0.2.2/gpt_api.egg-info/top_level.txt
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)       38 2023-04-14 10:19:31.539057 gpt-api-0.2.2/setup.cfg
+-rw-r--r--   0 yuanchangjun   (501) staff       (20)      765 2023-04-13 02:23:39.000000 gpt-api-0.2.2/setup.py
```

### Comparing `gpt-api-0.2.1/api/gpt.py` & `gpt-api-0.2.2/api/gpt.py`

 * *Files identical despite different names*

### Comparing `gpt-api-0.2.1/setup.py` & `gpt-api-0.2.2/setup.py`

 * *Files identical despite different names*

