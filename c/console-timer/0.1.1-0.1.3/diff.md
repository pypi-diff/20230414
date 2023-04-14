# Comparing `tmp/console_timer-0.1.1.tar.gz` & `tmp/console-timer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "console_timer-0.1.1.tar", last modified: Fri Apr 14 04:10:00 2023, max compression
+gzip compressed data, was "console-timer-0.1.3.tar", last modified: Fri Apr 14 05:40:53 2023, max compression
```

## Comparing `console_timer-0.1.1.tar` & `console-timer-0.1.3.tar`

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
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:40:53.150937 console-timer-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 05:40:53.150937 console-timer-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 05:40:41.000000 console-timer-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:40:53.150937 console-timer-0.1.3/console_timer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 05:40:53.000000 console-timer-0.1.3/console_timer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 05:40:53.000000 console-timer-0.1.3/console_timer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:40:53.000000 console-timer-0.1.3/console_timer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:40:53.000000 console-timer-0.1.3/console_timer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 05:40:53.150937 console-timer-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 05:40:41.000000 console-timer-0.1.3/setup.py
```

