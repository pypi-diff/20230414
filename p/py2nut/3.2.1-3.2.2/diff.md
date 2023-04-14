# Comparing `tmp/py2nut-3.2.1.tar.gz` & `tmp/py2nut-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2nut-3.2.1.tar", last modified: Wed Mar 22 10:31:37 2023, max compression
+gzip compressed data, was "py2nut-3.2.2.tar", last modified: Fri Apr 14 05:36:28 2023, max compression
```

## Comparing `py2nut-3.2.1.tar` & `py2nut-3.2.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.482339 py2nut-3.2.1/
--rw-rw-rw-   0        0        0    35803 2022-07-21 09:01:30.000000 py2nut-3.2.1/LICENSE
--rw-rw-rw-   0        0        0       22 2022-12-05 05:43:45.000000 py2nut-3.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    21795 2023-03-22 10:31:37.480227 py2nut-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    21290 2022-12-05 05:43:25.000000 py2nut-3.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.356572 py2nut-3.2.1/py2Nut/
--rw-rw-rw-   0        0        0       23 2023-03-22 07:43:39.000000 py2nut-3.2.1/py2Nut/__init__.py
--rw-rw-rw-   0        0        0        3 2022-12-05 07:43:05.000000 py2nut-3.2.1/py2Nut/_lib.py
--rw-rw-rw-   0        0        0       42 2022-12-05 07:42:35.000000 py2nut-3.2.1/py2Nut/nutApi.py
--rw-rw-rw-   0        0        0       52 2022-12-05 05:21:51.000000 py2nut-3.2.1/py2Nut/nutDataframe.py
--rw-rw-rw-   0        0        0       45 2022-12-05 07:42:04.000000 py2nut-3.2.1/py2Nut/nutDate.py
--rw-rw-rw-   0        0        0       37 2022-12-05 09:05:13.000000 py2nut-3.2.1/py2Nut/nutDb.py
--rw-rw-rw-   0        0        0       46 2022-12-05 09:05:55.000000 py2nut-3.2.1/py2Nut/nutEmail.py
--rw-rw-rw-   0        0        0       48 2022-12-05 09:04:21.000000 py2nut-3.2.1/py2Nut/nutFiles.py
--rw-rw-rw-   0        0        0       40 2022-12-05 09:20:39.000000 py2nut-3.2.1/py2Nut/nutFtp.py
--rw-rw-rw-   0        0        0       48 2022-12-05 07:42:53.000000 py2nut-3.2.1/py2Nut/nutOther.py
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.360093 py2nut-3.2.1/py2Nut/xlrd/
--rw-rw-rw-   0        0        0    34373 2022-07-21 09:01:30.000000 py2nut-3.2.1/py2Nut/xlrd/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.378482 py2nut-3.2.1/py2nut.egg-info/
--rw-rw-rw-   0        0        0    21795 2023-03-22 10:31:37.000000 py2nut-3.2.1/py2nut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1164 2023-03-22 10:31:37.000000 py2nut-3.2.1/py2nut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 10:31:37.000000 py2nut-3.2.1/py2nut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-22 10:31:37.000000 py2nut-3.2.1/py2nut.egg-info/requires.txt
--rw-rw-rw-   0        0        0       78 2023-03-22 10:31:37.000000 py2nut-3.2.1/py2nut.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.382472 py2nut-3.2.1/pynut_1tools/
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.401420 py2nut-3.2.1/pynut_1tools/pyNutTools/
--rw-rw-rw-   0        0        0       25 2023-03-07 04:16:50.000000 py2nut-3.2.1/pynut_1tools/pyNutTools/__init__.py
--rw-rw-rw-   0        0        0     2054 2022-12-07 03:56:44.000000 py2nut-3.2.1/pynut_1tools/pyNutTools/_lib.py
--rw-rw-rw-   0        0        0    31616 2023-03-07 04:16:53.000000 py2nut-3.2.1/pynut_1tools/pyNutTools/nutDataframe.py
--rw-rw-rw-   0        0        0    18046 2022-12-07 03:57:19.000000 py2nut-3.2.1/pynut_1tools/pyNutTools/nutDate.py
--rw-rw-rw-   0        0        0     8711 2023-03-07 04:16:53.000000 py2nut-3.2.1/pynut_1tools/pyNutTools/nutOther.py
--rw-rw-rw-   0        0        0     1029 2023-03-07 04:16:55.000000 py2nut-3.2.1/pynut_1tools/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.404412 py2nut-3.2.1/pynut_2api/
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.415383 py2nut-3.2.1/pynut_2api/pyNutApi/
--rw-rw-rw-   0        0        0       23 2023-03-07 04:16:57.000000 py2nut-3.2.1/pynut_2api/pyNutApi/__init__.py
--rw-rw-rw-   0        0        0     3274 2022-12-05 13:28:05.000000 py2nut-3.2.1/pynut_2api/pyNutApi/_lib.py
--rw-rw-rw-   0        0        0    24252 2023-02-21 05:55:17.000000 py2nut-3.2.1/pynut_2api/pyNutApi/nutApi.py
--rw-rw-rw-   0        0        0     1079 2023-03-01 09:03:57.000000 py2nut-3.2.1/pynut_2api/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.419431 py2nut-3.2.1/pynut_2files/
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.430361 py2nut-3.2.1/pynut_2files/pyNutFiles/
--rw-rw-rw-   0        0        0       23 2023-03-22 07:43:59.000000 py2nut-3.2.1/pynut_2files/pyNutFiles/__init__.py
--rw-rw-rw-   0        0        0     6710 2022-12-07 04:06:54.000000 py2nut-3.2.1/pynut_2files/pyNutFiles/_lib.py
--rw-rw-rw-   0        0        0   128051 2023-03-22 10:22:54.000000 py2nut-3.2.1/pynut_2files/pyNutFiles/nutFiles.py
--rw-rw-rw-   0        0        0     1170 2023-03-07 04:17:04.000000 py2nut-3.2.1/pynut_2files/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.436345 py2nut-3.2.1/pynut_3db/
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.447343 py2nut-3.2.1/pynut_3db/pyNutDB/
--rw-rw-rw-   0        0        0       23 2023-03-07 04:17:04.000000 py2nut-3.2.1/pynut_3db/pyNutDB/__init__.py
--rw-rw-rw-   0        0        0     2591 2022-12-05 13:21:28.000000 py2nut-3.2.1/pynut_3db/pyNutDB/_lib.py
--rw-rw-rw-   0        0        0    21550 2023-03-07 04:17:05.000000 py2nut-3.2.1/pynut_3db/pyNutDB/nutDb.py
--rw-rw-rw-   0        0        0     1051 2023-03-07 04:17:05.000000 py2nut-3.2.1/pynut_3db/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.451305 py2nut-3.2.1/pynut_3email/
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.461278 py2nut-3.2.1/pynut_3email/pyNutEmail/
--rw-rw-rw-   0        0        0       21 2023-03-07 04:17:06.000000 py2nut-3.2.1/pynut_3email/pyNutEmail/__init__.py
--rw-rw-rw-   0        0        0     4303 2022-12-05 13:20:03.000000 py2nut-3.2.1/pynut_3email/pyNutEmail/_lib.py
--rw-rw-rw-   0        0        0    35893 2023-01-04 05:22:20.000000 py2nut-3.2.1/pynut_3email/pyNutEmail/nutEmail.py
--rw-rw-rw-   0        0        0     1064 2023-03-07 04:17:07.000000 py2nut-3.2.1/pynut_3email/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.465268 py2nut-3.2.1/pynut_3ftp/
-drwxrwxrwx   0        0        0        0 2023-03-22 10:31:37.474948 py2nut-3.2.1/pynut_3ftp/pyNutFtp/
--rw-rw-rw-   0        0        0       23 2023-03-07 04:17:07.000000 py2nut-3.2.1/pynut_3ftp/pyNutFtp/__init__.py
--rw-rw-rw-   0        0        0     3476 2023-01-04 05:34:31.000000 py2nut-3.2.1/pynut_3ftp/pyNutFtp/_lib.py
--rw-rw-rw-   0        0        0    29570 2023-01-04 05:57:55.000000 py2nut-3.2.1/pynut_3ftp/pyNutFtp/nutFtp.py
--rw-rw-rw-   0        0        0     1072 2023-03-07 04:17:08.000000 py2nut-3.2.1/pynut_3ftp/setup.py
--rw-rw-rw-   0        0        0       42 2023-03-22 10:31:37.483220 py2nut-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1565 2023-02-08 10:26:55.000000 py2nut-3.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.970569 py2nut-3.2.2/
+-rw-rw-rw-   0        0        0    35803 2022-07-21 09:01:30.000000 py2nut-3.2.2/LICENSE
+-rw-rw-rw-   0        0        0       22 2022-12-05 05:43:45.000000 py2nut-3.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    21795 2023-04-14 05:36:28.969574 py2nut-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    21290 2022-12-05 05:43:25.000000 py2nut-3.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.827928 py2nut-3.2.2/py2Nut/
+-rw-rw-rw-   0        0        0       23 2023-03-30 09:09:08.000000 py2nut-3.2.2/py2Nut/__init__.py
+-rw-rw-rw-   0        0        0        3 2022-12-05 07:43:05.000000 py2nut-3.2.2/py2Nut/_lib.py
+-rw-rw-rw-   0        0        0       42 2022-12-05 07:42:35.000000 py2nut-3.2.2/py2Nut/nutApi.py
+-rw-rw-rw-   0        0        0       52 2022-12-05 05:21:51.000000 py2nut-3.2.2/py2Nut/nutDataframe.py
+-rw-rw-rw-   0        0        0       45 2022-12-05 07:42:04.000000 py2nut-3.2.2/py2Nut/nutDate.py
+-rw-rw-rw-   0        0        0       37 2022-12-05 09:05:13.000000 py2nut-3.2.2/py2Nut/nutDb.py
+-rw-rw-rw-   0        0        0       46 2022-12-05 09:05:55.000000 py2nut-3.2.2/py2Nut/nutEmail.py
+-rw-rw-rw-   0        0        0       48 2022-12-05 09:04:21.000000 py2nut-3.2.2/py2Nut/nutFiles.py
+-rw-rw-rw-   0        0        0       40 2022-12-05 09:20:39.000000 py2nut-3.2.2/py2Nut/nutFtp.py
+-rw-rw-rw-   0        0        0       48 2022-12-05 07:42:53.000000 py2nut-3.2.2/py2Nut/nutOther.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.831060 py2nut-3.2.2/py2Nut/xlrd/
+-rw-rw-rw-   0        0        0    34373 2022-07-21 09:01:30.000000 py2nut-3.2.2/py2Nut/xlrd/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.852879 py2nut-3.2.2/py2nut.egg-info/
+-rw-rw-rw-   0        0        0    21795 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1164 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       78 2023-04-14 05:36:28.000000 py2nut-3.2.2/py2nut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.856851 py2nut-3.2.2/pynut_1tools/
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.881936 py2nut-3.2.2/pynut_1tools/pyNutTools/
+-rw-rw-rw-   0        0        0       25 2023-04-04 08:29:08.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/__init__.py
+-rw-rw-rw-   0        0        0     2054 2022-12-07 03:56:44.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/_lib.py
+-rw-rw-rw-   0        0        0    32349 2023-04-04 08:31:33.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/nutDataframe.py
+-rw-rw-rw-   0        0        0    18046 2022-12-07 03:57:19.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/nutDate.py
+-rw-rw-rw-   0        0        0     8711 2023-03-07 04:16:53.000000 py2nut-3.2.2/pynut_1tools/pyNutTools/nutOther.py
+-rw-rw-rw-   0        0        0     1029 2023-03-07 04:16:55.000000 py2nut-3.2.2/pynut_1tools/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.885775 py2nut-3.2.2/pynut_2api/
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.896767 py2nut-3.2.2/pynut_2api/pyNutApi/
+-rw-rw-rw-   0        0        0       23 2023-03-07 04:16:57.000000 py2nut-3.2.2/pynut_2api/pyNutApi/__init__.py
+-rw-rw-rw-   0        0        0     3607 2023-04-14 05:30:35.000000 py2nut-3.2.2/pynut_2api/pyNutApi/_lib.py
+-rw-rw-rw-   0        0        0    28921 2023-04-14 05:32:54.000000 py2nut-3.2.2/pynut_2api/pyNutApi/nutApi.py
+-rw-rw-rw-   0        0        0     1079 2023-04-14 05:27:51.000000 py2nut-3.2.2/pynut_2api/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.901114 py2nut-3.2.2/pynut_2files/
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.913720 py2nut-3.2.2/pynut_2files/pyNutFiles/
+-rw-rw-rw-   0        0        0       23 2023-03-30 09:07:33.000000 py2nut-3.2.2/pynut_2files/pyNutFiles/__init__.py
+-rw-rw-rw-   0        0        0     6710 2022-12-07 04:06:54.000000 py2nut-3.2.2/pynut_2files/pyNutFiles/_lib.py
+-rw-rw-rw-   0        0        0   128574 2023-04-14 05:25:41.000000 py2nut-3.2.2/pynut_2files/pyNutFiles/nutFiles.py
+-rw-rw-rw-   0        0        0     1170 2023-04-14 05:28:03.000000 py2nut-3.2.2/pynut_2files/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.920208 py2nut-3.2.2/pynut_3db/
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.931917 py2nut-3.2.2/pynut_3db/pyNutDB/
+-rw-rw-rw-   0        0        0       23 2023-03-07 04:17:04.000000 py2nut-3.2.2/pynut_3db/pyNutDB/__init__.py
+-rw-rw-rw-   0        0        0     2591 2022-12-05 13:21:28.000000 py2nut-3.2.2/pynut_3db/pyNutDB/_lib.py
+-rw-rw-rw-   0        0        0    21550 2023-03-07 04:17:05.000000 py2nut-3.2.2/pynut_3db/pyNutDB/nutDb.py
+-rw-rw-rw-   0        0        0     1051 2023-04-14 05:28:19.000000 py2nut-3.2.2/pynut_3db/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.936317 py2nut-3.2.2/pynut_3email/
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.947539 py2nut-3.2.2/pynut_3email/pyNutEmail/
+-rw-rw-rw-   0        0        0       21 2023-04-14 05:29:30.000000 py2nut-3.2.2/pynut_3email/pyNutEmail/__init__.py
+-rw-rw-rw-   0        0        0     4303 2022-12-05 13:20:03.000000 py2nut-3.2.2/pynut_3email/pyNutEmail/_lib.py
+-rw-rw-rw-   0        0        0    35893 2023-01-04 05:22:20.000000 py2nut-3.2.2/pynut_3email/pyNutEmail/nutEmail.py
+-rw-rw-rw-   0        0        0     1064 2023-04-14 05:28:29.000000 py2nut-3.2.2/pynut_3email/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.951619 py2nut-3.2.2/pynut_3ftp/
+drwxrwxrwx   0        0        0        0 2023-04-14 05:36:28.964039 py2nut-3.2.2/pynut_3ftp/pyNutFtp/
+-rw-rw-rw-   0        0        0       23 2023-04-14 05:29:30.000000 py2nut-3.2.2/pynut_3ftp/pyNutFtp/__init__.py
+-rw-rw-rw-   0        0        0     3476 2023-01-04 05:34:31.000000 py2nut-3.2.2/pynut_3ftp/pyNutFtp/_lib.py
+-rw-rw-rw-   0        0        0    29570 2023-01-04 05:57:55.000000 py2nut-3.2.2/pynut_3ftp/pyNutFtp/nutFtp.py
+-rw-rw-rw-   0        0        0     1072 2023-04-14 05:28:37.000000 py2nut-3.2.2/pynut_3ftp/setup.py
+-rw-rw-rw-   0        0        0       42 2023-04-14 05:36:28.971630 py2nut-3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1565 2023-02-08 10:26:55.000000 py2nut-3.2.2/setup.py
```

### Comparing `py2nut-3.2.1/LICENSE` & `py2nut-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/PKG-INFO` & `py2nut-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2nut
-Version: 3.2.1
+Version: 3.2.2
 Summary: This Library allows you to make Misc operations in various domain
 Home-page: https://github.com/Laurent-Tupin/py2nut
 Author: Laurent Tupin
 Author-email: laurent.tupinn@gmail.com
 License: Copyright 2022-2035
 Platform: UNKNOWN
 Classifier: License :: Free For Home Use
