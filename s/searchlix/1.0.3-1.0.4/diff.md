# Comparing `tmp/searchlix-1.0.3.tar.gz` & `tmp/searchlix-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\searchlix-1.0.3.tar", last modified: Fri Apr 14 20:34:41 2023, max compression
+gzip compressed data, was "dist\searchlix-1.0.4.tar", last modified: Fri Apr 14 20:50:57 2023, max compression
```

## Comparing `searchlix-1.0.3.tar` & `searchlix-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 20:34:41.000000 searchlix-1.0.3/
--rw-rw-rw-   0        0        0     1738 2023-04-14 20:34:41.000000 searchlix-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      986 2023-04-14 20:09:39.000000 searchlix-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix/
--rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 searchlix-1.0.3/searchlix/__init__.py
--rw-rw-rw-   0        0        0     2682 2023-04-14 19:50:21.000000 searchlix-1.0.3/searchlix/searchlix.py
-drwxrwxrwx   0        0        0        0 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/
--rw-rw-rw-   0        0        0     1738 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 20:34:41.000000 searchlix-1.0.3/searchlix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 20:34:41.000000 searchlix-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-04-14 20:33:56.000000 searchlix-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:50:57.000000 searchlix-1.0.4/
+-rw-rw-rw-   0        0        0     2162 2023-04-14 20:50:57.000000 searchlix-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1298 2023-04-14 20:50:21.000000 searchlix-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix/
+-rw-rw-rw-   0        0        0        0 2023-04-14 00:19:50.000000 searchlix-1.0.4/searchlix/__init__.py
+-rw-rw-rw-   0        0        0     2682 2023-04-14 19:50:21.000000 searchlix-1.0.4/searchlix/searchlix.py
+drwxrwxrwx   0        0        0        0 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/
+-rw-rw-rw-   0        0        0     2162 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 20:50:57.000000 searchlix-1.0.4/searchlix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 20:50:57.000000 searchlix-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-04-14 20:50:48.000000 searchlix-1.0.4/setup.py
```

### Comparing `searchlix-1.0.3/PKG-INFO` & `searchlix-1.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-Metadata-Version: 2.1
-Name: searchlix
-Version: 1.0.3
-Summary: A package for extract data from websites and text
-Home-page: UNKNOWN
-Author: Hashem
-Author-email: hashem.a.muhammad@gmail.com
-License: UNKNOWN
-Description: # Searchlix
-        ## _powerful python pakage to search in text and websites_
-        
-        
-        
-        ## Features
-        
-        - Find emails in text / Email validation
-        - Find emails in website page
-        - Find phone number in text / Phone number validation
-        - Find phone number in website page
-        - Pattern search in text
-        - Search for page name in website
-        
-        
-        
-        
-        ## Installation
-        
-        python 3.6+
-        
-        ```sh
-        pip install searchlix
-        ```
-        
-        ## Functions
-        
-        How you can use it.
-        
-        | Features | Function |
-        | ------ | ------ |
-        | Find emails in text / Email validation | find_email(text) |
-        | Find emails in website page | extract_email_from_link(url) |
-        | Find phone number in text / Phone number validation | find_phone_number(text) |
-        | Find phone number in website page | extract_phone_from_link(url) |
-        | Pattern search in text | pattern_search(text, pattern) |
-        | Search for page name in website | extract_page_url(url, page_name) |
-        
-        ## Example
-        
-        
-        
-        
-        ```sh
-        from searchlix import searchlix
-        ```
-        
-        
-        
-        ## License
-        
-        MIT
-Keywords: python,web scraping,emails,phone,data,search
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Searchlix
+## _powerful python pakage to search in text and websites_
+
+
+
+## Features
+
+- Find emails in text / Email validation
+- Find emails in website page
+- Find phone number in text / Phone number validation
+- Find phone number in website page
+- Pattern search in text
+- Search for page name in website
+
+
+
+
+## Installation
+
+python 3.6+
+
+```sh
+pip install searchlix
+```
+
+## Functions
+
+How you can use it.
+
+| Features | Function |
+| ------ | ------ |
+| Find emails in text / Email validation | find_email(text) |
+| Find emails in website page | extract_email_from_link(url) |
+| Find phone number in text / Phone number validation | find_phone_number(text) |
+| Find phone number in website page | extract_phone_from_link(url) |
+| Pattern search in text | pattern_search(text, pattern) |
+| Search for page name in website | extract_page_url(url, page_name) |
+
+## Import
+
+
+
+
+```sh
+from searchlix import searchlix
+```
+
+## Future Works
+
+- Add proper error handiling
+- Add test cases
+- Add more features
+
+## Notes
+
+- this is a beta version
+- if you have any suggestions please feel free to send email to me
+
+## Contact Information 
+- email: hashem.a.muhammad@gmail.com
+- linkedin https://linkedin.com/in/hashem-muhammad
+
+
+## License
+
+MIT
```

### Comparing `searchlix-1.0.3/searchlix/searchlix.py` & `searchlix-1.0.4/searchlix/searchlix.py`

 * *Files identical despite different names*

### Comparing `searchlix-1.0.3/setup.py` & `searchlix-1.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='searchlix',
-    version='1.0.3',
+    version='1.0.4',
     description='A package for extract data from websites and text',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Hashem',
     author_email='hashem.a.muhammad@gmail.com',
     packages=find_packages(),
     install_requires=[
```

