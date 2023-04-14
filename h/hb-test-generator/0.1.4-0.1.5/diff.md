# Comparing `tmp/hb-test-generator-0.1.4.tar.gz` & `tmp/hb-test-generator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hb-test-generator-0.1.4.tar", last modified: Fri Apr 14 11:20:18 2023, max compression
+gzip compressed data, was "hb-test-generator-0.1.5.tar", last modified: Fri Apr 14 11:25:13 2023, max compression
```

## Comparing `hb-test-generator-0.1.4.tar` & `hb-test-generator-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:20:18.514618 hb-test-generator-0.1.4/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:20:18.514618 hb-test-generator-0.1.4/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)     1297 2023-04-14 10:54:19.000000 hb-test-generator-0.1.4/README.md
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:20:18.514618 hb-test-generator-0.1.4/hb_test_generator/
--rw-r--r--   0 atei      (1000) atei      (1000)     2489 2023-04-14 10:15:36.000000 hb-test-generator-0.1.4/hb_test_generator/generate_tests.py
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:20:18.514618 hb-test-generator-0.1.4/hb_test_generator.egg-info/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:20:18.000000 hb-test-generator-0.1.4/hb_test_generator.egg-info/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:20:18.000000 hb-test-generator-0.1.4/hb_test_generator.egg-info/SOURCES.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:20:18.000000 hb-test-generator-0.1.4/hb_test_generator.egg-info/dependency_links.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       77 2023-04-14 11:20:18.000000 hb-test-generator-0.1.4/hb_test_generator.egg-info/entry_points.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:20:18.000000 hb-test-generator-0.1.4/hb_test_generator.egg-info/requires.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:20:18.000000 hb-test-generator-0.1.4/hb_test_generator.egg-info/top_level.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:20:18.514618 hb-test-generator-0.1.4/setup.cfg
--rw-r--r--   0 atei      (1000) atei      (1000)     1008 2023-04-14 11:20:08.000000 hb-test-generator-0.1.4/setup.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)     1299 2023-04-14 11:21:55.000000 hb-test-generator-0.1.5/README.md
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/hb_test_generator/
+-rw-r--r--   0 atei      (1000) atei      (1000)     2489 2023-04-14 10:15:36.000000 hb-test-generator-0.1.5/hb_test_generator/generate_tests.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/hb_test_generator.egg-info/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       59 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/entry_points.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/requires.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/top_level.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/setup.cfg
+-rw-r--r--   0 atei      (1000) atei      (1000)      990 2023-04-14 11:24:51.000000 hb-test-generator-0.1.5/setup.py
```

### Comparing `hb-test-generator-0.1.4/PKG-INFO` & `hb-test-generator-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.4/README.md` & `hb-test-generator-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 1. Run: `pip install hb_test_generator`
 
 2. Set the `OPENAI_API_KEY` environment variable with your OpenAI API key
 
 ## Usage examples
 
-- `hb_generate_test app/helpers/membership_helper.rb` will create a `spec/helpers/membership_helper_spec.rb`.
-- `hb_generate_test src/components/MyComponent.vue` will create a `tests/components/MyComponent.spec.js`. 
+- `hb-generate-tests app/helpers/membership_helper.rb` will create a `spec/helpers/membership_helper_spec.rb`.
+- `hb-generate-tests src/components/MyComponent.vue` will create a `tests/components/MyComponent.spec.js`. 
 
 ### Prompt
 Create a `test_generator_prompt.txt` file containing the base prompt. Default prompt is:
 
 ```text
 Write tests for below code. Name and place it according to best practices.
 ```
```

### Comparing `hb-test-generator-0.1.4/hb_test_generator/generate_tests.py` & `hb-test-generator-0.1.5/hb_test_generator/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hb-test-generator-0.1.4/hb_test_generator.egg-info/PKG-INFO` & `hb-test-generator-0.1.5/hb_test_generator.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.4/setup.py` & `hb-test-generator-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hb-test-generator",
-    version="0.1.4",
+    version="0.1.5",
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

