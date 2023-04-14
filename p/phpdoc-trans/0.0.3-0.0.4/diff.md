# Comparing `tmp/phpdoc-trans-0.0.3.tar.gz` & `tmp/phpdoc-trans-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/phpdoc-trans-0.0.3.tar", last modified: Fri Apr 14 01:38:24 2023, max compression
+gzip compressed data, was "phpdoc-trans-0.0.4.tar", last modified: Fri Apr 14 09:58:05 2023, max compression
```

## Comparing `phpdoc-trans-0.0.3.tar` & `phpdoc-trans-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-04-14 01:38:24.810662 phpdoc-trans-0.0.3/
--rw-r--r--   0 matt       (501) staff       (20)     1068 2023-04-14 01:08:12.000000 phpdoc-trans-0.0.3/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)     1020 2023-04-14 01:38:24.810136 phpdoc-trans-0.0.3/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      601 2023-04-14 00:21:20.000000 phpdoc-trans-0.0.3/README.md
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-04-14 01:38:24.806927 phpdoc-trans-0.0.3/phpdoc_trans/
--rw-r--r--   0 matt       (501) staff       (20)        0 2023-04-14 00:34:49.000000 phpdoc-trans-0.0.3/phpdoc_trans/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     3600 2023-04-14 00:37:26.000000 phpdoc-trans-0.0.3/phpdoc_trans/main.py
--rw-r--r--   0 matt       (501) staff       (20)     1127 2023-04-13 23:58:06.000000 phpdoc-trans-0.0.3/phpdoc_trans/spinner.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-04-14 01:38:24.809566 phpdoc-trans-0.0.3/phpdoc_trans.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     1020 2023-04-14 01:38:24.000000 phpdoc-trans-0.0.3/phpdoc_trans.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      314 2023-04-14 01:38:24.000000 phpdoc-trans-0.0.3/phpdoc_trans.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-04-14 01:38:24.000000 phpdoc-trans-0.0.3/phpdoc_trans.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)       56 2023-04-14 01:38:24.000000 phpdoc-trans-0.0.3/phpdoc_trans.egg-info/entry_points.txt
--rw-r--r--   0 matt       (501) staff       (20)       26 2023-04-14 01:38:24.000000 phpdoc-trans-0.0.3/phpdoc_trans.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)       13 2023-04-14 01:38:24.000000 phpdoc-trans-0.0.3/phpdoc_trans.egg-info/top_level.txt
--rw-r--r--   0 matt       (501) staff       (20)       38 2023-04-14 01:38:24.810824 phpdoc-trans-0.0.3/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)      894 2023-04-14 01:38:21.000000 phpdoc-trans-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/phpdoc_trans/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/phpdoc_trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/phpdoc_trans/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/phpdoc_trans/spinner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 09:58:05.000000 phpdoc-trans-0.0.4/phpdoc_trans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:58:05.839954 phpdoc-trans-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-14 09:57:56.000000 phpdoc-trans-0.0.4/setup.py
```

### Comparing `phpdoc-trans-0.0.3/LICENSE` & `phpdoc-trans-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `phpdoc-trans-0.0.3/PKG-INFO` & `phpdoc-trans-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phpdoc-trans
-Version: 0.0.3
+Version: 0.0.4
 Summary: PHP doc transaction tool
 Home-page: https://github.com/AtlanticF/phpdoc-openai-trans
 Author: meifeng.song
 Author-email: atlanticfeng@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phpdoc-trans-0.0.3/README.md` & `phpdoc-trans-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `phpdoc-trans-0.0.3/phpdoc_trans/main.py` & `phpdoc-trans-0.0.4/phpdoc_trans/main.py`

 * *Files identical despite different names*

### Comparing `phpdoc-trans-0.0.3/phpdoc_trans/spinner.py` & `phpdoc-trans-0.0.4/phpdoc_trans/spinner.py`

 * *Files identical despite different names*

### Comparing `phpdoc-trans-0.0.3/phpdoc_trans.egg-info/PKG-INFO` & `phpdoc-trans-0.0.4/phpdoc_trans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phpdoc-trans
-Version: 0.0.3
+Version: 0.0.4
 Summary: PHP doc transaction tool
 Home-page: https://github.com/AtlanticF/phpdoc-openai-trans
 Author: meifeng.song
 Author-email: atlanticfeng@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phpdoc-trans-0.0.3/setup.py` & `phpdoc-trans-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open("README.md", encoding="utf8") as f_r:
         _long_description = f_r.read()
 except FileNotFoundError:
     _long_description = ""
 
 setup(
     name='phpdoc-trans',
-    version='0.0.3',
+    version='0.0.4',
     packages=['phpdoc_trans'],
     install_requires=[
         'click',
         'openai',
         'bs4',
         'progress'
     ],
```

