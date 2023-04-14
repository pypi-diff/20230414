# Comparing `tmp/daskcheck-0.0.3.tar.gz` & `tmp/daskcheck-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daskcheck-0.0.3.tar", last modified: Tue Jan 10 15:07:12 2023, max compression
+gzip compressed data, was "daskcheck-0.0.4.tar", last modified: Fri Apr 14 12:43:18 2023, max compression
```

## Comparing `daskcheck-0.0.3.tar` & `daskcheck-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:07:12.868768 daskcheck-0.0.3/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1903 2023-01-10 15:07:12.868768 daskcheck-0.0.3/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1211 2023-01-10 15:07:10.000000 daskcheck-0.0.3/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:07:12.868768 daskcheck-0.0.3/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      680 2023-01-10 14:50:05.000000 daskcheck-0.0.3/bin/daskcheck
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:07:12.868768 daskcheck-0.0.3/daskcheck/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-01-10 14:48:06.000000 daskcheck-0.0.3/daskcheck/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6840 2023-01-10 14:48:06.000000 daskcheck-0.0.3/daskcheck/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6875 2023-01-10 14:51:58.000000 daskcheck-0.0.3/daskcheck/daskcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1090 2023-01-10 14:48:06.000000 daskcheck-0.0.3/daskcheck/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-01-10 15:07:12.000000 daskcheck-0.0.3/daskcheck/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:07:12.868768 daskcheck-0.0.3/daskcheck.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1903 2023-01-10 15:07:12.000000 daskcheck-0.0.3/daskcheck.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      304 2023-01-10 15:07:12.000000 daskcheck-0.0.3/daskcheck.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-01-10 15:07:12.000000 daskcheck-0.0.3/daskcheck.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-01-10 15:07:12.000000 daskcheck-0.0.3/daskcheck.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-01-10 15:07:12.000000 daskcheck-0.0.3/daskcheck.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-01-10 15:07:12.868768 daskcheck-0.0.3/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1103 2023-01-10 14:48:06.000000 daskcheck-0.0.3/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-14 12:43:18.034442 daskcheck-0.0.4/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2802 2023-04-14 12:43:18.034442 daskcheck-0.0.4/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2524 2023-04-14 12:43:15.000000 daskcheck-0.0.4/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-14 12:43:18.030442 daskcheck-0.0.4/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      680 2023-01-13 14:22:42.000000 daskcheck-0.0.4/bin/daskcheck
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-14 12:43:18.030442 daskcheck-0.0.4/daskcheck/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2023-01-13 14:22:42.000000 daskcheck-0.0.4/daskcheck/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6840 2023-01-13 14:22:42.000000 daskcheck-0.0.4/daskcheck/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6892 2023-01-13 14:22:42.000000 daskcheck-0.0.4/daskcheck/daskcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1090 2023-01-13 14:22:42.000000 daskcheck-0.0.4/daskcheck/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-04-14 12:43:17.000000 daskcheck-0.0.4/daskcheck/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-04-14 12:43:18.030442 daskcheck-0.0.4/daskcheck.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2802 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      304 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-04-14 12:43:18.000000 daskcheck-0.0.4/daskcheck.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-04-14 12:43:18.034442 daskcheck-0.0.4/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1151 2023-04-14 12:41:57.000000 daskcheck-0.0.4/setup.py
```

### Comparing `daskcheck-0.0.3/README.md` & `daskcheck-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,95 @@
+Metadata-Version: 2.1
+Name: daskcheck
+Version: 0.0.4
+Summary: Automatically created environment for python package
+Home-page: http://gitlab.com/jaromrax/daskcheck
+Author: me
+Author-email: mail@gmail.com
+License: GPL2
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 Project daskcheck
 =================
 
-This should allow an easy use of **dask**.
+Help with a simple use of the **dask**
+
+The idea
+--------
 
-Instalation
------------
+1.  define properly the *core function* (*xcorefunc* in the example)
+    with **THE return**
+2.  `daskcheck` then will take care about:
+    -   sending the parameters
+    -   collecting results and saving them to **local json file**
 
