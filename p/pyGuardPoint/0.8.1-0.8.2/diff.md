# Comparing `tmp/pyGuardPoint-0.8.1.tar.gz` & `tmp/pyGuardPoint-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.8.1.tar", last modified: Thu Apr 13 16:30:51 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.8.2.tar", last modified: Fri Apr 14 10:55:20 2023, max compression
```

## Comparing `pyGuardPoint-0.8.1.tar` & `pyGuardPoint-0.8.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 16:30:51.259477 pyGuardPoint-0.8.1/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2384 2023-04-13 16:30:51.258474 pyGuardPoint-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2123 2023-04-13 16:30:14.000000 pyGuardPoint-0.8.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 16:30:51.247476 pyGuardPoint-0.8.1/pyGuardPoint/
--rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.8.1/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.8.1/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.1/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.8.1/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 16:30:51.257471 pyGuardPoint-0.8.1/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     2384 2023-04-13 16:30:51.000000 pyGuardPoint-0.8.1/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-04-13 16:30:51.000000 pyGuardPoint-0.8.1/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 16:30:51.000000 pyGuardPoint-0.8.1/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.1/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-13 16:30:51.000000 pyGuardPoint-0.8.1/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-13 16:30:51.000000 pyGuardPoint-0.8.1/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 16:30:51.259477 pyGuardPoint-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-13 16:30:34.000000 pyGuardPoint-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:55:20.309746 pyGuardPoint-0.8.2/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     5233 2023-04-14 10:55:20.309746 pyGuardPoint-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4970 2023-04-14 10:55:03.000000 pyGuardPoint-0.8.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-14 10:55:20.286422 pyGuardPoint-0.8.2/pyGuardPoint/
+-rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.8.2/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.8.2/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.2/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.8.2/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:55:20.308746 pyGuardPoint-0.8.2/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     5233 2023-04-14 10:55:20.000000 pyGuardPoint-0.8.2/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-04-14 10:55:20.000000 pyGuardPoint-0.8.2/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:55:20.000000 pyGuardPoint-0.8.2/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.2/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-14 10:55:20.000000 pyGuardPoint-0.8.2/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 10:55:20.000000 pyGuardPoint-0.8.2/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:55:20.309746 pyGuardPoint-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-04-14 10:55:03.000000 pyGuardPoint-0.8.2/setup.py
```

### Comparing `pyGuardPoint-0.8.1/LICENSE.txt` & `pyGuardPoint-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.8.2/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.8.2/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.8.2/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.8.2/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.1/setup.py` & `pyGuardPoint-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.8.1",
+      version="0.8.2",
       author="John Owen",
       description="Easy-to-use Python module implementing GuardPoint's WebAPI",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein'],
       packages=['pyGuardPoint'],
```

