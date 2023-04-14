# Comparing `tmp/webshoter-1.0.1.tar.gz` & `tmp/webshoter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webshoter-1.0.1.tar", last modified: Fri Apr 14 08:48:36 2023, max compression
+gzip compressed data, was "webshoter-1.0.2.tar", last modified: Fri Apr 14 09:34:31 2023, max compression
```

## Comparing `webshoter-1.0.1.tar` & `webshoter-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:48:36.719298 webshoter-1.0.1/
--rw-rw-rw-   0        0        0     1094 2023-04-14 07:20:26.000000 webshoter-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1745 2023-04-14 08:48:36.718298 webshoter-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2023-04-14 08:44:53.000000 webshoter-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 08:48:36.719298 webshoter-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1141 2023-04-14 08:44:44.000000 webshoter-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:48:36.700791 webshoter-1.0.1/webshoter/
--rw-rw-rw-   0        0        0       21 2023-04-14 08:46:40.000000 webshoter-1.0.1/webshoter/__init__.py
--rw-rw-rw-   0        0        0     1738 2023-04-14 08:48:28.000000 webshoter-1.0.1/webshoter/utils.py
--rw-rw-rw-   0        0        0     1440 2023-04-14 08:44:49.000000 webshoter-1.0.1/webshoter/webshoter.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:48:36.716302 webshoter-1.0.1/webshoter.egg-info/
--rw-rw-rw-   0        0        0     1745 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 09:34:31.581679 webshoter-1.0.2/
+-rw-rw-rw-   0        0        0     1094 2023-04-14 07:20:26.000000 webshoter-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1745 2023-04-14 09:34:31.581679 webshoter-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2023-04-14 08:44:53.000000 webshoter-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:34:31.582679 webshoter-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1141 2023-04-14 08:44:44.000000 webshoter-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:34:31.568680 webshoter-1.0.2/webshoter/
+-rw-rw-rw-   0        0        0       21 2023-04-14 09:34:17.000000 webshoter-1.0.2/webshoter/__init__.py
+-rw-rw-rw-   0        0        0     1738 2023-04-14 09:34:16.000000 webshoter-1.0.2/webshoter/utils.py
+-rw-rw-rw-   0        0        0     1444 2023-04-14 09:34:14.000000 webshoter-1.0.2/webshoter/webshoter.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:34:31.579693 webshoter-1.0.2/webshoter.egg-info/
+-rw-rw-rw-   0        0        0     1745 2023-04-14 09:34:31.000000 webshoter-1.0.2/webshoter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-14 09:34:31.000000 webshoter-1.0.2/webshoter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:34:31.000000 webshoter-1.0.2/webshoter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-14 09:34:31.000000 webshoter-1.0.2/webshoter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 09:34:31.000000 webshoter-1.0.2/webshoter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 09:34:31.000000 webshoter-1.0.2/webshoter.egg-info/top_level.txt
```

### Comparing `webshoter-1.0.1/LICENSE` & `webshoter-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.1/PKG-INFO` & `webshoter-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: webshoter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python tool to take screenshots for urls
 Home-page: https://github.com/americo/webshoter
-Download-URL: https://github.com/americo/webshoter/archive/v1.0.1.zip
+Download-URL: https://github.com/americo/webshoter/archive/v1.0.2.zip
 Author: americo
 License: MIT License
 Keywords: screenshot,web,recon
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `webshoter-1.0.1/README.md` & `webshoter-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.1/setup.py` & `webshoter-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.1/webshoter/utils.py` & `webshoter-1.0.2/webshoter/utils.py`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.1/webshoter/webshoter.py` & `webshoter-1.0.2/webshoter/webshoter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import sys
 import os
 from utils import get_host_by_url, get_bgp_toolkit, download_screenshot, banner, generate_html_report
 from huepy import *
 
-def main():
+def __main__():
     print('\033c')
     print(banner())
     parser = argparse.ArgumentParser()
     parser.add_argument("-o", "--output", help="Output directory", required=True)
     urls = []
 
     # Check if there is data piped into the script
```

### Comparing `webshoter-1.0.1/webshoter.egg-info/PKG-INFO` & `webshoter-1.0.2/webshoter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: webshoter
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python tool to take screenshots for urls
 Home-page: https://github.com/americo/webshoter
-Download-URL: https://github.com/americo/webshoter/archive/v1.0.1.zip
+Download-URL: https://github.com/americo/webshoter/archive/v1.0.2.zip
 Author: americo
 License: MIT License
 Keywords: screenshot,web,recon
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

