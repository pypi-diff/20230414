# Comparing `tmp/EmailEctractor-0.2.2.tar.gz` & `tmp/EmailEctractor-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\EmailEctractor-0.2.2.tar", last modified: Fri Apr 14 00:16:01 2023, max compression
+gzip compressed data, was "dist\EmailEctractor-0.2.3.tar", last modified: Fri Apr 14 00:21:14 2023, max compression
```

## Comparing `EmailEctractor-0.2.2.tar` & `EmailEctractor-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/EmailEctractor.egg-info/
--rw-rw-rw-   0        0        0      285 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/EmailEctractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/EmailEctractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/EmailEctractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/EmailEctractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/EmailEctractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      285 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-14 00:16:01.000000 EmailEctractor-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      407 2023-04-14 00:15:55.000000 EmailEctractor-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/EmailEctractor/
+-rw-rw-rw-   0        0        0      404 2023-04-13 23:42:29.000000 EmailEctractor-0.2.3/EmailEctractor/EmailEctractor.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 EmailEctractor-0.2.3/EmailEctractor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/EmailEctractor.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/EmailEctractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/EmailEctractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/EmailEctractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/EmailEctractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/EmailEctractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      285 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-14 00:21:14.000000 EmailEctractor-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      407 2023-04-14 00:21:07.000000 EmailEctractor-0.2.3/setup.py
```

