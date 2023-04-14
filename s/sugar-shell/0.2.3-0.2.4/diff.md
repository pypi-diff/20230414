# Comparing `tmp/sugar_shell-0.2.3.tar.gz` & `tmp/sugar_shell-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sugar_shell-0.2.3.tar", last modified: Tue Feb 28 07:49:20 2023, max compression
+gzip compressed data, was "sugar_shell-0.2.4.tar", last modified: Fri Apr 14 06:36:53 2023, max compression
```

## Comparing `sugar_shell-0.2.3.tar` & `sugar_shell-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 07:49:20.855554 sugar_shell-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-28 07:49:18.000000 sugar_shell-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-28 07:49:20.855554 sugar_shell-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-28 07:49:18.000000 sugar_shell-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 07:49:20.855554 sugar_shell-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-02-28 07:49:18.000000 sugar_shell-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 07:49:20.855554 sugar_shell-0.2.3/sugar_shell/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-02-28 07:49:18.000000 sugar_shell-0.2.3/sugar_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 07:49:20.855554 sugar_shell-0.2.3/sugar_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-28 07:49:20.000000 sugar_shell-0.2.3/sugar_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-02-28 07:49:20.000000 sugar_shell-0.2.3/sugar_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 07:49:20.000000 sugar_shell-0.2.3/sugar_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-28 07:49:20.000000 sugar_shell-0.2.3/sugar_shell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-28 07:49:20.000000 sugar_shell-0.2.3/sugar_shell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:36:53.392594 sugar_shell-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 06:36:50.000000 sugar_shell-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 06:36:53.392594 sugar_shell-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-14 06:36:50.000000 sugar_shell-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:36:53.392594 sugar_shell-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 06:36:50.000000 sugar_shell-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:36:53.388594 sugar_shell-0.2.4/sugar_shell/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-14 06:36:50.000000 sugar_shell-0.2.4/sugar_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:36:53.392594 sugar_shell-0.2.4/sugar_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 06:36:53.000000 sugar_shell-0.2.4/sugar_shell.egg-info/top_level.txt
```

### Comparing `sugar_shell-0.2.3/LICENSE` & `sugar_shell-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sugar_shell-0.2.3/README.md` & `sugar_shell-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sugar_shell-0.2.3/sugar_shell/__init__.py` & `sugar_shell-0.2.4/sugar_shell/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 # encoding=utf-8
 import os
 import signal
 import sys
 
 ssh_config_file = '~/.ssh/config'
 
+title = '''
+                                  _          _ _ 
+ ___ _   _  __ _  __ _ _ __   ___| |__   ___| | |
+/ __| | | |/ _` |/ _` | '__| / __| '_ \ / _ \ | |
+\__ \ |_| | (_| | (_| | |    \__ \ | | |  __/ | |
+|___/\__,_|\__, |\__,_|_|    |___/_| |_|\___|_|_|
+           |___/                                 
+'''
+
 
 def signal_handler(signal, frame):
     print()
     print('GoodBye %s' % (os.environ['USER']))
     sys.exit(0)
 
 
@@ -62,14 +71,15 @@
     signal.signal(signal.SIGINT, signal_handler)
     entry_id = 0
     entry_list, status_code = parse_config()
 
     if not entry_list and status_code == 1:
         return
 
+    print(title)
     print('Hello %s, Welcome to use SugarShell~ :)' % (os.environ['USER']))
 
     entry_id = show(entry_id, entry_list)
 
     select = ''
 
     while select != 'q':
```

