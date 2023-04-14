# Comparing `tmp/dr-buster-1.0.9.tar.gz` & `tmp/dr-buster-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dr-buster-1.0.9.tar", last modified: Fri Apr 14 00:22:40 2023, max compression
+gzip compressed data, was "dr-buster-1.1.0.tar", last modified: Fri Apr 14 00:26:25 2023, max compression
```

## Comparing `dr-buster-1.0.9.tar` & `dr-buster-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:22:40.337988 dr-buster-1.0.9/
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1062 2023-04-13 14:02:32.000000 dr-buster-1.0.9/LICENSE
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-14 00:22:40.337988 dr-buster-1.0.9/PKG-INFO
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1880 2023-04-13 14:02:32.000000 dr-buster-1.0.9/README.md
-drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:22:40.337988 dr-buster-1.0.9/dr_buster/
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:02:32.000000 dr-buster-1.0.9/dr_buster/__init__.py
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)      367 2023-04-13 14:02:32.000000 dr-buster-1.0.9/dr_buster/__main__.py
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     6348 2023-04-14 00:22:05.000000 dr-buster-1.0.9/dr_buster/core.py
-drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:22:40.337988 dr-buster-1.0.9/dr_buster.egg-info/
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-14 00:22:40.000000 dr-buster-1.0.9/dr_buster.egg-info/PKG-INFO
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)      265 2023-04-14 00:22:40.000000 dr-buster-1.0.9/dr_buster.egg-info/SOURCES.txt
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)        1 2023-04-14 00:22:40.000000 dr-buster-1.0.9/dr_buster.egg-info/dependency_links.txt
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)       10 2023-04-14 00:22:40.000000 dr-buster-1.0.9/dr_buster.egg-info/top_level.txt
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)      105 2023-04-13 14:02:32.000000 dr-buster-1.0.9/pyproject.toml
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)      602 2023-04-14 00:22:40.337988 dr-buster-1.0.9/setup.cfg
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)       38 2023-04-13 14:02:32.000000 dr-buster-1.0.9/setup.py
-drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:22:40.337988 dr-buster-1.0.9/tests/
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1643 2023-04-13 14:02:32.000000 dr-buster-1.0.9/tests/testserver.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:26:25.117980 dr-buster-1.1.0/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1062 2023-04-13 14:02:32.000000 dr-buster-1.1.0/LICENSE
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-14 00:26:25.117980 dr-buster-1.1.0/PKG-INFO
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1880 2023-04-13 14:02:32.000000 dr-buster-1.1.0/README.md
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:26:25.117980 dr-buster-1.1.0/dr_buster/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:02:32.000000 dr-buster-1.1.0/dr_buster/__init__.py
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      367 2023-04-13 14:02:32.000000 dr-buster-1.1.0/dr_buster/__main__.py
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     6181 2023-04-14 00:25:52.000000 dr-buster-1.1.0/dr_buster/core.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:26:25.117980 dr-buster-1.1.0/dr_buster.egg-info/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-14 00:26:25.000000 dr-buster-1.1.0/dr_buster.egg-info/PKG-INFO
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      265 2023-04-14 00:26:25.000000 dr-buster-1.1.0/dr_buster.egg-info/SOURCES.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)        1 2023-04-14 00:26:25.000000 dr-buster-1.1.0/dr_buster.egg-info/dependency_links.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)       10 2023-04-14 00:26:25.000000 dr-buster-1.1.0/dr_buster.egg-info/top_level.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      105 2023-04-13 14:02:32.000000 dr-buster-1.1.0/pyproject.toml
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      602 2023-04-14 00:26:25.117980 dr-buster-1.1.0/setup.cfg
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)       38 2023-04-13 14:02:32.000000 dr-buster-1.1.0/setup.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:26:25.117980 dr-buster-1.1.0/tests/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1643 2023-04-13 14:02:32.000000 dr-buster-1.1.0/tests/testserver.py
```

### Comparing `dr-buster-1.0.9/LICENSE` & `dr-buster-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dr-buster-1.0.9/PKG-INFO` & `dr-buster-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dr-buster
-Version: 1.0.9
+Version: 1.1.0
 Summary: Simple, yet effective web path finder implemented with multiprocessing in Python
 Home-page: https://github.com/kelj0/dr_buster
 Author: kelj0
 Author-email: kelj0@protonmail.com
 Project-URL: Bug Tracker, https://github.com/kelj0/dr_buster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dr-buster-1.0.9/README.md` & `dr-buster-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dr-buster-1.0.9/dr_buster/core.py` & `dr-buster-1.1.0/dr_buster/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,20 +147,15 @@
         procs.append(Process(target=scan_host, args=(host, port, wordlist, runtime, results_path, n+1, path)))
     for p in procs:
         p.start()
     for p in procs:
         p.join()
 
 def write_to_report(finding, runtime, results_path=None):
-    if results_path is not None:
-        fname = os.path.join(results_path, f"dr.buster.report.{runtime}.txt")
-    else:
-        fname = f"./dr.buster.report.{runtime}.txt"
-
-    with open(fname, "a") as f:
+    with open(results_path, "a") as f:
         f.write(finding)
 
 def main(url, wordlist_path, cli_run=True):
     '''
         returns a path to the result of a scan
         @url: url that you want to scan, it can be ip or an url to root, or to some specific path
         @wordlist_path: provide a path to a wordlist that you want to use to scan that path
```

### Comparing `dr-buster-1.0.9/dr_buster.egg-info/PKG-INFO` & `dr-buster-1.1.0/dr_buster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dr-buster
-Version: 1.0.9
+Version: 1.1.0
 Summary: Simple, yet effective web path finder implemented with multiprocessing in Python
 Home-page: https://github.com/kelj0/dr_buster
 Author: kelj0
 Author-email: kelj0@protonmail.com
 Project-URL: Bug Tracker, https://github.com/kelj0/dr_buster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dr-buster-1.0.9/tests/testserver.py` & `dr-buster-1.1.0/tests/testserver.py`

 * *Files identical despite different names*