```

### Comparing `py2nut-3.2.1/README.md` & `py2nut-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/py2Nut/xlrd/xlsx.py` & `py2nut-3.2.2/py2Nut/xlrd/xlsx.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/py2nut.egg-info/PKG-INFO` & `py2nut-3.2.2/py2nut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2nut
-Version: 3.2.1
+Version: 3.2.2
 Summary: This Library allows you to make Misc operations in various domain
 Home-page: https://github.com/Laurent-Tupin/py2nut
 Author: Laurent Tupin
 Author-email: laurent.tupinn@gmail.com
 License: Copyright 2022-2035
 Platform: UNKNOWN
 Classifier: License :: Free For Home Use
```

### Comparing `py2nut-3.2.1/py2nut.egg-info/SOURCES.txt` & `py2nut-3.2.2/py2nut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_1tools/pyNutTools/_lib.py` & `py2nut-3.2.2/pynut_1tools/pyNutTools/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_1tools/pyNutTools/nutDataframe.py` & `py2nut-3.2.2/pynut_1tools/pyNutTools/nutDataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -627,14 +627,18 @@
 
 
 
 
 #-------------------------------------------
 # GROUP BY
 #-------------------------------------------
+def fDf_resetIndex(df):
+    df.reset_index(inplace=True)
+    return df
+
 def fDf_putBackColPivot_afGroupBy(df, str_colPivot):
     df[str_colPivot] = df.index                 # Put again the Column Pivot that disapear into index
     df.reset_index(drop = True, inplace = True) # reset_index
     df = df[[df.columns[-1]] + list(df.columns[:-1])]   # Put the col Pivot on first Position
     return df
 
 def fDf_GroupBy(df_in, str_colPivot, str_colMeasure, d_aggPerCol = {}):