-``` {.example}
+Instalation of daskcheck
+------------------------
+
+``` {.bash org-language="sh"}
 pip install daskcheck
 ```
 
+Installation of dask
+--------------------
+
+See <https://docs.dask.org/en/stable/install.html>
+
+``` {.bash org-language="sh"}
+pip install "dask[complete]"
+```
+
+Launching dask scheduler/workers
+--------------------------------
+
+*Pay attention to correct/compatible libraries on different workers*
+
+### Environment needed
+
+    to be done
+
+### Launching scheduler
+
+``` {.bash org-language="sh"}
+dask scheduler --port 8786
+```
+
+### Launching worker
+
+``` {.bash org-language="sh"}
+dask     worker 127.0.0.1:8786 --nworkers 5 --nthreads 1
+```
+
+Testing dask
+------------
+
+*IN DEVELOPMENT...*
+
+This runs (sched and workers are ON) 40x get~cpuinfo~
+
+``` {.bash org-language="sh"}
+./daskcheck.py test
+```
+
+This is solved .... possible to load (unload first). See `tesmod.py`
+
+``` {.bash org-language="sh"}
+./daskcheck.py dask py_file_with_main  1,3
+./daskcheck.py dask py_file_with_main  11..33
+```
+
+Monitoring dask
+---------------
+
+    xdg-open http://localhost:8787
+
+Recollection the data from json
+-------------------------------
+
 Usage
 -----
 
 ``` {.python}
 from daskcheck import daskcheck
 
 from fire import Fire
@@ -48,7 +124,9 @@
     return order, [platform.node(),  f"{time.perf_counter() - start_time:.1f} s" , ni]
 
 
 if __name__=="__main__":
     Fire(main)
 
 ```
+
+
```

### Comparing `daskcheck-0.0.3/bin/daskcheck` & `daskcheck-0.0.4/bin/daskcheck`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.3/daskcheck/config.py` & `daskcheck-0.0.4/daskcheck/config.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.3/daskcheck/daskcheck.py` & `daskcheck-0.0.4/daskcheck/daskcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,20 +116,20 @@
     #print(futures)
     # #li = client.gather(futures)
 
     my_results = {} # DICT - the key is the order of submission
     for future in as_completed(futures):
         n = future.result()
         my_results[n[0]] = n[1] # ORDER IS 1st and the DICT KEY TOO
-        print(f"i... {n[0]:5d}. has ended, totaly {len(my_results)} or {len(parameters)}        ", end="\r")
+        print(f"i... #{n[0]:5d} has ended, totaly {len(my_results):5d} or {len(parameters):5d}        ", end="\r")
 
-    #for k in  sorted(my_results.keys()):
-    #    print(f"{k:5d}", my_results[k] )
+    for k in  sorted(my_results.keys()):
+        print(f"{k:5d}", my_results[k] )
 
-    print("____________________________ Dataframe with results")
+    print("____________________________ Dataframe with results_____________")
     df = pd.DataFrame( my_results ).transpose() # nodes are on rows
     print( df.sort_values( by=[0], ascending = True)  ) # sort by name ==1st member of the list)
     # SORT BY library version.... e.g
     #print( df.sort_values(0).groupby(4, group_keys=True).apply(lambda x:x)  )
 
     # Write LOG file.
     now = dt.datetime.now()
```

### Comparing `daskcheck-0.0.3/daskcheck/unitname.py` & `daskcheck-0.0.4/daskcheck/unitname.py`

 * *Files identical despite different names*

### Comparing `daskcheck-0.0.3/setup.py` & `daskcheck-0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     else:
         raise RuntimeError("Unable to find version string.")
 
 setup(
     name="daskcheck",
     description="Automatically created environment for python package",
     author="me",
+    url="http://gitlab.com/jaromrax/daskcheck",
     author_email="mail@gmail.com",
     license="GPL2",
     version=get_version("daskcheck/version.py"),
     packages=['daskcheck'],
     package_data={'daskcheck': ['data/*']},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
```

