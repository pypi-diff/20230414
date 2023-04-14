# Comparing `tmp/webshoter-1.0.3.tar.gz` & `tmp/webshoter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webshoter-1.0.3.tar", last modified: Fri Apr 14 09:39:42 2023, max compression
+gzip compressed data, was "webshoter-1.0.4.tar", last modified: Fri Apr 14 09:48:43 2023, max compression
```

## Comparing `webshoter-1.0.3.tar` & `webshoter-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:42.340995 webshoter-1.0.3/
--rw-rw-rw-   0        0        0     1094 2023-04-14 07:20:26.000000 webshoter-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1745 2023-04-14 09:39:42.340995 webshoter-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2023-04-14 08:44:53.000000 webshoter-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 09:39:42.341997 webshoter-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1141 2023-04-14 09:38:04.000000 webshoter-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:42.325000 webshoter-1.0.3/webshoter/
--rw-rw-rw-   0        0        0       21 2023-04-14 09:39:27.000000 webshoter-1.0.3/webshoter/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-04-14 09:39:10.000000 webshoter-1.0.3/webshoter/__main__.py
--rw-rw-rw-   0        0        0     1738 2023-04-14 09:34:16.000000 webshoter-1.0.3/webshoter/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 09:39:42.338993 webshoter-1.0.3/webshoter.egg-info/
--rw-rw-rw-   0        0        0     1745 2023-04-14 09:39:42.000000 webshoter-1.0.3/webshoter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-04-14 09:39:42.000000 webshoter-1.0.3/webshoter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 09:39:42.000000 webshoter-1.0.3/webshoter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-14 09:39:42.000000 webshoter-1.0.3/webshoter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 09:39:42.000000 webshoter-1.0.3/webshoter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 09:39:42.000000 webshoter-1.0.3/webshoter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:48:43.128646 webshoter-1.0.4/
+-rw-rw-rw-   0        0        0     1094 2023-04-14 07:20:26.000000 webshoter-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1869 2023-04-14 09:48:43.127647 webshoter-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1321 2023-04-14 09:47:46.000000 webshoter-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:48:43.128646 webshoter-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1141 2023-04-14 09:38:04.000000 webshoter-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:48:43.110644 webshoter-1.0.4/webshoter/
+-rw-rw-rw-   0        0        0       21 2023-04-14 09:48:39.000000 webshoter-1.0.4/webshoter/__init__.py
+-rw-rw-rw-   0        0        0     3045 2023-04-14 09:45:34.000000 webshoter-1.0.4/webshoter/webshoter.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:48:43.126648 webshoter-1.0.4/webshoter.egg-info/
+-rw-rw-rw-   0        0        0     1869 2023-04-14 09:48:42.000000 webshoter-1.0.4/webshoter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-04-14 09:48:43.000000 webshoter-1.0.4/webshoter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:48:42.000000 webshoter-1.0.4/webshoter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-14 09:48:42.000000 webshoter-1.0.4/webshoter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 09:48:42.000000 webshoter-1.0.4/webshoter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 09:48:42.000000 webshoter-1.0.4/webshoter.egg-info/top_level.txt
```

### Comparing `webshoter-1.0.3/LICENSE` & `webshoter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.3/PKG-INFO` & `webshoter-1.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: webshoter
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python tool to take screenshots for urls
 Home-page: https://github.com/americo/webshoter
-Download-URL: https://github.com/americo/webshoter/archive/v1.0.3.zip
+Download-URL: https://github.com/americo/webshoter/archive/v1.0.4.zip
 Author: americo
 License: MIT License
 Keywords: screenshot,web,recon
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Screenshot Tool
+# WebShoter
 
 This tool takes screenshots of websites and saves them to a specified output directory in PNG format. It uses a headless browser to render the website and take the screenshot.
 
 ## Installation
 
 Before using the tool, make sure you have Python 3 installed on your system. You can download Python from the official website: https://www.python.org/downloads/
 
 Once you have Python installed, you can install the `webshoter` package using pip:
 
 ```sh
 pip install webshoter
 ```
+Or install manually:
+```sh
+1. git clone https://github.com/americo/webshoter
+2. cd webshoter
+3. python setup.py install
+```
 
 
 ## Usage
 
 To take a screenshot of a single website, use the following command:
 ```sh
 webshoter -u <url> -o <output_dir>
```

### Comparing `webshoter-1.0.3/README.md` & `webshoter-1.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-# Screenshot Tool
+# WebShoter
 
 This tool takes screenshots of websites and saves them to a specified output directory in PNG format. It uses a headless browser to render the website and take the screenshot.
 
 ## Installation
 
 Before using the tool, make sure you have Python 3 installed on your system. You can download Python from the official website: https://www.python.org/downloads/
 
 Once you have Python installed, you can install the `webshoter` package using pip:
 
 ```sh
 pip install webshoter
 ```
+Or install manually:
+```sh
+1. git clone https://github.com/americo/webshoter
+2. cd webshoter
+3. python setup.py install
+```
 
 
 ## Usage
 
 To take a screenshot of a single website, use the following command:
 ```sh
 webshoter -u <url> -o <output_dir>
```

### Comparing `webshoter-1.0.3/setup.py` & `webshoter-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.3/webshoter.egg-info/PKG-INFO` & `webshoter-1.0.4/webshoter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: webshoter
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python tool to take screenshots for urls
 Home-page: https://github.com/americo/webshoter
-Download-URL: https://github.com/americo/webshoter/archive/v1.0.3.zip
+Download-URL: https://github.com/americo/webshoter/archive/v1.0.4.zip
 Author: americo
 License: MIT License
 Keywords: screenshot,web,recon
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Screenshot Tool
+# WebShoter
 
 This tool takes screenshots of websites and saves them to a specified output directory in PNG format. It uses a headless browser to render the website and take the screenshot.
 
 ## Installation
 
 Before using the tool, make sure you have Python 3 installed on your system. You can download Python from the official website: https://www.python.org/downloads/
 
 Once you have Python installed, you can install the `webshoter` package using pip:
 
 ```sh
 pip install webshoter
 ```
+Or install manually:
+```sh
+1. git clone https://github.com/americo/webshoter
+2. cd webshoter
+3. python setup.py install
+```
 
 
 ## Usage
 
 To take a screenshot of a single website, use the following command:
 ```sh
 webshoter -u <url> -o <output_dir>
```