@@ -649,14 +653,30 @@
         df = df_group.agg(d_aggPerCol)          
     except Exception as err:
         logger.error('  error in fDf_GroupBy: |{}| '.format(err))
         df = df_group[str_colMeasure].sum()
     df = fDf_putBackColPivot_afGroupBy(df, str_colPivot)
     return df
 
+def fDf_GroupBy_sevColumns(df_in, l_colPivot, str_colMeasure, d_aggPerCol={}):
+    df = fDf_CleanPrepareDF(df_in, l_colToBeFloat = [str_colMeasure], l_colToDropNA = l_colPivot, o_fillNA_by = 0)
+    # Sum is by default
+    if d_aggPerCol == {}:
+        d_aggPerCol = {str_colMeasure: 'sum'}
+    # Group and have the colPivot as Index
+    df_group = df.groupby(l_colPivot)
+    # Aggregate the measures
+    try:
+        df = df_group.agg(d_aggPerCol)
+    except Exception as err:
+        logger.error('  error in fDf_GroupBy_sevColumns: |{}| '.format(err))
+        df = df_group[str_colMeasure].sum()
+    df = fDf_resetIndex(df)
+    return df
+
 def fDf_GroupBy_multiply(df_in, str_colPivot, l_colMeasure = []):
     df = fDf_CleanPrepareDF(df_in, l_colToBeFloat = l_colMeasure, l_colToDropNA = [str_colPivot], o_fillNA_by = 1)
     # Group and have the colPivot as Index
     df_group = df.groupby(str_colPivot)
     # Aggregate the measures
     try:
         df = df_group.prod()
