# Comparing `tmp/console_timer-0.1.0.tar.gz` & `tmp/console_timer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "console_timer-0.1.0.tar", last modified: Fri Apr 14 03:54:39 2023, max compression
+gzip compressed data, was "console_timer-0.1.1.tar", last modified: Fri Apr 14 04:10:00 2023, max compression
```

## Comparing `console_timer-0.1.0.tar` & `console_timer-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 03:54:39.019143 console_timer-0.1.0/
--rw-r--r--   0 alex       (501) staff       (20)      538 2023-04-14 03:54:39.019022 console_timer-0.1.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      225 2023-04-14 03:53:10.000000 console_timer-0.1.0/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-04-14 03:54:39.018884 console_timer-0.1.0/console_timer.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      538 2023-04-14 03:54:39.000000 console_timer-0.1.0/console_timer.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      166 2023-04-14 03:54:39.000000 console_timer-0.1.0/console_timer.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-14 03:54:39.000000 console_timer-0.1.0/console_timer.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-04-14 03:54:39.000000 console_timer-0.1.0/console_timer.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-04-14 03:54:39.019178 console_timer-0.1.0/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      677 2023-04-14 03:52:17.000000 console_timer-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:10:00.972527 console_timer-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 04:10:00.972527 console_timer-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 04:09:45.000000 console_timer-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 04:10:00.972527 console_timer-0.1.1/console_timer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-14 04:10:00.000000 console_timer-0.1.1/console_timer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 04:10:00.000000 console_timer-0.1.1/console_timer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:10:00.000000 console_timer-0.1.1/console_timer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 04:10:00.000000 console_timer-0.1.1/console_timer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 04:10:00.972527 console_timer-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-14 04:09:45.000000 console_timer-0.1.1/setup.py
```

