# Comparing `tmp/hb-test-generator-0.1.1.tar.gz` & `tmp/hb-test-generator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hb-test-generator-0.1.1.tar", last modified: Fri Apr 14 10:51:43 2023, max compression
+gzip compressed data, was "hb-test-generator-0.1.2.tar", last modified: Fri Apr 14 11:04:55 2023, max compression
```

## Comparing `hb-test-generator-0.1.1.tar` & `hb-test-generator-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 10:51:43.314617 hb-test-generator-0.1.1/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 10:51:43.314617 hb-test-generator-0.1.1/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)     1218 2023-04-14 10:16:53.000000 hb-test-generator-0.1.1/README.md
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 10:51:43.314617 hb-test-generator-0.1.1/hb_test_generator.egg-info/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 10:51:43.000000 hb-test-generator-0.1.1/hb_test_generator.egg-info/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)      266 2023-04-14 10:51:43.000000 hb-test-generator-0.1.1/hb_test_generator.egg-info/SOURCES.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 10:51:43.000000 hb-test-generator-0.1.1/hb_test_generator.egg-info/dependency_links.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       77 2023-04-14 10:51:43.000000 hb-test-generator-0.1.1/hb_test_generator.egg-info/entry_points.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 10:51:43.000000 hb-test-generator-0.1.1/hb_test_generator.egg-info/requires.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 10:51:43.000000 hb-test-generator-0.1.1/hb_test_generator.egg-info/top_level.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 10:51:43.314617 hb-test-generator-0.1.1/setup.cfg
--rw-r--r--   0 atei      (1000) atei      (1000)     1002 2023-04-14 10:51:20.000000 hb-test-generator-0.1.1/setup.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:04:55.084618 hb-test-generator-0.1.2/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:04:55.084618 hb-test-generator-0.1.2/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)     1297 2023-04-14 10:54:19.000000 hb-test-generator-0.1.2/README.md
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:04:55.084618 hb-test-generator-0.1.2/hb_test_generator.egg-info/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:04:55.000000 hb-test-generator-0.1.2/hb_test_generator.egg-info/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)      266 2023-04-14 11:04:55.000000 hb-test-generator-0.1.2/hb_test_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:04:55.000000 hb-test-generator-0.1.2/hb_test_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       59 2023-04-14 11:04:55.000000 hb-test-generator-0.1.2/hb_test_generator.egg-info/entry_points.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:04:55.000000 hb-test-generator-0.1.2/hb_test_generator.egg-info/requires.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:04:55.000000 hb-test-generator-0.1.2/hb_test_generator.egg-info/top_level.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:04:55.084618 hb-test-generator-0.1.2/setup.cfg
+-rw-r--r--   0 atei      (1000) atei      (1000)      984 2023-04-14 11:04:09.000000 hb-test-generator-0.1.2/setup.py
```

### Comparing `hb-test-generator-0.1.1/PKG-INFO` & `hb-test-generator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.1/README.md` & `hb-test-generator-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,7 +32,14 @@
 Write rspec tests for below code. Use factory instead of yml fixtures if needed. Put it into `spec/` dir. Name format `*_spec.rb`.
 ```
 
 #### Example for vue3 + jest:
 ```text
 Write jest tests for below code. Put it into `tests/` dir near `src/` dir. Name format `*.spec.js`.
 ```
+
+
+## Dev commands
+
+`python3 setup.py sdist bdist_wheel`
+
+`twine upload dist/*`
```

### Comparing `hb-test-generator-0.1.1/hb_test_generator.egg-info/PKG-INFO` & `hb-test-generator-0.1.2/hb_test_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.1/setup.py` & `hb-test-generator-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hb-test-generator",
-    version="0.1.1",
+    version="0.1.2",
     description="A package to generate tests & write it into files using OpenAI's GPT-3",
     author="Maksymenkov Eugene",
     author_email="foatei@gmail.com",
     url="https://github.com/halalbooking/hb_test_generator",
     packages=find_packages(),
     install_requires=[
         "openai",
     ],
     entry_points={
         "console_scripts": [
-            "hb-generate-tests=hb_test_generator.generate_tests:main",
+            "hb-generate-tests=generate_tests:main",
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

