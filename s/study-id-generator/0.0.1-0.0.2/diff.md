# Comparing `tmp/study_id_generator-0.0.1.tar.gz` & `tmp/study_id_generator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "study_id_generator-0.0.1.tar", last modified: Thu Apr 13 18:46:20 2023, max compression
+gzip compressed data, was "study_id_generator-0.0.2.tar", last modified: Fri Apr 14 01:43:25 2023, max compression
```

## Comparing `study_id_generator-0.0.1.tar` & `study_id_generator-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adpatter (223969) nobodyldap (65500)        0 2023-04-13 18:46:20.904306 study_id_generator-0.0.1/
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)      588 2023-04-13 18:46:20.904306 study_id_generator-0.0.1/PKG-INFO
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)       20 2023-04-13 18:45:43.000000 study_id_generator-0.0.1/README.md
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)      844 2023-04-13 18:45:43.000000 study_id_generator-0.0.1/pyproject.toml
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)       38 2023-04-13 18:46:20.904306 study_id_generator-0.0.1/setup.cfg
-drwxr-xr-x   0 adpatter (223969) nobodyldap (65500)        0 2023-04-13 18:46:20.903306 study_id_generator-0.0.1/src/
-drwxr-xr-x   0 adpatter (223969) nobodyldap (65500)        0 2023-04-13 18:46:20.903306 study_id_generator-0.0.1/src/study_id_generator/
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)        0 2023-04-13 18:45:43.000000 study_id_generator-0.0.1/src/study_id_generator/__init__.py
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)     4741 2023-04-13 18:45:43.000000 study_id_generator-0.0.1/src/study_id_generator/__main__.py
-drwxr-xr-x   0 adpatter (223969) nobodyldap (65500)        0 2023-04-13 18:46:20.904306 study_id_generator-0.0.1/src/study_id_generator.egg-info/
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)      588 2023-04-13 18:46:20.000000 study_id_generator-0.0.1/src/study_id_generator.egg-info/PKG-INFO
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)      323 2023-04-13 18:46:20.000000 study_id_generator-0.0.1/src/study_id_generator.egg-info/SOURCES.txt
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)        1 2023-04-13 18:46:20.000000 study_id_generator-0.0.1/src/study_id_generator.egg-info/dependency_links.txt
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)       86 2023-04-13 18:46:20.000000 study_id_generator-0.0.1/src/study_id_generator.egg-info/requires.txt
--rw-r--r--   0 adpatter (223969) nobodyldap (65500)       19 2023-04-13 18:46:20.000000 study_id_generator-0.0.1/src/study_id_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 01:43:25.312641 study_id_generator-0.0.2/
+-rw-rw-rw-   0        0        0     1380 2023-04-14 01:43:25.312641 study_id_generator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      798 2023-04-14 01:28:57.000000 study_id_generator-0.0.2/README.md
+-rw-rw-rw-   0        0        0      873 2023-04-14 01:42:56.000000 study_id_generator-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 01:43:25.312641 study_id_generator-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 01:43:25.283053 study_id_generator-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 01:43:25.295918 study_id_generator-0.0.2/src/study_id_generator/
+-rw-rw-rw-   0        0        0        0 2023-04-13 18:17:34.000000 study_id_generator-0.0.2/src/study_id_generator/__init__.py
+-rw-rw-rw-   0        0        0     5676 2023-04-14 01:31:11.000000 study_id_generator-0.0.2/src/study_id_generator/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 01:43:25.304622 study_id_generator-0.0.2/src/study_id_generator.egg-info/
+-rw-rw-rw-   0        0        0     1380 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-14 01:43:25.000000 study_id_generator-0.0.2/src/study_id_generator.egg-info/top_level.txt
```

### Comparing `study_id_generator-0.0.1/pyproject.toml` & `study_id_generator-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "study_id_generator"
-version = "0.0.1"
-authors = [
-    { name="Sushant Obeja", email="sobeja@umich.edu" },
-    { name="Adam Patterson", email="adpatter@umich.edu" },
-]
-description = "Study ID Generator."
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    'requests >=2.28, < 3',
-    'scikit-learn >= 1.1, < 2',
-    'pandas >= 1.5, < 2',
-    'numpy >= 1.23, < 2',
-    'wxpython >= 4.1, < 5'
-]
-
-[project.urls]
-"Homepage" = "https://git.umms.med.umich.edu/feldman-lab/study_id_generator"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "study_id_generator"
+version = "0.0.2"
+authors = [
+    { name="Sushant Obeja", email="sobeja@umich.edu" },
+    { name="Adam Patterson", email="adpatter@umich.edu" },
+]
+description = "Study ID Generator."
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    'requests >=2.28, < 3',
+    'scikit-learn >= 1.1, < 2',
+    'pandas >= 1.5, < 2',
+    'numpy >= 1.23, < 2',
+    'wxpython >= 4.1, < 5'
+]
+
+[project.urls]
+"Homepage" = "https://git.umms.med.umich.edu/feldman-lab/study_id_generator"
 "Bug Tracker" = "https://git.umms.med.umich.edu/feldman-lab/study_id_generator/-/issues"
```

