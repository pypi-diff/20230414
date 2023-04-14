# Comparing `tmp/cccrontab-1.1.tar.gz` & `tmp/cccrontab-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cccrontab-1.1.tar", last modified: Fri Apr 14 08:04:19 2023, max compression
+gzip compressed data, was "cccrontab-1.3.tar", last modified: Fri Apr 14 08:57:48 2023, max compression
```

## Comparing `cccrontab-1.1.tar` & `cccrontab-1.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:04:19.123686 cccrontab-1.1/
--rw-r--r--   0 openthread   (501) staff       (20)      199 2023-04-14 08:04:19.123583 cccrontab-1.1/PKG-INFO
--rw-r--r--   0 openthread   (501) staff       (20)      150 2023-04-14 07:40:41.000000 cccrontab-1.1/README.md
-drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:04:19.122828 cccrontab-1.1/cccrontab/
--rw-r--r--   0 openthread   (501) staff       (20)      583 2023-04-14 08:03:07.000000 cccrontab-1.1/cccrontab/__main__.py
-drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:04:19.123443 cccrontab-1.1/cccrontab.egg-info/
--rw-r--r--   0 openthread   (501) staff       (20)      199 2023-04-14 08:04:19.000000 cccrontab-1.1/cccrontab.egg-info/PKG-INFO
--rw-r--r--   0 openthread   (501) staff       (20)      204 2023-04-14 08:04:19.000000 cccrontab-1.1/cccrontab.egg-info/SOURCES.txt
--rw-r--r--   0 openthread   (501) staff       (20)        1 2023-04-14 08:04:19.000000 cccrontab-1.1/cccrontab.egg-info/dependency_links.txt
--rw-r--r--   0 openthread   (501) staff       (20)        1 2023-04-14 07:46:50.000000 cccrontab-1.1/cccrontab.egg-info/not-zip-safe
--rw-r--r--   0 openthread   (501) staff       (20)       10 2023-04-14 08:04:19.000000 cccrontab-1.1/cccrontab.egg-info/top_level.txt
--rw-r--r--   0 openthread   (501) staff       (20)       38 2023-04-14 08:04:19.123719 cccrontab-1.1/setup.cfg
--rw-r--r--   0 openthread   (501) staff       (20)      312 2023-04-14 08:03:31.000000 cccrontab-1.1/setup.py
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:57:48.308535 cccrontab-1.3/
+-rw-r--r--   0 openthread   (501) staff       (20)      199 2023-04-14 08:57:48.308403 cccrontab-1.3/PKG-INFO
+-rw-r--r--   0 openthread   (501) staff       (20)      150 2023-04-14 07:40:41.000000 cccrontab-1.3/README.md
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:57:48.307689 cccrontab-1.3/cccrontab/
+-rw-r--r--   0 openthread   (501) staff       (20)        0 2023-04-14 08:13:41.000000 cccrontab-1.3/cccrontab/__init__.py
+-rw-r--r--   0 openthread   (501) staff       (20)      583 2023-04-14 08:03:07.000000 cccrontab-1.3/cccrontab/__main__.py
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:57:48.308227 cccrontab-1.3/cccrontab.egg-info/
+-rw-r--r--   0 openthread   (501) staff       (20)      199 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/PKG-INFO
+-rw-r--r--   0 openthread   (501) staff       (20)      226 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/SOURCES.txt
+-rw-r--r--   0 openthread   (501) staff       (20)        1 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/dependency_links.txt
+-rw-r--r--   0 openthread   (501) staff       (20)        1 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/not-zip-safe
+-rw-r--r--   0 openthread   (501) staff       (20)       10 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/top_level.txt
+-rw-r--r--   0 openthread   (501) staff       (20)       38 2023-04-14 08:57:48.308571 cccrontab-1.3/setup.cfg
+-rw-r--r--   0 openthread   (501) staff       (20)      312 2023-04-14 08:29:23.000000 cccrontab-1.3/setup.py
```

### Comparing `cccrontab-1.1/cccrontab/__main__.py` & `cccrontab-1.3/cccrontab/__main__.py`

 * *Files identical despite different names*

