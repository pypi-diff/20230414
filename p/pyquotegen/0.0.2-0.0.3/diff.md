# Comparing `tmp/pyquotegen-0.0.2.tar.gz` & `tmp/pyquotegen-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquotegen-0.0.2.tar", last modified: Sat Apr  1 06:31:47 2023, max compression
+gzip compressed data, was "pyquotegen-0.0.3.tar", last modified: Fri Apr 14 12:21:17 2023, max compression
```

## Comparing `pyquotegen-0.0.2.tar` & `pyquotegen-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-01 06:31:47.100352 pyquotegen-0.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1068 2023-04-01 05:29:52.000000 pyquotegen-0.0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)      890 2023-04-01 06:31:47.100352 pyquotegen-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)       53 2023-04-01 05:29:52.000000 pyquotegen-0.0.2/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-01 06:31:47.100352 pyquotegen-0.0.2/pyquotegen/
--rw-r--r--   0 runner    (1000) runner    (1000)      686 2023-04-01 06:25:39.000000 pyquotegen-0.0.2/pyquotegen/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19158 2023-04-01 05:29:52.000000 pyquotegen-0.0.2/pyquotegen/all_quotes.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-01 06:31:47.100352 pyquotegen-0.0.2/pyquotegen.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      890 2023-04-01 06:31:46.000000 pyquotegen-0.0.2/pyquotegen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      210 2023-04-01 06:31:46.000000 pyquotegen-0.0.2/pyquotegen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-01 06:31:46.000000 pyquotegen-0.0.2/pyquotegen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-01 06:31:46.000000 pyquotegen-0.0.2/pyquotegen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-01 06:31:47.100352 pyquotegen-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1041 2023-04-01 06:30:58.000000 pyquotegen-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-14 12:21:17.372241 pyquotegen-0.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1068 2023-04-01 05:29:52.000000 pyquotegen-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2709 2023-04-14 12:21:17.372241 pyquotegen-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1912 2023-04-14 12:20:39.000000 pyquotegen-0.0.3/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-14 12:21:17.368241 pyquotegen-0.0.3/pyquotegen/
+-rw-r--r--   0 runner    (1000) runner    (1000)      686 2023-04-01 06:25:39.000000 pyquotegen-0.0.3/pyquotegen/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19158 2023-04-01 05:29:52.000000 pyquotegen-0.0.3/pyquotegen/all_quotes.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-04-14 12:21:17.372241 pyquotegen-0.0.3/pyquotegen.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2709 2023-04-14 12:21:16.000000 pyquotegen-0.0.3/pyquotegen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      210 2023-04-14 12:21:16.000000 pyquotegen-0.0.3/pyquotegen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-04-14 12:21:16.000000 pyquotegen-0.0.3/pyquotegen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2023-04-14 12:21:16.000000 pyquotegen-0.0.3/pyquotegen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-04-14 12:21:17.372241 pyquotegen-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1192 2023-04-14 12:21:01.000000 pyquotegen-0.0.3/setup.py
```

### Comparing `pyquotegen-0.0.2/LICENSE` & `pyquotegen-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquotegen-0.0.2/pyquotegen/__init__.py` & `pyquotegen-0.0.3/pyquotegen/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquotegen-0.0.2/pyquotegen/all_quotes.py` & `pyquotegen-0.0.3/pyquotegen/all_quotes.py`

 * *Files identical despite different names*

### Comparing `pyquotegen-0.0.2/setup.py` & `pyquotegen-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 from setuptools import setup, find_packages
+from os import path
+
+# read the contents of the README file
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
 
 setup(
     name="pyquotegen",
-    version="0.0.2",
+    version="0.0.3",
     author="Arman Idrisi",
     author_email="idrisiarman19@gmail.com",
     description="A Random Quote Generator Python Package",
-    long_description="This Is A package which can ve used for generating the random quotes in diffrent categories for example: motivation, technology etc.",
-
+    long_description=long_description,
+long_description_content_type='text/markdown',
+  
 
     url="https://github.com/Armanidrisi/pyquotegen",
     project_urls={
         "Bug Tracker": "https://github.com/Armanidrisi/pyquotegen/issues",
         "Documentation": "https://github.com/Armanidrisi/pyquotegen/blob/main/README.md",
         "Source Code": "https://github.com/Armanidrisi/pyquotegen",
     },
```