```

### Comparing `py2nut-3.2.1/pynut_1tools/pyNutTools/nutDate.py` & `py2nut-3.2.2/pynut_1tools/pyNutTools/nutDate.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_1tools/pyNutTools/nutOther.py` & `py2nut-3.2.2/pynut_1tools/pyNutTools/nutOther.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_1tools/setup.py` & `py2nut-3.2.2/pynut_1tools/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_2api/pyNutApi/_lib.py` & `py2nut-3.2.2/pynut_2api/pyNutApi/_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,25 @@
         try:
             from pyNutTools import nutOther
         except Exception as err:
             print('  Import FAIL PyNutApi |nutOther|, err:|{}|'.format(err))
             return None
     return nutOther
 
+def nutDataframe():
+    try:
+        from pynut_1tools.pyNutTools import nutDataframe
+    except:
+        try:
+            from pyNutTools import nutDataframe
+        except Exception as err:
+            print('  Import FAIL PyNutApi |nutDataframe|, err:|{}|'.format(err))
+            return None
+    return nutDataframe
+
 
 #-----------------------------------------------------------------
 # Generic Lib
 #-----------------------------------------------------------------
 def logging():
     try:    import logging
     except Exception as err:
```

### Comparing `py2nut-3.2.1/pynut_2api/pyNutApi/nutApi.py` & `py2nut-3.2.2/pynut_2api/pyNutApi/nutApi.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,23 +9,25 @@
         except:
             import _lib as lib
 
 import time, sys
 
 logger =    lib.logger()
 oth =       lib.nutOther()
+dframe =    lib.nutDataframe()
 pd =        lib.pandas()
 re =        lib.re()
 requests =  lib.requests()
 BeautifulSoup =     lib.BeautifulSoup()
 unicodedata =       lib.unicodedata()
 selenium =  lib.selenium()
 selenium_webdriver = lib.selenium_webdriver()
 
 
+
 # ---------------------------------------------------------------
 # ------------- Quick Function ----------------------------------
 # ---------------------------------------------------------------
 def fDf_convertJson(j_resp, l_otherKeys=[]):
     j_array = j_resp.copy()
     for _keyword in l_otherKeys:
         j_array = j_array[_keyword]
