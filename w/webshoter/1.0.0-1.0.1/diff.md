# Comparing `tmp/webshoter-1.0.0.tar.gz` & `tmp/webshoter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webshoter-1.0.0.tar", last modified: Fri Apr 14 08:45:12 2023, max compression
+gzip compressed data, was "webshoter-1.0.1.tar", last modified: Fri Apr 14 08:48:36 2023, max compression
```

## Comparing `webshoter-1.0.0.tar` & `webshoter-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 08:45:12.290497 webshoter-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-04-14 07:20:26.000000 webshoter-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1745 2023-04-14 08:45:12.290497 webshoter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2023-04-14 08:44:53.000000 webshoter-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 08:45:12.291485 webshoter-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1141 2023-04-14 08:44:44.000000 webshoter-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:45:12.266474 webshoter-1.0.0/webshoter/
--rw-rw-rw-   0        0        0       21 2023-04-14 08:30:38.000000 webshoter-1.0.0/webshoter/__init__.py
--rw-rw-rw-   0        0        0     1653 2023-04-14 08:26:54.000000 webshoter-1.0.0/webshoter/utils.py
--rw-rw-rw-   0        0        0     1440 2023-04-14 08:44:49.000000 webshoter-1.0.0/webshoter/webshoter.py
-drwxrwxrwx   0        0        0        0 2023-04-14 08:45:12.288511 webshoter-1.0.0/webshoter.egg-info/
--rw-rw-rw-   0        0        0     1745 2023-04-14 08:45:12.000000 webshoter-1.0.0/webshoter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-14 08:45:12.000000 webshoter-1.0.0/webshoter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 08:45:12.000000 webshoter-1.0.0/webshoter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-14 08:45:12.000000 webshoter-1.0.0/webshoter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-14 08:45:12.000000 webshoter-1.0.0/webshoter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-14 08:45:12.000000 webshoter-1.0.0/webshoter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 08:48:36.719298 webshoter-1.0.1/
+-rw-rw-rw-   0        0        0     1094 2023-04-14 07:20:26.000000 webshoter-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1745 2023-04-14 08:48:36.718298 webshoter-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2023-04-14 08:44:53.000000 webshoter-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 08:48:36.719298 webshoter-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1141 2023-04-14 08:44:44.000000 webshoter-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:48:36.700791 webshoter-1.0.1/webshoter/
+-rw-rw-rw-   0        0        0       21 2023-04-14 08:46:40.000000 webshoter-1.0.1/webshoter/__init__.py
+-rw-rw-rw-   0        0        0     1738 2023-04-14 08:48:28.000000 webshoter-1.0.1/webshoter/utils.py
+-rw-rw-rw-   0        0        0     1440 2023-04-14 08:44:49.000000 webshoter-1.0.1/webshoter/webshoter.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:48:36.716302 webshoter-1.0.1/webshoter.egg-info/
+-rw-rw-rw-   0        0        0     1745 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 08:48:36.000000 webshoter-1.0.1/webshoter.egg-info/top_level.txt
```

### Comparing `webshoter-1.0.0/LICENSE` & `webshoter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.0/PKG-INFO` & `webshoter-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: webshoter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python tool to take screenshots for urls
 Home-page: https://github.com/americo/webshoter
-Download-URL: https://github.com/americo/webshoter/archive/v1.0.0.zip
+Download-URL: https://github.com/americo/webshoter/archive/v1.0.1.zip
 Author: americo
 License: MIT License
 Keywords: screenshot,web,recon
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `webshoter-1.0.0/README.md` & `webshoter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.0/setup.py` & `webshoter-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.0/webshoter/utils.py` & `webshoter-1.0.1/webshoter/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import os
+from huepy import blue
 
 def banner():
-    return r"""┬ ┬┌─┐┌┐ ┌─┐┬ ┬┌─┐┌┬┐
-│││├┤ ├┴┐└─┐├─┤│ │ │  v1.0
-└┴┘└─┘└─┘└─┘┴ ┴└─┘ ┴ 
+    return f"""┬ ┬┌─┐┌┐ ┌─┐┬ ┬┌─┐┌┬┐┌─┐┬─┐
+│││├┤ ├┴┐└─┐├─┤│ │ │ ├┤ ├┬┘ {blue('v1')}
+└┴┘└─┘└─┘└─┘┴ ┴└─┘ ┴ └─┘┴└─ 
 Web screenshoting tool
      """
 
 # Get url host
 def get_host_by_url(url):
     return url.split("/")[2]
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-import requests import os def banner(): return r"""â¬ â¬âââââ
-ââââ¬ â¬âââââ¬â âââââ¤
-ââ´âââââââ¤â â â v1.0
-ââ´âââââââââââ´ â´âââ â´ Web screenshoting tool
-""" # Get url host def get_host_by_url(url): return url.split("/")[2] # Get
-first 2 chars of host def get_host_short(host): return host[0:2] # Request BGP
-toolkit def get_bgp_toolkit(host): url = "https://bgp.he.net/dns/" + host
-response = requests.get(url) return response.text # Download screenshot def
+import requests import os from huepy import blue def banner(): return f"""â¬
+â¬âââââ ââââ¬ â¬âââââ¬âââââ¬ââ
+âââââ¤ ââ´âââââââ¤â â â ââ¤ ââ¬â {blue
+('v1')} ââ´âââââââââââ´ â´âââ â´
+ââââ´ââ Web screenshoting tool """ # Get url host def
+get_host_by_url(url): return url.split("/")[2] # Get first 2 chars of host def
+get_host_short(host): return host[0:2] # Request BGP toolkit def
+get_bgp_toolkit(host): url = "https://bgp.he.net/dns/" + host response =
+requests.get(url) return response.text # Download screenshot def
 download_screenshot(host, output): url = f"https://bgp.he.net/webthumbs/{host[:
 1]}/{host[1:2]}/{host}_720.png" # Download image by url, using browser headers
 response = requests.get(url, headers={"User-Agent": "Mozilla/5.0"}) # Save
 image to file with open(f"{output}/{host}.png", "wb") as f: f.write
 (response.content) # Generate HTML report by directory def generate_html_report
 (dir): # Get all files in directory files = os.listdir(dir) # Filter out files
 that are not png files = list(filter(lambda x: x.endswith(".png"), files)) #
```

### Comparing `webshoter-1.0.0/webshoter/webshoter.py` & `webshoter-1.0.1/webshoter/webshoter.py`

 * *Files identical despite different names*

### Comparing `webshoter-1.0.0/webshoter.egg-info/PKG-INFO` & `webshoter-1.0.1/webshoter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: webshoter
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python tool to take screenshots for urls
 Home-page: https://github.com/americo/webshoter
-Download-URL: https://github.com/americo/webshoter/archive/v1.0.0.zip
+Download-URL: https://github.com/americo/webshoter/archive/v1.0.1.zip
 Author: americo
 License: MIT License
 Keywords: screenshot,web,recon
 Classifier: Topic :: Security
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

