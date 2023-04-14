# Comparing `tmp/shreycriclivemac-0.2.tar.gz` & `tmp/shreycriclivemac-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shreycriclivemac-0.2.tar", last modified: Fri Apr 14 21:44:37 2023, max compression
+gzip compressed data, was "shreycriclivemac-0.3.tar", last modified: Fri Apr 14 21:50:55 2023, max compression
```

## Comparing `shreycriclivemac-0.2.tar` & `shreycriclivemac-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 shreyansh   (501) staff       (20)        0 2023-04-14 21:44:37.195451 shreycriclivemac-0.2/
--rw-r--r--   0 shreyansh   (501) staff       (20)       18 2023-04-14 21:32:35.000000 shreycriclivemac-0.2/MANIFEST.in
--rw-r--r--   0 shreyansh   (501) staff       (20)       58 2023-04-14 21:44:37.195052 shreycriclivemac-0.2/PKG-INFO
--rw-r--r--   0 shreyansh   (501) staff       (20)      103 2023-04-14 21:32:06.000000 shreycriclivemac-0.2/README.md
--rw-r--r--   0 shreyansh   (501) staff       (20)       38 2023-04-14 21:44:37.195596 shreycriclivemac-0.2/setup.cfg
--rw-r--r--   0 shreyansh   (501) staff       (20)      319 2023-04-14 21:43:14.000000 shreycriclivemac-0.2/setup.py
-drwxr-xr-x   0 shreyansh   (501) staff       (20)        0 2023-04-14 21:44:37.194438 shreycriclivemac-0.2/shreycriclivemac.egg-info/
--rw-r--r--   0 shreyansh   (501) staff       (20)       58 2023-04-14 21:44:36.000000 shreycriclivemac-0.2/shreycriclivemac.egg-info/PKG-INFO
--rw-r--r--   0 shreyansh   (501) staff       (20)      272 2023-04-14 21:44:37.000000 shreycriclivemac-0.2/shreycriclivemac.egg-info/SOURCES.txt
--rw-r--r--   0 shreyansh   (501) staff       (20)        1 2023-04-14 21:44:36.000000 shreycriclivemac-0.2/shreycriclivemac.egg-info/dependency_links.txt
--rw-r--r--   0 shreyansh   (501) staff       (20)       63 2023-04-14 21:44:36.000000 shreycriclivemac-0.2/shreycriclivemac.egg-info/entry_points.txt
--rw-r--r--   0 shreyansh   (501) staff       (20)       29 2023-04-14 21:44:36.000000 shreycriclivemac-0.2/shreycriclivemac.egg-info/requires.txt
--rw-r--r--   0 shreyansh   (501) staff       (20)       13 2023-04-14 21:44:36.000000 shreycriclivemac-0.2/shreycriclivemac.egg-info/top_level.txt
+drwxr-xr-x   0 shreyansh   (501) staff       (20)        0 2023-04-14 21:50:55.884143 shreycriclivemac-0.3/
+-rw-r--r--   0 shreyansh   (501) staff       (20)       18 2023-04-14 21:32:35.000000 shreycriclivemac-0.3/MANIFEST.in
+-rw-r--r--   0 shreyansh   (501) staff       (20)       58 2023-04-14 21:50:55.883657 shreycriclivemac-0.3/PKG-INFO
+-rw-r--r--   0 shreyansh   (501) staff       (20)      103 2023-04-14 21:32:06.000000 shreycriclivemac-0.3/README.md
+-rw-r--r--   0 shreyansh   (501) staff       (20)       38 2023-04-14 21:50:55.884336 shreycriclivemac-0.3/setup.cfg
+-rw-r--r--   0 shreyansh   (501) staff       (20)      319 2023-04-14 21:50:44.000000 shreycriclivemac-0.3/setup.py
+drwxr-xr-x   0 shreyansh   (501) staff       (20)        0 2023-04-14 21:50:55.882932 shreycriclivemac-0.3/shreycriclivemac.egg-info/
+-rw-r--r--   0 shreyansh   (501) staff       (20)       58 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/PKG-INFO
+-rw-r--r--   0 shreyansh   (501) staff       (20)      272 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/SOURCES.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)        1 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/dependency_links.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)       63 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/entry_points.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)       29 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/requires.txt
+-rw-r--r--   0 shreyansh   (501) staff       (20)       13 2023-04-14 21:50:55.000000 shreycriclivemac-0.3/shreycriclivemac.egg-info/top_level.txt
```

