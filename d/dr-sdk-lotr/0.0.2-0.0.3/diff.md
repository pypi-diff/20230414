# Comparing `tmp/dr-sdk-lotr-0.0.2.tar.gz` & `tmp/dr-sdk-lotr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dr-sdk-lotr-0.0.2.tar", last modified: Fri Apr 14 13:39:49 2023, max compression
+gzip compressed data, was "dr-sdk-lotr-0.0.3.tar", last modified: Fri Apr 14 19:57:20 2023, max compression
```

## Comparing `dr-sdk-lotr-0.0.2.tar` & `dr-sdk-lotr-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:39:49.427645 dr-sdk-lotr-0.0.2/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1072 2023-04-14 12:36:30.000000 dr-sdk-lotr-0.0.2/LICENCE.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3199 2023-04-14 13:39:49.427491 dr-sdk-lotr-0.0.2/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2297 2023-04-14 13:34:32.000000 dr-sdk-lotr-0.0.2/README.md
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:39:49.424904 dr-sdk-lotr-0.0.2/dr_sdk_lotr/
--rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-14 12:39:34.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/__init__.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1560 2023-04-14 12:44:00.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/books.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1583 2023-04-14 12:44:19.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/chapters.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2127 2023-04-14 12:45:06.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/characters.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1678 2023-04-14 12:45:26.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/movies.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1077 2023-04-14 12:45:44.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/quotes.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)       40 2023-04-14 12:46:03.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/settings.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:39:49.425780 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3199 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)      522 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/SOURCES.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/dependency_links.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/requires.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       12 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/top_level.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-14 13:39:49.427689 dr-sdk-lotr-0.0.2/setup.cfg
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1157 2023-04-14 13:37:51.000000 dr-sdk-lotr-0.0.2/setup.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:39:49.427142 dr-sdk-lotr-0.0.2/tests/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1144 2023-04-14 13:36:41.000000 dr-sdk-lotr-0.0.2/tests/test_books.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1070 2023-04-14 13:36:50.000000 dr-sdk-lotr-0.0.2/tests/test_chapters.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1636 2023-04-14 13:36:57.000000 dr-sdk-lotr-0.0.2/tests/test_characters.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1086 2023-04-14 13:37:07.000000 dr-sdk-lotr-0.0.2/tests/test_movies_unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      925 2023-04-14 13:37:17.000000 dr-sdk-lotr-0.0.2/tests/test_quotes_unittest.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 19:57:20.562310 dr-sdk-lotr-0.0.3/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1072 2023-04-14 12:36:30.000000 dr-sdk-lotr-0.0.3/LICENCE.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3132 2023-04-14 19:57:20.562107 dr-sdk-lotr-0.0.3/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2297 2023-04-14 13:34:32.000000 dr-sdk-lotr-0.0.3/README.md
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 19:57:20.559234 dr-sdk-lotr-0.0.3/dr_sdk_lotr/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-14 12:39:34.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1573 2023-04-14 13:54:17.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr/books.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1588 2023-04-14 13:54:16.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr/chapters.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2127 2023-04-14 12:45:06.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr/characters.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1646 2023-04-14 13:54:14.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr/movies.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1077 2023-04-14 12:45:44.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr/quotes.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       40 2023-04-14 12:46:03.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr/settings.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 19:57:20.560129 dr-sdk-lotr-0.0.3/dr_sdk_lotr.egg-info/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3132 2023-04-14 19:57:20.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr.egg-info/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      522 2023-04-14 19:57:20.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr.egg-info/SOURCES.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-14 19:57:20.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr.egg-info/dependency_links.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-14 19:57:20.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr.egg-info/requires.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       12 2023-04-14 19:57:20.000000 dr-sdk-lotr-0.0.3/dr_sdk_lotr.egg-info/top_level.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-14 19:57:20.562359 dr-sdk-lotr-0.0.3/setup.cfg
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1090 2023-04-14 19:57:05.000000 dr-sdk-lotr-0.0.3/setup.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 19:57:20.561752 dr-sdk-lotr-0.0.3/tests/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1144 2023-04-14 13:36:41.000000 dr-sdk-lotr-0.0.3/tests/test_books.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1070 2023-04-14 13:36:50.000000 dr-sdk-lotr-0.0.3/tests/test_chapters.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1636 2023-04-14 13:36:57.000000 dr-sdk-lotr-0.0.3/tests/test_characters.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1086 2023-04-14 18:52:00.000000 dr-sdk-lotr-0.0.3/tests/test_movies_unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      925 2023-04-14 13:37:17.000000 dr-sdk-lotr-0.0.3/tests/test_quotes_unittest.py
```

### Comparing `dr-sdk-lotr-0.0.2/LICENCE.txt` & `dr-sdk-lotr-0.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/PKG-INFO` & `dr-sdk-lotr-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: dr-sdk-lotr
-Version: 0.0.2
+Version: 0.0.3
 Summary: SDK for interacting with the Lord of the Rings API
