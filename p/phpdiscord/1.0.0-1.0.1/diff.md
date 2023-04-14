# Comparing `tmp/phpdiscord-1.0.0.tar.gz` & `tmp/phpdiscord-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phpdiscord-1.0.0.tar", last modified: Fri Apr 14 13:28:14 2023, max compression
+gzip compressed data, was "phpdiscord-1.0.1.tar", last modified: Fri Apr 14 14:42:45 2023, max compression
```

## Comparing `phpdiscord-1.0.0.tar` & `phpdiscord-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 13:28:14.708744 phpdiscord-1.0.0/
--rw-rw----   0 root         (0) everybody  (9997)      221 2023-04-14 13:28:14.704744 phpdiscord-1.0.0/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1439 2023-04-10 13:24:56.000000 phpdiscord-1.0.0/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 13:28:14.640745 phpdiscord-1.0.0/phpdiscord/
--rw-rw----   0 root         (0) everybody  (9997)     2296 2023-04-14 13:24:00.000000 phpdiscord-1.0.0/phpdiscord/phpdiscord.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 13:28:14.696745 phpdiscord-1.0.0/phpdiscord.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      221 2023-04-14 13:28:14.000000 phpdiscord-1.0.0/phpdiscord.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      179 2023-04-14 13:28:14.000000 phpdiscord-1.0.0/phpdiscord.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-14 13:28:14.000000 phpdiscord-1.0.0/phpdiscord.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       11 2023-04-14 13:28:14.000000 phpdiscord-1.0.0/phpdiscord.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-14 13:28:14.712745 phpdiscord-1.0.0/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      237 2023-04-14 13:27:06.000000 phpdiscord-1.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 14:42:45.036392 phpdiscord-1.0.1/
+-rw-rw----   0 root         (0) everybody  (9997)      221 2023-04-14 14:42:45.028392 phpdiscord-1.0.1/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1439 2023-04-10 13:24:56.000000 phpdiscord-1.0.1/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 14:42:44.968392 phpdiscord-1.0.1/phpdiscord/
+-rw-rw----   0 root         (0) everybody  (9997)     2296 2023-04-14 13:24:00.000000 phpdiscord-1.0.1/phpdiscord/phpdiscord.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-14 14:42:45.020392 phpdiscord-1.0.1/phpdiscord.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      221 2023-04-14 14:42:44.000000 phpdiscord-1.0.1/phpdiscord.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      179 2023-04-14 14:42:44.000000 phpdiscord-1.0.1/phpdiscord.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-14 14:42:44.000000 phpdiscord-1.0.1/phpdiscord.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       11 2023-04-14 14:42:44.000000 phpdiscord-1.0.1/phpdiscord.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-14 14:42:45.036392 phpdiscord-1.0.1/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      237 2023-04-14 14:42:04.000000 phpdiscord-1.0.1/setup.py
```

### Comparing `phpdiscord-1.0.0/README.md` & `phpdiscord-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `phpdiscord-1.0.0/phpdiscord/phpdiscord.py` & `phpdiscord-1.0.1/phpdiscord/phpdiscord.py`

 * *Files identical despite different names*

