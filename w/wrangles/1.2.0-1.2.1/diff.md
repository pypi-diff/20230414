# Comparing `tmp/wrangles-1.2.0.tar.gz` & `tmp/wrangles-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrangles-1.2.0.tar", last modified: Tue Apr 11 22:32:34 2023, max compression
+gzip compressed data, was "wrangles-1.2.1.tar", last modified: Fri Apr 14 19:34:10 2023, max compression
```

## Comparing `wrangles-1.2.0.tar` & `wrangles-1.2.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.840601 wrangles-1.2.0/
--rw-rw-rw-   0        0        0     3615 2023-04-11 22:32:34.840601 wrangles-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3102 2023-03-30 14:19:22.000000 wrangles-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.816665 wrangles-1.2.0/Wrangles.egg-info/
--rw-rw-rw-   0        0        0     3615 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1538 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-11 22:32:34.000000 wrangles-1.2.0/Wrangles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-11 22:32:34.848579 wrangles-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1205 2023-04-11 22:14:24.000000 wrangles-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.814672 wrangles-1.2.0/wrangles/
--rw-rw-rw-   0        0        0      565 2022-06-23 19:42:00.000000 wrangles-1.2.0/wrangles/__init__.py
--rw-rw-rw-   0        0        0     1681 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/auth.py
--rw-rw-rw-   0        0        0      840 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/batching.py
--rw-rw-rw-   0        0        0     2069 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/classify.py
--rw-rw-rw-   0        0        0      559 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/config.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.831625 wrangles-1.2.0/wrangles/connectors/
--rw-rw-rw-   0        0        0      449 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/connectors/__init__.py
--rw-rw-rw-   0        0        0     7100 2023-04-11 22:29:27.000000 wrangles-1.2.0/wrangles/connectors/akeneo.py
--rw-rw-rw-   0        0        0    11023 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/ckan.py
--rw-rw-rw-   0        0        0     7811 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/file.py
--rw-rw-rw-   0        0        0     2498 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/http.py
--rw-rw-rw-   0        0        0     1883 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/jinja.py
--rw-rw-rw-   0        0        0     4537 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/mongodb.py
--rw-rw-rw-   0        0        0     6136 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/mssql.py
--rw-rw-rw-   0        0        0     4372 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/mysql.py
--rw-rw-rw-   0        0        0     6328 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/notification.py
--rw-rw-rw-   0        0        0     5892 2022-06-23 19:42:00.000000 wrangles-1.2.0/wrangles/connectors/postgres.py
--rw-rw-rw-   0        0        0    16169 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/pricefx.py
--rw-rw-rw-   0        0        0     4534 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/recipe.py
--rw-rw-rw-   0        0        0     8530 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/s3.py
--rw-rw-rw-   0        0        0     4756 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/salesforce.py
--rw-rw-rw-   0        0        0     4442 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/sftp.py
--rw-rw-rw-   0        0        0     2430 2022-08-10 19:07:21.000000 wrangles-1.2.0/wrangles/connectors/ssh.py
--rw-rw-rw-   0        0        0     5651 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/connectors/test.py
--rw-rw-rw-   0        0        0     8040 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/connectors/train.py
--rw-rw-rw-   0        0        0     1899 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/console.py
--rw-rw-rw-   0        0        0     1592 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/data.py
--rw-rw-rw-   0        0        0    10183 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/extract.py
--rw-rw-rw-   0        0        0     4412 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/format.py
--rw-rw-rw-   0        0        0    19601 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/recipe.py
-drwxrwxrwx   0        0        0        0 2023-04-11 22:32:34.839603 wrangles-1.2.0/wrangles/recipe_wrangles/
--rw-rw-rw-   0        0        0      562 2022-06-23 19:42:00.000000 wrangles-1.2.0/wrangles/recipe_wrangles/__init__.py
--rw-rw-rw-   0        0        0     6878 2023-03-30 21:18:55.000000 wrangles-1.2.0/wrangles/recipe_wrangles/convert.py
--rw-rw-rw-   0        0        0     8582 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/recipe_wrangles/create.py
--rw-rw-rw-   0        0        0    19584 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/recipe_wrangles/extract.py
--rw-rw-rw-   0        0        0     8055 2023-04-10 17:05:21.000000 wrangles-1.2.0/wrangles/recipe_wrangles/format.py
--rw-rw-rw-   0        0        0    26422 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/recipe_wrangles/main.py
--rw-rw-rw-   0        0        0     8570 2023-04-10 17:05:21.000000 wrangles-1.2.0/wrangles/recipe_wrangles/merge.py
--rw-rw-rw-   0        0        0     7681 2023-04-10 17:05:21.000000 wrangles-1.2.0/wrangles/recipe_wrangles/select.py
--rw-rw-rw-   0        0        0     6435 2023-04-10 17:05:21.000000 wrangles-1.2.0/wrangles/recipe_wrangles/split.py
--rw-rw-rw-   0        0        0     1875 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/select.py
--rw-rw-rw-   0        0        0     2099 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/standardize.py
--rw-rw-rw-   0        0        0     6100 2022-12-21 19:41:28.000000 wrangles-1.2.0/wrangles/train.py
--rw-rw-rw-   0        0        0     3502 2023-04-11 22:14:04.000000 wrangles-1.2.0/wrangles/translate.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.074519 wrangles-1.2.1/
+-rw-rw-rw-   0        0        0     3615 2023-04-14 19:34:10.074519 wrangles-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3102 2023-03-30 14:19:22.000000 wrangles-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.051580 wrangles-1.2.1/Wrangles.egg-info/
+-rw-rw-rw-   0        0        0     3615 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1538 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 19:34:09.000000 wrangles-1.2.1/Wrangles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-14 19:34:10.075520 wrangles-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2023-04-14 19:13:56.000000 wrangles-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.049586 wrangles-1.2.1/wrangles/
+-rw-rw-rw-   0        0        0      565 2022-06-23 19:42:00.000000 wrangles-1.2.1/wrangles/__init__.py
+-rw-rw-rw-   0        0        0     1681 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/auth.py
+-rw-rw-rw-   0        0        0      840 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/batching.py
+-rw-rw-rw-   0        0        0     2069 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/classify.py
+-rw-rw-rw-   0        0        0      559 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/config.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.066540 wrangles-1.2.1/wrangles/connectors/
+-rw-rw-rw-   0        0        0      449 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/connectors/__init__.py
+-rw-rw-rw-   0        0        0     7100 2023-04-11 22:29:27.000000 wrangles-1.2.1/wrangles/connectors/akeneo.py
+-rw-rw-rw-   0        0        0    11023 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/ckan.py
+-rw-rw-rw-   0        0        0     7811 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/file.py
+-rw-rw-rw-   0        0        0     2498 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/http.py
+-rw-rw-rw-   0        0        0     1883 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/jinja.py
+-rw-rw-rw-   0        0        0     4537 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/mongodb.py
+-rw-rw-rw-   0        0        0     6136 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/mssql.py
+-rw-rw-rw-   0        0        0     4372 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/mysql.py
+-rw-rw-rw-   0        0        0     6328 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/notification.py
+-rw-rw-rw-   0        0        0     5892 2022-06-23 19:42:00.000000 wrangles-1.2.1/wrangles/connectors/postgres.py
+-rw-rw-rw-   0        0        0    16169 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/pricefx.py
+-rw-rw-rw-   0        0        0     4534 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/recipe.py
+-rw-rw-rw-   0        0        0     8530 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/s3.py
+-rw-rw-rw-   0        0        0     4756 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/salesforce.py
+-rw-rw-rw-   0        0        0     4442 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/sftp.py
+-rw-rw-rw-   0        0        0     2430 2022-08-10 19:07:21.000000 wrangles-1.2.1/wrangles/connectors/ssh.py
+-rw-rw-rw-   0        0        0     5651 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/connectors/test.py
+-rw-rw-rw-   0        0        0     8040 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/connectors/train.py
+-rw-rw-rw-   0        0        0     1899 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/console.py
+-rw-rw-rw-   0        0        0     1592 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/data.py
+-rw-rw-rw-   0        0        0    10183 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/extract.py
+-rw-rw-rw-   0        0        0     4412 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/format.py
+-rw-rw-rw-   0        0        0    19918 2023-04-14 15:48:30.000000 wrangles-1.2.1/wrangles/recipe.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:34:10.073521 wrangles-1.2.1/wrangles/recipe_wrangles/
+-rw-rw-rw-   0        0        0      562 2022-06-23 19:42:00.000000 wrangles-1.2.1/wrangles/recipe_wrangles/__init__.py
+-rw-rw-rw-   0        0        0     6878 2023-03-30 21:18:55.000000 wrangles-1.2.1/wrangles/recipe_wrangles/convert.py
+-rw-rw-rw-   0        0        0     8582 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/recipe_wrangles/create.py
+-rw-rw-rw-   0        0        0    20328 2023-04-14 19:14:11.000000 wrangles-1.2.1/wrangles/recipe_wrangles/extract.py
+-rw-rw-rw-   0        0        0     8055 2023-04-10 17:05:21.000000 wrangles-1.2.1/wrangles/recipe_wrangles/format.py
+-rw-rw-rw-   0        0        0    26422 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/recipe_wrangles/main.py
+-rw-rw-rw-   0        0        0     8570 2023-04-10 17:05:21.000000 wrangles-1.2.1/wrangles/recipe_wrangles/merge.py
+-rw-rw-rw-   0        0        0     7681 2023-04-10 17:05:21.000000 wrangles-1.2.1/wrangles/recipe_wrangles/select.py
+-rw-rw-rw-   0        0        0     6435 2023-04-10 17:05:21.000000 wrangles-1.2.1/wrangles/recipe_wrangles/split.py
+-rw-rw-rw-   0        0        0     1875 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/select.py
+-rw-rw-rw-   0        0        0     2099 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/standardize.py
+-rw-rw-rw-   0        0        0     6100 2022-12-21 19:41:28.000000 wrangles-1.2.1/wrangles/train.py
+-rw-rw-rw-   0        0        0     3502 2023-04-11 22:14:04.000000 wrangles-1.2.1/wrangles/translate.py
```

### Comparing `wrangles-1.2.0/PKG-INFO` & `wrangles-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrangles
-Version: 1.2.0
+Version: 1.2.1
 Summary: Wrangle your data into shape with machine learning
 Home-page: https://github.com/wrangleworks/WranglesPy
 Author: WrangleWorks
 Author-email: chris@wrangleworks.com
 License: Apache License 2.0
 Keywords: data,wrangling
 Platform: UNKNOWN
