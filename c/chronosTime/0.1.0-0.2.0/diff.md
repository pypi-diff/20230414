# Comparing `tmp/chronosTime-0.1.0.tar.gz` & `tmp/chronosTime-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronosTime-0.1.0.tar", last modified: Fri Apr 14 00:13:13 2023, max compression
+gzip compressed data, was "chronosTime-0.2.0.tar", last modified: Fri Apr 14 00:19:00 2023, max compression
```

## Comparing `chronosTime-0.1.0.tar` & `chronosTime-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 00:13:13.489191 chronosTime-0.1.0/
--rw-rw-rw-   0        0        0      548 2023-04-14 00:13:13.489191 chronosTime-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 00:13:13.487196 chronosTime-0.1.0/chronosTime.egg-info/
--rw-rw-rw-   0        0        0      548 2023-04-14 00:13:13.000000 chronosTime-0.1.0/chronosTime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-04-14 00:13:13.000000 chronosTime-0.1.0/chronosTime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:13:13.000000 chronosTime-0.1.0/chronosTime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 00:13:13.000000 chronosTime-0.1.0/chronosTime.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 00:13:13.000000 chronosTime-0.1.0/chronosTime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 00:13:13.490190 chronosTime-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      765 2023-04-14 00:12:42.000000 chronosTime-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:19:00.972815 chronosTime-0.2.0/
+-rw-rw-rw-   0        0        0      703 2023-04-14 00:19:00.971819 chronosTime-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 00:19:00.968826 chronosTime-0.2.0/chronosTime.egg-info/
+-rw-rw-rw-   0        0        0      703 2023-04-14 00:19:00.000000 chronosTime-0.2.0/chronosTime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-04-14 00:19:00.000000 chronosTime-0.2.0/chronosTime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:19:00.000000 chronosTime-0.2.0/chronosTime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 00:19:00.000000 chronosTime-0.2.0/chronosTime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:19:00.000000 chronosTime-0.2.0/chronosTime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 00:19:00.972815 chronosTime-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-04-14 00:18:54.000000 chronosTime-0.2.0/setup.py
```

