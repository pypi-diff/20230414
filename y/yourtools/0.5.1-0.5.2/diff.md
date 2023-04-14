# Comparing `tmp/yourtools-0.5.1.tar.gz` & `tmp/yourtools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yourtools-0.5.1.tar", last modified: Fri Apr 14 10:39:04 2023, max compression
+gzip compressed data, was "dist/yourtools-0.5.2.tar", last modified: Fri Apr 14 10:47:33 2023, max compression
```

## Comparing `yourtools-0.5.1.tar` & `yourtools-0.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:39:04.000000 yourtools-0.5.1/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools/db/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.1/yourtools/db/__init__.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.1/yourtools/db/dbutils.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.1/yourtools/db/hive.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.1/yourtools/db/mysql.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.1/yourtools/Azkaban.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      723 2023-04-14 09:47:09.000000 yourtools-0.5.1/yourtools/Time.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     5929 2023-04-14 10:23:17.000000 yourtools-0.5.1/yourtools/WeChat.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      469 2023-04-13 08:48:52.000000 yourtools-0.5.1/yourtools/__init__.py
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/SOURCES.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/dependency_links.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/requires.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-14 10:39:04.000000 yourtools-0.5.1/yourtools.egg-info/top_level.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.1/README.md
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.1/requirements.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-07 10:28:09.000000 yourtools-0.5.1/setup.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 10:39:04.000000 yourtools-0.5.1/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-14 10:39:04.000000 yourtools-0.5.1/setup.cfg
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:47:33.000000 yourtools-0.5.2/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:47:33.000000 yourtools-0.5.2/yourtools/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:47:33.000000 yourtools-0.5.2/yourtools/db/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.2/yourtools/db/__init__.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.2/yourtools/db/dbutils.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.2/yourtools/db/hive.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.2/yourtools/db/mysql.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.2/yourtools/Azkaban.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      723 2023-04-14 09:47:09.000000 yourtools-0.5.2/yourtools/Time.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     5929 2023-04-14 10:23:17.000000 yourtools-0.5.2/yourtools/WeChat.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      474 2023-04-14 10:42:59.000000 yourtools-0.5.2/yourtools/__init__.py
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 10:47:33.000000 yourtools-0.5.2/yourtools.egg-info/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 10:47:33.000000 yourtools-0.5.2/yourtools.egg-info/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-14 10:47:33.000000 yourtools-0.5.2/yourtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-14 10:47:33.000000 yourtools-0.5.2/yourtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-14 10:47:33.000000 yourtools-0.5.2/yourtools.egg-info/requires.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-14 10:47:33.000000 yourtools-0.5.2/yourtools.egg-info/top_level.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.2/README.md
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.2/requirements.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-14 10:46:10.000000 yourtools-0.5.2/setup.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 10:47:33.000000 yourtools-0.5.2/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-14 10:47:33.000000 yourtools-0.5.2/setup.cfg
```

### Comparing `yourtools-0.5.1/yourtools/db/dbutils.py` & `yourtools-0.5.2/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.1/yourtools/db/hive.py` & `yourtools-0.5.2/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.1/yourtools/db/mysql.py` & `yourtools-0.5.2/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.1/yourtools/Azkaban.py` & `yourtools-0.5.2/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.1/yourtools/Time.py` & `yourtools-0.5.2/yourtools/Time.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.1/yourtools/WeChat.py` & `yourtools-0.5.2/yourtools/WeChat.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.1/yourtools.egg-info/PKG-INFO` & `yourtools-0.5.2/yourtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.5.1/README.md` & `yourtools-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.1/setup.py` & `yourtools-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.1/PKG-INFO` & `yourtools-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.5.1
+Version: 0.5.2
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

