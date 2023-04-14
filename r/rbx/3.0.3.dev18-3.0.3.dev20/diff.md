# Comparing `tmp/rbx-3.0.3.dev18.tar.gz` & `tmp/rbx-3.0.3.dev20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbx-3.0.3.dev18.tar", last modified: Wed Jan 11 17:27:19 2023, max compression
+gzip compressed data, was "rbx-3.0.3.dev20.tar", last modified: Fri Apr 14 14:31:26 2023, max compression
```

## Comparing `rbx-3.0.3.dev18.tar` & `rbx-3.0.3.dev20.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.363740 rbx-3.0.3.dev18/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-11 17:27:19.363740 rbx-3.0.3.dev18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.355740 rbx-3.0.3.dev18/rbx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/auth/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/auth/keystore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/aws/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/buildtools/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/buildtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-11 17:27:13.000000 rbx-3.0.3.dev18/rbx/buildtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/buildtools/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/buildtools/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/buildtools/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/buildtools/tasks/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/buildtools/tasks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/buildtools/tasks/pypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/clients/adsquare.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/clients/broadsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/clients/oxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/clients/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/clients/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/clients/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/clients/uslicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/gcp/cloud_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/geo/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/geo/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/geo/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/geo/packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/manifest/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/manifest/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/manifest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/queues/
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/queues/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/queues/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.359740 rbx-3.0.3.dev18/rbx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/utils/mdm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.363740 rbx-3.0.3.dev18/rbx/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-01-11 17:26:54.000000 rbx-3.0.3.dev18/rbx/web/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:27:19.355740 rbx-3.0.3.dev18/rbx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-11 17:27:19.000000 rbx-3.0.3.dev18/rbx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-11 17:27:19.000000 rbx-3.0.3.dev18/rbx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 17:27:19.000000 rbx-3.0.3.dev18/rbx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-11 17:27:19.000000 rbx-3.0.3.dev18/rbx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-01-11 17:27:19.000000 rbx-3.0.3.dev18/rbx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-11 17:27:19.000000 rbx-3.0.3.dev18/rbx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 17:27:19.363740 rbx-3.0.3.dev18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-01-11 17:27:13.000000 rbx-3.0.3.dev18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.718585 rbx-3.0.3.dev20/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 14:31:26.718585 rbx-3.0.3.dev20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.710585 rbx-3.0.3.dev20/rbx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.710585 rbx-3.0.3.dev20/rbx/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/auth/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/auth/keystore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.710585 rbx-3.0.3.dev20/rbx/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/aws/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.714585 rbx-3.0.3.dev20/rbx/buildtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/buildtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-14 14:31:25.000000 rbx-3.0.3.dev20/rbx/buildtools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.714585 rbx-3.0.3.dev20/rbx/buildtools/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/buildtools/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/buildtools/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/buildtools/tasks/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/buildtools/tasks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/buildtools/tasks/pypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.714585 rbx-3.0.3.dev20/rbx/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/clients/adsquare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/clients/broadsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/clients/oxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/clients/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/clients/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/clients/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/clients/uslicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.714585 rbx-3.0.3.dev20/rbx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/gcp/cloud_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/gcp/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.718585 rbx-3.0.3.dev20/rbx/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/geo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/geo/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/geo/packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.718585 rbx-3.0.3.dev20/rbx/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/manifest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/manifest/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/manifest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.718585 rbx-3.0.3.dev20/rbx/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/queues/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/queues/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.718585 rbx-3.0.3.dev20/rbx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/utils/mdm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.718585 rbx-3.0.3.dev20/rbx/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-14 14:31:10.000000 rbx-3.0.3.dev20/rbx/web/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:31:26.710585 rbx-3.0.3.dev20/rbx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-14 14:31:26.000000 rbx-3.0.3.dev20/rbx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-14 14:31:26.000000 rbx-3.0.3.dev20/rbx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:31:26.000000 rbx-3.0.3.dev20/rbx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 14:31:26.000000 rbx-3.0.3.dev20/rbx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-14 14:31:26.000000 rbx-3.0.3.dev20/rbx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 14:31:26.000000 rbx-3.0.3.dev20/rbx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:31:26.718585 rbx-3.0.3.dev20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-14 14:31:25.000000 rbx-3.0.3.dev20/setup.py
```

### Comparing `rbx-3.0.3.dev18/LICENSE` & `rbx-3.0.3.dev20/LICENSE`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/PKG-INFO` & `rbx-3.0.3.dev20/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.0.3.dev18
+Version: 3.0.3.dev20
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rbx-3.0.3.dev18/rbx/auth/decorators.py` & `rbx-3.0.3.dev20/rbx/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/auth/keystore.py` & `rbx-3.0.3.dev20/rbx/auth/keystore.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/aws/s3.py` & `rbx-3.0.3.dev20/rbx/aws/s3.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/buildtools/tasks/deploy.py` & `rbx-3.0.3.dev20/rbx/buildtools/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/buildtools/tasks/image.py` & `rbx-3.0.3.dev20/rbx/buildtools/tasks/image.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/buildtools/tasks/misc.py` & `rbx-3.0.3.dev20/rbx/buildtools/tasks/misc.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/clients/__init__.py` & `rbx-3.0.3.dev20/rbx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/clients/adsquare.py` & `rbx-3.0.3.dev20/rbx/clients/adsquare.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/clients/broadsign.py` & `rbx-3.0.3.dev20/rbx/clients/broadsign.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/clients/oxr.py` & `rbx-3.0.3.dev20/rbx/clients/oxr.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/clients/panels.py` & `rbx-3.0.3.dev20/rbx/clients/panels.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/clients/reporting.py` & `rbx-3.0.3.dev20/rbx/clients/reporting.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,31 +14,44 @@
         self.token = token
 
     @property
     def auth(self):
         """The Reporting Service uses Digest Authentication."""
         return HttpAuth(self.token, key="X-RBX-TOKEN")
 
-    def create_schedule(self, body, campaign, cron, format, name, recipients, reports):
+    def create_schedule(
+        self,
+        body,
+        campaign,
+        cron,
+        format,
+        name,
+        recipients,
+        reports,
+        api_version=None,
+    ):
         """Create a scheduled job.
 
         Return the job_id of the job just created.
         """
-        response = self._post(
-            "/schedule",
-            data={
-                "body": body,
-                "campaign": campaign,
-                "cron": cron,
-                "format": format,
-                "name": name,
-                "recipients": recipients,
-                "reports": reports,
-            },
-        )
+        data = {
+            "body": body,
+            "campaign": campaign,
+            "cron": cron,
+            "format": format,
+            "name": name,
+            "recipients": recipients,
+            "reports": reports,
+        }
+
+        if api_version is not None:
+            data["api_version"] = api_version
+
+        response = self._post("/schedule", data=data)
+
         return response.get("job_id")
 
     def delete_schedule(self, job_id):
         """Create the scheduled job."""
         response = self._post("/schedule/delete", data={"job_id": job_id})
         return response.get("job_id")
 
@@ -49,30 +62,42 @@
 
     def resume_schedule(self, job_id):
         """Resume the scheduled job."""
         response = self._post("/schedule/resume", data={"job_id": job_id})
         return response.get("job_id")
 
     def update_schedule(
-        self, body, campaign, cron, format, job_id, name, recipients, reports
+        self,
+        body,
+        campaign,
+        cron,
+        format,
+        job_id,
+        name,
+        recipients,
+        reports,
+        api_version=None,
     ):
         """Update the scheduled job."""
-        response = self._post(
-            "/schedule",
-            data={
-                "body": body,
-                "campaign": campaign,
-                "cron": cron,
-                "format": format,
-                "job_id": job_id,
-                "name": name,
-                "recipients": recipients,
-                "reports": reports,
-            },
-        )
+        data = {
+            "body": body,
+            "campaign": campaign,
+            "cron": cron,
+            "format": format,
+            "job_id": job_id,
+            "name": name,
+            "recipients": recipients,
+            "reports": reports,
+        }
+
+        if api_version is not None:
+            data["api_version"] = api_version
+
+        response = self._post("/schedule", data=data)
+
         return response.get("job_id")
 
     def get_report(
         self,
         breakdowns,
         metrics=None,
         custom_metrics=None,
```

