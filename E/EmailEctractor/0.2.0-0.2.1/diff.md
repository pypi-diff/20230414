# Comparing `tmp/EmailEctractor-0.2.0.tar.gz` & `tmp/EmailEctractor-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\EmailEctractor-0.2.0.tar", last modified: Fri Apr 14 00:01:55 2023, max compression
+gzip compressed data, was "dist\EmailEctractor-0.2.1.tar", last modified: Fri Apr 14 00:09:04 2023, max compression
```

## Comparing `EmailEctractor-0.2.0.tar` & `EmailEctractor-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/EmailEctractor.egg-info/
--rw-rw-rw-   0        0        0      285 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/EmailEctractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/EmailEctractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/EmailEctractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/EmailEctractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/EmailEctractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      285 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-14 00:01:55.000000 EmailEctractor-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      407 2023-04-14 00:01:49.000000 EmailEctractor-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/EmailEctractor.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/EmailEctractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/EmailEctractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/EmailEctractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/EmailEctractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/EmailEctractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      285 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-14 00:09:04.000000 EmailEctractor-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      407 2023-04-14 00:08:56.000000 EmailEctractor-0.2.1/setup.py
```

