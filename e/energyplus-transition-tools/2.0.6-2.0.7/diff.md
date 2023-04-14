# Comparing `tmp/energyplus_transition_tools-2.0.6.tar.gz` & `tmp/energyplus_transition_tools-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_transition_tools-2.0.6.tar", last modified: Sat Apr  8 13:00:02 2023, max compression
+gzip compressed data, was "energyplus_transition_tools-2.0.7.tar", last modified: Fri Apr 14 16:21:38 2023, max compression
```

## Comparing `energyplus_transition_tools-2.0.6.tar` & `energyplus_transition_tools-2.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 13:00:02.942344 energyplus_transition_tools-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-04-08 13:00:02.942344 energyplus_transition_tools-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 13:00:02.938344 energyplus_transition_tools-2.0.6/energyplus_transition/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/configure.py
--rw-r--r--   0 runner    (1001) docker     (122)     3769 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/energyplus_path.py
--rw-r--r--   0 runner    (1001) docker     (122)    20887 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/gui.py
--rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/international.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/transition_binary.py
--rw-r--r--   0 runner    (1001) docker     (122)     5286 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/energyplus_transition/transition_run_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 13:00:02.942344 energyplus_transition_tools-2.0.6/energyplus_transition_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-04-08 13:00:02.000000 energyplus_transition_tools-2.0.6/energyplus_transition_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-08 13:00:02.000000 energyplus_transition_tools-2.0.6/energyplus_transition_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 13:00:02.000000 energyplus_transition_tools-2.0.6/energyplus_transition_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-08 13:00:02.000000 energyplus_transition_tools-2.0.6/energyplus_transition_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-08 13:00:02.000000 energyplus_transition_tools-2.0.6/energyplus_transition_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-08 13:00:02.000000 energyplus_transition_tools-2.0.6/energyplus_transition_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-04-08 13:00:02.942344 energyplus_transition_tools-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1154 2023-04-08 12:59:58.000000 energyplus_transition_tools-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1426 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/energyplus_transition/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/configure.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3769 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/energyplus_path.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20887 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/gui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9640 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/international.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/transition_binary.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5286 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/energyplus_transition/transition_run_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2566 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-14 16:21:38.000000 energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-04-14 16:21:38.865039 energyplus_transition_tools-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-04-14 16:21:32.000000 energyplus_transition_tools-2.0.7/setup.py
```

### Comparing `energyplus_transition_tools-2.0.6/LICENSE.txt` & `energyplus_transition_tools-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.6/README.md` & `energyplus_transition_tools-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.6/energyplus_transition/energyplus_path.py` & `energyplus_transition_tools-2.0.7/energyplus_transition/energyplus_path.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.6/energyplus_transition/gui.py` & `energyplus_transition_tools-2.0.7/energyplus_transition/gui.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.6/energyplus_transition/international.py` & `energyplus_transition_tools-2.0.7/energyplus_transition/international.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.6/energyplus_transition/transition_binary.py` & `energyplus_transition_tools-2.0.7/energyplus_transition/transition_binary.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.6/energyplus_transition/transition_run_thread.py` & `energyplus_transition_tools-2.0.7/energyplus_transition/transition_run_thread.py`

 * *Files identical despite different names*

### Comparing `energyplus_transition_tools-2.0.6/energyplus_transition_tools.egg-info/SOURCES.txt` & `energyplus_transition_tools-2.0.7/energyplus_transition_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

