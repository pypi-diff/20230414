# Comparing `tmp/cbstorage-0.1.5.tar.gz` & `tmp/cbstorage-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbstorage-0.1.5.tar", max compression
+gzip compressed data, was "cbstorage-0.1.6.tar", max compression
```

## Comparing `cbstorage-0.1.5.tar` & `cbstorage-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       22 2023-04-14 13:09:33.104854 cbstorage-0.1.5/cbstorage/__init__.py
--rw-r--r--   0        0        0     7499 2023-04-14 16:56:03.669299 cbstorage-0.1.5/cbstorage/storage.py
--rw-r--r--   0        0        0      649 2023-04-14 16:56:09.426934 cbstorage-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      901 2023-04-14 16:56:11.934224 cbstorage-0.1.5/setup.py
--rw-r--r--   0        0        0      748 2023-04-14 16:56:11.934348 cbstorage-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-04-14 13:09:33.104854 cbstorage-0.1.6/cbstorage/__init__.py
+-rw-r--r--   0        0        0     7502 2023-04-14 17:14:59.570367 cbstorage-0.1.6/cbstorage/storage.py
+-rw-r--r--   0        0        0      649 2023-04-14 17:15:05.344370 cbstorage-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      901 2023-04-14 17:15:07.507126 cbstorage-0.1.6/setup.py
+-rw-r--r--   0        0        0      748 2023-04-14 17:15:07.507267 cbstorage-0.1.6/PKG-INFO
```

### Comparing `cbstorage-0.1.5/cbstorage/storage.py` & `cbstorage-0.1.6/cbstorage/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
 class Local(Storage):
     """
         A class for managing local file cbstorage.
     """
 
     def __init__(self):
-        self.basedir = '/data/notebooks/Lev2/backupS3/'
+        self.basedir = '/vk/data/notebooks/Lev2/backupS3/'
 
     def searching_all_files(self, directory):
         """
             Return a sorted list of full paths to all files in the given directory and its subdirectories.
         """
         dirpath = pathlib.Path(directory)
         assert dirpath.is_dir()
```

### Comparing `cbstorage-0.1.5/pyproject.toml` & `cbstorage-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbstorage"
-version = "0.1.5"
+version = "0.1.6"
 description = "The code is a Python package for managing file storage on either AWS S3 or a local machine. It provides methods for listing, searching, and storing files. The package includes two classes, Aws and Local, which implement the same set of methods for accessing and manipulating files in S3 and a local directory."
 authors = ["germangerken <germangerken@yandex.ru>", "lybchansckii"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 boto3 = "^1.26.113"
```

### Comparing `cbstorage-0.1.5/setup.py` & `cbstorage-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.26.113,<2.0.0']
 
 setup_kwargs = {
     'name': 'cbstorage',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'The code is a Python package for managing file storage on either AWS S3 or a local machine. It provides methods for listing, searching, and storing files. The package includes two classes, Aws and Local, which implement the same set of methods for accessing and manipulating files in S3 and a local directory.',
     'long_description': None,
     'author': 'germangerken',
     'author_email': 'germangerken@yandex.ru',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `cbstorage-0.1.5/PKG-INFO` & `cbstorage-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbstorage
-Version: 0.1.5
+Version: 0.1.6
 Summary: The code is a Python package for managing file storage on either AWS S3 or a local machine. It provides methods for listing, searching, and storing files. The package includes two classes, Aws and Local, which implement the same set of methods for accessing and manipulating files in S3 and a local directory.
 Author: germangerken
 Author-email: germangerken@yandex.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

