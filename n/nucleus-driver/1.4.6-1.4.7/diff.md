# Comparing `tmp/nucleus_driver-1.4.6.tar.gz` & `tmp/nucleus_driver-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus_driver-1.4.6.tar", last modified: Fri Mar 31 14:14:16 2023, max compression
+gzip compressed data, was "nucleus_driver-1.4.7.tar", last modified: Fri Apr 14 09:59:03 2023, max compression
```

## Comparing `nucleus_driver-1.4.6.tar` & `nucleus_driver-1.4.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 14:14:16.342569 nucleus_driver-1.4.6/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/LICENSE.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-03-31 14:14:16.342569 nucleus_driver-1.4.6/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-03-31 14:14:16.342569 nucleus_driver-1.4.6/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 14:14:16.342569 nucleus_driver-1.4.6/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 14:14:16.342569 nucleus_driver-1.4.6/src/nucleus_driver/
--rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/src/nucleus_driver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/src/nucleus_driver/_assert.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-03-31 07:31:19.000000 nucleus_driver-1.4.6/src/nucleus_driver/_commands.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16923 2023-03-31 13:35:24.000000 nucleus_driver-1.4.6/src/nucleus_driver/_connection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    24616 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/src/nucleus_driver/_download.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16554 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/src/nucleus_driver/_flash.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9653 2023-03-30 13:39:24.000000 nucleus_driver-1.4.6/src/nucleus_driver/_logger.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/src/nucleus_driver/_messages.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    40241 2023-03-30 13:38:55.000000 nucleus_driver-1.4.6/src/nucleus_driver/_parser.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.4.6/src/nucleus_driver/_syslog.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    19018 2023-03-31 07:24:36.000000 nucleus_driver-1.4.6/src/nucleus_driver/app.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11367 2023-03-31 14:09:44.000000 nucleus_driver-1.4.6/src/nucleus_driver/nucleus_driver.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-03-31 14:14:16.342569 nucleus_driver-1.4.6/src/nucleus_driver.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-03-31 14:14:16.000000 nucleus_driver-1.4.6/src/nucleus_driver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-03-31 14:14:16.000000 nucleus_driver-1.4.6/src/nucleus_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-03-31 14:14:16.000000 nucleus_driver-1.4.6/src/nucleus_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-03-31 14:14:16.000000 nucleus_driver-1.4.6/src/nucleus_driver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-03-31 14:14:16.000000 nucleus_driver-1.4.6/src/nucleus_driver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-03-31 14:14:16.000000 nucleus_driver-1.4.6/src/nucleus_driver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/LICENSE.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/src/nucleus_driver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_assert.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    50233 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/_commands.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16923 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/_connection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    24616 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_download.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16554 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_flash.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9653 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/_logger.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_messages.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    40241 2023-03-30 13:38:55.000000 nucleus_driver-1.4.7/src/nucleus_driver/_parser.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.4.7/src/nucleus_driver/_syslog.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    19018 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/app.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11367 2023-04-14 09:56:26.000000 nucleus_driver-1.4.7/src/nucleus_driver/nucleus_driver.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-14 09:59:03.559152 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     9458 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-04-14 09:59:03.000000 nucleus_driver-1.4.7/src/nucleus_driver.egg-info/top_level.txt
```

### Comparing `nucleus_driver-1.4.6/LICENSE.txt` & `nucleus_driver-1.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/PKG-INFO` & `nucleus_driver-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus_driver
-Version: 1.4.6
+Version: 1.4.7
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.4.6/README.md` & `nucleus_driver-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/setup.cfg` & `nucleus_driver-1.4.7/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nucleus_driver
-version = 1.4.6
+version = 1.4.7
 author = Martin Bergene Johansen
 author_email = martin.johansen@nortekgroup.com
 description = driver for the Nortek Nucleus
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nortekgroup/nucleus_driver
 classifiers =
```

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/_assert.py` & `nucleus_driver-1.4.7/src/nucleus_driver/_assert.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/_commands.py` & `nucleus_driver-1.4.7/src/nucleus_driver/_commands.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/_connection.py` & `nucleus_driver-1.4.7/src/nucleus_driver/_connection.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/_download.py` & `nucleus_driver-1.4.7/src/nucleus_driver/_download.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/_flash.py` & `nucleus_driver-1.4.7/src/nucleus_driver/_flash.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/_logger.py` & `nucleus_driver-1.4.7/src/nucleus_driver/_logger.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/_parser.py` & `nucleus_driver-1.4.7/src/nucleus_driver/_parser.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/_syslog.py` & `nucleus_driver-1.4.7/src/nucleus_driver/_syslog.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/app.py` & `nucleus_driver-1.4.7/src/nucleus_driver/app.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver/nucleus_driver.py` & `nucleus_driver-1.4.7/src/nucleus_driver/nucleus_driver.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver.egg-info/PKG-INFO` & `nucleus_driver-1.4.7/src/nucleus_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucleus-driver
-Version: 1.4.6
+Version: 1.4.7
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.4.6/src/nucleus_driver.egg-info/SOURCES.txt` & `nucleus_driver-1.4.7/src/nucleus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

