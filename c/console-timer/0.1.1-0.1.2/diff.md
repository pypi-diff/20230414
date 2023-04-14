# Comparing `tmp/console_timer-0.1.1.tar.gz` & `tmp/console_timer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "console_timer-0.1.1.tar", last modified: Fri Apr 14 04:10:00 2023, max compression
+gzip compressed data, was "console_timer-0.1.2.tar", last modified: Fri Apr 14 04:19:23 2023, max compression
```

## Comparing `console_timer-0.1.1.tar` & `console_timer-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:10:00.972527 console_timer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 04:10:00.972527 console_timer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 04:09:45.000000 console_timer-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:10:00.972527 console_timer-0.1.1/console_timer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 04:10:00.000000 console_timer-0.1.1/console_timer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 04:10:00.000000 console_timer-0.1.1/console_timer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:10:00.000000 console_timer-0.1.1/console_timer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:10:00.000000 console_timer-0.1.1/console_timer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:10:00.972527 console_timer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 04:09:45.000000 console_timer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:23.468969 console_timer-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 04:19:23.468969 console_timer-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 04:19:15.000000 console_timer-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:19:23.468969 console_timer-0.1.2/console_timer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 04:19:23.000000 console_timer-0.1.2/console_timer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 04:19:23.000000 console_timer-0.1.2/console_timer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:19:23.000000 console_timer-0.1.2/console_timer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:19:23.000000 console_timer-0.1.2/console_timer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:19:23.468969 console_timer-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 04:19:15.000000 console_timer-0.1.2/setup.py
```

