# Comparing `tmp/yaml_requests-0.8.0.tar.gz` & `tmp/yaml_requests-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/yaml_requests/yaml_requests/dist/tmpyn4f6obl/yaml_requests-0.8.0.tar", last modified: Fri Jan 14 01:18:18 2022, max compression
+gzip compressed data, was "/home/runner/work/yaml_requests/yaml_requests/dist/.tmp-_8w_5ass/yaml_requests-0.9.0.tar", last modified: Thu Apr 13 22:35:41 2023, max compression
```

## Comparing `yaml_requests-0.8.0.tar` & `yaml_requests-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4770 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     4287 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)       80 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/bin/yaml_requests
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/yaml_requests/
--rwxr-xr-x   0 runner    (1001) docker     (121)       58 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       88 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6766 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/_logger.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2198 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/_main.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1105 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/_plan.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5069 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/_request.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2729 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/_runner.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       22 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/yaml_requests/utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1991 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/utils/args.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2185 2022-01-14 01:18:10.000000 yaml_requests-0.8.0/yaml_requests/utils/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/yaml_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4770 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/yaml_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/yaml_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/yaml_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/yaml_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-01-14 01:18:18.000000 yaml_requests-0.8.0/yaml_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4287 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/bin/yaml_requests
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2207 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/_plan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5069 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/_runner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/logger/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/logger/_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1991 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/utils/args.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2185 2023-04-13 22:35:32.000000 yaml_requests-0.9.0/yaml_requests/utils/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:35:41.000000 yaml_requests-0.9.0/yaml_requests.egg-info/top_level.txt
```

### Comparing `yaml_requests-0.8.0/LICENSE` & `yaml_requests-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml_requests-0.8.0/PKG-INFO` & `yaml_requests-0.9.0/yaml_requests.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
-Name: yaml_requests
-Version: 0.8.0
+Name: yaml-requests
+Version: 0.9.0
 Summary: A simple python app for sending a set of consecutive HTTP requests defined in YAML requests plan.
 Home-page: https://github.com/kangasta/yaml_requests
 Author: Toni Kangas
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yaml_requests
@@ -122,9 +120,7 @@
 
 Get test coverage with commands:
 
 ```bash
 coverage run --branch --source yaml_requests/ -m unittest discover -s tst/
 coverage report -m
 ```
-
-
```

### Comparing `yaml_requests-0.8.0/README.md` & `yaml_requests-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `yaml_requests-0.8.0/setup.py` & `yaml_requests-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     description="A simple python app for sending a set of consecutive HTTP requests defined in YAML requests plan.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kangasta/yaml_requests",
     packages=setuptools.find_packages(),
     scripts=["bin/yaml_requests"],
     install_requires=[
-        "Jinja2~=2.0",
+        "Jinja2~=3.0",
         "pyyaml~=5.0",
         "requests~=2.0",
     ],
     classifiers=(
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `yaml_requests-0.8.0/yaml_requests/_logger.py` & `yaml_requests-0.9.0/yaml_requests/logger/_console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import yaml
 import re
 from shutil import get_terminal_size
 from threading import Event, Thread
 
-from ._request import RequestState
+from .._request import RequestState
 
 # From cli-spinners (https://www.npmjs.com/package/cli-spinners)
 INTERVAL = 0.080  # seconds
 FRAMES = ['⠋', '⠙', '⠹', '⠸', '⠼', '⠴', '⠦', '⠧', '⠇', '⠏']
 
 COLORS = dict(red=31, green=32, yellow=33, blue=34, grey=90)
 
@@ -54,15 +54,15 @@
         return ('green', '✔',)
     elif state in (RequestState.FAILURE, RequestState.ERROR,):
         return ('red', '✘',)
     elif state == RequestState.SKIPPED:
         return ('blue', '⮟',)
 
 
-class RequestLogger:
+class ConsoleLogger:
     def __init__(self, animations, colors):
         self._animations = animations
         self._colors = colors
 
         self._active = None
         self._stop_event = Event()
 
