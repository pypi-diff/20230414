# Comparing `tmp/hb-test-generator-0.1.6.tar.gz` & `tmp/hb-test-generator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hb-test-generator-0.1.6.tar", last modified: Fri Apr 14 11:31:18 2023, max compression
+gzip compressed data, was "hb-test-generator-0.1.7.tar", last modified: Fri Apr 14 11:37:42 2023, max compression
```

## Comparing `hb-test-generator-0.1.6.tar` & `hb-test-generator-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:31:18.154617 hb-test-generator-0.1.6/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:31:18.154617 hb-test-generator-0.1.6/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)     1299 2023-04-14 11:21:55.000000 hb-test-generator-0.1.6/README.md
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:31:18.144617 hb-test-generator-0.1.6/hb_test_generator/
--rw-r--r--   0 atei      (1000) atei      (1000)     2492 2023-04-14 11:31:01.000000 hb-test-generator-0.1.6/hb_test_generator/generate_tests.py
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:31:18.154617 hb-test-generator-0.1.6/hb_test_generator.egg-info/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/SOURCES.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/dependency_links.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       59 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/entry_points.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/requires.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/top_level.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:31:18.154617 hb-test-generator-0.1.6/setup.cfg
--rw-r--r--   0 atei      (1000) atei      (1000)      990 2023-04-14 11:27:10.000000 hb-test-generator-0.1.6/setup.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)     1299 2023-04-14 11:21:55.000000 hb-test-generator-0.1.7/README.md
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/hb_test_generator/
+-rw-r--r--   0 atei      (1000) atei      (1000)     2492 2023-04-14 11:31:01.000000 hb-test-generator-0.1.7/hb_test_generator/generate_tests.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/hb_test_generator.egg-info/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       77 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/entry_points.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/requires.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/top_level.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/setup.cfg
+-rw-r--r--   0 atei      (1000) atei      (1000)      993 2023-04-14 11:36:34.000000 hb-test-generator-0.1.7/setup.py
```

### Comparing `hb-test-generator-0.1.6/PKG-INFO` & `hb-test-generator-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.6/README.md` & `hb-test-generator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hb-test-generator-0.1.6/hb_test_generator/generate_tests.py` & `hb-test-generator-0.1.7/hb_test_generator/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hb-test-generator-0.1.6/hb_test_generator.egg-info/PKG-INFO` & `hb-test-generator-0.1.7/hb_test_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.6/setup.py` & `hb-test-generator-0.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 setup(
     name="hb-test-generator",
-    version="0.1.6",
+    version="0.1.7",
     description="A package to generate tests & write it into files using OpenAI's GPT-3",
     author="Maksymenkov Eugene",
     author_email="foatei@gmail.com",
     url="https://github.com/halalbooking/hb_test_generator",
     packages=['hb_test_generator'],
     install_requires=[
         "openai",
     ],
     entry_points={
         "console_scripts": [
-            "hb-generate-tests=generate_tests:main",
+            "hb-generate-tests=hb_test_generator.generate_tests:main",
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