@@ -325,93 +327,191 @@
             logger.error('  Connexion close for the status code of the page is not 200')
             logger.error('  - Status code of the page is: |{}|'.format(o_page.status_code))
     except:
         logger.error('  ERROR in fBL_checkConnexion: Connexion fails because the input is not a page')
     return False
 
 
-# ==============================================================================
+#==============================================================================
 # BEAUTIFUL SOUP
-# ==============================================================================
-def fDf_htmlGetArray_Soup(str_url, bl_th=False, bl_waitForTranslation=False, int_waitTime=0,
-                          bl_cleanXA0=True, int_waitTimeLimit=5, bl_verify=True):
+#==============================================================================
+def fArr_webScrapTableTr(bs_soup, bl_th = False, bl_cleanXA0 = True):
+    l_doublon = []
+    arr_result = []
+    for o_table in bs_soup.find_all('table'):
+        for o_row in o_table.find_all('tr'):
+            # Remove doublons
+            if o_row in l_doublon:
+                break
+            l_doublon.append(o_row)
+            # Balise Th = Text / Titre
+            o_th = [o_cell.text.strip() for o_cell in o_row.find_all('th')]
+            if bl_th and o_th:      o_cells = o_th
+            else:                   o_cells = []
+            # Balise TD = Chiffre
+            o_td = [o_cell.text.strip() for o_cell in o_row.find_all('td')]
+            if o_td:                o_cells = o_cells + o_td
+            elif o_th:              o_cells = o_th
+            else:                   o_cells = []
+            # Clean Cells
+            if bl_cleanXA0:
+                o_cells = [unicodedata.normalize("NFKD",cel_Text) for cel_Text in o_cells]
+                o_cells = [cel_Text.replace('\n', '  ').replace('\r', '') for cel_Text in o_cells]
+            # add the row to result
+            if o_cells:   arr_result.append(o_cells)
+    return arr_result
+
+def fArr_webScrapUlLi(bs_soup, bl_title = False, bl_cleanXA0 = True):
+    l_doublon = []
     arr_result = []
+    for o_table in bs_soup.find_all('ul'):
+        for o_row in o_table.find_all('li'):
+            # Remove doublons
+            if o_row in l_doublon:
+                break
+            l_doublon.append(o_row)
+            # Balise XXXX = Text / Titre
+            if bl_title is True:
+                o_title = [o_cell.text.strip() for o_cell in o_row.find_all('XXXXX')]
+                if o_title:     o_cells = o_title
+                else:           o_cells = []
+            else:
+                o_title = []
+                o_cells = []
+            # Balise p
+            o_p = [o_cell.text.strip() for o_cell in o_row.find_all('p')]
+            if o_p:             o_cells = o_cells + o_p
+            elif o_title:       o_cells = o_title
+            else:               o_cells = []
+            # add the row to result
+            if o_cells:
+                # Clean Cells
+                if bl_cleanXA0 is True:
+                    o_cells = [unicodedata.normalize("NFKD",cel_Text) for cel_Text in o_cells]
+                    o_cells = [cel_Text.replace('\n', '  ').replace('\r', '') for cel_Text in o_cells]
+                arr_result.append(o_cells)
+    return arr_result
+
+
+def fDf_bSoup_GetArray(str_url, bl_th = False, bl_waitForTranslation = False, int_waitTime = 0,
+                       bl_cleanXA0 = True, int_waitTimeLimit = 5, bl_verify = True):
     try:
         d_headers = {'User-Agent': 'Chrome/71.0.3578.98'}
-        o_page = requests.get(str_url, headers=d_headers, verify=bl_verify)
+        o_page = requests.get(str_url, headers = d_headers, verify = bl_verify)
         if bl_waitForTranslation and int_waitTime != 0:     Act_WaitTranslation(int_waitTime)
     except Exception as err:
-        logger.error(' ERROR in fDf_htmlGetArray_Soup: requests.get(str_url) : |{}|'.format(err))
+        logger.error(' ERROR in fDf_bSoup_GetArray: requests.get(str_url) : |{}|'.format(err))
+        logger.error('  - URL : |{}|'.format( str_url ))
+        raise
+    if not fBL_checkConnexion(o_page):
+        logger.error(' ERROR in fDf_bSoup_GetArray: fBL_checkConnexion(o_page): ')
+        logger.error('  - URL : |{}|'.format(str_url))
+        return False
+    try:
+        bs_soup = BeautifulSoup(o_page.content, "html.parser")      # lxml   # html5lib
+    except Exception as err:
+        logger.error(' ERROR in fDf_bSoup_GetArray: BeautifulSoup(o_page.content, "html.parser") : |{}|'.format(err))
+        logger.error('  - URL : |{}|'.format( str_url ))
+        raise
+    try:
+        arr_result_tr = fArr_webScrapTableTr(bs_soup, bl_th = bl_th, bl_cleanXA0 = bl_cleanXA0)
+        arr_result_li = fArr_webScrapUlLi(bs_soup, bl_cleanXA0 = bl_cleanXA0)
+    except Exception as err:
+        logger.error('  ERROR in fDf_bSoup_GetArray: LOOP on tables / rows / cells: |{}|'.format(err))
         logger.error('  - URL : |{}|'.format(str_url))
         raise
