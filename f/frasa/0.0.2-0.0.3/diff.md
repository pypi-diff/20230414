# Comparing `tmp/frasa-0.0.2.tar.gz` & `tmp/frasa-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frasa-0.0.2.tar", last modified: Fri Apr 14 20:40:09 2023, max compression
+gzip compressed data, was "frasa-0.0.3.tar", last modified: Fri Apr 14 20:44:21 2023, max compression
```

## Comparing `frasa-0.0.2.tar` & `frasa-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 20:40:09.465725 frasa-0.0.2/
--rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.0.2/LICENSE
--rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 20:40:09.465535 frasa-0.0.2/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     1700 2023-04-12 08:34:25.000000 frasa-0.0.2/README.md
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 20:40:09.464093 frasa-0.0.2/frasa/
--rw-r--r--   0 novay      (501) staff       (20)      605 2023-04-14 20:22:13.000000 frasa-0.0.2/frasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 20:40:09.465093 frasa-0.0.2/frasa.egg-info/
--rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 20:40:09.000000 frasa-0.0.2/frasa.egg-info/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)      188 2023-04-14 20:40:09.000000 frasa-0.0.2/frasa.egg-info/SOURCES.txt
--rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-14 20:40:09.000000 frasa-0.0.2/frasa.egg-info/dependency_links.txt
--rw-r--r--   0 novay      (501) staff       (20)        9 2023-04-14 20:40:09.000000 frasa-0.0.2/frasa.egg-info/requires.txt
--rw-r--r--   0 novay      (501) staff       (20)        6 2023-04-14 20:40:09.000000 frasa-0.0.2/frasa.egg-info/top_level.txt
--rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-14 20:40:09.465790 frasa-0.0.2/setup.cfg
--rw-r--r--   0 novay      (501) staff       (20)     1072 2023-04-14 20:22:04.000000 frasa-0.0.2/setup.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 20:44:21.276977 frasa-0.0.3/
+-rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.0.3/LICENSE
+-rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 20:44:21.276836 frasa-0.0.3/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     1700 2023-04-12 08:34:25.000000 frasa-0.0.3/README.md
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 20:44:21.275941 frasa-0.0.3/frasa/
+-rw-r--r--   0 novay      (501) staff       (20)      599 2023-04-14 20:44:11.000000 frasa-0.0.3/frasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-04-14 20:44:21.276611 frasa-0.0.3/frasa.egg-info/
+-rw-r--r--   0 novay      (501) staff       (20)     2426 2023-04-14 20:44:21.000000 frasa-0.0.3/frasa.egg-info/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)      188 2023-04-14 20:44:21.000000 frasa-0.0.3/frasa.egg-info/SOURCES.txt
+-rw-r--r--   0 novay      (501) staff       (20)        1 2023-04-14 20:44:21.000000 frasa-0.0.3/frasa.egg-info/dependency_links.txt
+-rw-r--r--   0 novay      (501) staff       (20)        9 2023-04-14 20:44:21.000000 frasa-0.0.3/frasa.egg-info/requires.txt
+-rw-r--r--   0 novay      (501) staff       (20)        6 2023-04-14 20:44:21.000000 frasa-0.0.3/frasa.egg-info/top_level.txt
+-rw-r--r--   0 novay      (501) staff       (20)       38 2023-04-14 20:44:21.277023 frasa-0.0.3/setup.cfg
+-rw-r--r--   0 novay      (501) staff       (20)     1072 2023-04-14 20:44:16.000000 frasa-0.0.3/setup.py
```

### Comparing `frasa-0.0.2/LICENSE` & `frasa-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `frasa-0.0.2/PKG-INFO` & `frasa-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/python/tree/main/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.0.2/README.md` & `frasa-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `frasa-0.0.2/frasa/__init__.py` & `frasa-0.0.3/frasa/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 Kunjungi http://frasa.id untuk informasi selengkapnya.
 """
 
 import os
 
 __name__ = "frasa"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __license__ = 'MIT'
 __author__ = 'Novianto Rahmadi'
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 
-from frasa.sensor import *
 from frasa.deteksi import *
+# from frasa.sensor import *
 
-from frasa import sensor, deteksi
+from frasa import deteksi
```

### Comparing `frasa-0.0.2/frasa.egg-info/PKG-INFO` & `frasa-0.0.3/frasa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.0.2
+Version: 0.0.3
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/python/tree/main/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.0.2/setup.py` & `frasa-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="frasa",
-    version="0.0.2",
+    version="0.0.3",
     description="Koleksi NLP Pribadi untuk Bahasa Indonesia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novay/python/tree/main/frasa",
     author="Novianto Rahmadi",
     author_email="novay@btekno.id",
     license="MIT",
```

