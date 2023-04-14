# Comparing `tmp/energyplus_regressions-2.0.2.tar.gz` & `tmp/energyplus_regressions-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_regressions-2.0.2.tar", last modified: Thu Apr  6 18:31:03 2023, max compression
+gzip compressed data, was "energyplus_regressions-2.0.3.tar", last modified: Fri Apr 14 15:26:48 2023, max compression
```

## Comparing `energyplus_regressions-2.0.2.tar` & `energyplus_regressions-2.0.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.138130 energyplus_regressions-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3751 2023-04-06 18:31:03.138130 energyplus_regressions-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2985 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.130130 energyplus_regressions-2.0.2/energyplus_regressions/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11982 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/build_files_to_run.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.130130 energyplus_regressions-2.0.2/energyplus_regressions/builds/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/builds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/builds/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2835 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/builds/install.py
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/builds/makefile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3649 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/builds/visualstudio.py
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.130130 energyplus_regressions-2.0.2/energyplus_regressions/diffs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/diffs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13954 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/diffs/ci_compare_script.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1528 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/diffs/math_diff.config
--rwxr-xr-x   0 runner    (1001) docker     (122)    25132 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/diffs/math_diff.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4120 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/diffs/mycsv.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    21208 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/diffs/table_diff.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4270 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/diffs/thresh_dict.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     9426 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/energyplus.py
--rw-r--r--   0 runner    (1001) docker     (122)      860 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/ep_platform.py
--rw-r--r--   0 runner    (1001) docker     (122)    64569 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/epw_map.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.134130 energyplus_regressions-2.0.2/energyplus_regressions/icons/
--rw-r--r--   0 runner    (1001) docker     (122)    18638 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/icons/icon.icns
--rw-r--r--   0 runner    (1001) docker     (122)    15187 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/icons/icon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    25254 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/icons/icon.png
--rwxr-xr-x   0 runner    (1001) docker     (122)      766 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/runner.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    64399 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    20990 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.134130 energyplus_regressions-2.0.2/energyplus_regressions/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.134130 energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1695 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/test_install.py
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/test_makefile.py
--rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/test_visualstudio.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.134130 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.134130 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/csv_resources/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1530 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/csv_resources/test_math_diff.config
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.134130 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/tbl_resources/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1530 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/tbl_resources/test_table_diff.config
--rw-r--r--   0 runner    (1001) docker     (122)    18306 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_ci_compare_script.py
--rw-r--r--   0 runner    (1001) docker     (122)    17039 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_math_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     5252 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_mycsv.py
--rw-r--r--   0 runner    (1001) docker     (122)    23636 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_table_diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_thresh_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     9624 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/test_build_files_to_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     8230 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/test_energyplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/test_epw_map.py
--rw-r--r--   0 runner    (1001) docker     (122)      895 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (122)   113719 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/test_runtests.py
--rw-r--r--   0 runner    (1001) docker     (122)     9993 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)    55441 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/energyplus_regressions/tk_window.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-06 18:31:03.130130 energyplus_regressions-2.0.2/energyplus_regressions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3751 2023-04-06 18:31:03.000000 energyplus_regressions-2.0.2/energyplus_regressions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-06 18:31:03.000000 energyplus_regressions-2.0.2/energyplus_regressions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-06 18:31:03.000000 energyplus_regressions-2.0.2/energyplus_regressions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-06 18:31:03.000000 energyplus_regressions-2.0.2/energyplus_regressions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-06 18:31:03.000000 energyplus_regressions-2.0.2/energyplus_regressions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-06 18:31:03.000000 energyplus_regressions-2.0.2/energyplus_regressions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-06 18:31:03.138130 energyplus_regressions-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-04-06 18:30:49.000000 energyplus_regressions-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2985 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.418517 energyplus_regressions-2.0.3/energyplus_regressions/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11982 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/build_files_to_run.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.418517 energyplus_regressions-2.0.3/energyplus_regressions/builds/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/builds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5426 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/builds/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2835 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/builds/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3292 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/builds/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3649 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/builds/visualstudio.py
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/energyplus_regressions/diffs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/diffs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13954 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/diffs/ci_compare_script.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1528 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/diffs/math_diff.config
+-rwxr-xr-x   0 runner    (1001) docker     (122)    25132 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/diffs/math_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4120 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/diffs/mycsv.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    21208 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/diffs/table_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4270 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/diffs/thresh_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     9426 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/energyplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/ep_platform.py
+-rw-r--r--   0 runner    (1001) docker     (122)    64569 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/epw_map.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/energyplus_regressions/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)    18638 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/icons/icon.icns
+-rw-r--r--   0 runner    (1001) docker     (122)    15187 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/icons/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    25254 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/icons/icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)      766 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    64399 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20990 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/energyplus_regressions/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1695 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/test_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2968 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/test_visualstudio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/csv_resources/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1530 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/csv_resources/test_math_diff.config
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.422518 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/tbl_resources/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1530 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/tbl_resources/test_table_diff.config
+-rw-r--r--   0 runner    (1001) docker     (122)    18306 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_ci_compare_script.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17039 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_math_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5252 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_mycsv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23636 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_table_diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3154 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_thresh_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9624 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/test_build_files_to_run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8230 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/test_energyplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/test_epw_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (122)   113719 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/test_runtests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9993 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55441 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/energyplus_regressions/tk_window.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 15:26:48.418517 energyplus_regressions-2.0.3/energyplus_regressions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4375 2023-04-14 15:26:48.000000 energyplus_regressions-2.0.3/energyplus_regressions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-14 15:26:48.000000 energyplus_regressions-2.0.3/energyplus_regressions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 15:26:48.000000 energyplus_regressions-2.0.3/energyplus_regressions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-14 15:26:48.000000 energyplus_regressions-2.0.3/energyplus_regressions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-14 15:26:48.000000 energyplus_regressions-2.0.3/energyplus_regressions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-14 15:26:48.000000 energyplus_regressions-2.0.3/energyplus_regressions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-14 15:26:48.426518 energyplus_regressions-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-04-14 15:26:38.000000 energyplus_regressions-2.0.3/setup.py
```

### Comparing `energyplus_regressions-2.0.2/LICENSE` & `energyplus_regressions-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/PKG-INFO` & `energyplus_regressions-2.0.3/energyplus_regressions.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
-Name: energyplus_regressions
-Version: 2.0.2
+Name: energyplus-regressions
+Version: 2.0.3
 Summary: A Python 3 library for evaluating regressions between EnergyPlus builds.
 Home-page: https://github.com/NREL/EnergyPlusRegressionTool