+    # END
+    try:
+        df1 =   pd.DataFrame(arr_result_tr)
+        df2 =   pd.DataFrame(arr_result_li)
+        df =    dframe.fDf_Concat_wColOfDf1(df1, df2)
+    except Exception as err:
+        logger.error('  ERROR in fDf_bSoup_GetArray: Pandas Dataframe: |{}|'.format(err))
+        logger.error('  - URL : |{}|'.format(str_url))
+        raise
+    return df
+
+
+def fDf_htmlGetArray_Soup(str_url, bl_th = False, bl_waitForTranslation = False, int_waitTime = 0,
+                          bl_cleanXA0 = True, int_waitTimeLimit = 5, bl_verify = True):
+    try:
+        d_headers = {'User-Agent': 'Chrome/71.0.3578.98'}
+        o_page = requests.get(str_url, headers = d_headers, verify = bl_verify)
+        if bl_waitForTranslation and int_waitTime != 0:     Act_WaitTranslation(int_waitTime)
+    except Exception as err:
+        logger.error(' ERROR in fDf_htmlGetArray_Soup: requests.get(str_url) : |{}|'.format(err))
+        logger.error('  - URL : |{}|'.format( str_url ))
+        raise
     if not fBL_checkConnexion(o_page):
         logger.error(' ERROR in fDf_htmlGetArray_Soup: fBL_checkConnexion(o_page): ')
         logger.error('  - URL : |{}|'.format(str_url))
         return False
     try:
-        bs_soup = BeautifulSoup(o_page.content, "html.parser")  # lxml   # html5lib
+        bs_soup = BeautifulSoup(o_page.content, "html.parser")      # lxml   # html5lib
         # bs_soup = bs_soup.replace(u'\xa0', ' ')
         # bs_soup.prettify(formatter = lambda x: x.replace(u'\xa0', ' '))
         # bs_soup.prettify(formatter = lambda x: x.replace(r'&nbsp;', ' '))
     except Exception as err:
         logger.error(' ERROR in fDf_htmlGetArray_Soup: BeautifulSoup(o_page.content, "html.parser") : |{}|'.format(err))
-        logger.error('  - URL : |{}|'.format(str_url))
+        logger.error('  - URL : |{}|'.format( str_url ))
         raise
     try:
+        arr_result = []
         l_doublon = []
         for o_table in bs_soup.find_all('table'):
             for o_row in o_table.find_all('tr'):
                 # Remove doublons
                 if o_row in l_doublon:
                     break
                 l_doublon.append(o_row)
                 # Balise Th = Text / Titre
                 o_th = [o_cell.text.strip() for o_cell in o_row.find_all('th')]
-                if bl_th and o_th:
-                    o_cells = o_th
-                else:
-                    o_cells = []
+                if bl_th and o_th:      o_cells = o_th
+                else:                   o_cells = []
                 # Balise TD = Chiffre
                 o_td = [o_cell.text.strip() for o_cell in o_row.find_all('td')]
-                if o_td:
-                    o_cells = o_cells + o_td
-                elif o_th:
-                    o_cells = o_th
-                else:
-                    o_cells = []
+                if o_td:                o_cells = o_cells + o_td
+                elif o_th:              o_cells = o_th
+                else:                   o_cells = []
                 # Clean Cells
                 if bl_cleanXA0:
-                    o_cells = [unicodedata.normalize("NFKD", cel_Text) for cel_Text in o_cells]
+                    o_cells = [unicodedata.normalize("NFKD",cel_Text) for cel_Text in o_cells]
                     o_cells = [cel_Text.replace('\n', '  ').replace('\r', '') for cel_Text in o_cells]
                 # add the row to result
                 if o_cells:   arr_result.append(o_cells)
                 # Chinese Translation - Recursive
                 if bl_waitForTranslation:
                     for cell in o_cells:
                         if fBl_ChineseInString(cell):
                             if int_waitTime > int_waitTimeLimit:
                                 logger.warning('   *_* ERROR : still Chinese within Result: ')
                                 logger.warning(cell)
                                 logger.warning('   *_!!!_* Cannot wait anymore, Do it manually: ')
-                                logger.warning('   - URL : |{}|'.format(str_url))
+                                logger.warning('   - URL : |{}|'.format(str_url) )
                                 break
                             else:
-                                int_waitTime = (int_waitTime + 1) * 2
+                                int_waitTime = (int_waitTime + 1)*2
                             logger.warning('   *_* ERROR : still Chinese within Result: ')
                             logger.warning(cell)
                             df_return = fDf_htmlGetArray_Soup(str_url, bl_th, True, int_waitTime)
                             return df_return
-        df = pd.DataFrame(arr_result)
     except Exception as err:
         logger.error('  ERROR in fDf_htmlGetArray_Soup: LOOP on tables / rows / cells: |{}|'.format(err))
         logger.error('  - URL : |{}|'.format(str_url))
         raise
+    # END
+    try:    df = pd.DataFrame(arr_result)
+    except Exception as err:
+        logger.error('  ERROR in fDf_htmlGetArray_Soup: Pandas Dataframe: |{}|'.format(err))
+        logger.error('  - URL : |{}|'.format(str_url))
+        raise
     return df
 
 
+
 # ==============================================================================
 # SELENIUM
 # ==============================================================================
 class c_Selenium_InteractInternet:
     # ----------------------------------------------------
     # To use Chrome Driver
     #  Go to chromedriver.chromium.org || https://sites.google.com/a/chromium.org/chromedriver/downloads
```

### Comparing `py2nut-3.2.1/pynut_2api/setup.py` & `py2nut-3.2.2/pynut_2api/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     classifiers=[
         "License :: Free For Home Use",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     packages = find_packages(exclude = ("test",)),
     include_package_data = True,
-    install_requires = ["pynut-tools==3.1.3", "beautifulsoup4==4.11.2", "selenium==4.8.0"]
+    install_requires = ["pynut-tools==3.1.2", "beautifulsoup4==4.11.2", "selenium==4.8.0"]
     #entry_points={"console_scripts": ["EXEnameFile=FolderName.__main__:main"]},
 )
