# Comparing `tmp/eisenmp_examples-0.4.tar.gz` & `tmp/eisenmp_examples-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eisenmp_examples-0.4.tar", last modified: Thu Apr 13 16:32:09 2023, max compression
+gzip compressed data, was "eisenmp_examples-0.4.1.tar", last modified: Fri Apr 14 09:12:24 2023, max compression
```

## Comparing `eisenmp_examples-0.4.tar` & `eisenmp_examples-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.618106 eisenmp_examples-0.4/
--rw-rw-rw-   0        0        0     1525 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/LICENSE
--rw-rw-rw-   0        0        0     1525 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/LICENSE.rst
--rw-rw-rw-   0        0        0      230 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4328 2023-04-13 16:32:09.618106 eisenmp_examples-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3581 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.469852 eisenmp_examples-0.4/eisenmp_examples/
--rw-rw-rw-   0        0        0      344 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/__init__.py
--rw-rw-rw-   0        0        0     2141 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/cmd.py
--rw-rw-rw-   0        0        0    20480 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/database.db
--rw-rw-rw-   0        0        0    10180 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_bruteforce.py
--rw-rw-rw-   0        0        0     6212 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_double_q.py
--rw-rw-rw-   0        0        0     3389 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     6573 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_entry.py
--rw-rw-rw-   0        0        0     8812 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_http.py
--rw-rw-rw-   0        0        0     4457 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     8104 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_prime.py
--rw-rw-rw-   0        0        0     6670 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_web_csv.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.537151 eisenmp_examples-0.4/eisenmp_examples/utils_exa/
--rw-rw-rw-   0        0        0        0 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/utils_exa/__init__.py
--rw-rw-rw-   0        0        0     1921 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_download.py
--rw-rw-rw-   0        0        0     4139 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_search.py
--rw-rw-rw-   0        0        0     6183 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.616156 eisenmp_examples-0.4/eisenmp_examples/worker/
--rw-rw-rw-   0        0        0        0 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/__init__.py
--rw-rw-rw-   0        0        0     3812 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
--rw-rw-rw-   0        0        0     5300 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
--rw-rw-rw-   0        0        0     3621 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
--rw-rw-rw-   0        0        0     4412 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
--rw-rw-rw-   0        0        0     1920 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
--rw-rw-rw-   0        0        0     2382 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
--rw-rw-rw-   0        0        0     1571 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:32:09.509845 eisenmp_examples-0.4/eisenmp_examples.egg-info/
--rw-rw-rw-   0        0        0     4328 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1369 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 16:32:09.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 16:32:08.000000 eisenmp_examples-0.4/eisenmp_examples.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1064 2023-04-13 16:31:24.000000 eisenmp_examples-0.4/pyproject.toml
--rw-rw-rw-   0        0        0      406 2023-04-13 16:32:09.621035 eisenmp_examples-0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.730656 eisenmp_examples-0.4.1/
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     1525 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/LICENSE.rst
+-rw-rw-rw-   0        0        0      230 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4330 2023-04-14 09:12:24.730656 eisenmp_examples-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3581 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.522563 eisenmp_examples-0.4.1/eisenmp_examples/
+-rw-rw-rw-   0        0        0      344 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/__init__.py
+-rw-rw-rw-   0        0        0     2141 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/cmd.py
+-rw-rw-rw-   0        0        0    20480 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/database.db
+-rw-rw-rw-   0        0        0    10406 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_bruteforce.py
+-rw-rw-rw-   0        0        0     6249 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_double_q.py
+-rw-rw-rw-   0        0        0     3330 2023-04-13 20:55:03.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     6573 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_entry.py
+-rw-rw-rw-   0        0        0     8641 2023-04-13 20:55:03.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_http.py
+-rw-rw-rw-   0        0        0     4614 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     8136 2023-04-14 09:04:53.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_prime.py
+-rw-rw-rw-   0        0        0     6608 2023-04-14 09:04:53.000000 eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_web_csv.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.569645 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/
+-rw-rw-rw-   0        0        0        0 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/__init__.py
+-rw-rw-rw-   0        0        0     1921 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_download.py
+-rw-rw-rw-   0        0        0     4139 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_search.py
+-rw-rw-rw-   0        0        0     6183 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.730656 eisenmp_examples-0.4.1/eisenmp_examples/worker/
+-rw-rw-rw-   0        0        0        0 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/__init__.py
+-rw-rw-rw-   0        0        0     3812 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py
+-rw-rw-rw-   0        0        0     5300 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py
+-rw-rw-rw-   0        0        0     3621 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py
+-rw-rw-rw-   0        0        0     4603 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py
+-rw-rw-rw-   0        0        0     2059 2023-04-14 09:04:53.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py
+-rw-rw-rw-   0        0        0     2507 2023-04-14 09:04:52.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py
+-rw-rw-rw-   0        0        0     1571 2023-04-13 16:31:24.000000 eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:12:24.555629 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/
+-rw-rw-rw-   0        0        0     4330 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1369 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-14 09:12:24.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 09:12:23.000000 eisenmp_examples-0.4.1/eisenmp_examples.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1066 2023-04-14 09:07:07.000000 eisenmp_examples-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0      406 2023-04-14 09:12:24.735628 eisenmp_examples-0.4.1/setup.cfg
```

### Comparing `eisenmp_examples-0.4/LICENSE` & `eisenmp_examples-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/LICENSE.rst` & `eisenmp_examples-0.4.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/PKG-INFO` & `eisenmp_examples-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp_examples
-Version: 0.4
+Version: 0.4.1
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
```

### Comparing `eisenmp_examples-0.4/README.md` & `eisenmp_examples-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/cmd.py` & `eisenmp_examples-0.4.1/eisenmp_examples/cmd.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/database.db` & `eisenmp_examples-0.4.1/eisenmp_examples/database.db`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_bruteforce.py` & `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_bruteforce.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Generator module, Worker in /worker folder
 
 Mandatory:
 - import eisenmp
-- worker must have the 'toolbox' as arg in entry function (arg count 1)
+- worker must have the 'toolbox' (kwargs) as arg in entry function (arg count 1)
 - path to worker module and the entry function reference, all are str
 
 """
 import os
 import io
 import time
-import platform
 from zipfile import ZipFile
 
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 
 try:
     from eisenmp.utils_exa.eisenmp_search import SearchStr
@@ -55,38 +54,36 @@
             'german.dic',
         'https://github.com/44xtc44/eisenmp_examples/raw/dev/eisenmp_examples/lang_dictionaries/eng/SCOWL-wl.zip':
             'words.txt',
     }
 
     def __init__(self):
         # load order list, first module is called in an endless loop, you can append your own loop inside the worker
-        self.worker_modules = []  # init for kwargs/toolbox, 'worker_module_set'
+        self.worker_modules = []  # this example sets it later in `worker_module_set`
 
         # Multiprocess vars - override default
         # self.NUM_PROCS = 2  # your process count, default is None: one proc/CPU core
-        # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         # self.NUM_ROWS = 2  # your workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
-        if platform.system() == 'Linux':
-            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # Worker part - toolbox vars survive multiple worker calls
         self.multi_tool_get = None  # custom var to allow only one download of MULTI_TOOL; init later in this example
         self.MULTI_TOOL = None  # pre-defined toolbox.MULTI_TOOL can host the dict from mp_tools_q
         self.INFO_THREAD_MAX = None  # target value for info thread to calculate % and ETA if 'enable_info' set
 
         # custom
         self.use_file_system = False  # False: download and unzip in mem        ------------ SWITCH --------------------
         self.result_lbl = None  # set by caller
         self.num_lists = 0  # add one for each list done, print out worker
         self.lowercase = True
         self.url = None  # 'use_file_system' False, URL of csv file
-        self.zipped_filename = None  # None: we have to loop over two; name of the uncompressed file in zip archive
+        self.zipped_filename = None  # None: have to loop over two archives; name of the uncompressed file in zip arch.
         self.str_permutation = None  # the search string we want to find in the dictionary/wordlist
 
 
 modConf = ModuleConfiguration()  # accessible in module
 searchStr = SearchStr()
 
 
@@ -102,32 +99,33 @@
     Decide raid tactics.
     Brute force on smaller strings. List reduce attempt for larger strings.
 
     Grab config values and push it to the two possible functions.
 
     - (A) len(String) <=  10, combined brute force dictionary attack.
     - (B) len(String) >=  11, Reduce a dictionary len(str) condensed list and count characters.
+
+    See `mp_brute_force` and `mp_reduce` for more info.
     """
-    pass
     modConf.str_permutation = searchStr.search_string
     if modConf.lowercase:
         modConf.str_permutation = modConf.str_permutation.lower()
     searchStr.create_key_word_val_none_shrink(lowercase=modConf.lowercase)  # dict, remove words != len(search str)
     modConf.INFO_THREAD_MAX = len(searchStr.words_dict)  # info thread calc rows done and len
 
-    # ---------- selection of generator function reference ----------
+    # ---------- selection of generator function reference, no () ----------
     brute_force = True if len(modConf.str_permutation) <= 10 else False
     function_ref = mp_brute_force if brute_force else mp_reduce  # decide which function to call
     worker_module_set(function_ref)
 
     msg_b, msg_r = f'\n\t[BRUTE_FORCE]\t{modConf.str_permutation}', f'\n\t[LIST_REDUCTION]\t{modConf.str_permutation}'
     msg = msg_b if function_ref == mp_brute_force else msg_r
     print(msg)
 
-    generator = function_ref(searchStr)
+    generator = function_ref(searchStr)  # `mp_brute_force` or `mp_reduce`
     words_dict = searchStr.words_dict if function_ref == mp_brute_force else None
 
     mP = eisenmp.Mp()
     mP.start(**modConf.__dict__)
     if brute_force:
         for _ in mP.proc_list:
             mP.mp_tools_q.put(words_dict)
@@ -145,27 +143,30 @@
         modConf.multi_tool_get = False
         modConf.worker_modules.append(modConf.list_reducer_module)
 
 
 def mp_brute_force(search_instance):
     """Generator Part
 
-    - Worker 1
+    - Worker 1 - only one worker is active at any time
 
     Produce str permutations for len(str), if len(str) = 3 we have 3! = 6 permutations
+    Have a string and two tools. (A) wordlist as a dict and (B) itertools permutation generator.
+    Searched string is hiding in the permutations.
+    Check if the permutation makes sense and compare it with the wordlist.
     """
     generator = search_instance.generator(lowercase=modConf.lowercase)  # itertools
     return generator
 
 
 def mp_reduce(search_instance):
     """
     - Worker 2
 
-    We took all language word list and put em in a dict.
+    Took all language word list and put them in a dict.
     Deleted all words with more or less characters.
 
     Worker will now reduce the list generated from dict.
     Remove all words not matching characters and
     character count in search str from list.
     Worker puts result in output q.
     """
@@ -216,15 +217,15 @@
 
 
 def wordlists_in_memory(downloader):
     """Open zip archive and load one file 'zipped_filename'
     Return as text.
     """
     archive = downloader.unzip_mem()
-    # text files are all utf-8 encoded, py try open cp1252 on my windows
+    # text files are all utf-8 encoded, else python tries to open cp1252 format on german windows
     with io.TextIOWrapper(archive.open(modConf.zipped_filename, 'r'), encoding="UTF-8") as file:
         txt_lst = file.readlines()
     return txt_lst
 
 
 def wordlist_download(downloader):
     """Store response object in downloader instance.
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_double_q.py` & `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_double_q.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Template for Manager
 
 - Watchdog Thread included, shows pid of its proc
 - double feeder
 - custom queues and queues in category
 - fake production of audio and video coding, is loop through to result dict
-- two processors work on different streams (src is same here, so what)
+- two processors work on different streams, batches, (src is same here, so what)
 
 """
 import os
 import threading
 import time
 import platform
 import eisenmp
@@ -81,22 +81,21 @@
         super().__init__()
         self.worker_modules = [  # in-bld-res
             self.template_module,  # other modules must start threaded, else we hang
             self.watchdog_module  # second; thread function call mandatory, last module loaded first
         ]
 
         # Multiprocess vars - override default
-        self.NUM_PROCS = 2  # your process count, default is None: one proc/CPU core
+        self.NUM_PROCS = 2  # your process count, each 'batch' on one CPU core, default is None: one proc/CPU core
         self.NUM_ROWS = 3  # arbitrary num here
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
-        self.RESULT_LABEL = 'fake production of audio and video coding for WHO studios'
+        self.RESULT_LABEL = 'fake production of audio and video for WHO studios'  # RESULT_LABEL for RESULTS_PRINT
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
-        if platform.system() == 'Linux':
-            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # work to do
         self.sleep_time = 20  # watchdog
         self.num_of_lists = 0  # worker lists done counter
 
         # vars lived before in worker module classes
         self.header_aud = None  # pre-defined, use in whole worker mod, save input list header to mark output header
@@ -117,23 +116,23 @@
     -
     """
     q_cat_name_maxsize = [
         # q_category, q_name, q_maxsize; find your 100 Queues in the debugger, toolbox
         ('batch_1', 'audio_lg', 5),  # queues for batch_1
         ('batch_1', 'video_in', 1),  # dict avail. in worker module: toolbox.batch_1['video_in'].get()
         ('batch_7', 'audio_lg', 3),  # queues for batch_7, created but not used so far, can play with
-        ('batch_7', 'video_in', 1),
+        ('batch_7', 'video_in', 1)
     ]
     mP = eisenmp.Mp()
 
     # create custom queues with category and name
     mP.queue_cust_dict_category_create(*q_cat_name_maxsize)  # create queues, store in {custom} {category} dict
 
     audio_q_b1 = mP.queue_cust_dict_cat['batch_1']['audio_lg']  # USE Queue:
-    video_q_b1 = mP.queue_cust_dict_cat['batch_1']['video_in']  # toolbox.batch_1['video_in'].get()
+    video_q_b1 = mP.queue_cust_dict_cat['batch_1']['video_in']  # worker module: toolbox.batch_1['video_in'].get()
     audio_q_b7 = mP.queue_cust_dict_cat['batch_7']['audio_lg']
     video_q_b7 = mP.queue_cust_dict_cat['batch_7']['video_in']  # toolbox.batch_7['video_in'].get()
 
     mP.start(**modConf.__dict__)  # create processes, load worker mods, start threads (output_p coll, info)
     mP.run_q_feeder(generator=audio_generator_batch_1(), input_q=audio_q_b1)
     mP.run_q_feeder(generator=video_generator_batch_1(), input_q=video_q_b1)
     mP.run_q_feeder(generator=audio_generator_batch_7(), input_q=audio_q_b7)
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_each_flask_orm_srv_one_cpu.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """See some examples,
 it's always the same process,
 you extend or switch off defaults
 
 """
 import os
 import time
-import platform
+
 import eisenmp
 
 
 class ModuleConfiguration:
     """
     You can use the class to have your variables available in the module.
 
@@ -30,16 +30,15 @@
         # Multiprocess vars - override default
         self.NUM_PROCS = 6  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 1  # tell iterator to make only one list row, each worker needs only one number
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULT_LABEL = 'No result, server blocks'  # pretty print as result header for RESULTS_PRINT
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
-        if platform.system() == 'Linux':
-            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
 
 modConf = ModuleConfiguration()  # Accessible in the module.
 
 
 def manager():
     """
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_entry.py` & `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_entry.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_http.py` & `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Python 3 server example
 # https://pythonbasics.org/webserver/
 # mod by 44xtc44
 
 import os
 import time
-import platform
+
 from http.server import BaseHTTPRequestHandler, HTTPServer
 
 import eisenmp
 
 hostName = "localhost"
 serverPort = 12_000
 
@@ -60,18 +60,16 @@
 
         # Multiprocess vars - override default
         self.NUM_PROCS = 16  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 1  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
-        # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         self.RESULT_LABEL = 'revised.csv, Average calculation'  # pretty print as result header for RESULTS_PRINT
-        if platform.system() == 'Linux':
-            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # 'not enough work example', useless worker auto shutdown, the modules return False
         self.radio_name = None  # define to get it as key in 'modConf' dictionary and worker use 'toolbox.radio_name'
         self.radio_url = None
         self.sleep_time = 60  # if watchdog enabled, toolbox.sleep_time = 60
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py` & `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_multi_srv_each_cpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """See some examples,
 it's always the same process,
 you extend or switch off defaults
 
 
 Multiple server on each CPU core, if server has that many cores.
 needs Flask_SQLAlchemy_Project_Template >=1.3
+
+module_loader mod of eisenmp must be informed, STOP_MSG_DISABLE=True.
+All worker are thread started -> and can not send 'return False' (run_forever()),
+no stop confirmation of module_loader mod of eisenmp avail
 """
 import os
 import time
-import platform
+
 import eisenmp
 
 
 class ModuleConfiguration:
     """
     You can use the class to have your variables available in the module.
 
@@ -39,16 +43,15 @@
 
         # Multiprocess vars - override default
         self.NUM_PROCS = 3  # your process count, default is None: one proc/CPU core
         self.NUM_ROWS = 1  # tell iterator to make only one list row, each worker needs only one number
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = False  # shows content of results dict with ticket numbers, check tickets
-        if platform.system() == 'Linux':
-            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         self.STOP_MSG_DISABLE = True  # module_loader leaves worker loop and waits for stop msg in mp_process_q
 
         # worker port groups, nailed on one cpu
         self.blue_lst = [0]  # one CPU core for blue list, if toolbox.kwargs['START_SEQUENCE_NUM'] in worker_blue_lst,
         self.yellow_lst = [1]  # one CPU core for yellow, process spawn num 1; (class ProcEnv 'run_proc -> core')
         self.green_lst = [2]
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_prime.py` & `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_prime.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 This is NOT ADVISABLE and only to show the mechanics.
 Use a separate worker module to not import your 'Generator' imports twice.
 That is what the loader is for.
 """
 import os
 import time
 import math
-import platform
 
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 
 dir_name = os.path.dirname(__file__)
 
 
@@ -43,16 +42,15 @@
         # Multiprocess vars - override default
         self.NUM_PROCS = 5  # your process count, default is None: one proc/CPU core
         # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         self.NUM_ROWS = 42  # your workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
-        if platform.system() == 'Linux':
-            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # custom part, write your own Attributes
         self.range_num = 10 ** 4  # got a target/max value and NUM_ROWS for each proc, can calc ETA est. time arrival
         self.INFO_THREAD_MAX = self.range_num  # target value for info thread to calculate % and ETA
         # self.INFO_ENABLE = True  # [baustelle]
         self.n = 10 ** 12  # ten with zero count, 10_000_000_000_000_000
         self.say_hello = 'Hello'  # just to show that worker can [read] all attributes of instance, in 'worker_prime()'
@@ -189,16 +187,18 @@
 
 def main():
     """
     """
     start = time.perf_counter()
 
     mP = generator_prime()
+
     while 1:
-        # running threads, wait
+        # running generator threads and procs,
+        # keep main() alive, else procs end, and we can not access results
         if mP.begin_proc_shutdown:
             break
         time.sleep(1)
 
     msg_time = 'Example Prime numbers, Time in sec: ', round((time.perf_counter() - start))
     print(msg_time)
     msg_result = e_utils.Result.result_dict
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/eisenmp_exa_web_csv.py` & `eisenmp_examples-0.4.1/eisenmp_examples/eisenmp_exa_web_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Green CSV generator / Worker in folder /worker
 
-We download a NZ government report and calculate the average of split lists.
+Download a NZ government report and calculate the average of split lists.
 See URL. Try your own URL. They have a lot.
 """
 
 import os
 import csv
 import time
-import platform
+
 from io import TextIOWrapper
 from zipfile import ZipFile
 
 import eisenmp
 import eisenmp.utils.eisenmp_utils as e_utils
 try:
     from eisenmp.utils_exa.eisenmp_download import DownLoad
@@ -46,22 +46,21 @@
         self.worker_modules = [
             self.first_module,  # second module must be started by a thread, else we hang
             self.watchdog_module,
         ]
 
         # Multiprocess vars - override default
         self.NUM_PROCS = 5  # your process count, default is None: one proc/CPU core
+        # max generator / NUM_ROWS = number of tickets; 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         self.NUM_ROWS = 50_000  # workload spread, list (generator items) to calc in one loop, default is None: 1_000
         self.RESULTS_STORE = True  # keep in dictionary, will crash the system if store GB network chunks in mem
         self.RESULTS_PRINT = True  # result rows of output are collected in a list, display if processes are stopped
         self.RESULTS_DICT_PRINT = True  # shows content of results dict with ticket numbers, check tickets
-        # max generator / NUM_ROWS = number of tickets, 10_000 / 42 = 238.095 -> 238 lists with ticket numbers
         self.RESULT_LABEL = 'revised.csv, Average calculation'  # pretty print as result header for RESULTS_PRINT
-        if platform.system() == 'Linux':
-            self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
+        # self.START_METHOD = 'fork'  # 'spawn' is default if unused; also use 'forkserver' or 'fork' on Unix only
 
         # CSV part
         self.use_file_system = False  # False: download and unzip in mem; True must exist on fs ------------- SWITCH ---
         self.url = self.dl_url  # False 'use_file_system', URL of csv file
         self.zipped_filename = 'revised.csv'  # name of the uncompressed file in zip archive
         self.csv_col_name = 'value'  # CSV table column header
         self.sleep_time = 45  # watchdog module in 'worker_modules' list
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_download.py` & `eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_download.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_search.py` & `eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_search.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/utils_exa/eisenmp_utils.py` & `eisenmp_examples-0.4.1/eisenmp_examples/utils_exa/eisenmp_utils.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py` & `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_bruteforce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py` & `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_bf_reduce.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py` & `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_csv.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_double.py` & `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_double.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-"""
+"""Worker of fake production
 
+Output queue list header must be different for audio and video to save results.
+``header_aud`` and ``header_vid`` are pre-defined in ``ModuleConfiguration``
 """
 import time
 
 
 def worker_entrance(toolbox):
     """
     - WORKER - Called in a loop.
@@ -23,15 +25,15 @@
 
 
 def batch_1_video_get(toolbox):
     """"""
     while 1:
         if not toolbox.batch_1['video_in'].empty():
             lst = toolbox.batch_1['video_in'].get()
-            toolbox.num_of_lists += 1  # list counter prn screen
+            toolbox.num_of_lists += 1  # list counter prn screen, ModuleConfiguration self.num_of_lists
             return lst
 
 
 def batch_1_audio_get(toolbox):
     """"""
     while 1:
         if not toolbox.batch_1['audio_lg'].empty():
@@ -56,22 +58,21 @@
             return lst
 
 
 def remove_header(lst):
     """Transport ticket with consecutive number.
     Remove if no recreation of order is necessary.
     Can reuse list for result, if rebuild order.
-
-    Use self.header_msg attribute to overwrite default header string
     """
     del lst[0]  # remove header str
 
 
 def send_eta_data(toolbox, lst):
     """list of [PERF_HEADER_ETA, PERF_CURRENT_ETA] to ProcInfo, to calc arrival time ETA
+    pure option, broken in version 0.4
     """
     toolbox.PERF_CURRENT_ETA = len(lst)
     perf_lst = [toolbox.PERF_HEADER_ETA + toolbox.WORKER_NAME,  # binary head
                 toolbox.PERF_CURRENT_ETA]
     # disable info q will block all
     toolbox.mp_info_q.put(perf_lst)  # ProcInfo calc arrival time and % from info_q, of all proc lists
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py` & `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_flask_orm_srv_one_cpu.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,30 +30,32 @@
         port = yellow_q_get(toolbox)[1]
 
     col_end = color_dict['END']
 
     msg = col + f'\nWORKER_MSG worker: {toolbox.WORKER_ID} pid: {toolbox.WORKER_PID} server port: {port}' + col_end
     toolbox.mp_print_q.put(msg)
 
-    # Flask
+    # Flask - app_factory, start Flask via function call
     app_factory = create_app(port)  # flask, we feed port number to update the route -> Html page with our address
     if not os.path.isfile(db_path):  # do not kill db, if exists; MUST exist if many srv, else create by many srv, crash
         setup_database(app_factory)
     app_factory.run(host="localhost", port=port)
 
 
 def blue_q_get(toolbox):
-    """"""
+    """Receive port numbers from queue.
+    Same as list.pop()
+    """
     while 1:
         if not toolbox.mp_blue_q.empty():
             port_lst = toolbox.mp_blue_q.get()  # has header with serial number
             return port_lst
 
 
 def yellow_q_get(toolbox):
-    """"""
+    """Receive port numbers from queue."""
     while 1:
         if not toolbox.mp_yellow_q.empty():
             port_lst = toolbox.mp_yellow_q.get()  # has header with serial number
             return port_lst
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py` & `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_multi_srv_each_cpu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import threading
 from Flask_SQLAlchemy_Project_Template import create_app, setup_database, db_path
 
+# can use classes here also
 color_dict = {
     'PURPLE': '\033[1;35;48m',
     'CYAN': '\033[1;36;48m',
     'BOLD': '\033[1;37;48m',
     'BLUE': '\033[1;34;48m',
     'GREEN': '\033[1;32;48m',
     'YELLOW': '\033[1;33;48m',
@@ -51,28 +52,28 @@
                 f'SERVER: http://{network}:{port}' + col_end
     toolbox.mp_print_q.put(msg)
 
     # end, return None (Nothing is None), loader leaves worker loop and waits for stop msg in mp_process_q
 
 
 def blue_q_get(toolbox):
-    """"""
+    """Receive port numbers from queue."""
     while 1:
         if not toolbox.mp_blue_q.empty():
             port_lst = toolbox.mp_blue_q.get()  # has header with serial number
             return port_lst
 
 
 def yellow_q_get(toolbox):
-    """"""
+    """Receive port numbers from queue."""
     while 1:
         if not toolbox.mp_yellow_q.empty():
             port_lst = toolbox.mp_yellow_q.get()
             return port_lst
 
 
 def green_q_get(toolbox):
-    """"""
+    """Receive port numbers from queue."""
     while 1:
         if not toolbox.mp_green_q.empty():
             port_lst = toolbox.mp_green_q.get()
             return port_lst
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py` & `eisenmp_examples-0.4.1/eisenmp_examples/worker/eisenmp_exa_wrk_watchdog.py`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/eisenmp_examples.egg-info/PKG-INFO` & `eisenmp_examples-0.4.1/eisenmp_examples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eisenmp-examples
-Version: 0.4
+Version: 0.4.1
 Summary: eisenmp multiprocess(or) example collection for server and mobiles
 Author: René Horn
 Author-email: René Horn <rene_horn@gmx.net>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/44xtc44
 Project-URL: documentation, https://eisenmp.readthedocs.io/
 Project-URL: repository, https://github.com/44xtc44/eisenmp
```

### Comparing `eisenmp_examples-0.4/eisenmp_examples.egg-info/SOURCES.txt` & `eisenmp_examples-0.4.1/eisenmp_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eisenmp_examples-0.4/pyproject.toml` & `eisenmp_examples-0.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eisenmp_examples"
-version = "0.4"
+version = "0.4.1"
 authors = [{name = "René Horn", email = "rene_horn@gmx.net" }]
 description = "eisenmp multiprocess(or) example collection for server and mobiles"
 keywords = ['multiprocess framework', 'examples eisenmp']
 license = {text = "BSD-3-Clause"}
 readme = "README.md"
 requires-python = ">=3.7"
```

