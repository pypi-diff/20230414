# Comparing `tmp/searchkit-0.2.0.tar.gz` & `tmp/searchkit-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.0.tar", last modified: Wed Apr 12 11:04:56 2023, max compression
+gzip compressed data, was "searchkit-0.2.1.tar", last modified: Fri Apr 14 16:21:25 2023, max compression
```

## Comparing `searchkit-0.2.0.tar` & `searchkit-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-12 11:04:56.827556 searchkit-0.2.0/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.0/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     3103 2023-04-12 11:04:56.827556 searchkit-0.2.0/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.0/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      335 2023-04-12 11:04:37.000000 searchkit-0.2.0/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-12 11:04:56.827556 searchkit-0.2.0/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      100 2023-01-29 21:35:16.000000 searchkit-0.2.0/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-04-11 08:53:59.000000 searchkit-0.2.0/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.0/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    43588 2023-04-12 11:04:01.000000 searchkit-0.2.0/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4406 2023-04-11 08:53:59.000000 searchkit-0.2.0/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-12 11:04:56.827556 searchkit-0.2.0/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     3103 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-04-12 11:04:56.000000 searchkit-0.2.0/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-04-12 11:04:56.827556 searchkit-0.2.0/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.0/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-14 16:21:25.241528 searchkit-0.2.1/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.1/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-04-14 16:21:25.241528 searchkit-0.2.1/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.1/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      337 2023-04-14 15:40:17.000000 searchkit-0.2.1/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-14 16:21:25.241528 searchkit-0.2.1/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      100 2023-01-29 21:35:16.000000 searchkit-0.2.1/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-04-11 08:53:59.000000 searchkit-0.2.1/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.1/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    44338 2023-04-13 19:54:24.000000 searchkit-0.2.1/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4743 2023-04-13 20:08:39.000000 searchkit-0.2.1/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-14 16:21:25.241528 searchkit-0.2.1/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-04-14 16:21:25.000000 searchkit-0.2.1/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-04-14 16:21:25.000000 searchkit-0.2.1/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-04-14 16:21:25.000000 searchkit-0.2.1/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-04-14 16:21:25.000000 searchkit-0.2.1/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-04-14 16:21:25.000000 searchkit-0.2.1/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-04-14 16:21:25.241528 searchkit-0.2.1/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.1/setup.py
```

### Comparing `searchkit-0.2.0/LICENSE` & `searchkit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.0/PKG-INFO` & `searchkit-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.0
-Summary: Library provided tools used to search files concurrently.
+Version: 0.2.1
+Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
 
 Python library providing tools to search files in parallel.
```

### Comparing `searchkit-0.2.0/README.md` & `searchkit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.0/searchkit/constraints.py` & `searchkit-0.2.1/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.0/searchkit/search.py` & `searchkit-0.2.1/searchkit/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1167,26 +1167,34 @@
 
             try:
                 log.debug('sending SIGKILL to worker process %s', wpid)
                 os.kill(wpid, signal.SIGILL)
             except Exception:
                 log.debug('worker process %s already killed', wpid)
 
-    def _run(self, mgr):
-        """ Run all searches.
+    def _run_single(self, results):
+        """ Run a single search using this process.
 
-        @param mgr: multiprocessing.Manager object
-        @return: SearchResultsCollection object
+        @param results: SearchResultsCollection object
         """
-        self.stats.reset()
-        results = SearchResultsCollection(self.catalog)
-        if len(self.catalog) == 0:
-            log.debug("catalog is empty - nothing to run")
-            return results
+        queue = multiprocessing.Queue()
+        for info in self.catalog:
+            task = SearchTask(info,
+                              constraints_manager=self.constraints_manager,
+                              results_queue=queue)
+            self.stats.update(task.execute())
+
+        self._purge_results(results, queue, self.stats['results'])
 
+    def _run_mp(self, mgr, results):
+        """ Run searches in parallel.
+
+        @param mgr: multiprocessing.Manager object
+        @param results: SearchResultsCollection object
+        """
         queue = mgr.Queue()
         results_thread, event = self._create_results_thread(results, queue,
                                                             self.stats)
         results_thread_started = False
         try:
             num_workers = self.num_parallel_tasks
             with concurrent.futures.ProcessPoolExecutor(
@@ -1233,17 +1241,29 @@
                 log.debug("terminating pool")
         finally:
             if results_thread is not None and results_thread_started:
                 self._stop_results_thread(results_thread, event)
 
         log.debug("filesearcher: stats=%s", self.stats)
         log.debug("filesearcher: completed (results=%s)", len(results))
-        return results
 
     def run(self):
         """ Run all searches.
 
         @return: SearchResultsCollection object
         """
         log.debug("filesearcher: starting")
-        with multiprocessing.Manager() as mgr:
-            return self._run(mgr)
+        self.stats.reset()
+        results = SearchResultsCollection(self.catalog)
+        if len(self.catalog) == 0:
+            log.debug("catalog is empty - nothing to run")
+            return results
+
+        if len(self.files) > 1:
+            log.debug("running searches (parallel=True)")
+            with multiprocessing.Manager() as mgr:
+                self._run_mp(mgr, results)
+        else:
+            log.debug("running searches (parallel=False)")
+            self._run_single(results)
+
+        return results
```

### Comparing `searchkit-0.2.0/searchkit/utils.py` & `searchkit-0.2.1/searchkit/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,20 @@
         @param path: path to cache contents file.
         """
         if not path or not os.path.exists(path):
             log.debug("no cache found at '%s'", path)
             return
 
         with open(path, 'rb') as fd:
-            contents = pickle.load(fd)
+            try:
+                contents = pickle.load(fd)
+            except Exception:
+                log.exception("failed to load contents from cache '%s'", path)
+                contents = None
+
             if not contents:
                 return
 
             return contents
 
     def get(self, key):
         """
@@ -126,11 +131,15 @@
                 else:
                     contents = {key: value}
 
                 log.debug("saving to cache '%s' (key=%s, items=%s)", path, key,
                           len(contents))
 
             with open(path, 'wb') as fd:
-                pickle.dump(contents, fd)
+                try:
+                    pickle.dump(contents, fd)
+                except Exception:
+                    log.exception("failed to save contents to cache '%s'",
+                                  path)
 
             log.debug("cache id=%s size=%s", self.cache_id,
                       os.path.getsize(path))
```

### Comparing `searchkit-0.2.0/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.1/searchkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.0
-Summary: Library provided tools used to search files concurrently.
+Version: 0.2.1
+Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
 
 Python library providing tools to search files in parallel.
```

