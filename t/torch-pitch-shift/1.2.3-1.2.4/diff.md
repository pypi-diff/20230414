# Comparing `tmp/torch_pitch_shift-1.2.3.tar.gz` & `tmp/torch_pitch_shift-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_pitch_shift-1.2.3.tar", last modified: Wed Mar 29 19:29:26 2023, max compression
+gzip compressed data, was "torch_pitch_shift-1.2.4.tar", last modified: Thu Apr 13 23:00:34 2023, max compression
```

## Comparing `torch_pitch_shift-1.2.3.tar` & `torch_pitch_shift-1.2.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:29:26.042914 torch_pitch_shift-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-29 19:29:08.000000 torch_pitch_shift-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-29 19:29:08.000000 torch_pitch_shift-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-29 19:29:26.042914 torch_pitch_shift-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-29 19:29:08.000000 torch_pitch_shift-1.2.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 19:29:26.042914 torch_pitch_shift-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-03-29 19:29:08.000000 torch_pitch_shift-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:29:26.042914 torch_pitch_shift-1.2.3/torch_pitch_shift/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-29 19:29:08.000000 torch_pitch_shift-1.2.3/torch_pitch_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-03-29 19:29:08.000000 torch_pitch_shift-1.2.3/torch_pitch_shift/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 19:29:26.042914 torch_pitch_shift-1.2.3/torch_pitch_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-29 19:29:25.000000 torch_pitch_shift-1.2.3/torch_pitch_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-29 19:29:26.000000 torch_pitch_shift-1.2.3/torch_pitch_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 19:29:25.000000 torch_pitch_shift-1.2.3/torch_pitch_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-29 19:29:25.000000 torch_pitch_shift-1.2.3/torch_pitch_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-29 19:29:25.000000 torch_pitch_shift-1.2.3/torch_pitch_shift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:00:34.761875 torch_pitch_shift-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 23:00:22.000000 torch_pitch_shift-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-13 23:00:22.000000 torch_pitch_shift-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 23:00:34.761875 torch_pitch_shift-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-13 23:00:22.000000 torch_pitch_shift-1.2.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 23:00:22.000000 torch_pitch_shift-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 23:00:34.761875 torch_pitch_shift-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-13 23:00:22.000000 torch_pitch_shift-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:00:34.761875 torch_pitch_shift-1.2.4/torch_pitch_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 23:00:22.000000 torch_pitch_shift-1.2.4/torch_pitch_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-04-13 23:00:22.000000 torch_pitch_shift-1.2.4/torch_pitch_shift/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:00:34.761875 torch_pitch_shift-1.2.4/torch_pitch_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-13 23:00:34.000000 torch_pitch_shift-1.2.4/torch_pitch_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-13 23:00:34.000000 torch_pitch_shift-1.2.4/torch_pitch_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:00:34.000000 torch_pitch_shift-1.2.4/torch_pitch_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 23:00:34.000000 torch_pitch_shift-1.2.4/torch_pitch_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 23:00:34.000000 torch_pitch_shift-1.2.4/torch_pitch_shift.egg-info/top_level.txt
```

### Comparing `torch_pitch_shift-1.2.3/LICENSE` & `torch_pitch_shift-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_pitch_shift-1.2.3/PKG-INFO` & `torch_pitch_shift-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_pitch_shift
-Version: 1.2.3
+Version: 1.2.4
 Home-page: https://github.com/KentoNishi/torch-pitch-shift
 Author: KentoNishi
 Author-email: kento24gs@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `torch_pitch_shift-1.2.3/readme.md` & `torch_pitch_shift-1.2.4/readme.md`

 * *Files identical despite different names*

### Comparing `torch_pitch_shift-1.2.3/setup.py` & `torch_pitch_shift-1.2.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 with open("readme.md", "r") as f:
     long_description = f.read()
 
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().split("\n")
 
-versionName = sys.argv[1].replace("refs/tags/v", "")
-del sys.argv[1]
+versionName = "1.2.4"
 
 setuptools.setup(
     name="torch_pitch_shift",
     version=versionName,
     author="KentoNishi",
     author_email="kento24gs@outlook.com",
     description=long_description.split("\n")[1],
```

### Comparing `torch_pitch_shift-1.2.3/torch_pitch_shift/main.py` & `torch_pitch_shift-1.2.4/torch_pitch_shift/main.py`

 * *Files identical despite different names*

### Comparing `torch_pitch_shift-1.2.3/torch_pitch_shift.egg-info/PKG-INFO` & `torch_pitch_shift-1.2.4/torch_pitch_shift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-pitch-shift
-Version: 1.2.3
+Version: 1.2.4
 Home-page: https://github.com/KentoNishi/torch-pitch-shift
 Author: KentoNishi
 Author-email: kento24gs@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

