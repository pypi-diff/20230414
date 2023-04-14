# Comparing `tmp/test23414234234-0.5.tar.gz` & `tmp/test23414234234-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test23414234234-0.5.tar", last modified: Fri Apr 14 10:38:43 2023, max compression
+gzip compressed data, was "test23414234234-0.6.tar", last modified: Fri Apr 14 10:40:27 2023, max compression
```

## Comparing `test23414234234-0.5.tar` & `test23414234234-0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:38:43.829902 test23414234234-0.5/
--rw-rw-rw-   0        0        0      487 2023-04-14 10:38:43.829902 test23414234234-0.5/PKG-INFO
--rw-rw-rw-   0        0        0   193906 2023-04-14 10:38:09.788868 test23414234234-0.5/build.pypi
-drwxrwxrwx   0        0        0        0 2023-04-14 10:38:43.829902 test23414234234-0.5/test23414234234/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:35:46.561337 test23414234234-0.5/test23414234234/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:40:27.974325 test23414234234-0.6/
+-rw-rw-rw-   0        0        0      487 2023-04-14 10:40:27.974325 test23414234234-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0   193906 2023-04-14 10:40:24.750030 test23414234234-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:40:27.974325 test23414234234-0.6/test23414234234/
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:35:46.561337 test23414234234-0.6/test23414234234/__init__.py
```

### Comparing `test23414234234-0.5/build.pypi` & `test23414234234-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'test23414234234',
   packages = ['test23414234234'],
-  version = '0.5',
+  version = '0.6',
   license='MIT',
   description = '',
   author = 'WS',
   keywords = [],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',
```