-Author: Edwin Lee
-Author-email: 
-License: UNKNOWN
+Author: Edwin Lee, for NREL, for United States Department of Energy
+License: ModifiedBSD
 Description: # EnergyPlus Regressions
         
         [![Documentation Status](https://readthedocs.org/projects/energyplusregressiontool/badge/?version=latest)](https://energyplusregressiontool.readthedocs.io/en/latest/?badge=latest)
         [![Run Tests](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/test.yml/badge.svg)](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/test.yml)
         [![PyPIRelease](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/release.yml/badge.svg)](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/release.yml)
         [![Flake8](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/flake8.yml/badge.svg)](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/flake8.yml)
         [![Coverage Status](https://coveralls.io/repos/github/NREL/EnergyPlusRegressionTool/badge.svg?branch=master)](https://coveralls.io/github/NREL/EnergyPlusRegressionTool?branch=master)
@@ -52,11 +51,22 @@
         
         ## Testing
         
         Exhaustive unit tests have been added to the "underneath the hood" code, like the functions that calculate diffs and run builds.
         The unit tests are run on [Github Actions](https://github.com/NREL/EnergyPlusRegressionTool/actions).
         The GUI code is not unit tested, but tested routinely on all platforms.
         
-Keywords: energyplus
-Platform: UNKNOWN
+Keywords: energyplus_launch,ep_launch,EnergyPlus,eplus,Energy+,Building Simulation,Whole Building Energy Simulation,Heat Transfer,HVAC,Modeling
+Platform: Linux (Tested on Ubuntu)
+Platform: MacOSX
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Utilities
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `energyplus_regressions-2.0.2/README.md` & `energyplus_regressions-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/build_files_to_run.py` & `energyplus_regressions-2.0.3/energyplus_regressions/build_files_to_run.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/builds/base.py` & `energyplus_regressions-2.0.3/energyplus_regressions/builds/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/builds/install.py` & `energyplus_regressions-2.0.3/energyplus_regressions/builds/install.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/builds/makefile.py` & `energyplus_regressions-2.0.3/energyplus_regressions/builds/makefile.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/builds/visualstudio.py` & `energyplus_regressions-2.0.3/energyplus_regressions/builds/visualstudio.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/diffs/ci_compare_script.py` & `energyplus_regressions-2.0.3/energyplus_regressions/diffs/ci_compare_script.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/diffs/math_diff.config` & `energyplus_regressions-2.0.3/energyplus_regressions/diffs/math_diff.config`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/diffs/math_diff.py` & `energyplus_regressions-2.0.3/energyplus_regressions/diffs/math_diff.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/diffs/mycsv.py` & `energyplus_regressions-2.0.3/energyplus_regressions/diffs/mycsv.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/diffs/table_diff.py` & `energyplus_regressions-2.0.3/energyplus_regressions/diffs/table_diff.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/diffs/thresh_dict.py` & `energyplus_regressions-2.0.3/energyplus_regressions/diffs/thresh_dict.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/energyplus.py` & `energyplus_regressions-2.0.3/energyplus_regressions/energyplus.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/ep_platform.py` & `energyplus_regressions-2.0.3/energyplus_regressions/ep_platform.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/epw_map.py` & `energyplus_regressions-2.0.3/energyplus_regressions/epw_map.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/icons/icon.icns` & `energyplus_regressions-2.0.3/energyplus_regressions/icons/icon.icns`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/icons/icon.ico` & `energyplus_regressions-2.0.3/energyplus_regressions/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/icons/icon.png` & `energyplus_regressions-2.0.3/energyplus_regressions/icons/icon.png`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/runner.py` & `energyplus_regressions-2.0.3/energyplus_regressions/runner.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/runtests.py` & `energyplus_regressions-2.0.3/energyplus_regressions/runtests.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/structures.py` & `energyplus_regressions-2.0.3/energyplus_regressions/structures.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/test_base.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/test_base.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/test_install.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/test_install.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/test_makefile.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/test_makefile.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/builds/test_visualstudio.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/builds/test_visualstudio.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/csv_resources/test_math_diff.config` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/csv_resources/test_math_diff.config`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/tbl_resources/test_table_diff.config` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/tbl_resources/test_table_diff.config`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_ci_compare_script.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_ci_compare_script.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_math_diff.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_math_diff.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_mycsv.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_mycsv.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_table_diff.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_table_diff.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/diffs/test_thresh_dict.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/diffs/test_thresh_dict.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/test_build_files_to_run.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/test_build_files_to_run.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/test_energyplus.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/test_energyplus.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/test_epw_map.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/test_epw_map.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/test_platform.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/test_runtests.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/test_runtests.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tests/test_structures.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions/tk_window.py` & `energyplus_regressions-2.0.3/energyplus_regressions/tk_window.py`

 * *Files identical despite different names*

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions.egg-info/PKG-INFO` & `energyplus_regressions-2.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
-Name: energyplus-regressions
-Version: 2.0.2
+Name: energyplus_regressions
+Version: 2.0.3
 Summary: A Python 3 library for evaluating regressions between EnergyPlus builds.
 Home-page: https://github.com/NREL/EnergyPlusRegressionTool
-Author: Edwin Lee
-Author-email: 
-License: UNKNOWN
+Author: Edwin Lee, for NREL, for United States Department of Energy
+License: ModifiedBSD
 Description: # EnergyPlus Regressions
         
         [![Documentation Status](https://readthedocs.org/projects/energyplusregressiontool/badge/?version=latest)](https://energyplusregressiontool.readthedocs.io/en/latest/?badge=latest)
         [![Run Tests](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/test.yml/badge.svg)](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/test.yml)
         [![PyPIRelease](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/release.yml/badge.svg)](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/release.yml)
         [![Flake8](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/flake8.yml/badge.svg)](https://github.com/NREL/EnergyPlusRegressionTool/actions/workflows/flake8.yml)
         [![Coverage Status](https://coveralls.io/repos/github/NREL/EnergyPlusRegressionTool/badge.svg?branch=master)](https://coveralls.io/github/NREL/EnergyPlusRegressionTool?branch=master)
@@ -52,11 +51,22 @@
         
         ## Testing
         
         Exhaustive unit tests have been added to the "underneath the hood" code, like the functions that calculate diffs and run builds.
         The unit tests are run on [Github Actions](https://github.com/NREL/EnergyPlusRegressionTool/actions).
         The GUI code is not unit tested, but tested routinely on all platforms.
         
-Keywords: energyplus
-Platform: UNKNOWN
+Keywords: energyplus_launch,ep_launch,EnergyPlus,eplus,Energy+,Building Simulation,Whole Building Energy Simulation,Heat Transfer,HVAC,Modeling
+Platform: Linux (Tested on Ubuntu)
+Platform: MacOSX
+Platform: Windows
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Utilities
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `energyplus_regressions-2.0.2/energyplus_regressions.egg-info/SOURCES.txt` & `energyplus_regressions-2.0.3/energyplus_regressions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

