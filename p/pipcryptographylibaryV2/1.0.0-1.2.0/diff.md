# Comparing `tmp/pipcryptographylibaryV2-1.0.0.tar.gz` & `tmp/pipcryptographylibaryV2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcryptographylibaryV2-1.0.0.tar", last modified: Fri Apr 14 20:07:28 2023, max compression
+gzip compressed data, was "pipcryptographylibaryV2-1.2.0.tar", last modified: Fri Apr 14 21:30:59 2023, max compression
```

## Comparing `pipcryptographylibaryV2-1.0.0.tar` & `pipcryptographylibaryV2-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 20:07:28.737609 pipcryptographylibaryV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-14 20:07:28.733609 pipcryptographylibaryV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 20:07:28.733609 pipcryptographylibaryV2-1.0.0/pipcryptographylibaryV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-14 20:07:28.000000 pipcryptographylibaryV2-1.0.0/pipcryptographylibaryV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 20:07:28.733609 pipcryptographylibaryV2-1.0.0/pipcryptographylibaryV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-14 20:07:28.000000 pipcryptographylibaryV2-1.0.0/pipcryptographylibaryV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-14 20:07:28.000000 pipcryptographylibaryV2-1.0.0/pipcryptographylibaryV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 20:07:28.000000 pipcryptographylibaryV2-1.0.0/pipcryptographylibaryV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 20:07:28.000000 pipcryptographylibaryV2-1.0.0/pipcryptographylibaryV2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 20:07:28.737609 pipcryptographylibaryV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      544 2023-04-14 20:07:27.000000 pipcryptographylibaryV2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:30:59.209087 pipcryptographylibaryV2-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      337 2023-04-14 21:30:59.209087 pipcryptographylibaryV2-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:30:59.209087 pipcryptographylibaryV2-1.2.0/pipcryptographylibaryV2/
+-rw-r--r--   0 root         (0) root         (0)    70957 2023-04-14 21:30:58.000000 pipcryptographylibaryV2-1.2.0/pipcryptographylibaryV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:30:59.209087 pipcryptographylibaryV2-1.2.0/pipcryptographylibaryV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      337 2023-04-14 21:30:59.000000 pipcryptographylibaryV2-1.2.0/pipcryptographylibaryV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-14 21:30:59.000000 pipcryptographylibaryV2-1.2.0/pipcryptographylibaryV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 21:30:59.000000 pipcryptographylibaryV2-1.2.0/pipcryptographylibaryV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-14 21:30:59.000000 pipcryptographylibaryV2-1.2.0/pipcryptographylibaryV2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 21:30:59.209087 pipcryptographylibaryV2-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-04-14 21:30:58.000000 pipcryptographylibaryV2-1.2.0/setup.py
```

