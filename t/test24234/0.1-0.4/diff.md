# Comparing `tmp/test24234-0.1.tar.gz` & `tmp/test24234-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test24234-0.1.tar", last modified: Fri Apr 14 10:10:25 2023, max compression
+gzip compressed data, was "test24234-0.4.tar", last modified: Fri Apr 14 10:14:29 2023, max compression
```

## Comparing `test24234-0.1.tar` & `test24234-0.4.tar`

### file list

```diff
@@ -1,3 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:10:25.676134 test24234-0.1/
--rw-rw-rw-   0        0        0      651 2023-04-14 10:10:25.676134 test24234-0.1/PKG-INFO
--rw-rw-rw-   0        0        0   204584 2023-04-14 10:09:13.637490 test24234-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:14:29.578209 test24234-0.4/
+-rw-rw-rw-   0        0        0      651 2023-04-14 10:14:29.578209 test24234-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0   204584 2023-04-14 10:14:23.861359 test24234-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:14:29.577212 test24234-0.4/test24234/
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:12:30.863148 test24234-0.4/test24234/__init__.py
```

### Comparing `test24234-0.1/PKG-INFO` & `test24234-0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: test24234
-Version: 0.1
+Version: 0.4
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/user/reponame
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Description: UNKNOWN
```

### Comparing `test24234-0.1/setup.py` & `test24234-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 from distutils.core import setup
 setup(
   name = 'test24234',         # How you named your package folder (MyLib)
   packages = ['test24234'],   # Chose the same as "name"
-  version = '0.1',      # Start with a small number and increase it with every change you make
+  version = '0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```