### Comparing `rbx-3.0.3.dev18/rbx/clients/retry.py` & `rbx-3.0.3.dev20/rbx/clients/retry.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/clients/uslicer.py` & `rbx-3.0.3.dev20/rbx/clients/uslicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
                     )
                 else:
                     raise
 
         results = []
 
         for row in response["rows"]:
-
             # Annoyingly Iponweb have decided to call the Panel ID field 'supply.panel_id',
             # which is not namedtuple-friendly. So here we apply that logic to all fields in an
             # attempt to be future-proof, namely to remove all dot prefixes.
             # Plus, empty/null breakdowns get replaced with custom value (which defaults to 'N/A').
             fields = {}
             for i, breakdown in enumerate(breakdowns):
                 fields[breakdown.split(".")[-1]] = row["name"][i] or none_default
```

### Comparing `rbx-3.0.3.dev18/rbx/exceptions.py` & `rbx-3.0.3.dev20/rbx/exceptions.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/gcp/cloud_tasks.py` & `rbx-3.0.3.dev20/rbx/gcp/cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/gcp/pubsub.py` & `rbx-3.0.3.dev20/rbx/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/gcp/storage.py` & `rbx-3.0.3.dev20/rbx/gcp/storage.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/geo/__init__.py` & `rbx-3.0.3.dev20/rbx/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/geo/cli.py` & `rbx-3.0.3.dev20/rbx/geo/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/geo/maps.py` & `rbx-3.0.3.dev20/rbx/geo/maps.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/geo/packer.py` & `rbx-3.0.3.dev20/rbx/geo/packer.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
         - Must be read after countries.
 
         """
         database = path.join(self.db_path, "GeoIP2-City-Locations-en.csv")
         with open(database, encoding=self.encoding) as fd:
             reader = csv.DictReader(fd)
             for row in reader:
-
                 # Skip entries with no city.
                 if not row["city_name"]:
                     continue
 
                 # Case 1: both sub-divisions are present; the region code is compiled from both
                 # codes, separated by a dot (i.e.: '<sd1_code>.<sd2_code>'); the second division
                 # name is used as the region name, with the first division in brackets.
```

### Comparing `rbx-3.0.3.dev18/rbx/logging.py` & `rbx-3.0.3.dev20/rbx/logging.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/manifest/cli.py` & `rbx-3.0.3.dev20/rbx/manifest/cli.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/manifest/processor.py` & `rbx-3.0.3.dev20/rbx/manifest/processor.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/manifest/utils.py` & `rbx-3.0.3.dev20/rbx/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/queues/__init__.py` & `rbx-3.0.3.dev20/rbx/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/queues/jobs.py` & `rbx-3.0.3.dev20/rbx/queues/jobs.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/queues/scheduler.py` & `rbx-3.0.3.dev20/rbx/queues/scheduler.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/utils/__init__.py` & `rbx-3.0.3.dev20/rbx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx/web/handlers.py` & `rbx-3.0.3.dev20/rbx/web/handlers.py`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx.egg-info/PKG-INFO` & `rbx-3.0.3.dev20/rbx.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbx
-Version: 3.0.3.dev18
+Version: 3.0.3.dev20
 Summary: Scoota Platform utilities
 Home-page: http://scoota.com/
 Author: The Scoota Engineering Team
 Author-email: engineering@scoota.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `rbx-3.0.3.dev18/rbx.egg-info/SOURCES.txt` & `rbx-3.0.3.dev20/rbx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/rbx.egg-info/requires.txt` & `rbx-3.0.3.dev20/rbx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rbx-3.0.3.dev18/setup.py` & `rbx-3.0.3.dev20/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ]
 STORAGE = ["google-cloud-storage>=2.1,<3"]
 TASKS = ["google-cloud-tasks>=2.7,<3"]
 
 
 setup(
     name="rbx",
-    version="3.0.3.dev18",
+    version="3.0.3.dev20",
     license="Apache 2.0",
     description="Scoota Platform utilities",
     long_description="A collection of common tools for Scoota services.",
     url="http://scoota.com/",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
```

