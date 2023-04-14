# Comparing `tmp/sball-0.9.1.tar.gz` & `tmp/sball-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sball-0.9.1.tar", last modified: Fri Apr 14 13:14:44 2023, max compression
+gzip compressed data, was "sball-0.9.2.tar", last modified: Fri Apr 14 13:32:28 2023, max compression
```

## Comparing `sball-0.9.1.tar` & `sball-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 13:14:44.901799 sball-0.9.1/
--rw-rw-rw-   0        0        0      401 2023-04-14 13:14:44.900798 sball-0.9.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 13:14:44.894800 sball-0.9.1/sball.egg-info/
--rw-rw-rw-   0        0        0      401 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-04-14 13:14:44.000000 sball-0.9.1/sball.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 13:14:44.901799 sball-0.9.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 13:14:44.898800 sball-0.9.1/src/
--rw-rw-rw-   0        0        0       14 2023-04-14 12:15:27.000000 sball-0.9.1/src/__init__.py
--rw-rw-rw-   0        0        0     4957 2023-04-14 12:48:14.000000 sball-0.9.1/src/sball.py
--rw-rw-rw-   0        0        0      659 2023-04-14 13:11:12.000000 sball-0.9.1/src/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:32:28.274572 sball-0.9.2/
+-rw-rw-rw-   0        0        0      401 2023-04-14 13:32:28.274572 sball-0.9.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 13:32:28.268574 sball-0.9.2/sball.egg-info/
+-rw-rw-rw-   0        0        0      401 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-04-14 13:32:28.000000 sball-0.9.2/sball.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:32:28.275575 sball-0.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 13:32:28.272571 sball-0.9.2/src/
+-rw-rw-rw-   0        0        0       14 2023-04-14 12:15:27.000000 sball-0.9.2/src/__init__.py
+-rw-rw-rw-   0        0        0     4957 2023-04-14 13:31:43.000000 sball-0.9.2/src/sball.py
+-rw-rw-rw-   0        0        0      659 2023-04-14 13:31:48.000000 sball-0.9.2/src/setup.py
```

### Comparing `sball-0.9.1/src/sball.py` & `sball-0.9.2/src/sball.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 	args = [arg for arg in s[:-1] if not arg.startswith('name=')]
 	name = [arg.split('=')[1] for arg in s[:-1] if arg.startswith('name=')]
 	name = name[0] if name else 'scripts'
 	
 	regex = [arg.split('=')[1] for arg in s[:-1] if arg.startswith('regex=')]
 	regex = regex[0] if regex else []
 	
-	status_dir = [arg.split('=')[1] for arg in [s:-1] if arg.startswith('status-dir=')]
+	status_dir = [arg.split('=')[1] for arg in s[:-1] if arg.startswith('status-dir=')]
 	status_dir = status_dir[0] if status_dir else None
 	
 	globbed = []
 	for script in scripts:
 		globbed.append(glob(script, recursive=True))
 	
 	globbed = [script for l in globbed for script in l if script.endswith('.sh')]
```

### Comparing `sball-0.9.1/src/setup.py` & `sball-0.9.2/src/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="sball",
-    version="0.9.1",
+    version="0.9.2",
     author="michael_a_wilson",
     author_email="michael.a.wilson@yale.edu",
     description=(
         "sball.py: a script to submit job arrays from individual "
         "scripts using Yale CRC's dSQ."
     ),
     url="https://github.com/mawilson1234/sball",
```

