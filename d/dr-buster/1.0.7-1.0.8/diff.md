# Comparing `tmp/dr-buster-1.0.7.tar.gz` & `tmp/dr-buster-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dr-buster-1.0.7.tar", last modified: Thu Apr 13 14:04:27 2023, max compression
+gzip compressed data, was "dr-buster-1.0.8.tar", last modified: Fri Apr 14 00:14:37 2023, max compression
```

## Comparing `dr-buster-1.0.7.tar` & `dr-buster-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:04:27.883455 dr-buster-1.0.7/
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1062 2023-04-13 14:02:32.000000 dr-buster-1.0.7/LICENSE
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-13 14:04:27.883455 dr-buster-1.0.7/PKG-INFO
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1880 2023-04-13 14:02:32.000000 dr-buster-1.0.7/README.md
-drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:04:27.883455 dr-buster-1.0.7/dr_buster/
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:02:32.000000 dr-buster-1.0.7/dr_buster/__init__.py
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)      367 2023-04-13 14:02:32.000000 dr-buster-1.0.7/dr_buster/__main__.py
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     5962 2023-04-13 14:02:32.000000 dr-buster-1.0.7/dr_buster/core.py
-drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:04:27.883455 dr-buster-1.0.7/dr_buster.egg-info/
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-13 14:04:27.000000 dr-buster-1.0.7/dr_buster.egg-info/PKG-INFO
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)      265 2023-04-13 14:04:27.000000 dr-buster-1.0.7/dr_buster.egg-info/SOURCES.txt
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)        1 2023-04-13 14:04:27.000000 dr-buster-1.0.7/dr_buster.egg-info/dependency_links.txt
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)       10 2023-04-13 14:04:27.000000 dr-buster-1.0.7/dr_buster.egg-info/top_level.txt
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)      105 2023-04-13 14:02:32.000000 dr-buster-1.0.7/pyproject.toml
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)      602 2023-04-13 14:04:27.883455 dr-buster-1.0.7/setup.cfg
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)       38 2023-04-13 14:02:32.000000 dr-buster-1.0.7/setup.py
-drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:04:27.883455 dr-buster-1.0.7/tests/
--rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1643 2023-04-13 14:02:32.000000 dr-buster-1.0.7/tests/testserver.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:14:37.418009 dr-buster-1.0.8/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1062 2023-04-13 14:02:32.000000 dr-buster-1.0.8/LICENSE
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-14 00:14:37.418009 dr-buster-1.0.8/PKG-INFO
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1880 2023-04-13 14:02:32.000000 dr-buster-1.0.8/README.md
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:14:37.418009 dr-buster-1.0.8/dr_buster/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)        0 2023-04-13 14:02:32.000000 dr-buster-1.0.8/dr_buster/__init__.py
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      367 2023-04-13 14:02:32.000000 dr-buster-1.0.8/dr_buster/__main__.py
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     6288 2023-04-14 00:10:09.000000 dr-buster-1.0.8/dr_buster/core.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:14:37.418009 dr-buster-1.0.8/dr_buster.egg-info/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     2416 2023-04-14 00:14:37.000000 dr-buster-1.0.8/dr_buster.egg-info/PKG-INFO
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      265 2023-04-14 00:14:37.000000 dr-buster-1.0.8/dr_buster.egg-info/SOURCES.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)        1 2023-04-14 00:14:37.000000 dr-buster-1.0.8/dr_buster.egg-info/dependency_links.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)       10 2023-04-14 00:14:37.000000 dr-buster-1.0.8/dr_buster.egg-info/top_level.txt
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      105 2023-04-13 14:02:32.000000 dr-buster-1.0.8/pyproject.toml
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)      602 2023-04-14 00:14:37.418009 dr-buster-1.0.8/setup.cfg
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)       38 2023-04-13 14:02:32.000000 dr-buster-1.0.8/setup.py
+drwxr-xr-x   0 lhpot     (1000) lhpot     (1000)        0 2023-04-14 00:14:37.418009 dr-buster-1.0.8/tests/
+-rw-r--r--   0 lhpot     (1000) lhpot     (1000)     1643 2023-04-13 14:02:32.000000 dr-buster-1.0.8/tests/testserver.py
```

### Comparing `dr-buster-1.0.7/LICENSE` & `dr-buster-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dr-buster-1.0.7/PKG-INFO` & `dr-buster-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dr-buster
-Version: 1.0.7
+Version: 1.0.8
 Summary: Simple, yet effective web path finder implemented with multiprocessing in Python
 Home-page: https://github.com/kelj0/dr_buster
 Author: kelj0
 Author-email: kelj0@protonmail.com
 Project-URL: Bug Tracker, https://github.com/kelj0/dr_buster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dr-buster-1.0.7/README.md` & `dr-buster-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `dr-buster-1.0.7/dr_buster/core.py` & `dr-buster-1.0.8/dr_buster/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,43 +115,49 @@
     for p in range(PROCESSES_COUNT):
         if p == PROCESSES_COUNT - 1:
             WORD_LISTS.append(lines[start:])
         else:
             WORD_LISTS.append(lines[start:start+words_per_process])
         start+=words_per_process
 
