# Comparing `tmp/visualimiss-0.0.3.tar.gz` & `tmp/visualimiss-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualimiss-0.0.3.tar", last modified: Fri Apr 14 16:05:16 2023, max compression
+gzip compressed data, was "visualimiss-0.0.4.tar", last modified: Fri Apr 14 16:31:09 2023, max compression
```

## Comparing `visualimiss-0.0.3.tar` & `visualimiss-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:05:16.401132 visualimiss-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-04-14 15:05:45.000000 visualimiss-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      846 2023-04-14 16:05:16.399117 visualimiss-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-14 15:46:13.000000 visualimiss-0.0.3/README.md
--rw-rw-rw-   0        0        0      632 2023-04-14 16:04:58.000000 visualimiss-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 16:05:16.401132 visualimiss-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 16:05:16.379415 visualimiss-0.0.3/visualimiss/
--rw-rw-rw-   0        0        0       94 2023-04-14 16:04:41.000000 visualimiss-0.0.3/visualimiss/__init__.py
--rw-rw-rw-   0        0        0      431 2023-04-13 16:51:12.000000 visualimiss-0.0.3/visualimiss/utils.py
--rw-rw-rw-   0        0        0     2467 2023-04-14 02:12:37.000000 visualimiss-0.0.3/visualimiss/visualimiss.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:05:16.397001 visualimiss-0.0.3/visualimiss.egg-info/
--rw-rw-rw-   0        0        0      846 2023-04-14 16:05:16.000000 visualimiss-0.0.3/visualimiss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-04-14 16:05:16.000000 visualimiss-0.0.3/visualimiss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:05:16.000000 visualimiss-0.0.3/visualimiss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-14 16:05:16.000000 visualimiss-0.0.3/visualimiss.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 16:31:09.996724 visualimiss-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2023-04-14 15:05:45.000000 visualimiss-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      767 2023-04-14 16:31:09.995724 visualimiss-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-04-14 16:28:41.000000 visualimiss-0.0.4/README.md
+-rw-rw-rw-   0        0        0      514 2023-04-14 16:30:55.000000 visualimiss-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 16:31:09.996724 visualimiss-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 16:31:09.983693 visualimiss-0.0.4/visualimiss/
+-rw-rw-rw-   0        0        0       94 2023-04-14 16:04:41.000000 visualimiss-0.0.4/visualimiss/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-04-13 16:51:12.000000 visualimiss-0.0.4/visualimiss/utils.py
+-rw-rw-rw-   0        0        0     2467 2023-04-14 02:12:37.000000 visualimiss-0.0.4/visualimiss/visualimiss.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:31:09.994723 visualimiss-0.0.4/visualimiss.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-04-14 16:31:09.000000 visualimiss-0.0.4/visualimiss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-04-14 16:31:09.000000 visualimiss-0.0.4/visualimiss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:31:09.000000 visualimiss-0.0.4/visualimiss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 16:31:09.000000 visualimiss-0.0.4/visualimiss.egg-info/top_level.txt
```

### Comparing `visualimiss-0.0.3/LICENSE` & `visualimiss-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `visualimiss-0.0.3/visualimiss/visualimiss.py` & `visualimiss-0.0.4/visualimiss/visualimiss.py`

 * *Files identical despite different names*

