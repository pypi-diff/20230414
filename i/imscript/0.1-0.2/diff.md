# Comparing `tmp/imscript-0.1.tar.gz` & `tmp/imscript-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imscript-0.1.tar", last modified: Thu Apr 13 15:53:53 2023, max compression
+gzip compressed data, was "imscript-0.2.tar", last modified: Fri Apr 14 07:26:57 2023, max compression
```

## Comparing `imscript-0.1.tar` & `imscript-0.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-13 15:53:53.422592 imscript-0.1/
--rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-04-13 15:53:53.422592 imscript-0.1/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)       26 2023-04-13 15:15:06.000000 imscript-0.1/README
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-13 15:53:53.418592 imscript-0.1/bin/
--rwxrwxr-x   0 coco      (1000) coco      (1000)   336208 2023-04-13 15:10:57.000000 imscript-0.1/bin/plambda
--rwxrwxr-x   0 coco      (1000) coco      (1000)   242816 2023-04-13 15:10:58.000000 imscript-0.1/bin/qauto
-drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-13 15:53:53.422592 imscript-0.1/imscript.egg-info/
--rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-04-13 15:53:53.000000 imscript-0.1/imscript.egg-info/PKG-INFO
--rw-rw-r--   0 coco      (1000) coco      (1000)      165 2023-04-13 15:53:53.000000 imscript-0.1/imscript.egg-info/SOURCES.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-04-13 15:53:53.000000 imscript-0.1/imscript.egg-info/dependency_links.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-04-13 15:53:53.000000 imscript-0.1/imscript.egg-info/top_level.txt
--rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-04-13 15:53:53.422592 imscript-0.1/setup.cfg
--rw-rw-r--   0 coco      (1000) coco      (1000)      730 2023-04-13 15:47:28.000000 imscript-0.1/setup.py
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-14 07:26:57.825003 imscript-0.2/
+-rw-rw-r--   0 coco      (1000) coco      (1000)       10 2023-04-14 07:25:46.000000 imscript-0.2/MANIFEST.in
+-rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-04-14 07:26:57.825003 imscript-0.2/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)       26 2023-04-13 15:15:06.000000 imscript-0.2/README
+drwxrwxr-x   0 coco      (1000) coco      (1000)        0 2023-04-14 07:26:57.821003 imscript-0.2/imscript.egg-info/
+-rw-rw-r--   0 coco      (1000) coco      (1000)      503 2023-04-14 07:26:57.000000 imscript-0.2/imscript.egg-info/PKG-INFO
+-rw-rw-r--   0 coco      (1000) coco      (1000)      155 2023-04-14 07:26:57.000000 imscript-0.2/imscript.egg-info/SOURCES.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-04-14 07:26:57.000000 imscript-0.2/imscript.egg-info/dependency_links.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)        1 2023-04-14 07:26:57.000000 imscript-0.2/imscript.egg-info/top_level.txt
+-rw-rw-r--   0 coco      (1000) coco      (1000)       38 2023-04-14 07:26:57.825003 imscript-0.2/setup.cfg
+-rw-rw-r--   0 coco      (1000) coco      (1000)      780 2023-04-14 07:25:46.000000 imscript-0.2/setup.py
```

### Comparing `imscript-0.1/setup.py` & `imscript-0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 
 from setuptools.command.install import install
 class myinstall(install):
 	def run(self):
 		import os
-		os.system("make")
+		os.system("mkdir -p bin")
+		os.system("make bin/plambda bin/qauto")
 		install.run(self)
 
 
 import setuptools
 setuptools.setup(
 	name = "imscript",
-	version = "0.1",
+	version = "0.2",
 	author = "Enric Meinhardt-Llopis",
 	author_email = "enric.meinhardt@fastmail.com",
 	description = "Image Processing with Unix Pipes",
 	url = "https://github.com/mnhrdt/imscript",
 	classifiers = [
 		"Operating System :: OS Independent",
 		"License :: OSI Approved :: GNU Affero General Public License v3",
```

