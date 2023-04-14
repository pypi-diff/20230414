# Comparing `tmp/testflows.uexpect-1.7.220902.1112725.tar.gz` & `tmp/testflows.uexpect-1.7.230414.1210501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.uexpect-1.7.220902.1112725.tar", last modified: Fri Sep  2 11:27:25 2022, max compression
+gzip compressed data, was "testflows.uexpect-1.7.230414.1210501.tar", last modified: Fri Apr 14 21:05:01 2023, max compression
```

## Comparing `testflows.uexpect-1.7.220902.1112725.tar` & `testflows.uexpect-1.7.230414.1210501.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-02 11:27:25.460822 testflows.uexpect-1.7.220902.1112725/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2020-09-12 20:32:26.000000 testflows.uexpect-1.7.220902.1112725/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       16 2020-09-12 20:32:26.000000 testflows.uexpect-1.7.220902.1112725/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     1513 2022-09-02 11:27:25.460822 testflows.uexpect-1.7.220902.1112725/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      656 2020-09-12 20:32:26.000000 testflows.uexpect-1.7.220902.1112725/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-09-02 11:27:25.460822 testflows.uexpect-1.7.220902.1112725/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1542 2022-09-02 11:27:25.000000 testflows.uexpect-1.7.220902.1112725/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-02 11:27:25.459822 testflows.uexpect-1.7.220902.1112725/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-02 11:27:25.460822 testflows.uexpect-1.7.220902.1112725/testflows/uexpect/
--rw-rw-r--   0 user      (1000) user      (1000)     1447 2022-09-02 11:27:25.000000 testflows.uexpect-1.7.220902.1112725/testflows/uexpect/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9028 2022-09-02 11:24:56.000000 testflows.uexpect-1.7.220902.1112725/testflows/uexpect/uexpect.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-02 11:27:25.460822 testflows.uexpect-1.7.220902.1112725/testflows.uexpect.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1513 2022-09-02 11:27:25.000000 testflows.uexpect-1.7.220902.1112725/testflows.uexpect.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      341 2022-09-02 11:27:25.000000 testflows.uexpect-1.7.220902.1112725/testflows.uexpect.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-02 11:27:25.000000 testflows.uexpect-1.7.220902.1112725/testflows.uexpect.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2020-09-19 15:05:46.000000 testflows.uexpect-1.7.220902.1112725/testflows.uexpect.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       27 2022-09-02 11:27:25.000000 testflows.uexpect-1.7.220902.1112725/testflows.uexpect.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2022-09-02 11:27:25.000000 testflows.uexpect-1.7.220902.1112725/testflows.uexpect.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:05:01.789231 testflows.uexpect-1.7.230414.1210501/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-03-13 20:06:30.000000 testflows.uexpect-1.7.230414.1210501/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2023-03-13 20:06:30.000000 testflows.uexpect-1.7.230414.1210501/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     1096 2023-04-14 21:05:01.789231 testflows.uexpect-1.7.230414.1210501/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      536 2023-03-13 20:06:32.000000 testflows.uexpect-1.7.230414.1210501/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-14 21:05:01.789231 testflows.uexpect-1.7.230414.1210501/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1542 2023-04-14 21:05:01.000000 testflows.uexpect-1.7.230414.1210501/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:05:01.789231 testflows.uexpect-1.7.230414.1210501/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:05:01.789231 testflows.uexpect-1.7.230414.1210501/testflows/uexpect/
+-rw-rw-r--   0 user      (1000) user      (1000)     1447 2023-04-14 21:05:01.000000 testflows.uexpect-1.7.230414.1210501/testflows/uexpect/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9185 2023-04-14 21:04:34.000000 testflows.uexpect-1.7.230414.1210501/testflows/uexpect/uexpect.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:05:01.789231 testflows.uexpect-1.7.230414.1210501/testflows.uexpect.egg-info/
+-rwxrwxr-x   0 user      (1000) user      (1000)     1096 2023-04-14 21:05:01.000000 testflows.uexpect-1.7.230414.1210501/testflows.uexpect.egg-info/PKG-INFO
+-rwxrwxr-x   0 user      (1000) user      (1000)      356 2023-04-14 21:05:01.000000 testflows.uexpect-1.7.230414.1210501/testflows.uexpect.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)        1 2023-04-14 21:05:01.000000 testflows.uexpect-1.7.230414.1210501/testflows.uexpect.egg-info/dependency_links.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)        1 2022-12-23 06:55:08.000000 testflows.uexpect-1.7.230414.1210501/testflows.uexpect.egg-info/not-zip-safe
+-rwxrwxr-x   0 user      (1000) user      (1000)       27 2023-04-14 21:05:01.000000 testflows.uexpect-1.7.230414.1210501/testflows.uexpect.egg-info/requires.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)       10 2023-04-14 21:05:01.000000 testflows.uexpect-1.7.230414.1210501/testflows.uexpect.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-14 21:05:01.789231 testflows.uexpect-1.7.230414.1210501/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     1921 2023-03-13 20:06:30.000000 testflows.uexpect-1.7.230414.1210501/tests/tests.py
```

### Comparing `testflows.uexpect-1.7.220902.1112725/LICENSE` & `testflows.uexpect-1.7.230414.1210501/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.uexpect-1.7.220902.1112725/setup.py` & `testflows.uexpect-1.7.230414.1210501/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name="testflows.uexpect",
-    version="1.7.220902.1112725",
+    version="1.7.230414.1210501",
     description="TestFlows - uExpect",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     url="https://github.com/testflows/testflows-uexpect",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `testflows.uexpect-1.7.220902.1112725/testflows/uexpect/__init__.py` & `testflows.uexpect-1.7.230414.1210501/testflows/uexpect/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.7.220902.1112725"
+__version__ = "1.7.230414.1210501"
 __license__ = f"""
 Copyright 2019 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.uexpect-1.7.220902.1112725/testflows/uexpect/uexpect.py` & `testflows.uexpect-1.7.230414.1210501/testflows/uexpect/uexpect.py`

 * *Files 4% similar despite different names*

```diff
@@ -261,17 +261,23 @@
             queue.put(e)
             if kill_event.is_set():
                 return
             raise
 
 
 def spawn(command):
+    new_env = os.environ.copy()
+    if "PS1" in new_env:
+        del new_env["PS1"]
+    if "PS2" in new_env:
+        del new_env["PS2"]
     master, slave = pty.openpty()
     process = Popen(
         command,
+        env=new_env,
         preexec_fn=os.setsid,
         stdout=slave,
         close_fds=False,
         stdin=slave,
         stderr=slave,
         bufsize=0,
     )
```