-Home-page: https://github.com/DannyBuffet/dr-lord-of-the-rings-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dr-sdk-lotr-0.0.2/README.md` & `dr-sdk-lotr-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/dr_sdk_lotr/books.py` & `dr-sdk-lotr-0.0.3/dr_sdk_lotr/books.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     def get_books(self):
         try:
             url = f"{self.base_url}"
             headers = {
                 'Accept': 'application/json',
                 'Authorization': f"Bearer {self.api_key}"
             }
+            
             books = requests.request("GET", url, headers=headers).json()
             return books
 
         except Exception as e:
             return e
 
     """
```

### Comparing `dr-sdk-lotr-0.0.2/dr_sdk_lotr/chapters.py` & `dr-sdk-lotr-0.0.3/dr_sdk_lotr/chapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
     def __init__(self, api_key: str):
         self.api_key = api_key
 
     """
     Lists of all book chapters
     """
+    
     def get_all_book_chapters(self):
         try:
             url = f"{self.base_url}"
             headers = {
                 'Accept': 'application/json',
                 'Authorization': f"Bearer {self.api_key}"
             }
```

### Comparing `dr-sdk-lotr-0.0.2/dr_sdk_lotr/characters.py` & `dr-sdk-lotr-0.0.3/dr_sdk_lotr/characters.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/dr_sdk_lotr/movies.py` & `dr-sdk-lotr-0.0.3/dr_sdk_lotr/movies.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,26 +8,26 @@
         self.api_key = api_key
 
     """
     List of all movies including "The Lord of the Rings" and the "The Hobbit" trilogies
     """
 
     def get_movies(self):
-            try:
-                url = f"{self.base_url}"
-                headers = {
-                    'Accept': 'application/json',
-                    'Authorization': f"Bearer {self.api_key}"
-                }
-
-                movies = requests.request("GET", url, headers=headers).json()['docs']
-                return movies
-
-            except Exception as e:
-                return e
+        try:
+            url = f"{self.base_url}"
+            headers = {
+                'Accept': 'application/json',
+                'Authorization': f"Bearer {self.api_key}"
+            }
+
+            movies = requests.request("GET", url, headers=headers).json()['docs']
+            return movies
+        
+        except Exception as e:
+            return e
 
     """
     Request one specific movie by id
     """
 
     def get_movie_by_id(self, id):
         try:
```

### Comparing `dr-sdk-lotr-0.0.2/dr_sdk_lotr/quotes.py` & `dr-sdk-lotr-0.0.3/dr_sdk_lotr/quotes.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/PKG-INFO` & `dr-sdk-lotr-0.0.3/dr_sdk_lotr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: dr-sdk-lotr
-Version: 0.0.2
+Version: 0.0.3
 Summary: SDK for interacting with the Lord of the Rings API
-Home-page: https://github.com/DannyBuffet/dr-lord-of-the-rings-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/SOURCES.txt` & `dr-sdk-lotr-0.0.3/dr_sdk_lotr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/setup.py` & `dr-sdk-lotr-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='dr-sdk-lotr',
-    version='0.0.2',
+    version='0.0.3',
     description='SDK for interacting with the Lord of the Rings API',
     author='Daniel Reliford',
     author_email='dreliford@gmail.com',
-    url='https://github.com/DannyBuffet/dr-lord-of-the-rings-sdk',
     packages=setuptools.find_packages(),
     install_requires=['requests'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `dr-sdk-lotr-0.0.2/tests/test_books.unittest.py` & `dr-sdk-lotr-0.0.3/tests/test_books.unittest.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/tests/test_chapters.unittest.py` & `dr-sdk-lotr-0.0.3/tests/test_chapters.unittest.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/tests/test_characters.unittest.py` & `dr-sdk-lotr-0.0.3/tests/test_characters.unittest.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/tests/test_movies_unittest.py` & `dr-sdk-lotr-0.0.3/tests/test_movies_unittest.py`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.2/tests/test_quotes_unittest.py` & `dr-sdk-lotr-0.0.3/tests/test_quotes_unittest.py`

 * *Files identical despite different names*

