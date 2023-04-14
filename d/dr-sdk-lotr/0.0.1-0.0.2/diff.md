# Comparing `tmp/dr-sdk-lotr-0.0.1.tar.gz` & `tmp/dr-sdk-lotr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dr-sdk-lotr-0.0.1.tar", last modified: Fri Apr 14 13:08:35 2023, max compression
+gzip compressed data, was "dr-sdk-lotr-0.0.2.tar", last modified: Fri Apr 14 13:39:49 2023, max compression
```

## Comparing `dr-sdk-lotr-0.0.1.tar` & `dr-sdk-lotr-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:08:35.300920 dr-sdk-lotr-0.0.1/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1072 2023-04-14 12:36:30.000000 dr-sdk-lotr-0.0.1/LICENCE.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3153 2023-04-14 13:08:35.300751 dr-sdk-lotr-0.0.1/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)     2251 2023-04-14 13:04:39.000000 dr-sdk-lotr-0.0.1/README.md
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:08:35.298793 dr-sdk-lotr-0.0.1/dr_sdk_lotr.egg-info/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     3153 2023-04-14 13:08:35.000000 dr-sdk-lotr-0.0.1/dr_sdk_lotr.egg-info/PKG-INFO
--rw-r--r--   0 dannyreliford   (501) staff       (20)      359 2023-04-14 13:08:35.000000 dr-sdk-lotr-0.0.1/dr_sdk_lotr.egg-info/SOURCES.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-14 13:08:35.000000 dr-sdk-lotr-0.0.1/dr_sdk_lotr.egg-info/dependency_links.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-14 13:08:35.000000 dr-sdk-lotr-0.0.1/dr_sdk_lotr.egg-info/requires.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-14 13:08:35.000000 dr-sdk-lotr-0.0.1/dr_sdk_lotr.egg-info/top_level.txt
--rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-14 13:08:35.300965 dr-sdk-lotr-0.0.1/setup.cfg
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1157 2023-04-14 13:04:52.000000 dr-sdk-lotr-0.0.1/setup.py
-drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:08:35.300343 dr-sdk-lotr-0.0.1/tests/
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1197 2023-04-14 12:58:39.000000 dr-sdk-lotr-0.0.1/tests/test_books.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1123 2023-04-14 12:59:00.000000 dr-sdk-lotr-0.0.1/tests/test_chapters.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1689 2023-04-14 12:59:16.000000 dr-sdk-lotr-0.0.1/tests/test_characters.unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)     1140 2023-04-14 12:59:32.000000 dr-sdk-lotr-0.0.1/tests/test_movies_unittest.py
--rw-r--r--   0 dannyreliford   (501) staff       (20)      979 2023-04-14 13:00:15.000000 dr-sdk-lotr-0.0.1/tests/test_quotes_unittest.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:39:49.427645 dr-sdk-lotr-0.0.2/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1072 2023-04-14 12:36:30.000000 dr-sdk-lotr-0.0.2/LICENCE.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3199 2023-04-14 13:39:49.427491 dr-sdk-lotr-0.0.2/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2297 2023-04-14 13:34:32.000000 dr-sdk-lotr-0.0.2/README.md
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:39:49.424904 dr-sdk-lotr-0.0.2/dr_sdk_lotr/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        0 2023-04-14 12:39:34.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/__init__.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1560 2023-04-14 12:44:00.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/books.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1583 2023-04-14 12:44:19.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/chapters.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     2127 2023-04-14 12:45:06.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/characters.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1678 2023-04-14 12:45:26.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/movies.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1077 2023-04-14 12:45:44.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/quotes.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       40 2023-04-14 12:46:03.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr/settings.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:39:49.425780 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     3199 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/PKG-INFO
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      522 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/SOURCES.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        1 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/dependency_links.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)        9 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/requires.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       12 2023-04-14 13:39:49.000000 dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/top_level.txt
+-rw-r--r--   0 dannyreliford   (501) staff       (20)       38 2023-04-14 13:39:49.427689 dr-sdk-lotr-0.0.2/setup.cfg
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1157 2023-04-14 13:37:51.000000 dr-sdk-lotr-0.0.2/setup.py
+drwxr-xr-x   0 dannyreliford   (501) staff       (20)        0 2023-04-14 13:39:49.427142 dr-sdk-lotr-0.0.2/tests/
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1144 2023-04-14 13:36:41.000000 dr-sdk-lotr-0.0.2/tests/test_books.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1070 2023-04-14 13:36:50.000000 dr-sdk-lotr-0.0.2/tests/test_chapters.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1636 2023-04-14 13:36:57.000000 dr-sdk-lotr-0.0.2/tests/test_characters.unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)     1086 2023-04-14 13:37:07.000000 dr-sdk-lotr-0.0.2/tests/test_movies_unittest.py
+-rw-r--r--   0 dannyreliford   (501) staff       (20)      925 2023-04-14 13:37:17.000000 dr-sdk-lotr-0.0.2/tests/test_quotes_unittest.py
```

### Comparing `dr-sdk-lotr-0.0.1/LICENCE.txt` & `dr-sdk-lotr-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `dr-sdk-lotr-0.0.1/PKG-INFO` & `dr-sdk-lotr-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dr-sdk-lotr
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for interacting with the Lord of the Rings API
-Home-page: https://github.com/DannyBuffet/dr-Lord-of-the-rings-sdk
+Home-page: https://github.com/DannyBuffet/dr-lord-of-the-rings-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -20,23 +20,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # The Lord Of The Rings SDK
 A SDK built upon The One API (https://the-one-api.dev/) written in Python.
 
 ## Installation
+```bash
 pip install dr-sdk-lotr==0.0.1
