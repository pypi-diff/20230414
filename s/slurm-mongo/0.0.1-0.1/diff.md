# Comparing `tmp/slurm_mongo-0.0.1.tar.gz` & `tmp/slurm_mongo-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurm_mongo-0.0.1.tar", last modified: Fri Apr 14 12:52:30 2023, max compression
+gzip compressed data, was "slurm_mongo-0.1.tar", last modified: Fri Apr 14 09:30:17 2023, max compression
```

## Comparing `slurm_mongo-0.0.1.tar` & `slurm_mongo-0.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:30.920234 slurm_mongo-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-14 12:52:30.920234 slurm_mongo-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-14 12:52:21.000000 slurm_mongo-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:52:30.920234 slurm_mongo-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-14 12:52:24.000000 slurm_mongo-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:30.920234 slurm_mongo-0.0.1/slurm_mongo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-14 12:52:30.000000 slurm_mongo-0.0.1/slurm_mongo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 12:52:30.000000 slurm_mongo-0.0.1/slurm_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:52:30.000000 slurm_mongo-0.0.1/slurm_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 12:52:30.000000 slurm_mongo-0.0.1/slurm_mongo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 12:52:30.000000 slurm_mongo-0.0.1/slurm_mongo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:52:30.000000 slurm_mongo-0.0.1/slurm_mongo.egg-info/top_level.txt
+drwxrwxr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-14 09:30:17.772435 slurm_mongo-0.1/
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)      686 2023-04-14 09:30:17.768435 slurm_mongo-0.1/PKG-INFO
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-14 09:30:17.772435 slurm_mongo-0.1/setup.cfg
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)      975 2023-04-14 08:32:10.000000 slurm_mongo-0.1/setup.py
+drwxrwxr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-14 09:30:17.768435 slurm_mongo-0.1/slurm_mongo.egg-info/
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)      686 2023-04-14 09:30:17.000000 slurm_mongo-0.1/slurm_mongo.egg-info/PKG-INFO
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)      220 2023-04-14 09:30:17.000000 slurm_mongo-0.1/slurm_mongo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-14 09:30:17.000000 slurm_mongo-0.1/slurm_mongo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)       60 2023-04-14 09:30:17.000000 slurm_mongo-0.1/slurm_mongo.egg-info/entry_points.txt
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)        8 2023-04-14 09:30:17.000000 slurm_mongo-0.1/slurm_mongo.egg-info/requires.txt
+-rw-rw-r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-14 09:30:17.000000 slurm_mongo-0.1/slurm_mongo.egg-info/top_level.txt
```