```

### Comparing `wrangles-1.2.0/README.md` & `wrangles-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/Wrangles.egg-info/PKG-INFO` & `wrangles-1.2.1/Wrangles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrangles
-Version: 1.2.0
+Version: 1.2.1
 Summary: Wrangle your data into shape with machine learning
 Home-page: https://github.com/wrangleworks/WranglesPy
 Author: WrangleWorks
 Author-email: chris@wrangleworks.com
 License: Apache License 2.0
 Keywords: data,wrangling
 Platform: UNKNOWN
```

### Comparing `wrangles-1.2.0/Wrangles.egg-info/SOURCES.txt` & `wrangles-1.2.1/Wrangles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/setup.py` & `wrangles-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     license_files = ('LICENSE.txt',),
     license = 'Apache License 2.0',
     classifiers = [
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent'
     ],
-    version = '1.2.0',
+    version = '1.2.1',
     url = 'https://github.com/wrangleworks/WranglesPy',
     author = 'WrangleWorks',
     author_email = 'chris@wrangleworks.com',
     keywords = ['data','wrangling'],
     install_requires = requirements,
     entry_points ={
         'console_scripts': ['wrangles.recipe = wrangles.console:recipe']
```

### Comparing `wrangles-1.2.0/wrangles/__init__.py` & `wrangles-1.2.1/wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/auth.py` & `wrangles-1.2.1/wrangles/auth.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/batching.py` & `wrangles-1.2.1/wrangles/batching.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/classify.py` & `wrangles-1.2.1/wrangles/classify.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/config.py` & `wrangles-1.2.1/wrangles/config.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/akeneo.py` & `wrangles-1.2.1/wrangles/connectors/akeneo.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/ckan.py` & `wrangles-1.2.1/wrangles/connectors/ckan.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/file.py` & `wrangles-1.2.1/wrangles/connectors/file.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/http.py` & `wrangles-1.2.1/wrangles/connectors/http.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/jinja.py` & `wrangles-1.2.1/wrangles/connectors/jinja.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/mongodb.py` & `wrangles-1.2.1/wrangles/connectors/mongodb.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/mssql.py` & `wrangles-1.2.1/wrangles/connectors/mssql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/mysql.py` & `wrangles-1.2.1/wrangles/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/notification.py` & `wrangles-1.2.1/wrangles/connectors/notification.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/postgres.py` & `wrangles-1.2.1/wrangles/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/pricefx.py` & `wrangles-1.2.1/wrangles/connectors/pricefx.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/recipe.py` & `wrangles-1.2.1/wrangles/connectors/recipe.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/s3.py` & `wrangles-1.2.1/wrangles/connectors/s3.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/salesforce.py` & `wrangles-1.2.1/wrangles/connectors/salesforce.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/sftp.py` & `wrangles-1.2.1/wrangles/connectors/sftp.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/ssh.py` & `wrangles-1.2.1/wrangles/connectors/ssh.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/test.py` & `wrangles-1.2.1/wrangles/connectors/test.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/connectors/train.py` & `wrangles-1.2.1/wrangles/connectors/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/console.py` & `wrangles-1.2.1/wrangles/console.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/data.py` & `wrangles-1.2.1/wrangles/data.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/extract.py` & `wrangles-1.2.1/wrangles/extract.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/format.py` & `wrangles-1.2.1/wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/recipe.py` & `wrangles-1.2.1/wrangles/recipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,24 +146,31 @@
     
     # Check if there are any templated valued to update
     recipe_object = _replace_templated_values(recipe_object=recipe_object, variables=variables)
 
     return recipe_object
 
 
-def _run_actions(recipe: _Union[dict, list], functions: dict = {}) -> None:
+def _run_actions(recipe: _Union[dict, list], functions: dict = {}, error: Exception = None) -> None:
     # If user has entered a dictionary, convert to list
     if isinstance(recipe, dict):
         recipe = [recipe]
 
     for action in recipe:
         for action_type, params in action.items():
             if action_type.split('.')[0] == 'custom':
+                # Get custom function
+                custom_function = functions[action_type[7:]]
+
+                # Check if error is one of the user's function arguments
+                if 'error' in _inspect.getfullargspec(custom_function).args:
+                    params['error'] = error
+
                 # Execute a user's custom function
-                functions[action_type[7:]](**params)
+                custom_function(**params)
             else:
                 # Get run function of requested connector and pass user defined params
                 obj = _connectors
                 for element in action_type.split('.'):
                     obj = getattr(obj, element)
 
                 if action_type == 'recipe':
@@ -463,12 +470,12 @@
 
         return df
 
     except Exception as e:
         try:
             # Run any actions requested if the recipe fails
             if 'on_failure' in recipe.get('run', {}).keys():
-                _run_actions(recipe['run']['on_failure'], functions)
+                _run_actions(recipe['run']['on_failure'], functions, e)
         except:
             pass
 
-        raise e
+        raise
```

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/__init__.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/__init__.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/convert.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/convert.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/create.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/create.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/extract.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         # Iterate through the inputs, outputs and model_ids
         for in_col, out_col, model in zip(input, output, model_id):
             df[out_col] = _extract.custom(df[in_col].astype(str).tolist(), model_id=model, first_element=first_element)
 
     # if use_labels is true and output is only one column
     if (use_labels and len(output) == 1):
         
-        # if first_element is checked, then the output must be converted to lists
+        # if first_element is checked, then the output must be converted to lists to iterate
         if first_element: df[output[0]] = [[x] for x in df[output[0]]]
         
         # Run the custom dictionary maker after normal operation from extract
         # This will be triggered only if a parameter is set
         result = []
         for out_row in df[output[0]]:
         
@@ -286,30 +286,44 @@
             # Iterating over the results
             for item in out_row:
                 
                 try:
                     item = item.strip()
                     # Check if the item contains a colon
                     if (item.count(':') == 1 and item.split(':')[0] != ''):
-                        dict_output[item.split(':')[0].strip()] = item.split(':')[1].strip()
+                        
+                        # get the key and value from item split
+                        key, value = map(str.strip, item.split(':', 1))
+                        
+                        if dict_output.get(key, ''):
+                            # if the keys is already present, then append to the list
+                            dict_output[key].append(value)
+
+                        else:
+                            dict_output[key] = [value]
+                            
                     else:
                         dict_output['Unlabeled'].append(item)
                 except:
                     dict_output['Unlabeled'].append(item)
-                    
+            
+            # putting Unlabeled at the end of the dictionary
             tmp_unlabeled = dict_output['Unlabeled']
             del dict_output['Unlabeled']
             output_dict = _OrderedDict(dict_output)
             output_dict['Unlabeled'] = tmp_unlabeled
             
             # check if the Unlabeled key is empty if yes, delete the key
-            if len(output_dict['Unlabeled']) == 0:
-                del output_dict['Unlabeled']
-                            
-            result.append(dict(output_dict))
+            if len(output_dict['Unlabeled']) == 0: del output_dict['Unlabeled']
+            
+            # if first element is set then get the first value as string in dictionary, else return the dictionary
+            if first_element: output_dict = {list(dict(output_dict).keys())[0]: list(dict(output_dict).values())[0][0]}
+            else: output_dict = dict(output_dict)
+            
+            result.append(output_dict)
             
         df[output[0]] = result
         
     return df
 
 
 def date_properties(df: _pd.DataFrame, input: _pd.Timestamp, property: str, output: _Union[str, list] = None) -> _pd.DataFrame:
```

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/format.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/format.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/main.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/main.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/merge.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/merge.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/select.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/select.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/recipe_wrangles/split.py` & `wrangles-1.2.1/wrangles/recipe_wrangles/split.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/select.py` & `wrangles-1.2.1/wrangles/select.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/standardize.py` & `wrangles-1.2.1/wrangles/standardize.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/train.py` & `wrangles-1.2.1/wrangles/train.py`

 * *Files identical despite different names*

### Comparing `wrangles-1.2.0/wrangles/translate.py` & `wrangles-1.2.1/wrangles/translate.py`

 * *Files identical despite different names*

