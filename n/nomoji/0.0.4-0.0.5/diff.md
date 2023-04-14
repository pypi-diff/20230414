# Comparing `tmp/nomoji-0.0.4.tar.gz` & `tmp/nomoji-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomoji-0.0.4.tar", last modified: Fri Apr 14 01:03:29 2023, max compression
+gzip compressed data, was "nomoji-0.0.5.tar", last modified: Fri Apr 14 01:34:08 2023, max compression
```

## Comparing `nomoji-0.0.4.tar` & `nomoji-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-14 01:03:29.985165 nomoji-0.0.4/
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1799 2023-04-13 13:18:27.000000 nomoji-0.0.4/.gitignore
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1071 2023-04-13 13:18:27.000000 nomoji-0.0.4/LICENSE
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1634 2023-04-14 01:03:29.985258 nomoji-0.0.4/PKG-INFO
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1096 2023-04-14 00:59:37.000000 nomoji-0.0.4/README.md
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-14 01:03:29.983740 nomoji-0.0.4/nomoji/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      547 2023-04-13 13:52:15.000000 nomoji-0.0.4/nomoji/__init__.py
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-14 01:03:29.984535 nomoji-0.0.4/nomoji.egg-info/
--rw-r--r--   0 leriomaggio   (502) staff       (20)     1634 2023-04-14 01:03:29.000000 nomoji-0.0.4/nomoji.egg-info/PKG-INFO
--rw-r--r--   0 leriomaggio   (502) staff       (20)      233 2023-04-14 01:03:29.000000 nomoji-0.0.4/nomoji.egg-info/SOURCES.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)        1 2023-04-14 01:03:29.000000 nomoji-0.0.4/nomoji.egg-info/dependency_links.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)        7 2023-04-14 01:03:29.000000 nomoji-0.0.4/nomoji.egg-info/top_level.txt
--rw-r--r--   0 leriomaggio   (502) staff       (20)       99 2023-04-13 13:44:11.000000 nomoji-0.0.4/pyproject.toml
--rw-r--r--   0 leriomaggio   (502) staff       (20)       34 2023-04-13 13:10:31.000000 nomoji-0.0.4/pytest.ini
--rw-r--r--   0 leriomaggio   (502) staff       (20)      312 2023-04-14 01:03:29.985525 nomoji-0.0.4/setup.cfg
--rw-r--r--   0 leriomaggio   (502) staff       (20)      632 2023-04-14 01:00:33.000000 nomoji-0.0.4/setup.py
-drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-14 01:03:29.984713 nomoji-0.0.4/tests/
--rw-r--r--   0 leriomaggio   (502) staff       (20)      707 2023-04-13 13:52:09.000000 nomoji-0.0.4/tests/test_nomoji.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-14 01:34:08.094187 nomoji-0.0.5/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1799 2023-04-13 13:18:27.000000 nomoji-0.0.5/.gitignore
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1071 2023-04-13 13:18:27.000000 nomoji-0.0.5/LICENSE
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1634 2023-04-14 01:34:08.094297 nomoji-0.0.5/PKG-INFO
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1096 2023-04-14 00:59:37.000000 nomoji-0.0.5/README.md
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-14 01:34:08.092665 nomoji-0.0.5/nomoji/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      867 2023-04-14 01:27:10.000000 nomoji-0.0.5/nomoji/__init__.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-14 01:34:08.093496 nomoji-0.0.5/nomoji.egg-info/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)     1634 2023-04-14 01:34:08.000000 nomoji-0.0.5/nomoji.egg-info/PKG-INFO
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      233 2023-04-14 01:34:08.000000 nomoji-0.0.5/nomoji.egg-info/SOURCES.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)        1 2023-04-14 01:34:08.000000 nomoji-0.0.5/nomoji.egg-info/dependency_links.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)        7 2023-04-14 01:34:08.000000 nomoji-0.0.5/nomoji.egg-info/top_level.txt
+-rw-r--r--   0 leriomaggio   (502) staff       (20)       99 2023-04-13 13:44:11.000000 nomoji-0.0.5/pyproject.toml
+-rw-r--r--   0 leriomaggio   (502) staff       (20)       34 2023-04-13 13:10:31.000000 nomoji-0.0.5/pytest.ini
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      312 2023-04-14 01:34:08.094621 nomoji-0.0.5/setup.cfg
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      632 2023-04-14 01:19:34.000000 nomoji-0.0.5/setup.py
+drwxr-xr-x   0 leriomaggio   (502) staff       (20)        0 2023-04-14 01:34:08.093684 nomoji-0.0.5/tests/
+-rw-r--r--   0 leriomaggio   (502) staff       (20)      707 2023-04-13 13:52:09.000000 nomoji-0.0.5/tests/test_nomoji.py
```

### Comparing `nomoji-0.0.4/.gitignore` & `nomoji-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.4/LICENSE` & `nomoji-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.4/PKG-INFO` & `nomoji-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomoji
-Version: 0.0.4
+Version: 0.0.5
 Summary: Silly Python Package to print digits using emojis
 Home-page: https://github.com/leriomaggio/emoji-numbers/
 Author: Valerio Maggio
 Author-email: vmaggio@anaconda.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `nomoji-0.0.4/README.md` & `nomoji-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nomoji-0.0.4/nomoji.egg-info/PKG-INFO` & `nomoji-0.0.5/nomoji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomoji
-Version: 0.0.4
+Version: 0.0.5
 Summary: Silly Python Package to print digits using emojis
 Home-page: https://github.com/leriomaggio/emoji-numbers/
 Author: Valerio Maggio
 Author-email: vmaggio@anaconda.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `nomoji-0.0.4/setup.py` & `nomoji-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(os.path.join(CURRENT_FOLDER, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="nomoji",
     author="Valerio Maggio",
-    version="0.0.4",
+    version="0.0.5",
     author_email="vmaggio@anaconda.com",
     description="Silly Python Package to print digits using emojis",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/leriomaggio/emoji-numbers/",
     packages=find_packages(exclude=[]),
     include_package_data=True,
```

### Comparing `nomoji-0.0.4/tests/test_nomoji.py` & `nomoji-0.0.5/tests/test_nomoji.py`

 * *Files identical despite different names*

