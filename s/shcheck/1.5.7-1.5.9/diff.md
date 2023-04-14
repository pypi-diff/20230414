# Comparing `tmp/shcheck-1.5.7.tar.gz` & `tmp/shcheck-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shcheck-1.5.7.tar", last modified: Sat Nov 19 18:12:05 2022, max compression
+gzip compressed data, was "shcheck-1.5.9.tar", last modified: Fri Apr 14 09:16:11 2023, max compression
```

## Comparing `shcheck-1.5.7.tar` & `shcheck-1.5.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 18:12:05.115112 shcheck-1.5.7/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-11-19 18:11:45.000000 shcheck-1.5.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-11-19 18:12:05.111112 shcheck-1.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-11-19 18:11:45.000000 shcheck-1.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-19 18:12:05.115112 shcheck-1.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-11-19 18:11:45.000000 shcheck-1.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 18:12:05.111112 shcheck-1.5.7/shcheck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-11-19 18:12:05.000000 shcheck-1.5.7/shcheck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-19 18:12:05.000000 shcheck-1.5.7/shcheck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-19 18:12:05.000000 shcheck-1.5.7/shcheck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-19 18:12:05.000000 shcheck-1.5.7/shcheck.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    14149 2022-11-19 18:11:45.000000 shcheck-1.5.7/shcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:16:11.345353 shcheck-1.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-14 09:16:00.000000 shcheck-1.5.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-14 09:16:11.345353 shcheck-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-14 09:16:00.000000 shcheck-1.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:16:11.345353 shcheck-1.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-14 09:16:00.000000 shcheck-1.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:16:11.345353 shcheck-1.5.9/shcheck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-14 09:16:11.000000 shcheck-1.5.9/shcheck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-14 09:16:11.000000 shcheck-1.5.9/shcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:16:11.000000 shcheck-1.5.9/shcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 09:16:11.000000 shcheck-1.5.9/shcheck.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14346 2023-04-14 09:16:00.000000 shcheck-1.5.9/shcheck.py
```

### Comparing `shcheck-1.5.7/LICENSE.txt` & `shcheck-1.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shcheck-1.5.7/PKG-INFO` & `shcheck-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcheck
-Version: 1.5.7
+Version: 1.5.9
 Summary: A basic tool to check security headers of a website
 Home-page: https://github.com/santoru/shcheck
 Author: santoru
 Author-email: santoru@pm.me
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shcheck Version: 1.5.7 Summary: A basic tool to
+Metadata-Version: 2.1 Name: shcheck Version: 1.5.9 Summary: A basic tool to
 check security headers of a website Home-page: https://github.com/santoru/
 shcheck Author: santoru Author-email: santoru@pm.me Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE.txt # shcheck -
 Security Header Check
                  [PyPI] [Pypi] [Updated] [Output on Facebook]
 ## Check security headers on a target website I did this tool to help me to
 check which security headers are enabled on certain websites. The tool is very
```

### Comparing `shcheck-1.5.7/README.md` & `shcheck-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `shcheck-1.5.7/setup.py` & `shcheck-1.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import setup
 
 PACKAGE_NAME = "shcheck"
-VERSION = "1.5.7"
+VERSION = "1.5.9"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 def parse_requirements(filename):
     """Load requirements from a pip requirements file."""
```

### Comparing `shcheck-1.5.7/shcheck.egg-info/PKG-INFO` & `shcheck-1.5.9/shcheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcheck
-Version: 1.5.7
+Version: 1.5.9
 Summary: A basic tool to check security headers of a website
 Home-page: https://github.com/santoru/shcheck
 Author: santoru
 Author-email: santoru@pm.me
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shcheck Version: 1.5.7 Summary: A basic tool to
+Metadata-Version: 2.1 Name: shcheck Version: 1.5.9 Summary: A basic tool to
 check security headers of a website Home-page: https://github.com/santoru/
 shcheck Author: santoru Author-email: santoru@pm.me Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE.txt # shcheck -
 Security Header Check
                  [PyPI] [Pypi] [Updated] [Output on Facebook]
 ## Check security headers on a target website I did this tool to help me to
 check which security headers are enabled on certain websites. The tool is very
```

### Comparing `shcheck-1.5.7/shcheck.py` & `shcheck-1.5.9/shcheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,17 @@
     'Cross-Origin-Embedder-Policy': 'warning',
     'Cross-Origin-Resource-Policy': 'warning',
     'Cross-Origin-Opener-Policy': 'warning'
 }
 
 information_headers = {
     'X-Powered-By',
-    'Server'
+    'Server',
+    'X-AspNet-Version',
+    'X-AspNetMvc-Version'
 }
 
 cache_headers = {
     'Cache-Control',
     'Pragma',
     'Last-Modified'
     'Expires',
@@ -167,25 +169,28 @@
 
 
 def print_error(target, e):
     sys.stdout = sys.__stdout__
     if isinstance(e, ValueError):
         print("Unknown url type")
 
-    if isinstance(e, urllib.error.HTTPError):
+    elif isinstance(e, urllib.error.HTTPError):
         print("[!] URL Returned an HTTP error: {}".format(
               colorize(str(e.code), 'error')))
 
-    if isinstance(e, urllib.error.URLError):
+    elif isinstance(e, urllib.error.URLError):
         if "CERTIFICATE_VERIFY_FAILED" in str(e.reason):
             print("SSL: Certificate validation error.\nIf you want to \
     ignore it run the program with the \"-d\" option.")
         else:
             print("Target host {} seems to be unreachable ({})".format(target, e.reason))
 
+    else:
+        print("{}".format(str(e)))
+
 
 def check_target(target, options):
     '''
     Just put a protocol to a valid IP and check if connection works,
     returning HEAD response
     '''
     # Recover used options
@@ -206,16 +211,19 @@
     try:
         response = urllib.request.urlopen(request, timeout=10)
 
     # Handling issues with HTTP/2
     except http.client.UnknownProtocol as e:
         print("Unknown protocol: {}. Are you using a proxy? Try disabling it".format(e))
     except Exception as e:
-        print_error(target, e)
-        return None
+        if hasattr(e, 'code') and e.code == 404:
+            response = e
+        else:
+            print_error(target, e)
+            return None
 
     if response is not None:
         return response
     print("Couldn't read a response from server.")
     return None
```

