# Comparing `tmp/aws-ket-0.1.2.tar.gz` & `tmp/aws-ket-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ket-0.1.2.tar", last modified: Fri Apr 14 14:13:09 2023, max compression
+gzip compressed data, was "aws-ket-0.1.3.tar", last modified: Fri Apr 14 18:57:23 2023, max compression
```

## Comparing `aws-ket-0.1.2.tar` & `aws-ket-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 14:13:09.846471 aws-ket-0.1.2/
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     1452 2023-03-18 01:01:48.000000 aws-ket-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 sayefiqbal   (502) staff       (20)    11357 2023-02-09 13:04:42.000000 aws-ket-0.1.2/LICENSE
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      396 2023-03-24 00:07:58.000000 aws-ket-0.1.2/MANIFEST.in
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2150 2023-04-14 14:05:00.000000 aws-ket-0.1.2/Makefile
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      329 2023-04-14 14:13:09.846202 aws-ket-0.1.2/PKG-INFO
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2699 2023-04-14 13:55:20.000000 aws-ket-0.1.2/README.md
-drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 14:13:09.845838 aws-ket-0.1.2/aws_ket.egg-info/
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      329 2023-04-14 14:13:09.000000 aws-ket-0.1.2/aws_ket.egg-info/PKG-INFO
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      202 2023-04-14 14:13:09.000000 aws-ket-0.1.2/aws_ket.egg-info/SOURCES.txt
--rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-04-14 14:13:09.000000 aws-ket-0.1.2/aws_ket.egg-info/dependency_links.txt
--rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-04-14 14:13:09.000000 aws-ket-0.1.2/aws_ket.egg-info/top_level.txt
--rw-r--r--   0 sayefiqbal   (502) staff       (20)     2253 2023-04-14 14:05:00.000000 aws-ket-0.1.2/pyproject.toml
--rw-r--r--   0 sayefiqbal   (502) staff       (20)       38 2023-04-14 14:13:09.846563 aws-ket-0.1.2/setup.cfg
--rw-r--r--   0 sayefiqbal   (502) staff       (20)      523 2023-04-14 14:05:00.000000 aws-ket-0.1.2/setup.py
+drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 18:57:23.390257 aws-ket-0.1.3/
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     1452 2023-03-18 01:01:48.000000 aws-ket-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)    11357 2023-02-09 13:04:42.000000 aws-ket-0.1.3/LICENSE
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      396 2023-03-24 00:07:58.000000 aws-ket-0.1.3/MANIFEST.in
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     2150 2023-04-14 14:05:00.000000 aws-ket-0.1.3/Makefile
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     3061 2023-04-14 18:57:23.389952 aws-ket-0.1.3/PKG-INFO
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     2699 2023-04-14 13:55:20.000000 aws-ket-0.1.3/README.md
+drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 18:57:23.388644 aws-ket-0.1.3/aws_ket.egg-info/
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     3061 2023-04-14 18:57:23.000000 aws-ket-0.1.3/aws_ket.egg-info/PKG-INFO
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      216 2023-04-14 18:57:23.000000 aws-ket-0.1.3/aws_ket.egg-info/SOURCES.txt
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-04-14 18:57:23.000000 aws-ket-0.1.3/aws_ket.egg-info/dependency_links.txt
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)        1 2023-04-14 18:57:23.000000 aws-ket-0.1.3/aws_ket.egg-info/top_level.txt
+drwxr-xr-x   0 sayefiqbal   (502) staff       (20)        0 2023-04-14 18:57:23.389091 aws-ket-0.1.3/awsket/
+-rwxr-xr-x   0 sayefiqbal   (502) staff       (20)     2882 2023-04-14 14:05:00.000000 aws-ket-0.1.3/awsket/app.py
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)     2253 2023-04-14 18:53:37.000000 aws-ket-0.1.3/pyproject.toml
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)       38 2023-04-14 18:57:23.390359 aws-ket-0.1.3/setup.cfg
+-rw-r--r--   0 sayefiqbal   (502) staff       (20)      772 2023-04-14 18:53:37.000000 aws-ket-0.1.3/setup.py
```

### Comparing `aws-ket-0.1.2/CONTRIBUTING.md` & `aws-ket-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.2/LICENSE` & `aws-ket-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.2/Makefile` & `aws-ket-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.2/README.md` & `aws-ket-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-ket-0.1.2/pyproject.toml` & `aws-ket-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "aws-ket"
 authors = [{name = "Sayef Iqbal", email = "si2400@columbia.edu"}]
 description="Utility tool to encrypt data using AWS KMS and store it in preferred backend."
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.9"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

