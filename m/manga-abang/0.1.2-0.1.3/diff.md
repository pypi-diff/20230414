# Comparing `tmp/manga-abang-0.1.2.tar.gz` & `tmp/manga-abang-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manga-abang-0.1.2.tar", last modified: Fri Apr 14 09:06:34 2023, max compression
+gzip compressed data, was "manga-abang-0.1.3.tar", last modified: Fri Apr 14 09:07:54 2023, max compression
```

## Comparing `manga-abang-0.1.2.tar` & `manga-abang-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tanyihan   (501) staff       (20)        0 2023-04-14 09:06:34.273197 manga-abang-0.1.2/
--rw-r--r--   0 tanyihan   (501) staff       (20)    11357 2023-01-05 01:34:27.000000 manga-abang-0.1.2/LICENSE
--rw-r--r--   0 tanyihan   (501) staff       (20)       27 2023-01-05 01:34:27.000000 manga-abang-0.1.2/MANIFEST.in
--rw-r--r--   0 tanyihan   (501) staff       (20)     1693 2023-04-14 09:06:34.273066 manga-abang-0.1.2/PKG-INFO
--rw-r--r--   0 tanyihan   (501) staff       (20)     6508 2023-04-14 09:04:51.000000 manga-abang-0.1.2/README.md
-drwxr-xr-x   0 tanyihan   (501) staff       (20)        0 2023-04-14 09:06:34.260579 manga-abang-0.1.2/assets/
--rw-r--r--   0 tanyihan   (501) staff       (20)    56623 2023-01-05 01:34:27.000000 manga-abang-0.1.2/assets/example.jpg
-drwxr-xr-x   0 tanyihan   (501) staff       (20)        0 2023-04-14 09:06:34.262982 manga-abang-0.1.2/manga_abang/
--rw-r--r--   0 tanyihan   (501) staff       (20)       60 2023-04-14 08:56:35.000000 manga-abang-0.1.2/manga_abang/__init__.py
--rw-r--r--   0 tanyihan   (501) staff       (20)      118 2023-04-14 08:56:35.000000 manga-abang-0.1.2/manga_abang/__main__.py
--rw-r--r--   0 tanyihan   (501) staff       (20)     2103 2023-01-05 02:08:03.000000 manga-abang-0.1.2/manga_abang/ocr.py
--rw-r--r--   0 tanyihan   (501) staff       (20)     5214 2023-04-14 09:04:52.000000 manga-abang-0.1.2/manga_abang/run.py
-drwxr-xr-x   0 tanyihan   (501) staff       (20)        0 2023-04-14 09:06:34.272782 manga-abang-0.1.2/manga_abang.egg-info/
--rw-r--r--   0 tanyihan   (501) staff       (20)     1693 2023-04-14 09:06:34.000000 manga-abang-0.1.2/manga_abang.egg-info/PKG-INFO
--rw-r--r--   0 tanyihan   (501) staff       (20)      355 2023-04-14 09:06:34.000000 manga-abang-0.1.2/manga_abang.egg-info/SOURCES.txt
--rw-r--r--   0 tanyihan   (501) staff       (20)        1 2023-04-14 09:06:34.000000 manga-abang-0.1.2/manga_abang.egg-info/dependency_links.txt
--rw-r--r--   0 tanyihan   (501) staff       (20)       58 2023-04-14 09:06:34.000000 manga-abang-0.1.2/manga_abang.egg-info/entry_points.txt
--rw-r--r--   0 tanyihan   (501) staff       (20)      117 2023-04-14 09:06:34.000000 manga-abang-0.1.2/manga_abang.egg-info/requires.txt
--rw-r--r--   0 tanyihan   (501) staff       (20)       12 2023-04-14 09:06:34.000000 manga-abang-0.1.2/manga_abang.egg-info/top_level.txt
--rw-r--r--   0 tanyihan   (501) staff       (20)       38 2023-04-14 09:06:34.273248 manga-abang-0.1.2/setup.cfg
--rw-r--r--   0 tanyihan   (501) staff       (20)     1321 2023-04-14 09:05:51.000000 manga-abang-0.1.2/setup.py
+drwxr-xr-x   0 tanyihan   (501) staff       (20)        0 2023-04-14 09:07:54.527781 manga-abang-0.1.3/
+-rw-r--r--   0 tanyihan   (501) staff       (20)    11357 2023-01-05 01:34:27.000000 manga-abang-0.1.3/LICENSE
+-rw-r--r--   0 tanyihan   (501) staff       (20)       27 2023-01-05 01:34:27.000000 manga-abang-0.1.3/MANIFEST.in
+-rw-r--r--   0 tanyihan   (501) staff       (20)     1693 2023-04-14 09:07:54.527648 manga-abang-0.1.3/PKG-INFO
+-rw-r--r--   0 tanyihan   (501) staff       (20)     6508 2023-04-14 09:04:51.000000 manga-abang-0.1.3/README.md
+drwxr-xr-x   0 tanyihan   (501) staff       (20)        0 2023-04-14 09:07:54.519745 manga-abang-0.1.3/assets/
+-rw-r--r--   0 tanyihan   (501) staff       (20)    56623 2023-01-05 01:34:27.000000 manga-abang-0.1.3/assets/example.jpg
+drwxr-xr-x   0 tanyihan   (501) staff       (20)        0 2023-04-14 09:07:54.521655 manga-abang-0.1.3/manga_abang/
+-rw-r--r--   0 tanyihan   (501) staff       (20)       60 2023-04-14 08:56:35.000000 manga-abang-0.1.3/manga_abang/__init__.py
+-rw-r--r--   0 tanyihan   (501) staff       (20)      118 2023-04-14 08:56:35.000000 manga-abang-0.1.3/manga_abang/__main__.py
+-rw-r--r--   0 tanyihan   (501) staff       (20)     2103 2023-01-05 02:08:03.000000 manga-abang-0.1.3/manga_abang/ocr.py
+-rw-r--r--   0 tanyihan   (501) staff       (20)     5214 2023-04-14 09:04:52.000000 manga-abang-0.1.3/manga_abang/run.py
+drwxr-xr-x   0 tanyihan   (501) staff       (20)        0 2023-04-14 09:07:54.527433 manga-abang-0.1.3/manga_abang.egg-info/
+-rw-r--r--   0 tanyihan   (501) staff       (20)     1693 2023-04-14 09:07:54.000000 manga-abang-0.1.3/manga_abang.egg-info/PKG-INFO
+-rw-r--r--   0 tanyihan   (501) staff       (20)      355 2023-04-14 09:07:54.000000 manga-abang-0.1.3/manga_abang.egg-info/SOURCES.txt
+-rw-r--r--   0 tanyihan   (501) staff       (20)        1 2023-04-14 09:07:54.000000 manga-abang-0.1.3/manga_abang.egg-info/dependency_links.txt
+-rw-r--r--   0 tanyihan   (501) staff       (20)       58 2023-04-14 09:07:54.000000 manga-abang-0.1.3/manga_abang.egg-info/entry_points.txt
+-rw-r--r--   0 tanyihan   (501) staff       (20)      117 2023-04-14 09:07:54.000000 manga-abang-0.1.3/manga_abang.egg-info/requires.txt
+-rw-r--r--   0 tanyihan   (501) staff       (20)       12 2023-04-14 09:07:54.000000 manga-abang-0.1.3/manga_abang.egg-info/top_level.txt
+-rw-r--r--   0 tanyihan   (501) staff       (20)       38 2023-04-14 09:07:54.527820 manga-abang-0.1.3/setup.cfg
+-rw-r--r--   0 tanyihan   (501) staff       (20)     1321 2023-04-14 09:07:51.000000 manga-abang-0.1.3/setup.py
```

### Comparing `manga-abang-0.1.2/LICENSE` & `manga-abang-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manga-abang-0.1.2/PKG-INFO` & `manga-abang-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga-abang
-Version: 0.1.2
+Version: 0.1.3
 Summary: OCR for Japanese manga
 Home-page: https://github.com/AbangTanYiHan/manga_abang
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `manga-abang-0.1.2/README.md` & `manga-abang-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `manga-abang-0.1.2/assets/example.jpg` & `manga-abang-0.1.3/assets/example.jpg`

 * *Files identical despite different names*

### Comparing `manga-abang-0.1.2/manga_abang/ocr.py` & `manga-abang-0.1.3/manga_abang/ocr.py`

 * *Files identical despite different names*

### Comparing `manga-abang-0.1.2/manga_abang/run.py` & `manga-abang-0.1.3/manga_abang/run.py`

 * *Files identical despite different names*

### Comparing `manga-abang-0.1.2/manga_abang.egg-info/PKG-INFO` & `manga-abang-0.1.3/manga_abang.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manga-abang
-Version: 0.1.2
+Version: 0.1.3
 Summary: OCR for Japanese manga
 Home-page: https://github.com/AbangTanYiHan/manga_abang
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `manga-abang-0.1.2/setup.py` & `manga-abang-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 '''
 Author: AbangTan tan_yihan@housei-inc.com
 Date: 2023-01-05 10:34:27
 LastEditors: AbangTan tan_yihan@housei-inc.com
-LastEditTime: 2023-04-14 18:05:51
+LastEditTime: 2023-04-14 18:07:51
 FilePath: /manga-ocr/setup.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 from pathlib import Path
 from setuptools import setup
 
 long_description = (Path(__file__).parent / "README.md").read_text('utf-8').split('# Installation')[0]
 
 setup(
     name="manga-abang",
-    version='0.1.2',
+    version='0.1.3',
     description="OCR for Japanese manga",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AbangTanYiHan/manga_abang",
     license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
```

