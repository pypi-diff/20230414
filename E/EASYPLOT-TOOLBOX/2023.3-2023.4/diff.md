# Comparing `tmp/EASYPLOT_TOOLBOX-2023.3.tar.gz` & `tmp/EASYPLOT_TOOLBOX-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EASYPLOT_TOOLBOX-2023.3.tar", last modified: Sat Feb 18 22:02:44 2023, max compression
+gzip compressed data, was "EASYPLOT_TOOLBOX-2023.4.tar", last modified: Fri Apr 14 12:06:10 2023, max compression
```

## Comparing `EASYPLOT_TOOLBOX-2023.3.tar` & `EASYPLOT_TOOLBOX-2023.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-18 22:02:44.858969 EASYPLOT_TOOLBOX-2023.3/
-drwxrwxrwx   0        0        0        0 2023-02-18 22:02:44.846966 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX/
--rw-rw-rw-   0        0        0     3159 2023-02-18 21:20:10.000000 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX/EASYPLOT.py
--rw-rw-rw-   0        0        0       23 2023-02-18 15:01:30.000000 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-18 22:02:44.856968 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX.egg-info/
--rw-rw-rw-   0        0        0      271 2023-02-18 22:02:44.000000 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-02-18 22:02:44.000000 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-18 22:02:44.000000 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-02-18 22:02:44.000000 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-02-18 22:02:44.000000 EASYPLOT_TOOLBOX-2023.3/EASYPLOT_TOOLBOX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      271 2023-02-18 22:02:44.857969 EASYPLOT_TOOLBOX-2023.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-02-18 22:02:44.858969 EASYPLOT_TOOLBOX-2023.3/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-02-18 22:00:47.000000 EASYPLOT_TOOLBOX-2023.3/setup.py
+drwxrwxr-x   0 mateus    (1000) mateus    (1000)        0 2023-04-14 12:06:10.755847 EASYPLOT_TOOLBOX-2023.4/
+drwxrwxr-x   0 mateus    (1000) mateus    (1000)        0 2023-04-14 12:06:10.751847 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX/
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)    13335 2023-04-13 15:49:20.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX/EASYPLOT.py
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)       23 2023-04-13 15:05:35.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX/__init__.py
+drwxrwxr-x   0 mateus    (1000) mateus    (1000)        0 2023-04-14 12:06:10.755847 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)      426 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/PKG-INFO
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)      265 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)        1 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)       19 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/requires.txt
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)       17 2023-04-14 12:06:10.000000 EASYPLOT_TOOLBOX-2023.4/EASYPLOT_TOOLBOX.egg-info/top_level.txt
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)      426 2023-04-14 12:06:10.755847 EASYPLOT_TOOLBOX-2023.4/PKG-INFO
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)       38 2023-04-14 12:06:10.755847 EASYPLOT_TOOLBOX-2023.4/setup.cfg
+-rw-rw-r--   0 mateus    (1000) mateus    (1000)      913 2023-04-14 12:05:08.000000 EASYPLOT_TOOLBOX-2023.4/setup.py
```