@@ -72,15 +72,19 @@
         return f'\033[1m{text}\033[22m'
 
     def color(self, text, color):
         if not self._colors or color not in COLORS:
             return text
         return f'\033[{COLORS[color]}m{text}\033[0m'
 
-    def error(self, text):
+    def error(self, error):
+        text = str(error)
+        if not text:
+            return
+
         error_text = self.bold(self.color('ERROR:', 'red'))
         print(f'{error_text} {text}')
 
     def _repeat_text(self, repeat_index):
         if repeat_index is None:
             return ''
         return f' (repeat_index={repeat_index})'
@@ -181,22 +185,22 @@
 
         self._active = Thread(
             target=_print_spinner_and_text, args=[
                 text, self._stop_event])
         self._stop_event.clear()
         self._active.start()
 
-    def stop_progress_animation(self):
+    def close(self):
         self._stop_event.set()
         if self._active:
             self._active.join()
             self._active = None
 
     def finish_request(self, request):
-        self.stop_progress_animation()
+        self.close()
 
         name_text = self._get_name_text(request)
         name_separator = name_text and '\n  '
         code_text = self._get_response_code_text(request)
         message_text = self._get_message_text(request)
         message_separator = '\n  ' if message_text and code_text else ''
```

### Comparing `yaml_requests-0.8.0/yaml_requests/_plan.py` & `yaml_requests-0.9.0/yaml_requests/_plan.py`

 * *Files identical despite different names*

### Comparing `yaml_requests-0.8.0/yaml_requests/_request.py` & `yaml_requests-0.9.0/yaml_requests/_request.py`

 * *Files identical despite different names*

### Comparing `yaml_requests-0.8.0/yaml_requests/_runner.py` & `yaml_requests-0.9.0/yaml_requests/_runner.py`

 * *Files identical despite different names*

### Comparing `yaml_requests-0.8.0/yaml_requests/utils/args.py` & `yaml_requests-0.9.0/yaml_requests/utils/args.py`

 * *Files identical despite different names*

### Comparing `yaml_requests-0.8.0/yaml_requests/utils/template.py` & `yaml_requests-0.9.0/yaml_requests/utils/template.py`

 * *Files identical despite different names*

### Comparing `yaml_requests-0.8.0/yaml_requests.egg-info/PKG-INFO` & `yaml_requests-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
-Name: yaml-requests
-Version: 0.8.0
+Name: yaml_requests
+Version: 0.9.0
 Summary: A simple python app for sending a set of consecutive HTTP requests defined in YAML requests plan.
 Home-page: https://github.com/kangasta/yaml_requests
 Author: Toni Kangas
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yaml_requests
@@ -122,9 +120,7 @@
 
 Get test coverage with commands:
 
 ```bash
 coverage run --branch --source yaml_requests/ -m unittest discover -s tst/
 coverage report -m
 ```
-
-
```

### Comparing `yaml_requests-0.8.0/yaml_requests.egg-info/SOURCES.txt` & `yaml_requests-0.9.0/yaml_requests.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 LICENSE
 README.md
 setup.py
 bin/yaml_requests
 yaml_requests/__init__.py
 yaml_requests/__main__.py
-yaml_requests/_logger.py
 yaml_requests/_main.py
 yaml_requests/_plan.py
 yaml_requests/_request.py
 yaml_requests/_runner.py
 yaml_requests/_version.py
+yaml_requests/error.py
 yaml_requests.egg-info/PKG-INFO
 yaml_requests.egg-info/SOURCES.txt
 yaml_requests.egg-info/dependency_links.txt
 yaml_requests.egg-info/requires.txt
 yaml_requests.egg-info/top_level.txt
+yaml_requests/logger/__init__.py
+yaml_requests/logger/_console.py
+yaml_requests/logger/_request.py
 yaml_requests/utils/__init__.py
 yaml_requests/utils/args.py
 yaml_requests/utils/template.py
```

