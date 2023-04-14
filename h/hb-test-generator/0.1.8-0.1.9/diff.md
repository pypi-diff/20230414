# Comparing `tmp/hb-test-generator-0.1.8.tar.gz` & `tmp/hb-test-generator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hb-test-generator-0.1.8.tar", last modified: Fri Apr 14 11:47:34 2023, max compression
+gzip compressed data, was "hb-test-generator-0.1.9.tar", last modified: Fri Apr 14 11:53:57 2023, max compression
```

## Comparing `hb-test-generator-0.1.8.tar` & `hb-test-generator-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)     1299 2023-04-14 11:21:55.000000 hb-test-generator-0.1.8/README.md
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/hb_test_generator/
--rw-r--r--   0 atei      (1000) atei      (1000)     2505 2023-04-14 11:46:14.000000 hb-test-generator-0.1.8/hb_test_generator/generate_tests.py
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/hb_test_generator.egg-info/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/SOURCES.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/dependency_links.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       77 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/entry_points.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/requires.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/top_level.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/setup.cfg
--rw-r--r--   0 atei      (1000) atei      (1000)      993 2023-04-14 11:46:26.000000 hb-test-generator-0.1.8/setup.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:53:57.504617 hb-test-generator-0.1.9/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:53:57.504617 hb-test-generator-0.1.9/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)     1389 2023-04-14 11:53:38.000000 hb-test-generator-0.1.9/README.md
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:53:57.504617 hb-test-generator-0.1.9/hb_test_generator/
+-rw-r--r--   0 atei      (1000) atei      (1000)     2505 2023-04-14 11:53:38.000000 hb-test-generator-0.1.9/hb_test_generator/generate_tests.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:53:57.504617 hb-test-generator-0.1.9/hb_test_generator.egg-info/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:53:57.000000 hb-test-generator-0.1.9/hb_test_generator.egg-info/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:53:57.000000 hb-test-generator-0.1.9/hb_test_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:53:57.000000 hb-test-generator-0.1.9/hb_test_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)      239 2023-04-14 11:53:57.000000 hb-test-generator-0.1.9/hb_test_generator.egg-info/entry_points.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:53:57.000000 hb-test-generator-0.1.9/hb_test_generator.egg-info/requires.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:53:57.000000 hb-test-generator-0.1.9/hb_test_generator.egg-info/top_level.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:53:57.504617 hb-test-generator-0.1.9/setup.cfg
+-rw-r--r--   0 atei      (1000) atei      (1000)     1194 2023-04-14 11:53:38.000000 hb-test-generator-0.1.9/setup.py
```

### Comparing `hb-test-generator-0.1.8/PKG-INFO` & `hb-test-generator-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.8/README.md` & `hb-test-generator-0.1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 2. Set the `OPENAI_API_KEY` environment variable with your OpenAI API key
 
 ## Usage examples
 
 - `hb-generate-tests app/helpers/membership_helper.rb` will create a `spec/helpers/membership_helper_spec.rb`.
 - `hb-generate-tests src/components/MyComponent.vue` will create a `tests/components/MyComponent.spec.js`. 
 
+### Variants
+- `hb-generate-tests`
+- `hb-generate-test`
+- `hb-gen-tests`
+- `hb-gen-test`
+
 ### Prompt
 Create a `test_generator_prompt.txt` file containing the base prompt. Default prompt is:
 
 ```text
 Write tests for below code. Name and place it according to best practices.
 ```
```

### Comparing `hb-test-generator-0.1.8/hb_test_generator/generate_tests.py` & `hb-test-generator-0.1.9/hb_test_generator/generate_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     with open(test_file_path, "w") as test_file:
         test_file.write(test_code)
 
     return os.path.relpath(test_file_path, Path.cwd())
 
 def main():
     if len(sys.argv) < 2:
-        print("Usage: hb_generate_tests <file_path>")
+        print("Usage: hb-generate-tests <file_path>")
         sys.exit(1)
 
     file_path = sys.argv[1]
 
     prompt_file = get_prompt_file()
     base_prompt = read_file(prompt_file).strip()
```

### Comparing `hb-test-generator-0.1.8/hb_test_generator.egg-info/PKG-INFO` & `hb-test-generator-0.1.9/hb_test_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.8/setup.py` & `hb-test-generator-0.1.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup
 
 setup(
     name="hb-test-generator",
-    version="0.1.8",
+    version="0.1.9",
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
             "hb-generate-tests=hb_test_generator.generate_tests:main",
+            "hb-generate-test=hb_test_generator.generate_tests:main",
+            "hb-gen-tests=hb_test_generator.generate_tests:main",
+            "hb-gen-test=hb_test_generator.generate_tests:main",
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

