# Comparing `tmp/matemuzb-0.0.1.tar.gz` & `tmp/matemuzb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matemuzb-0.0.1.tar", last modified: Fri Apr 14 09:34:37 2023, max compression
+gzip compressed data, was "matemuzb-0.0.2.tar", last modified: Fri Apr 14 09:50:19 2023, max compression
```

## Comparing `matemuzb-0.0.1.tar` & `matemuzb-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:34:37.241712 matemuzb-0.0.1/
--rw-rw-rw-   0        0        0      166 2023-04-14 09:34:37.241712 matemuzb-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 09:34:37.237722 matemuzb-0.0.1/matemuzb/
--rw-rw-rw-   0        0        0      477 2023-04-14 09:34:12.000000 matemuzb-0.0.1/matemuzb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:34:37.240715 matemuzb-0.0.1/matemuzb.egg-info/
--rw-rw-rw-   0        0        0      166 2023-04-14 09:34:37.000000 matemuzb-0.0.1/matemuzb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-04-14 09:34:37.000000 matemuzb-0.0.1/matemuzb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:34:37.000000 matemuzb-0.0.1/matemuzb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 09:34:37.000000 matemuzb-0.0.1/matemuzb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 09:34:37.241712 matemuzb-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      217 2023-04-14 09:34:34.000000 matemuzb-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:50:19.162273 matemuzb-0.0.2/
+-rw-rw-rw-   0        0        0      154 2023-04-14 09:50:19.162273 matemuzb-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 09:50:19.158970 matemuzb-0.0.2/matemuzb/
+-rw-rw-rw-   0        0        0      701 2023-04-14 09:49:53.000000 matemuzb-0.0.2/matemuzb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:50:19.161274 matemuzb-0.0.2/matemuzb.egg-info/
+-rw-rw-rw-   0        0        0      154 2023-04-14 09:50:19.000000 matemuzb-0.0.2/matemuzb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-04-14 09:50:19.000000 matemuzb-0.0.2/matemuzb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:50:19.000000 matemuzb-0.0.2/matemuzb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 09:50:19.000000 matemuzb-0.0.2/matemuzb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:50:19.162273 matemuzb-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      205 2023-04-14 09:50:09.000000 matemuzb-0.0.2/setup.py
```

