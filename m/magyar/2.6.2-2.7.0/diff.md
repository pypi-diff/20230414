# Comparing `tmp/magyar-2.6.2.tar.gz` & `tmp/magyar-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.6.2.tar", last modified: Fri Apr 14 15:16:18 2023, max compression
+gzip compressed data, was "magyar-2.7.0.tar", last modified: Fri Apr 14 16:27:17 2023, max compression
```

## Comparing `magyar-2.6.2.tar` & `magyar-2.7.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 15:16:18.249393 magyar-2.6.2/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-14 15:16:18.249393 magyar-2.6.2/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 19:21:03.000000 magyar-2.6.2/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 15:16:18.249393 magyar-2.6.2/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1822 2023-04-14 15:16:18.000000 magyar-2.6.2/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      138 2023-04-14 15:16:18.000000 magyar-2.6.2/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 15:16:18.000000 magyar-2.6.2/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 15:16:18.000000 magyar-2.6.2/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-14 15:16:18.249393 magyar-2.6.2/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      972 2023-04-14 15:12:58.000000 magyar-2.6.2/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 16:27:17.017003 magyar-2.7.0/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1535 2023-04-14 16:27:17.017003 magyar-2.7.0/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 19:21:03.000000 magyar-2.7.0/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 16:27:17.017003 magyar-2.7.0/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1535 2023-04-14 16:27:16.000000 magyar-2.7.0/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-14 16:27:16.000000 magyar-2.7.0/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 16:27:16.000000 magyar-2.7.0/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-14 16:27:16.000000 magyar-2.7.0/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)     9057 2023-04-13 19:56:03.000000 magyar-2.7.0/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-14 16:27:17.017003 magyar-2.7.0/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-14 16:26:47.000000 magyar-2.7.0/setup.py
```

### Comparing `magyar-2.6.2/PKG-INFO` & `magyar-2.7.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.6.2
-Summary: Magyar nevek listája
-Home-page: https://github.com/kobanya
+Version: 2.7.0
+Summary: Hungarian names...
+Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
-Author-email: nagy.bela.budapest@gmail.com
-License: MIT
-Keywords: magyar nevek
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # magyar
 
 
 ## Leírás
```

### Comparing `magyar-2.6.2/README.md` & `magyar-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `magyar-2.6.2/magyar.egg-info/PKG-INFO` & `magyar-2.7.0/magyar.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.6.2
-Summary: Magyar nevek listája
-Home-page: https://github.com/kobanya
+Version: 2.7.0
+Summary: Hungarian names...
+Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
-Author-email: nagy.bela.budapest@gmail.com
-License: MIT
-Keywords: magyar nevek
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
+Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # magyar
 
 
 ## Leírás
```