-def scan_host(host, port, wordlist, runtime, process_id=None, path=""):
+def scan_host(host, port, wordlist, runtime, results_path, process_id=None, path=""):
     for word in wordlist:
         try:
             code = get_code(host, port, path+word)
         except Exception:
             print(host,port,path,word)
             exit(1)
         if code != NOT_FOUND_CODE and code != 400:
             print("%s:%s/%s%s returned [%s]!                \r" 
                     % ("http://"+host if not SSL_SUPPORTED else "https://"+host, port, path, word, code))
             finding = ("%s:%s/%s%s [%s]\n"
                     % ("http://"+host if not SSL_SUPPORTED else "https://"+host, port, path, word, code))
-            write_to_report(finding, runtime)
+            write_to_report(finding, runtime, results_path)
 
-def start_scan(url, wordlist_path, runtime):
+def start_scan(url, wordlist_path, runtime, results_path=None):
     global WORD_LISTS
     print("Starting scan on %s.." % (url,))
     host, port, path = parse_url(url)
     prepare_wordlists(wordlist_path)
     procs = []
+    if results_path is None:
+        results_path = os.path.join(dir_path, f"dr.buster.report.{runtime}.txt")
     for n, wordlist in enumerate(WORD_LISTS):
-        procs.append(Process(target=scan_host, args=(host, port, wordlist, runtime, n+1, path)))
+        procs.append(Process(target=scan_host, args=(host, port, wordlist, runtime, results_path, n+1, path)))
     for p in procs:
         p.start()
     for p in procs:
         p.join()
 
-def write_to_report(finding, runtime):
-    fname = "./dr.buster.report."+runtime
+def write_to_report(finding, runtime, results_path=None):
+    if results_path is not None:
+        fname = os.path.join(results_path, f"dr.buster.report.{runtime}.txt")
+    else:
+        fname = f"./dr.buster.report.{runtime}.txt"
+
     with open(fname, "a") as f:
         f.write(finding)
 
 def main(url, wordlist_path, cli_run=True):
     '''
         returns a path to the result of a scan
         @url: url that you want to scan, it can be ip or an url to root, or to some specific path
@@ -169,9 +175,9 @@
     end_time = time()
     if cli_run:
         print()
         print("\nScanned %s paths in %s s." % (len(list(itertools.chain.from_iterable(WORD_LISTS))), end_time-start_time))
     
     dir_path = os.path.dirname(os.path.realpath(__file__))
     
-    return os.path.join(dir_path, f"dr.buster.report.{runtime}")
+    return os.path.join(dir_path, f"dr.buster.report.{runtime}.txt")
```

### Comparing `dr-buster-1.0.7/dr_buster.egg-info/PKG-INFO` & `dr-buster-1.0.8/dr_buster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dr-buster
-Version: 1.0.7
+Version: 1.0.8
 Summary: Simple, yet effective web path finder implemented with multiprocessing in Python
 Home-page: https://github.com/kelj0/dr_buster
 Author: kelj0
 Author-email: kelj0@protonmail.com
 Project-URL: Bug Tracker, https://github.com/kelj0/dr_buster/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dr-buster-1.0.7/setup.cfg` & `dr-buster-1.0.8/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dr-buster
-version = 1.0.7
+version = 1.0.8
 author = kelj0
 author_email = kelj0@protonmail.com
 description = Simple, yet effective web path finder implemented with multiprocessing in Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kelj0/dr_buster
 project_urls =
```

### Comparing `dr-buster-1.0.7/tests/testserver.py` & `dr-buster-1.0.8/tests/testserver.py`

 * *Files identical despite different names*

