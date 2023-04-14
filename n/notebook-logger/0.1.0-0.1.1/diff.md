# Comparing `tmp/notebook-logger-0.1.0.tar.gz` & `tmp/notebook-logger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\notebook-logger-0.1.0.tar", last modified: Wed Apr 12 21:09:44 2023, max compression
+gzip compressed data, was "dist\notebook-logger-0.1.1.tar", last modified: Fri Apr 14 18:40:11 2023, max compression
```

## Comparing `notebook-logger-0.1.0.tar` & `notebook-logger-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/
--rw-rw-rw-   0        0        0    11558 2023-04-12 20:57:02.000000 notebook-logger-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      514 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-04-12 21:02:46.000000 notebook-logger-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/notebook_logger/
--rw-rw-rw-   0        0        0       34 2023-04-12 21:08:00.000000 notebook-logger-0.1.0/notebook_logger/__init__.py
--rw-rw-rw-   0        0        0      504 2023-04-12 21:07:31.000000 notebook-logger-0.1.0/notebook_logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/notebook_logger.egg-info/
--rw-rw-rw-   0        0        0      514 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/notebook_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/notebook_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/notebook_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/notebook_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-12 21:09:44.000000 notebook-logger-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      571 2023-04-12 21:02:06.000000 notebook-logger-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-12 20:57:02.000000 notebook-logger-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-04-14 18:37:38.000000 notebook-logger-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/notebook_logger/
+-rw-rw-rw-   0        0        0       34 2023-04-12 21:08:00.000000 notebook-logger-0.1.1/notebook_logger/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-04-14 18:35:51.000000 notebook-logger-0.1.1/notebook_logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/notebook_logger.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/notebook_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/notebook_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/notebook_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/notebook_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-14 18:40:11.000000 notebook-logger-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      571 2023-04-14 18:37:55.000000 notebook-logger-0.1.1/setup.py
```

### Comparing `notebook-logger-0.1.0/LICENSE` & `notebook-logger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebook-logger-0.1.0/setup.py` & `notebook-logger-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='notebook-logger',
-    version='0.1.0',
+    version='0.1.1',
     license='Apache-2.0',
     author='Daniel Lee',
     author_email='rootuser.kr@gmail.com',
     description='Simple logger for jupyter notebook user',
     long_description=open('README.md').read(),
     url='https://github.com/asulikeit/notebook-logger',
     packages=['notebook_logger'],
```

