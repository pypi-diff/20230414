# Comparing `tmp/arlq-1.0.0.tar.gz` & `tmp/arlq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arlq-1.0.0.tar", last modified: Fri Apr 14 17:07:43 2023, max compression
+gzip compressed data, was "arlq-1.0.1.tar", last modified: Fri Apr 14 17:24:26 2023, max compression
```

## Comparing `arlq-1.0.0.tar` & `arlq-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:07:43.915008 arlq-1.0.0/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-13 14:12:27.000000 arlq-1.0.0/LICENSE
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4902 2023-04-14 17:07:43.915008 arlq-1.0.0/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4215 2023-04-14 16:29:26.000000 arlq-1.0.0/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:07:43.915008 arlq-1.0.0/arlq/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 16:48:02.000000 arlq-1.0.0/arlq/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-14 16:29:26.000000 arlq-1.0.0/arlq/_version.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    17399 2023-04-14 17:06:07.000000 arlq-1.0.0/arlq/arlq.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:07:43.915008 arlq-1.0.0/arlq.egg-info/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4902 2023-04-14 17:07:43.000000 arlq-1.0.0/arlq.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-14 17:07:43.000000 arlq-1.0.0/arlq.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-14 17:07:43.000000 arlq-1.0.0/arlq.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-14 17:07:43.000000 arlq-1.0.0/arlq.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-14 17:07:43.000000 arlq-1.0.0/arlq.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-14 17:07:43.000000 arlq-1.0.0/arlq.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      831 2023-04-14 17:07:43.915008 arlq-1.0.0/setup.cfg
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 16:29:26.000000 arlq-1.0.0/setup.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:24:26.240857 arlq-1.0.1/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1305 2023-04-13 14:12:27.000000 arlq-1.0.1/LICENSE
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-14 17:24:26.240857 arlq-1.0.1/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     4216 2023-04-14 17:16:04.000000 arlq-1.0.1/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:24:26.240857 arlq-1.0.1/arlq/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       57 2023-04-14 17:09:07.000000 arlq-1.0.1/arlq/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       22 2023-04-14 17:17:51.000000 arlq-1.0.1/arlq/_version.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)    17399 2023-04-14 17:09:07.000000 arlq-1.0.1/arlq/arlq.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2023-04-14 17:24:26.240857 arlq-1.0.1/arlq.egg-info/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1046 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       36 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       43 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        5 2023-04-14 17:24:26.000000 arlq-1.0.1/arlq.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      836 2023-04-14 17:24:26.240857 arlq-1.0.1/setup.cfg
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2023-04-14 17:09:07.000000 arlq-1.0.1/setup.py
```

### Comparing `arlq-1.0.0/LICENSE` & `arlq-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arlq-1.0.0/PKG-INFO` & `arlq-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,16 @@
-Metadata-Version: 2.1
-Name: arlq
-Version: 1.0.0
-Summary: ARQL, another rogue-like quest game.
-Home-page: https://github.com/tos-kamiya/arlq
-Author: Toshihiro Kamiya
-Author-email: kamiya@mbj.nifty.com
-License: BSD 2-Clause License
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ARQL, another rogue-like quest game
+# ARLQ, another rogue-like quest game
 
 ARLQ (Another Rogue-Like Quest) game created as an experiment in developing code and manuals with humans and ChatGPT.
 
 * Code was generated by ChatGPT from a rough description of the game content and brushed up by humans working out the details.
   * However, many things were done by ChatGPT besides code generation, such as introducing algorithms (maze generation) and asking how to use the curses library.
   * Type hints are mostly generated by ChatGPT.
   * ChatGPT helped me with some ideas for new monsters.
-* The manual (show below) was intended to be generated by ChatGPT from the description of the code, but was given up halfway through, and the human explanation was finished by ChatGPT.
+* The manual (shown below) was intended to be generated by ChatGPT from the description of the code, but was given up halfway through, and the human explanation was finished by ChatGPT.
   * ChatGPT's contribution was a significant factor in the manual's rather informal tone.
 
 ![](screenshot.png)
 
 ## Game Description
 
 * Game Objective: The goal of this game is to explore a dungeon with different passages each time and find the treasure chest hidden by the dragon!
@@ -70,9 +50,7 @@
 ## License
 
 The license for this code is BSD-2.
 
 However, please note that the way the code generated by AI is treated depends on the laws in the country where you live, regardless of the license chosen by the developer (myself).
 Also, please note that I have not directly copied and pasted any source code other than what ChatGPT has generated.
 
-
-
```

### Comparing `arlq-1.0.0/arlq/arlq.py` & `arlq-1.0.1/arlq/arlq.py`

 * *Files identical despite different names*

### Comparing `arlq-1.0.0/setup.cfg` & `arlq-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = arlq
 version = attr: arlq._version.__version__
 description = ARQL, another rogue-like quest game.
-long_description = file: README.md
+long_description = file: README-pypi.md
 long_description_content_type = text/markdown
 url = https://github.com/tos-kamiya/arlq
 author = Toshihiro Kamiya
 author_email = kamiya@mbj.nifty.com
 license = BSD 2-Clause License
 classifiers = 
 	Programming Language :: Python :: 3.8
```

