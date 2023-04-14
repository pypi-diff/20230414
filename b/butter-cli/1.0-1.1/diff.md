# Comparing `tmp/butter-cli-1.0.tar.gz` & `tmp/butter-cli-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butter-cli-1.0.tar", last modified: Fri Apr 14 01:38:28 2023, max compression
+gzip compressed data, was "butter-cli-1.1.tar", last modified: Fri Apr 14 18:07:22 2023, max compression
```

## Comparing `butter-cli-1.0.tar` & `butter-cli-1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 01:38:28.231968 butter-cli-1.0/
--rw-r--r--   0 michaelequi   (501) staff       (20)      195 2023-04-14 01:38:28.231455 butter-cli-1.0/PKG-INFO
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 01:38:28.228107 butter-cli-1.0/butter_cli.egg-info/
--rw-r--r--   0 michaelequi   (501) staff       (20)      145 2023-04-14 01:30:14.000000 butter-cli-1.0/butter_cli.egg-info/PKG-INFO
--rw-r--r--   0 michaelequi   (501) staff       (20)      239 2023-04-14 01:28:01.000000 butter-cli-1.0/butter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)        1 2023-04-14 01:30:14.000000 butter-cli-1.0/butter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)       21 2023-04-14 01:30:14.000000 butter-cli-1.0/butter_cli.egg-info/requires.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)        7 2023-04-14 01:30:14.000000 butter-cli-1.0/butter_cli.egg-info/top_level.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)       38 2023-04-14 01:38:28.232106 butter-cli-1.0/setup.cfg
--rw-r--r--   0 michaelequi   (501) staff       (20)      460 2023-04-14 01:33:19.000000 butter-cli-1.0/setup.py
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 01:38:28.225730 butter-cli-1.0/src/
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 01:38:28.229026 butter-cli-1.0/src/butter/
--rw-r--r--   0 michaelequi   (501) staff       (20)       51 2023-04-14 01:34:57.000000 butter-cli-1.0/src/butter/__init__.py
--rw-r--r--   0 michaelequi   (501) staff       (20)     3796 2023-01-29 05:43:44.000000 butter-cli-1.0/src/butter/butter.py
--rw-r--r--   0 michaelequi   (501) staff       (20)     1140 2023-01-29 05:31:52.000000 butter-cli-1.0/src/butter/cli.py
-drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 01:38:28.230848 butter-cli-1.0/src/butter_cli.egg-info/
--rw-r--r--   0 michaelequi   (501) staff       (20)      195 2023-04-14 01:38:28.000000 butter-cli-1.0/src/butter_cli.egg-info/PKG-INFO
--rw-r--r--   0 michaelequi   (501) staff       (20)      428 2023-04-14 01:38:28.000000 butter-cli-1.0/src/butter_cli.egg-info/SOURCES.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)        1 2023-04-14 01:38:28.000000 butter-cli-1.0/src/butter_cli.egg-info/dependency_links.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)       21 2023-04-14 01:38:28.000000 butter-cli-1.0/src/butter_cli.egg-info/requires.txt
--rw-r--r--   0 michaelequi   (501) staff       (20)        7 2023-04-14 01:38:28.000000 butter-cli-1.0/src/butter_cli.egg-info/top_level.txt
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.017002 butter-cli-1.1/
+-rw-r--r--   0 michaelequi   (501) staff       (20)      195 2023-04-14 18:07:22.016690 butter-cli-1.1/PKG-INFO
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.012221 butter-cli-1.1/butter_cli.egg-info/
+-rw-r--r--   0 michaelequi   (501) staff       (20)      145 2023-04-14 01:30:14.000000 butter-cli-1.1/butter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 michaelequi   (501) staff       (20)      239 2023-04-14 01:28:01.000000 butter-cli-1.1/butter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)        1 2023-04-14 01:30:14.000000 butter-cli-1.1/butter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)       21 2023-04-14 01:30:14.000000 butter-cli-1.1/butter_cli.egg-info/requires.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)        7 2023-04-14 01:30:14.000000 butter-cli-1.1/butter_cli.egg-info/top_level.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)       38 2023-04-14 18:07:22.017095 butter-cli-1.1/setup.cfg
+-rw-r--r--   0 michaelequi   (501) staff       (20)      638 2023-04-14 18:07:04.000000 butter-cli-1.1/setup.py
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.009677 butter-cli-1.1/src/
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.014011 butter-cli-1.1/src/butter/
+-rw-r--r--   0 michaelequi   (501) staff       (20)       51 2023-04-14 01:34:57.000000 butter-cli-1.1/src/butter/__init__.py
+-rw-r--r--   0 michaelequi   (501) staff       (20)     3855 2023-04-14 07:32:50.000000 butter-cli-1.1/src/butter/butter.py
+-rw-r--r--   0 michaelequi   (501) staff       (20)     1140 2023-01-29 05:31:52.000000 butter-cli-1.1/src/butter/cli.py
+drwxr-xr-x   0 michaelequi   (501) staff       (20)        0 2023-04-14 18:07:22.016325 butter-cli-1.1/src/butter_cli.egg-info/
+-rw-r--r--   0 michaelequi   (501) staff       (20)      195 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/PKG-INFO
+-rw-r--r--   0 michaelequi   (501) staff       (20)      469 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)        1 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)       42 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/entry_points.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)       21 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/requires.txt
+-rw-r--r--   0 michaelequi   (501) staff       (20)        7 2023-04-14 18:07:21.000000 butter-cli-1.1/src/butter_cli.egg-info/top_level.txt
```

### Comparing `butter-cli-1.0/src/butter/butter.py` & `butter-cli-1.1/src/butter/butter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     return dec
 
 class Butter:
     tests = []
 
     def __init__(self) -> None:
         self.console = Console()
-        self.url = "https://butter-production.up.railway.app/run_analytics"
+        # self.url = "https://butter-production.up.railway.app/run_analytics"
+        self.url = "http://127.0.0.1:5000/run_analytics"
 
     def run_tests(self, path: Path, id, description: str, debug=False):
         self.console.print(f":sunglasses: Running tests...\n")
 
         tests = []
         json_files = set()
         for test, json_file, desc in Butter.tests:
```

### Comparing `butter-cli-1.0/src/butter/cli.py` & `butter-cli-1.1/src/butter/cli.py`

 * *Files identical despite different names*

