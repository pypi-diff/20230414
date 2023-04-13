# Comparing `tmp/codon-jit-0.1.3.tar.gz` & `tmp/codon-jit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codon-jit-0.1.3.tar", last modified: Mon Feb  6 03:46:45 2023, max compression
+gzip compressed data, was "codon-jit-0.1.4.tar", last modified: Thu Apr 13 21:43:26 2023, max compression
```

## Comparing `codon-jit-0.1.3.tar` & `codon-jit-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 03:46:45.873612 codon-jit-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 03:29:43.000000 codon-jit-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-06 03:46:45.873612 codon-jit-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-06 03:29:43.000000 codon-jit-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 03:46:45.869612 codon-jit-0.1.3/codon/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-06 03:29:43.000000 codon-jit-0.1.3/codon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-02-06 03:29:43.000000 codon-jit-0.1.3/codon/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-06 03:29:43.000000 codon-jit-0.1.3/codon/jit.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-02-06 03:29:43.000000 codon-jit-0.1.3/codon/jit.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-06 03:30:09.000000 codon-jit-0.1.3/codon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 03:46:45.873612 codon-jit-0.1.3/codon_jit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-06 03:46:45.000000 codon-jit-0.1.3/codon_jit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-06 03:46:45.000000 codon-jit-0.1.3/codon_jit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 03:46:45.000000 codon-jit-0.1.3/codon_jit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-06 03:46:45.000000 codon-jit-0.1.3/codon_jit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-06 03:46:45.000000 codon-jit-0.1.3/codon_jit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-06 03:29:43.000000 codon-jit-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 03:46:45.873612 codon-jit-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-02-06 03:29:43.000000 codon-jit-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:43:26.244500 codon-jit-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:26:20.000000 codon-jit-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-13 21:43:26.244500 codon-jit-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-13 21:26:20.000000 codon-jit-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:43:26.240500 codon-jit-0.1.4/codon/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-13 21:26:20.000000 codon-jit-0.1.4/codon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-13 21:26:20.000000 codon-jit-0.1.4/codon/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-13 21:26:20.000000 codon-jit-0.1.4/codon/jit.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-13 21:26:20.000000 codon-jit-0.1.4/codon/jit.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-13 21:26:50.000000 codon-jit-0.1.4/codon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:43:26.244500 codon-jit-0.1.4/codon_jit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-13 21:43:26.000000 codon-jit-0.1.4/codon_jit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-13 21:43:26.000000 codon-jit-0.1.4/codon_jit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:43:26.000000 codon-jit-0.1.4/codon_jit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 21:43:26.000000 codon-jit-0.1.4/codon_jit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 21:43:26.000000 codon-jit-0.1.4/codon_jit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 21:26:20.000000 codon-jit-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:43:26.244500 codon-jit-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-13 21:26:20.000000 codon-jit-0.1.4/setup.py
```

### Comparing `codon-jit-0.1.3/codon/decorator.py` & `codon-jit-0.1.4/codon/decorator.py`

 * *Files identical despite different names*

### Comparing `codon-jit-0.1.3/codon/jit.pxd` & `codon-jit-0.1.4/codon/jit.pxd`

 * *Files identical despite different names*

### Comparing `codon-jit-0.1.3/codon/jit.pyx` & `codon-jit-0.1.4/codon/jit.pyx`

 * *Files identical despite different names*

### Comparing `codon-jit-0.1.3/setup.py` & `codon-jit-0.1.4/setup.py`

 * *Files identical despite different names*

