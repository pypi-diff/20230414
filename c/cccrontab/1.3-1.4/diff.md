# Comparing `tmp/cccrontab-1.3.tar.gz` & `tmp/cccrontab-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cccrontab-1.3.tar", last modified: Fri Apr 14 08:57:48 2023, max compression
+gzip compressed data, was "cccrontab-1.4.tar", last modified: Fri Apr 14 08:59:24 2023, max compression
```

## Comparing `cccrontab-1.3.tar` & `cccrontab-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:57:48.308535 cccrontab-1.3/
--rw-r--r--   0 openthread   (501) staff       (20)      199 2023-04-14 08:57:48.308403 cccrontab-1.3/PKG-INFO
--rw-r--r--   0 openthread   (501) staff       (20)      150 2023-04-14 07:40:41.000000 cccrontab-1.3/README.md
-drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:57:48.307689 cccrontab-1.3/cccrontab/
--rw-r--r--   0 openthread   (501) staff       (20)        0 2023-04-14 08:13:41.000000 cccrontab-1.3/cccrontab/__init__.py
--rw-r--r--   0 openthread   (501) staff       (20)      583 2023-04-14 08:03:07.000000 cccrontab-1.3/cccrontab/__main__.py
-drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:57:48.308227 cccrontab-1.3/cccrontab.egg-info/
--rw-r--r--   0 openthread   (501) staff       (20)      199 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/PKG-INFO
--rw-r--r--   0 openthread   (501) staff       (20)      226 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/SOURCES.txt
--rw-r--r--   0 openthread   (501) staff       (20)        1 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/dependency_links.txt
--rw-r--r--   0 openthread   (501) staff       (20)        1 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/not-zip-safe
--rw-r--r--   0 openthread   (501) staff       (20)       10 2023-04-14 08:57:48.000000 cccrontab-1.3/cccrontab.egg-info/top_level.txt
--rw-r--r--   0 openthread   (501) staff       (20)       38 2023-04-14 08:57:48.308571 cccrontab-1.3/setup.cfg
--rw-r--r--   0 openthread   (501) staff       (20)      312 2023-04-14 08:29:23.000000 cccrontab-1.3/setup.py
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:59:24.476986 cccrontab-1.4/
+-rw-r--r--   0 openthread   (501) staff       (20)      199 2023-04-14 08:59:24.476874 cccrontab-1.4/PKG-INFO
+-rw-r--r--   0 openthread   (501) staff       (20)      150 2023-04-14 07:40:41.000000 cccrontab-1.4/README.md
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:59:24.476196 cccrontab-1.4/cccrontab/
+-rw-r--r--   0 openthread   (501) staff       (20)        0 2023-04-14 08:13:41.000000 cccrontab-1.4/cccrontab/__init__.py
+-rw-r--r--   0 openthread   (501) staff       (20)      583 2023-04-14 08:03:07.000000 cccrontab-1.4/cccrontab/__main__.py
+drwxr-xr-x   0 openthread   (501) staff       (20)        0 2023-04-14 08:59:24.476720 cccrontab-1.4/cccrontab.egg-info/
+-rw-r--r--   0 openthread   (501) staff       (20)      199 2023-04-14 08:59:24.000000 cccrontab-1.4/cccrontab.egg-info/PKG-INFO
+-rw-r--r--   0 openthread   (501) staff       (20)      226 2023-04-14 08:59:24.000000 cccrontab-1.4/cccrontab.egg-info/SOURCES.txt
+-rw-r--r--   0 openthread   (501) staff       (20)        1 2023-04-14 08:59:24.000000 cccrontab-1.4/cccrontab.egg-info/dependency_links.txt
+-rw-r--r--   0 openthread   (501) staff       (20)        1 2023-04-14 08:57:48.000000 cccrontab-1.4/cccrontab.egg-info/not-zip-safe
+-rw-r--r--   0 openthread   (501) staff       (20)       10 2023-04-14 08:59:24.000000 cccrontab-1.4/cccrontab.egg-info/top_level.txt
+-rw-r--r--   0 openthread   (501) staff       (20)       38 2023-04-14 08:59:24.477020 cccrontab-1.4/setup.cfg
+-rw-r--r--   0 openthread   (501) staff       (20)      312 2023-04-14 08:59:15.000000 cccrontab-1.4/setup.py
```

### Comparing `cccrontab-1.3/cccrontab/__main__.py` & `cccrontab-1.4/cccrontab/__main__.py`

 * *Files identical despite different names*

