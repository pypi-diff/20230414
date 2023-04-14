# Comparing `tmp/pyGuardPoint-0.8.4.tar.gz` & `tmp/pyGuardPoint-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.8.4.tar", last modified: Fri Apr 14 13:53:52 2023, max compression
+gzip compressed data, was "pyGuardPoint-0.8.5.tar", last modified: Fri Apr 14 14:00:54 2023, max compression
```

## Comparing `pyGuardPoint-0.8.4.tar` & `pyGuardPoint-0.8.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:53:52.280956 pyGuardPoint-0.8.4/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.4/LICENSE.txt
--rw-rw-rw-   0        0        0     5643 2023-04-14 13:53:52.280014 pyGuardPoint-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     5380 2023-04-14 13:51:48.000000 pyGuardPoint-0.8.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-14 13:53:52.271955 pyGuardPoint-0.8.4/pyGuardPoint/
--rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.8.4/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.8.4/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.4/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.8.4/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 13:53:52.278958 pyGuardPoint-0.8.4/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     5643 2023-04-14 13:53:52.000000 pyGuardPoint-0.8.4/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-04-14 13:53:52.000000 pyGuardPoint-0.8.4/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:53:52.000000 pyGuardPoint-0.8.4/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.4/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-14 13:53:52.000000 pyGuardPoint-0.8.4/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-14 13:53:52.000000 pyGuardPoint-0.8.4/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 13:53:52.280956 pyGuardPoint-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0      553 2023-04-14 13:53:31.000000 pyGuardPoint-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:00:54.819346 pyGuardPoint-0.8.5/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.8.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     5743 2023-04-14 14:00:54.819346 pyGuardPoint-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5480 2023-04-14 14:00:11.000000 pyGuardPoint-0.8.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-14 14:00:54.810320 pyGuardPoint-0.8.5/pyGuardPoint/
+-rw-rw-rw-   0        0        0      250 2023-03-30 08:56:57.000000 pyGuardPoint-0.8.5/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    11213 2023-04-13 12:36:08.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1175 2023-03-16 16:56:01.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5306 2023-04-13 10:30:08.000000 pyGuardPoint-0.8.5/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.8.5/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2393 2023-04-03 15:05:33.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0     5799 2023-04-05 10:41:13.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    16977 2023-04-06 11:06:08.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3012 2023-04-13 12:30:22.000000 pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:00:54.818328 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     5743 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-14 14:00:54.000000 pyGuardPoint-0.8.5/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:00:54.820320 pyGuardPoint-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0      553 2023-04-14 14:00:27.000000 pyGuardPoint-0.8.5/setup.py
```

### Comparing `pyGuardPoint-0.8.4/LICENSE.txt` & `pyGuardPoint-0.8.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/PKG-INFO` & `pyGuardPoint-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.8.4
+Version: 0.8.5
 Summary: Easy-to-use Python module implementing GuardPoint's WebAPI
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
@@ -25,16 +25,19 @@
 Rapid development of applications and scripts using the GuardPoint ACS.
 pyGuardPoint manages your authenticated connection to GuardPoint 10, so there is know need to construct complex OData URLs.
 The Python object Cardholder represents a user/person on the system.
 Modify your Cardholder's attributes and update them with just a couple of lines of code.
 
 Examples
 ------------------
+Firstly you will always need to import the module:
 
-For example, to retrieve a list of cardholders:
+    from pyGuardPoint import GuardPoint, Cardholder, Card
+
+To retrieve a list of cardholders:
 
     gp = GuardPoint(host="10.0.0.1", pwd="password")
     cardholders = gp.get_card_holders(search_terms="Jeff Buckley")
     for cardholder in cardholders:
         print(cardholder.lastName)
 
 To create a new cardholder:
```

### Comparing `pyGuardPoint-0.8.4/README.rst` & `pyGuardPoint-0.8.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 Rapid development of applications and scripts using the GuardPoint ACS.
 pyGuardPoint manages your authenticated connection to GuardPoint 10, so there is know need to construct complex OData URLs.
 The Python object Cardholder represents a user/person on the system.
 Modify your Cardholder's attributes and update them with just a couple of lines of code.
 
 Examples
 ------------------
+Firstly you will always need to import the module:
 
-For example, to retrieve a list of cardholders:
+    from pyGuardPoint import GuardPoint, Cardholder, Card
+
+To retrieve a list of cardholders:
 
     gp = GuardPoint(host="10.0.0.1", pwd="password")
     cardholders = gp.get_card_holders(search_terms="Jeff Buckley")
     for cardholder in cardholders:
         print(cardholder.lastName)
 
 To create a new cardholder:
```

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_areas.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_cards.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-0.8.5/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/guardpoint.py` & `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-0.8.5/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-0.8.5/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.8.4
+Version: 0.8.5
 Summary: Easy-to-use Python module implementing GuardPoint's WebAPI
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
@@ -25,16 +25,19 @@
 Rapid development of applications and scripts using the GuardPoint ACS.
 pyGuardPoint manages your authenticated connection to GuardPoint 10, so there is know need to construct complex OData URLs.
 The Python object Cardholder represents a user/person on the system.
 Modify your Cardholder's attributes and update them with just a couple of lines of code.
 
 Examples
 ------------------
+Firstly you will always need to import the module:
 
-For example, to retrieve a list of cardholders:
+    from pyGuardPoint import GuardPoint, Cardholder, Card
+
+To retrieve a list of cardholders:
 
     gp = GuardPoint(host="10.0.0.1", pwd="password")
     cardholders = gp.get_card_holders(search_terms="Jeff Buckley")
     for cardholder in cardholders:
         print(cardholder.lastName)
 
 To create a new cardholder:
```

### Comparing `pyGuardPoint-0.8.4/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-0.8.5/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.8.4/setup.py` & `pyGuardPoint-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.8.4",
+      version="0.8.5",
       author="John Owen",
       description="Easy-to-use Python module implementing GuardPoint's WebAPI",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein'],
       packages=['pyGuardPoint'],
```

