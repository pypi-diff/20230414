# Comparing `tmp/rucio-consistency-1.0.7.tar.gz` & `tmp/rucio-consistency-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rucio-consistency-1.0.7.tar", last modified: Thu Apr 13 19:04:42 2023, max compression
+gzip compressed data, was "rucio-consistency-1.0.9.tar", last modified: Thu Apr 13 19:15:48 2023, max compression
```

## Comparing `rucio-consistency-1.0.7.tar` & `rucio-consistency-1.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:04:42.882250 rucio-consistency-1.0.7/
--rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.7/LICENSE
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 19:04:42.881994 rucio-consistency-1.0.7/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.7/README.rst
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:04:42.875433 rucio-consistency-1.0.7/rucio_consistency/
--rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/cmplib.py
--rw-r--r--   0 ivm        (501) staff       (20)    11469 2023-04-13 15:28:19.000000 rucio-consistency-1.0.7/rucio_consistency/config.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/part.py
--rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/py3.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:04:42.880480 rucio-consistency-1.0.7/rucio_consistency/scripts/
--rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/scripts/cmp2.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/scripts/cmp3.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/scripts/cmp5.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    10051 2023-04-13 14:41:45.000000 rucio-consistency-1.0.7/rucio_consistency/scripts/db_dump.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/scripts/partition.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.7/rucio_consistency/scripts/update_stats.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.7/rucio_consistency/stats.py
--rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 19:04:15.000000 rucio-consistency-1.0.7/rucio_consistency/version.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:04:42.881642 rucio-consistency-1.0.7/rucio_consistency/xrootd/
--rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.7/rucio_consistency/xrootd/__init__.py
--rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.7/rucio_consistency/xrootd/xrootd_client.py
--rwxr-xr-x   0 ivm        (501) staff       (20)    27390 2023-04-13 19:04:08.000000 rucio-consistency-1.0.7/rucio_consistency/xrootd/xrootd_scanner.py
-drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:04:42.877514 rucio-consistency-1.0.7/rucio_consistency.egg-info/
--rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 19:04:42.000000 rucio-consistency-1.0.7/rucio_consistency.egg-info/PKG-INFO
--rw-r--r--   0 ivm        (501) staff       (20)      850 2023-04-13 19:04:42.000000 rucio-consistency-1.0.7/rucio_consistency.egg-info/SOURCES.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 19:04:42.000000 rucio-consistency-1.0.7/rucio_consistency.egg-info/dependency_links.txt
--rw-r--r--   0 ivm        (501) staff       (20)      388 2023-04-13 19:04:42.000000 rucio-consistency-1.0.7/rucio_consistency.egg-info/entry_points.txt
--rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 19:04:42.000000 rucio-consistency-1.0.7/rucio_consistency.egg-info/not-zip-safe
--rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 19:04:42.000000 rucio-consistency-1.0.7/rucio_consistency.egg-info/requires.txt
--rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 19:04:42.000000 rucio-consistency-1.0.7/rucio_consistency.egg-info/top_level.txt
--rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 19:04:42.882337 rucio-consistency-1.0.7/setup.cfg
--rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.0.7/setup.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.561073 rucio-consistency-1.0.9/
+-rw-r--r--   0 ivm        (501) staff       (20)    11357 2023-01-20 15:50:08.000000 rucio-consistency-1.0.9/LICENSE
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 19:15:48.560642 rucio-consistency-1.0.9/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)       60 2023-01-26 20:21:12.000000 rucio-consistency-1.0.9/README.rst
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.554672 rucio-consistency-1.0.9/rucio_consistency/
+-rw-r--r--   0 ivm        (501) staff       (20)      378 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2861 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/cmplib.py
+-rw-r--r--   0 ivm        (501) staff       (20)    11469 2023-04-13 15:28:19.000000 rucio-consistency-1.0.9/rucio_consistency/config.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3042 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/part.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)      372 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/py3.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.559180 rucio-consistency-1.0.9/rucio_consistency/scripts/
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3430 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/cmp2.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     3595 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/cmp3.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     4312 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/cmp5.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    10051 2023-04-13 14:41:45.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/db_dump.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2737 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/partition.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     1069 2023-04-13 13:48:02.000000 rucio-consistency-1.0.9/rucio_consistency/scripts/update_stats.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     2523 2023-04-13 13:48:36.000000 rucio-consistency-1.0.9/rucio_consistency/stats.py
+-rw-r--r--   0 ivm        (501) staff       (20)      124 2023-04-13 19:15:45.000000 rucio-consistency-1.0.9/rucio_consistency/version.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.560263 rucio-consistency-1.0.9/rucio_consistency/xrootd/
+-rw-r--r--   0 ivm        (501) staff       (20)       39 2023-04-12 14:55:53.000000 rucio-consistency-1.0.9/rucio_consistency/xrootd/__init__.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)     9449 2023-04-13 14:12:31.000000 rucio-consistency-1.0.9/rucio_consistency/xrootd/xrootd_client.py
+-rwxr-xr-x   0 ivm        (501) staff       (20)    27445 2023-04-13 19:14:40.000000 rucio-consistency-1.0.9/rucio_consistency/xrootd/xrootd_scanner.py
+drwxr-xr-x   0 ivm        (501) staff       (20)        0 2023-04-13 19:15:48.557038 rucio-consistency-1.0.9/rucio_consistency.egg-info/
+-rw-r--r--   0 ivm        (501) staff       (20)      350 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/PKG-INFO
+-rw-r--r--   0 ivm        (501) staff       (20)      850 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/SOURCES.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/dependency_links.txt
+-rw-r--r--   0 ivm        (501) staff       (20)      388 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/entry_points.txt
+-rw-r--r--   0 ivm        (501) staff       (20)        1 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/not-zip-safe
+-rw-r--r--   0 ivm        (501) staff       (20)       22 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/requires.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       18 2023-04-13 19:15:48.000000 rucio-consistency-1.0.9/rucio_consistency.egg-info/top_level.txt
+-rw-r--r--   0 ivm        (501) staff       (20)       38 2023-04-13 19:15:48.561190 rucio-consistency-1.0.9/setup.cfg
+-rw-r--r--   0 ivm        (501) staff       (20)     1391 2023-04-13 14:18:20.000000 rucio-consistency-1.0.9/setup.py
```

### Comparing `rucio-consistency-1.0.7/LICENSE` & `rucio-consistency-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/cmplib.py` & `rucio-consistency-1.0.9/rucio_consistency/cmplib.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/config.py` & `rucio-consistency-1.0.9/rucio_consistency/config.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/part.py` & `rucio-consistency-1.0.9/rucio_consistency/part.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/scripts/cmp2.py` & `rucio-consistency-1.0.9/rucio_consistency/scripts/cmp2.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/scripts/cmp3.py` & `rucio-consistency-1.0.9/rucio_consistency/scripts/cmp3.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/scripts/cmp5.py` & `rucio-consistency-1.0.9/rucio_consistency/scripts/cmp5.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/scripts/db_dump.py` & `rucio-consistency-1.0.9/rucio_consistency/scripts/db_dump.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/scripts/partition.py` & `rucio-consistency-1.0.9/rucio_consistency/scripts/partition.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/scripts/update_stats.py` & `rucio-consistency-1.0.9/rucio_consistency/scripts/update_stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/stats.py` & `rucio-consistency-1.0.9/rucio_consistency/stats.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/xrootd/xrootd_client.py` & `rucio-consistency-1.0.9/rucio_consistency/xrootd/xrootd_client.py`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/rucio_consistency/xrootd/xrootd_scanner.py` & `rucio-consistency-1.0.9/rucio_consistency/xrootd/xrootd_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,16 @@
     if rewrite_path is not None:
         if not rewrite_path.search(lfn):
             sys.stderr.write(f"Path rewrite pattern for root {root} did not find a match in path {lfn}\n")
             sys.exit(1)
         lfn = rewrite_path.sub(rewrite_out, lfn)   
     return lfn
 
-def scan_root(rse, config, client, root, root_expected, my_stats, stats, stats_key, quiet,
+def scan_root(rse, config, client, root, root_expected, my_stats, stats, stats_key, 
+            quiet, display_progress, max_files,
             recursive_threshold, max_scanners, timeout,
             file_list, dir_list, empty_dirs_file,
             ignore_failed_directories, include_sizes):
 
     failed = root_failed = False
     
     server = config.Server
@@ -579,21 +580,20 @@
         sys.exit(2)
 
     rse = args[0]
     config = ScannerConfiguration(rse, opts["-c"])
 
     quiet = "-q" in opts
     display_progress = not quiet and "-v" in opts
+    max_files = int(opts.get("-M", 0)) or None
 
     recursive_threshold = int(opts.get("-R", config.RecursionThreshold))
     max_scanners = int(opts.get("-m", config.NWorkers))
     timeout = int(opts.get("-t", config.ScannerTimeout))
     
-    max_files = opts.get("-M")
-    if max_files is not None: max_files = int(max_files)
     stats_file = opts.get("-s")
     stats_key = opts.get("-S", "scanner")
     ignore_directory_scan_errors = "-k" in opts
     root_file_counts = opts.get("-r")
     if root_file_counts:
         root_file_counts = json.load(open(root_file_counts, "r"))
     else:
@@ -683,15 +683,16 @@
 
     if not failed:
         all_roots_failed = not good_roots
         for client, root in good_roots:
             try:
                 print(f"Scanning root {root} ...", file=sys.stderr)
                 expected = root_file_counts.get(root, 0) > 0
-                failed = scan_root(rse, config, client, root, expected, my_stats, stats, stats_key, quiet,
+                failed = scan_root(rse, config, client, root, expected, my_stats, stats, stats_key, 
+                        quiet, display_progress, max_files,
                         recursive_threshold, max_scanners, timeout,
                         out_list, dir_list, empty_dirs_file,
                         ignore_directory_scan_errors, include_sizes)
             except:
                 exc = traceback.format_exc()
                 print(exc)
                 lines = exc.split("\n")
```

### Comparing `rucio-consistency-1.0.7/rucio_consistency.egg-info/SOURCES.txt` & `rucio-consistency-1.0.9/rucio_consistency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rucio-consistency-1.0.7/setup.py` & `rucio-consistency-1.0.9/setup.py`

 * *Files identical despite different names*