```

### Comparing `py2nut-3.2.1/pynut_2files/pyNutFiles/_lib.py` & `py2nut-3.2.2/pynut_2files/pyNutFiles/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_2files/pyNutFiles/nutFiles.py` & `py2nut-3.2.2/pynut_2files/pyNutFiles/nutFiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,17 +329,34 @@
     return ll_content
 
 
 # ------------------------------------------------------------------------------
 # Open Files
 # ------------------------------------------------------------------------------
 def fBk_OpenWk_xlrd(str_path):
-    o_Book = xlrd.open_workbook(str_path)
+    try:
+        o_Book = xlrd.open_workbook(str_path)
+    except Exception as err:
+        logger.error(f' ERROR in fBk_OpenWk_xlrd (fl): |{err}| ')
+        raise
     return o_Book
 
+def fL_getSheetName_xls(str_path):
+    try:
+        l_sheetName = pd.ExcelFile(str_path).sheet_names
+        # # LEGACY VERSION
+        # l_wkSheet = pd.read_excel(str_pathModel, None).keys()
+        # # OR
+        # o_Book = fBk_OpenWk_xlrd(str_path)
+        # l_sheetName = o_Book.sheet_names()
+    except Exception as err:
+        logger.error(f' ERROR in fL_getSheetName_xls (fl): |{err}| ')
+        raise
+    return l_sheetName
+
 
 # ------------------------------------------------------------------------------
 # Transform Names
 # ------------------------------------------------------------------------------
 def Act_Rename(str_folder, str_OriginalName, str_NewName, bl_message=True):
     """ Renaming a file and if it failed using the lib os, it will MOVE the file with shutil """
     try:
@@ -1080,96 +1097,89 @@
             xlWb.close()
         except:
             logger.error('  *** Could not close the file')
         return False
     return str_path
 
 
+
 # INSERT SHEET: 1 file out - 1 Dataframe - 1 Sheet
 def fStr_fillExcel_InsertNewSheet(str_folder, str_FileName, df_data, str_SheetName='', bl_header=False):
     """ Take an existing  Excel file and insert a new sheet
     Input is a list of Dataframe - Will use pd.ExcelWriter
     """
-    if str_FileName == '':
-        str_path = str_folder
-    else:
-        str_path = os.path.join(str_folder, str_FileName)
+    if str_FileName == '':      str_path = str_folder
+    else:                       str_path = os.path.join(str_folder, str_FileName)
 
     if sys.version_info.major == 3:
         if sys.version_info.minor >= 10:
             # Python 3.11 - Pandas 1.5
             str_path = fStr_fillExcel_InsertNewSheet_Py311Pand15(str_path, df_data, str_SheetName, bl_header)
         else:
             # Python 3.9 - Pandas 1.1
             str_path = fStr_fillExcel_InsertNewSheet_Py39Pand11(str_path, df_data, str_SheetName, bl_header)
     else:
         logger.warning('WARNING: do you use a Python 3 ???')
         str_path = fStr_fillExcel_InsertNewSheet_Py39Pand11(str_path, df_data, str_SheetName, bl_header)
     return str_path
 
-
-def fStr_fillExcel_InsertNewSheet_Py311Pand15(str_path, df_data, str_SheetName='', bl_header=False):
+def fStr_fillExcel_InsertNewSheet_Py311Pand15(str_path, df_data, str_SheetName = '', bl_header = False):
     try:
         # With
-        with pd.ExcelWriter(str_path, engine='openpyxl') as xl_writer:
+        with pd.ExcelWriter(str_path, mode = 'a', engine = 'openpyxl', if_sheet_exists = 'replace') as xl_writer:
             # ---------------------------------------------------------------
             # Manage Sheet Name
             if str_SheetName == '':     str_SheetName = 'Sh1'
             # Rename a sheet because we dont want to replace
             if str_SheetName in list(xl_writer.sheets):
                 logger.warning(" The sheet '{}' already exist".format(str_SheetName))
                 while str_SheetName in list(xl_writer.sheets):
                     str_SheetName = str_SheetName[1:] + str_SheetName[0] + 'x'
-                logger.warning(
-                    " We replace the sheet name: '{}'  but you need to improve the management of name".format(
-                        str_SheetName))
+                logger.warning(" We replace the sheet name: '{}'  but you need to improve the management of name".format(str_SheetName))
             # ---------------------------------------------------------------
             # Add the Sheet
-            df_data.to_excel(xl_writer, header=bl_header, index=False, sheet_name=str_SheetName)
+            df_data.to_excel(xl_writer, header = bl_header, index = False, sheet_name = str_SheetName)
     except Exception as err:
-        logger.error(
-            '  ERROR in fl.fStr_fillExcel_InsertNewSheet_Py311Pand15: Could not fill the file: |{}|'.format(err))
+        logger.error('  ERROR in fl.fStr_fillExcel_InsertNewSheet_Py311Pand15: Could not fill the file: |{}|'.format(err))
         logger.error('  - Path : |{}|'.format(str_path))
         logger.error('  - SheetName : |{}|'.format(str_SheetName))
         return False
     return str_path
 
-
-def fStr_fillExcel_InsertNewSheet_Py39Pand11(str_path, df_data, str_SheetName='', bl_header=False):
+def fStr_fillExcel_InsertNewSheet_Py39Pand11(str_path, df_data, str_SheetName = '', bl_header = False):
     try:
         # Define Book
         xl_book = openpyxl.load_workbook(filename=str_path)
         # With
