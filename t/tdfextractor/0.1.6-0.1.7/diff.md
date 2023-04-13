# Comparing `tmp/tdfextractor-0.1.6.tar.gz` & `tmp/tdfextractor-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdfextractor-0.1.6.tar", last modified: Thu Apr 13 22:44:55 2023, max compression
+gzip compressed data, was "tdfextractor-0.1.7.tar", last modified: Thu Apr 13 22:47:23 2023, max compression
```

## Comparing `tdfextractor-0.1.6.tar` & `tdfextractor-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 22:44:55.679804 tdfextractor-0.1.6/
--rw-rw-rw-   0        0        0      453 2023-04-13 22:44:55.679804 tdfextractor-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 22:44:55.679804 tdfextractor-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      641 2023-04-13 22:43:36.000000 tdfextractor-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:44:55.655045 tdfextractor-0.1.6/tdfextractor/
--rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.6/tdfextractor/__init__.py
--rw-rw-rw-   0        0        0       50 2023-04-13 19:43:40.000000 tdfextractor-0.1.6/tdfextractor/constants.py
--rw-rw-rw-   0        0        0     8951 2023-04-13 22:42:43.000000 tdfextractor-0.1.6/tdfextractor/ms2_extractor.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 19:43:40.000000 tdfextractor-0.1.6/tdfextractor/string_templates.py
--rw-rw-rw-   0        0        0     1602 2022-11-21 00:49:16.000000 tdfextractor-0.1.6/tdfextractor/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 22:44:55.677070 tdfextractor-0.1.6/tdfextractor.egg-info/
--rw-rw-rw-   0        0        0      453 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 22:44:55.000000 tdfextractor-0.1.6/tdfextractor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 22:44:55.678736 tdfextractor-0.1.6/test/
--rw-rw-rw-   0        0        0     2505 2023-04-13 22:38:23.000000 tdfextractor-0.1.6/test/test_ms2_extractor.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:47:23.957709 tdfextractor-0.1.7/
+-rw-rw-rw-   0        0        0      453 2023-04-13 22:47:23.957103 tdfextractor-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2022-09-29 06:42:08.000000 tdfextractor-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:47:23.957914 tdfextractor-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      641 2023-04-13 22:46:14.000000 tdfextractor-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:47:23.936122 tdfextractor-0.1.7/tdfextractor/
+-rw-rw-rw-   0        0        0        0 2022-09-29 06:09:12.000000 tdfextractor-0.1.7/tdfextractor/__init__.py
+-rw-rw-rw-   0        0        0       50 2023-04-13 19:43:40.000000 tdfextractor-0.1.7/tdfextractor/constants.py
+-rw-rw-rw-   0        0        0     8951 2023-04-13 22:42:43.000000 tdfextractor-0.1.7/tdfextractor/ms2_extractor.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 19:43:40.000000 tdfextractor-0.1.7/tdfextractor/string_templates.py
+-rw-rw-rw-   0        0        0     1602 2022-11-21 00:49:16.000000 tdfextractor-0.1.7/tdfextractor/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-13 22:47:23.953973 tdfextractor-0.1.7/tdfextractor.egg-info/
+-rw-rw-rw-   0        0        0      453 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 22:47:23.000000 tdfextractor-0.1.7/tdfextractor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 22:47:23.955309 tdfextractor-0.1.7/test/
+-rw-rw-rw-   0        0        0     2505 2023-04-13 22:38:23.000000 tdfextractor-0.1.7/test/test_ms2_extractor.py
```

### Comparing `tdfextractor-0.1.6/tdfextractor/ms2_extractor.py` & `tdfextractor-0.1.7/tdfextractor/ms2_extractor.py`

 * *Files identical despite different names*

### Comparing `tdfextractor-0.1.6/tdfextractor/string_templates.py` & `tdfextractor-0.1.7/tdfextractor/string_templates.py`

 * *Files identical despite different names*

### Comparing `tdfextractor-0.1.6/tdfextractor/utils.py` & `tdfextractor-0.1.7/tdfextractor/utils.py`

 * *Files identical despite different names*

### Comparing `tdfextractor-0.1.6/test/test_ms2_extractor.py` & `tdfextractor-0.1.7/test/test_ms2_extractor.py`

 * *Files identical despite different names*

