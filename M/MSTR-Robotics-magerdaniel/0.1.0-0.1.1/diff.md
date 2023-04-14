# Comparing `tmp/MSTR_Robotics_magerdaniel-0.1.0.tar.gz` & `tmp/MSTR_Robotics_magerdaniel-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MSTR_Robotics_magerdaniel-0.1.0.tar", last modified: Thu Feb  9 04:56:49 2023, max compression
+gzip compressed data, was "MSTR_Robotics_magerdaniel-0.1.1.tar", last modified: Fri Apr 14 12:39:35 2023, max compression
```

## Comparing `MSTR_Robotics_magerdaniel-0.1.0.tar` & `MSTR_Robotics_magerdaniel-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:56:49.455771 MSTR_Robotics_magerdaniel-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:56:49.451771 MSTR_Robotics_magerdaniel-0.1.0/MSTR_Robotics_magerdaniel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-09 04:56:49.000000 MSTR_Robotics_magerdaniel-0.1.0/MSTR_Robotics_magerdaniel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-09 04:56:49.000000 MSTR_Robotics_magerdaniel-0.1.0/MSTR_Robotics_magerdaniel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 04:56:49.000000 MSTR_Robotics_magerdaniel-0.1.0/MSTR_Robotics_magerdaniel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-09 04:56:49.000000 MSTR_Robotics_magerdaniel-0.1.0/MSTR_Robotics_magerdaniel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-02-09 04:56:49.455771 MSTR_Robotics_magerdaniel-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 04:56:49.455771 MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/lu_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/mstr_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16698 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/select_mig_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 04:56:49.455771 MSTR_Robotics_magerdaniel-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-09 04:56:38.000000 MSTR_Robotics_magerdaniel-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:39:35.740868 MSTR_Robotics_magerdaniel-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:39:35.736868 MSTR_Robotics_magerdaniel-0.1.1/MSTR_Robotics_magerdaniel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 12:39:35.000000 MSTR_Robotics_magerdaniel-0.1.1/MSTR_Robotics_magerdaniel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-14 12:39:35.000000 MSTR_Robotics_magerdaniel-0.1.1/MSTR_Robotics_magerdaniel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:39:35.000000 MSTR_Robotics_magerdaniel-0.1.1/MSTR_Robotics_magerdaniel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 12:39:35.000000 MSTR_Robotics_magerdaniel-0.1.1/MSTR_Robotics_magerdaniel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-14 12:39:35.740868 MSTR_Robotics_magerdaniel-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:39:35.740868 MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/lu_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/mstr_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16698 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/select_mig_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:39:35.740868 MSTR_Robotics_magerdaniel-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 12:39:23.000000 MSTR_Robotics_magerdaniel-0.1.1/setup.py
```

### Comparing `MSTR_Robotics_magerdaniel-0.1.0/MSTR_Robotics_magerdaniel.egg-info/PKG-INFO` & `MSTR_Robotics_magerdaniel-0.1.1/MSTR_Robotics_magerdaniel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MSTR-Robotics-magerdaniel
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroStrateg(P)ython
 Home-page: https://github.com/magerdaniel
 Author: Daniel Mager
 Author-email: "danielmager@gmx.de"
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MSTR_Robotics_magerdaniel-0.1.0/PKG-INFO` & `MSTR_Robotics_magerdaniel-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MSTR_Robotics_magerdaniel
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroStrateg(P)ython
 Home-page: https://github.com/magerdaniel
 Author: Daniel Mager
 Author-email: "danielmager@gmx.de"
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/helper.py` & `MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/helper.py`

 * *Files identical despite different names*

### Comparing `MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/logger.py` & `MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/logger.py`

 * *Files identical despite different names*

### Comparing `MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/lu_data.py` & `MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/lu_data.py`

 * *Files identical despite different names*

### Comparing `MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/mstr_classes.py` & `MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/mstr_classes.py`

 * *Files identical despite different names*

### Comparing `MSTR_Robotics_magerdaniel-0.1.0/mstr_robotics/select_mig_objects.py` & `MSTR_Robotics_magerdaniel-0.1.1/mstr_robotics/select_mig_objects.py`

 * *Files identical despite different names*

### Comparing `MSTR_Robotics_magerdaniel-0.1.0/setup.py` & `MSTR_Robotics_magerdaniel-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from distutils.core import setup
 #from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(name='MSTR_Robotics_magerdaniel',
-      version= "0.1.0",
+      version= "0.1.1",
       description="MicroStrateg(P)ython",
       author="Daniel Mager",
       author_email='"danielmager@gmx.de"',
       url="https://github.com/magerdaniel",
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=['mstr_robotics'],
```