-        with pd.ExcelWriter(str_path, mode='a', engine='openpyxl', if_sheet_exists='replace') as xl_writer:
+        with pd.ExcelWriter(str_path, mode = 'a', engine = 'openpyxl', if_sheet_exists = 'replace') as xl_writer:
             xl_writer.book = xl_book
             xl_writer.sheets = dict((ws.title, ws) for ws in xl_book.worksheets)
             # ---------------------------------------------------------------
             # ManAge Sheet Name
             if str_SheetName == '':     str_SheetName = 'Sh1'
             if str_SheetName in list(xl_writer.sheets):
                 logger.warning(" The sheet '{}' already exist".format(str_SheetName))
                 while str_SheetName in list(xl_writer.sheets):
                     str_SheetName = str_SheetName[1:] + str_SheetName[0] + 'x'
-                logger.warning(
-                    " We replace the sheet name: '{}'  but you need to improve the management of name".format(
-                        str_SheetName))
+                logger.warning(" We replace the sheet name: '{}'  but you need to improve the management of name".format(str_SheetName))
             # ---------------------------------------------------------------
             # Add the Sheet
             df_data.to_excel(xl_writer, header=bl_header, index=False, sheet_name=str_SheetName)
             # SAVE
             xl_writer.save()
     except Exception as err:
-        logger.error(
-            '  ERROR in fl.fStr_fillExcel_InsertNewSheet_Py39Pand11: Could not fill the file: |{}|'.format(err))
+        logger.error('  ERROR in fl.fStr_fillExcel_InsertNewSheet_Py39Pand11: Could not fill the file: |{}|'.format(err))
         logger.error('  - Path : |{}|'.format(str_path))
         logger.error('  - SheetName : |{}|'.format(str_SheetName))
         return False
     return str_path
 
 
+
+
 # 1 file out - 1 Dataframe - 1 Sheet
 def fStr_fillXls_celByCel(str_path, df_data, str_SheetName='', xlWs=0, int_nbRows=0, int_rowsWhere=1):
     """ Take an existing Excel file and an existing sheet and fill it with new data
     Input is a list of Dataframe - Will use c_win32_xlApp class"""
     try:
         # If Sheet is nothing, we must define it
         if xlWs == 0:
```

### Comparing `py2nut-3.2.1/pynut_2files/setup.py` & `py2nut-3.2.2/pynut_2files/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,12 +20,12 @@
     classifiers=[
         "License :: Free For Home Use",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     packages = find_packages(exclude = ("test",)),
     include_package_data = True,
-    install_requires = ["pynut-tools==3.1.3", "openpyxl==3.1.0", "psutil==5.9.4",
+    install_requires = ["pynut-tools==3.1.2", "openpyxl==3.1.0", "psutil==5.9.4",
                         "pywin32==305", "xlrd==2.0.1", "XlsxWriter==1.4.5",
                         "xlwings==0.29.1"]
     #entry_points={"console_scripts": ["EXEnameFile=FolderName.__main__:main"]},
 )
```

### Comparing `py2nut-3.2.1/pynut_3db/pyNutDB/_lib.py` & `py2nut-3.2.2/pynut_3db/pyNutDB/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_3db/pyNutDB/nutDb.py` & `py2nut-3.2.2/pynut_3db/pyNutDB/nutDb.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_3db/setup.py` & `py2nut-3.2.2/pynut_3db/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     classifiers=[
         "License :: Free For Home Use",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     packages = find_packages(exclude = ("test",)),
     include_package_data = True,
-    install_requires = ["pynut-Files==3.1.2", "pyodbc==4.0.35"]
+    install_requires = ["pynut-Files==3.2.2", "pyodbc==4.0.35"]
     #entry_points={"console_scripts": ["EXEnameFile=FolderName.__main__:main"]},
 )
```

### Comparing `py2nut-3.2.1/pynut_3email/pyNutEmail/_lib.py` & `py2nut-3.2.2/pynut_3email/pyNutEmail/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_3email/pyNutEmail/nutEmail.py` & `py2nut-3.2.2/pynut_3email/pyNutEmail/nutEmail.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_3email/setup.py` & `py2nut-3.2.2/pynut_3email/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     classifiers=[
         "License :: Free For Home Use",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     packages = find_packages(exclude = ("test",)),
     include_package_data = True,
-    install_requires = ["pynut-Files==3.1.2", "exchangelib==4.9.0"]
+    install_requires = ["pynut-Files==3.2.2", "exchangelib==4.9.0"]
     #entry_points={"console_scripts": ["EXEnameFile=FolderName.__main__:main"]},
 )
```

### Comparing `py2nut-3.2.1/pynut_3ftp/pyNutFtp/_lib.py` & `py2nut-3.2.2/pynut_3ftp/pyNutFtp/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_3ftp/pyNutFtp/nutFtp.py` & `py2nut-3.2.2/pynut_3ftp/pyNutFtp/nutFtp.py`

 * *Files identical despite different names*

### Comparing `py2nut-3.2.1/pynut_3ftp/setup.py` & `py2nut-3.2.2/pynut_3ftp/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,10 +22,10 @@
     classifiers=[
         "License :: Free For Home Use",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
     ],
     packages = find_packages(exclude = ("test",)),
     include_package_data = True,
-    install_requires = ["pynut-Files==3.1.2", "paramiko==3.0.0", "pysftp==0.2.9"]
+    install_requires = ["pynut-Files==3.2.2", "paramiko==3.0.0", "pysftp==0.2.9"]
     #entry_points={"console_scripts": ["EXEnameFile=FolderName.__main__:main"]},
 )
```

### Comparing `py2nut-3.2.1/setup.py` & `py2nut-3.2.2/setup.py`

 * *Files identical despite different names*