+```
 
 ## Usage
 To use the SDK, get an Access Token from https://the-one-api.dev/sign-up. Once installed and the Access Token is obtained, you can start using the SDK by following the below:
 
 ## Using the SDK
 
 ### Book Data
-```
+```python
 from dr_sdk_lotr.books import Books
 
 books = Books('YOUR_API_KEY')
 
 # Lists of all "The Lord of the Rings" Books
 books.get_books()
 
@@ -44,15 +46,15 @@
 books.get_book_by_id('5cf58077b53e011a64671583')
 
 # Request all chapters of one specific book
 books.get_book_by_id('5cf58077b53e011a64671583')
 ```
 
 ### Character Data
-```
+```python
 from dr_sdk_lotr.chracters import Characters
 
 characters = Characters('YOUR_API_KEY')
 
 # Lists of all characters including metadata like name, gender, realm, race and more
 characters.get_all_characters()
 
@@ -63,15 +65,15 @@
 characters.get_quotes_by_character_id('5cd99d4bde30eff6ebccfbed')
 
 # Get character details by name
 characters.get_character_by_name('Gandalf')
 ```
 
 ### Movie Data
-```
+```python
 from dr_sdk_lotr.movies import Movies
 
 movies = Movies('YOUR_API_KEY')
 
 # List of all movies including "The Lord of the Rings" and the "The Hobbit" trilogies
 movies.get_movies()
 
@@ -79,33 +81,34 @@
 movies.get_movie_by_id('5cd95395de30eff6ebccde56')
 
 # Request all movie quotes for one specific movie (only working for LOTR Trilogy)
 movies.get_all_quotes_by_movie('5cd95395de30eff6ebccde5c')
 ```
 
 ### Quote Data
