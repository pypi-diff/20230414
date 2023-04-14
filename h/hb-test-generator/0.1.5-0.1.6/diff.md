# Comparing `tmp/hb-test-generator-0.1.5.tar.gz` & `tmp/hb-test-generator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hb-test-generator-0.1.5.tar", last modified: Fri Apr 14 11:25:13 2023, max compression
+gzip compressed data, was "hb-test-generator-0.1.6.tar", last modified: Fri Apr 14 11:31:18 2023, max compression
```

## Comparing `hb-test-generator-0.1.5.tar` & `hb-test-generator-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)     1299 2023-04-14 11:21:55.000000 hb-test-generator-0.1.5/README.md
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/hb_test_generator/
--rw-r--r--   0 atei      (1000) atei      (1000)     2489 2023-04-14 10:15:36.000000 hb-test-generator-0.1.5/hb_test_generator/generate_tests.py
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/hb_test_generator.egg-info/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/SOURCES.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/dependency_links.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       59 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/entry_points.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/requires.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:25:13.000000 hb-test-generator-0.1.5/hb_test_generator.egg-info/top_level.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:25:13.844618 hb-test-generator-0.1.5/setup.cfg
--rw-r--r--   0 atei      (1000) atei      (1000)      990 2023-04-14 11:24:51.000000 hb-test-generator-0.1.5/setup.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:31:18.154617 hb-test-generator-0.1.6/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:31:18.154617 hb-test-generator-0.1.6/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)     1299 2023-04-14 11:21:55.000000 hb-test-generator-0.1.6/README.md
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:31:18.144617 hb-test-generator-0.1.6/hb_test_generator/
+-rw-r--r--   0 atei      (1000) atei      (1000)     2492 2023-04-14 11:31:01.000000 hb-test-generator-0.1.6/hb_test_generator/generate_tests.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:31:18.154617 hb-test-generator-0.1.6/hb_test_generator.egg-info/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       59 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/entry_points.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/requires.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:31:18.000000 hb-test-generator-0.1.6/hb_test_generator.egg-info/top_level.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:31:18.154617 hb-test-generator-0.1.6/setup.cfg
+-rw-r--r--   0 atei      (1000) atei      (1000)      990 2023-04-14 11:27:10.000000 hb-test-generator-0.1.6/setup.py
```

### Comparing `hb-test-generator-0.1.5/PKG-INFO` & `hb-test-generator-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.5/README.md` & `hb-test-generator-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hb-test-generator-0.1.5/hb_test_generator/generate_tests.py` & `hb-test-generator-0.1.6/hb_test_generator/generate_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     return response.choices[0].text.strip()
 
 def get_tests_file_info(file_path):
     prompt_file = get_prompt_file()
     base_prompt = read_file(prompt_file).strip()
     prompt = f"Origin file path is {file_path}. What should be the path and filename of the tests file? Response shouldn't include any text except path and filename of the tests file. If below prompt has any information about tests file, like format/path/name/directory, take it into account: \n\n {base_prompt}."
-    print(f"Prompt:\n {prompt}\n---\n")
     return send_to_chatgpt(prompt, "")
 
 def save_tests_to_file(test_code, test_file_path):
     test_file_path = Path(test_file_path)
     test_file_path.parent.mkdir(parents=True, exist_ok=True)
 
     with open(test_file_path, "w") as test_file:
@@ -68,13 +67,14 @@
 
     file_path = sys.argv[1]
 
     test_file_info = get_tests_file_info(file_path)
     print(f"Tests will be saved into file: {test_file_info}")
 
     file_content = read_file(file_path)
-    test_file_path = save_tests_to_file(file_content, test_file_info)
+    test_code = send_to_chatgpt(file_content)
+    test_file_path = save_tests_to_file(test_code, test_file_info)
 
     print(f"Tests created: {test_file_path}")
 
 if __name__ == "__main__":
     main()
```

### Comparing `hb-test-generator-0.1.5/hb_test_generator.egg-info/PKG-INFO` & `hb-test-generator-0.1.6/hb_test_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.5/setup.py` & `hb-test-generator-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hb-test-generator",
-    version="0.1.5",
+    version="0.1.6",
     description="A package to generate tests & write it into files using OpenAI's GPT-3",
     author="Maksymenkov Eugene",
     author_email="foatei@gmail.com",
     url="https://github.com/halalbooking/hb_test_generator",
     packages=['hb_test_generator'],
     install_requires=[
         "openai",
```