-```
+```python
 from dr_sdk_lotr.quotes import Quotes
 
 quotes = Quotes('YOUR_API_KEY')
 
 #  List of all movie quotes
 quotes.get_all_movie_quotes()
 
 # Request one specific movie quote
 quotes.get_movie_by_id("5cd96e05de30eff6ebccebce")
 ```
 
 ### Chapter Data
-```
+```python
 from dr_sdk_lotr.chapters import Chapters
 
 chapters = Chapters('YOUR_API_KEY')
 
 # Lists of all book chapters
 chapters.get_all_book_chapters()
 
 # Request one specific book chapter
 chapters.get_book_chapter_by_id('6091b6d6d58360f988133bc5')
 
 # Get book chapter by name
 chapters.get_book_chapter_by_name('A Long-expected Party')
+```
```

### Comparing `dr-sdk-lotr-0.0.1/README.md` & `dr-sdk-lotr-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # The Lord Of The Rings SDK
 A SDK built upon The One API (https://the-one-api.dev/) written in Python.
 
 ## Installation
+```bash
 pip install dr-sdk-lotr==0.0.1
+```
 
 ## Usage
 To use the SDK, get an Access Token from https://the-one-api.dev/sign-up. Once installed and the Access Token is obtained, you can start using the SDK by following the below:
 
 ## Using the SDK
 
 ### Book Data
-```
+```python
 from dr_sdk_lotr.books import Books
 
 books = Books('YOUR_API_KEY')
 
 # Lists of all "The Lord of the Rings" Books
 books.get_books()
 
@@ -22,15 +24,15 @@
 books.get_book_by_id('5cf58077b53e011a64671583')
 
 # Request all chapters of one specific book
 books.get_book_by_id('5cf58077b53e011a64671583')
 ```
 
 ### Character Data
-```
+```python
 from dr_sdk_lotr.chracters import Characters
 
 characters = Characters('YOUR_API_KEY')
 
 # Lists of all characters including metadata like name, gender, realm, race and more
 characters.get_all_characters()
 
@@ -41,15 +43,15 @@
 characters.get_quotes_by_character_id('5cd99d4bde30eff6ebccfbed')
 
 # Get character details by name
 characters.get_character_by_name('Gandalf')
 ```
 
 ### Movie Data
-```
+```python
 from dr_sdk_lotr.movies import Movies
 
 movies = Movies('YOUR_API_KEY')
 
 # List of all movies including "The Lord of the Rings" and the "The Hobbit" trilogies
 movies.get_movies()
 
@@ -57,33 +59,34 @@
 movies.get_movie_by_id('5cd95395de30eff6ebccde56')
 
 # Request all movie quotes for one specific movie (only working for LOTR Trilogy)
 movies.get_all_quotes_by_movie('5cd95395de30eff6ebccde5c')
 ```
 
 ### Quote Data
-```
+```python
 from dr_sdk_lotr.quotes import Quotes
 
 quotes = Quotes('YOUR_API_KEY')
 
 #  List of all movie quotes
 quotes.get_all_movie_quotes()
 
 # Request one specific movie quote
 quotes.get_movie_by_id("5cd96e05de30eff6ebccebce")
 ```
 
 ### Chapter Data
-```
+```python
 from dr_sdk_lotr.chapters import Chapters
 
 chapters = Chapters('YOUR_API_KEY')
 
 # Lists of all book chapters
 chapters.get_all_book_chapters()
 
 # Request one specific book chapter
 chapters.get_book_chapter_by_id('6091b6d6d58360f988133bc5')
 
 # Get book chapter by name
-chapters.get_book_chapter_by_name('A Long-expected Party')
+chapters.get_book_chapter_by_name('A Long-expected Party')
+```
```

### Comparing `dr-sdk-lotr-0.0.1/dr_sdk_lotr.egg-info/PKG-INFO` & `dr-sdk-lotr-0.0.2/dr_sdk_lotr.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dr-sdk-lotr
-Version: 0.0.1
+Version: 0.0.2
 Summary: SDK for interacting with the Lord of the Rings API
-Home-page: https://github.com/DannyBuffet/dr-Lord-of-the-rings-sdk
+Home-page: https://github.com/DannyBuffet/dr-lord-of-the-rings-sdk
 Author: Daniel Reliford
 Author-email: dreliford@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -20,23 +20,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # The Lord Of The Rings SDK
 A SDK built upon The One API (https://the-one-api.dev/) written in Python.
 
 ## Installation
+```bash
 pip install dr-sdk-lotr==0.0.1
+```
 
 ## Usage
 To use the SDK, get an Access Token from https://the-one-api.dev/sign-up. Once installed and the Access Token is obtained, you can start using the SDK by following the below:
 
 ## Using the SDK
 
 ### Book Data
-```
+```python
 from dr_sdk_lotr.books import Books
 
 books = Books('YOUR_API_KEY')
 
 # Lists of all "The Lord of the Rings" Books
 books.get_books()
 
@@ -44,15 +46,15 @@
 books.get_book_by_id('5cf58077b53e011a64671583')
 
 # Request all chapters of one specific book
 books.get_book_by_id('5cf58077b53e011a64671583')
 ```
 
 ### Character Data
-```
+```python
 from dr_sdk_lotr.chracters import Characters
 
 characters = Characters('YOUR_API_KEY')
 
 # Lists of all characters including metadata like name, gender, realm, race and more
 characters.get_all_characters()
 
@@ -63,15 +65,15 @@
 characters.get_quotes_by_character_id('5cd99d4bde30eff6ebccfbed')
 
 # Get character details by name
 characters.get_character_by_name('Gandalf')
 ```
 
 ### Movie Data
-```
+```python
 from dr_sdk_lotr.movies import Movies
 
 movies = Movies('YOUR_API_KEY')
 
 # List of all movies including "The Lord of the Rings" and the "The Hobbit" trilogies
 movies.get_movies()
 
@@ -79,33 +81,34 @@
 movies.get_movie_by_id('5cd95395de30eff6ebccde56')
 
 # Request all movie quotes for one specific movie (only working for LOTR Trilogy)
 movies.get_all_quotes_by_movie('5cd95395de30eff6ebccde5c')
 ```
 
 ### Quote Data
-```
+```python
 from dr_sdk_lotr.quotes import Quotes
 
 quotes = Quotes('YOUR_API_KEY')
 
 #  List of all movie quotes
 quotes.get_all_movie_quotes()
 
 # Request one specific movie quote
 quotes.get_movie_by_id("5cd96e05de30eff6ebccebce")
 ```
 
 ### Chapter Data
-```
+```python
 from dr_sdk_lotr.chapters import Chapters
 
 chapters = Chapters('YOUR_API_KEY')
 
 # Lists of all book chapters
 chapters.get_all_book_chapters()
 
 # Request one specific book chapter
 chapters.get_book_chapter_by_id('6091b6d6d58360f988133bc5')
 
 # Get book chapter by name
 chapters.get_book_chapter_by_name('A Long-expected Party')
+```
```

### Comparing `dr-sdk-lotr-0.0.1/setup.py` & `dr-sdk-lotr-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='dr-sdk-lotr',
-    version='0.0.1',
+    version='0.0.2',
     description='SDK for interacting with the Lord of the Rings API',
     author='Daniel Reliford',
     author_email='dreliford@gmail.com',
-    url='https://github.com/DannyBuffet/dr-Lord-of-the-rings-sdk',
+    url='https://github.com/DannyBuffet/dr-lord-of-the-rings-sdk',
     packages=setuptools.find_packages(),
     install_requires=['requests'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `dr-sdk-lotr-0.0.1/tests/test_books.unittest.py` & `dr-sdk-lotr-0.0.2/tests/test_books.unittest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import os
 import sys
-sys.path.insert(0, os.path.abspath( os.path.join(os.path.dirname(__file__),
-                                               '../src/') ))
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
 from dr_sdk_lotr.books import Books
 from config import access_token
 
 class TestBooks(unittest.TestCase):
 
     def test_get_books(self):
         books = Books(self.api_key)
```

### Comparing `dr-sdk-lotr-0.0.1/tests/test_chapters.unittest.py` & `dr-sdk-lotr-0.0.2/tests/test_chapters.unittest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import os
 import sys
-sys.path.insert(0, os.path.abspath( os.path.join(os.path.dirname(__file__),
-                                               '../src/') ))
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
 from dr_sdk_lotr.chapters import Chapters
 from config import access_token
 
 
 class TestChapters(unittest.TestCase):
 
     def test_get_chapters(self):
```

### Comparing `dr-sdk-lotr-0.0.1/tests/test_characters.unittest.py` & `dr-sdk-lotr-0.0.2/tests/test_characters.unittest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import os
 import sys
-sys.path.insert(0, os.path.abspath( os.path.join(os.path.dirname(__file__),
-                                               '../src/') ))
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+
 from dr_sdk_lotr.characters import Characters
 from config import access_token
 
 
 class TestCharacters(unittest.TestCase):
 
     def test_get_characters(self):
```

### Comparing `dr-sdk-lotr-0.0.1/tests/test_movies_unittest.py` & `dr-sdk-lotr-0.0.2/tests/test_movies_unittest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 import os
 import sys
-sys.path.insert(0, os.path.abspath( os.path.join(os.path.dirname(__file__),
-                                               '../src/') ))
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 from dr_sdk_lotr.movies import Movies
 from config import access_token
 
 
 class TestMovies(unittest.TestCase):
```

### Comparing `dr-sdk-lotr-0.0.1/tests/test_quotes_unittest.py` & `dr-sdk-lotr-0.0.2/tests/test_quotes_unittest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 import os
 import sys
-sys.path.insert(0, os.path.abspath( os.path.join(os.path.dirname(__file__),
-                                               '../src/') ))
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 from dr_sdk_lotr.quotes import Quotes
 from config import access_token
 
 
 class TestQuotes(unittest.TestCase):
```

