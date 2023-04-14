# Comparing `tmp/hb-test-generator-0.1.7.tar.gz` & `tmp/hb-test-generator-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hb-test-generator-0.1.7.tar", last modified: Fri Apr 14 11:37:42 2023, max compression
+gzip compressed data, was "hb-test-generator-0.1.8.tar", last modified: Fri Apr 14 11:47:34 2023, max compression
```

## Comparing `hb-test-generator-0.1.7.tar` & `hb-test-generator-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)     1299 2023-04-14 11:21:55.000000 hb-test-generator-0.1.7/README.md
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/hb_test_generator/
--rw-r--r--   0 atei      (1000) atei      (1000)     2492 2023-04-14 11:31:01.000000 hb-test-generator-0.1.7/hb_test_generator/generate_tests.py
-drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/hb_test_generator.egg-info/
--rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/PKG-INFO
--rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/SOURCES.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/dependency_links.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       77 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/entry_points.txt
--rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/requires.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:37:42.000000 hb-test-generator-0.1.7/hb_test_generator.egg-info/top_level.txt
--rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:37:42.384617 hb-test-generator-0.1.7/setup.cfg
--rw-r--r--   0 atei      (1000) atei      (1000)      993 2023-04-14 11:36:34.000000 hb-test-generator-0.1.7/setup.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)     1299 2023-04-14 11:21:55.000000 hb-test-generator-0.1.8/README.md
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/hb_test_generator/
+-rw-r--r--   0 atei      (1000) atei      (1000)     2505 2023-04-14 11:46:14.000000 hb-test-generator-0.1.8/hb_test_generator/generate_tests.py
+drwxr-xr-x   0 atei      (1000) atei      (1000)        0 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/hb_test_generator.egg-info/
+-rw-r--r--   0 atei      (1000) atei      (1000)      750 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/PKG-INFO
+-rw-r--r--   0 atei      (1000) atei      (1000)      302 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        1 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       77 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/entry_points.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)        7 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/requires.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       18 2023-04-14 11:47:34.000000 hb-test-generator-0.1.8/hb_test_generator.egg-info/top_level.txt
+-rw-r--r--   0 atei      (1000) atei      (1000)       38 2023-04-14 11:47:34.814618 hb-test-generator-0.1.8/setup.cfg
+-rw-r--r--   0 atei      (1000) atei      (1000)      993 2023-04-14 11:46:26.000000 hb-test-generator-0.1.8/setup.py
```

### Comparing `hb-test-generator-0.1.7/PKG-INFO` & `hb-test-generator-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.7/README.md` & `hb-test-generator-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hb-test-generator-0.1.7/hb_test_generator/generate_tests.py` & `hb-test-generator-0.1.8/hb_test_generator/generate_tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,17 +41,15 @@
         n=1,
         stop=None,
         temperature=0.5,
     )
 
     return response.choices[0].text.strip()
 
-def get_tests_file_info(file_path):
-    prompt_file = get_prompt_file()
-    base_prompt = read_file(prompt_file).strip()
+def get_tests_file_info(base_prompt, file_path):
     prompt = f"Origin file path is {file_path}. What should be the path and filename of the tests file? Response shouldn't include any text except path and filename of the tests file. If below prompt has any information about tests file, like format/path/name/directory, take it into account: \n\n {base_prompt}."
     return send_to_chatgpt(prompt, "")
 
 def save_tests_to_file(test_code, test_file_path):
     test_file_path = Path(test_file_path)
     test_file_path.parent.mkdir(parents=True, exist_ok=True)
 
@@ -63,18 +61,21 @@
 def main():
     if len(sys.argv) < 2:
         print("Usage: hb_generate_tests <file_path>")
         sys.exit(1)
 
     file_path = sys.argv[1]
 
-    test_file_info = get_tests_file_info(file_path)
-    print(f"Tests will be saved into file: {test_file_info}")
+    prompt_file = get_prompt_file()
+    base_prompt = read_file(prompt_file).strip()
 
     file_content = read_file(file_path)
-    test_code = send_to_chatgpt(file_content)
+    test_file_info = get_tests_file_info(base_prompt, file_path)
+    print(f"Tests will be saved into file: {test_file_info}")
+
+    test_code = send_to_chatgpt(base_prompt, file_content)
     test_file_path = save_tests_to_file(test_code, test_file_info)
 
-    print(f"Tests created: {test_file_path}")
+    print("Done!")
 
 if __name__ == "__main__":
     main()
```

### Comparing `hb-test-generator-0.1.7/hb_test_generator.egg-info/PKG-INFO` & `hb-test-generator-0.1.8/hb_test_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hb-test-generator
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package to generate tests & write it into files using OpenAI's GPT-3
 Home-page: https://github.com/halalbooking/hb_test_generator
 Author: Maksymenkov Eugene
 Author-email: foatei@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hb-test-generator-0.1.7/setup.py` & `hb-test-generator-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="hb-test-generator",
-    version="0.1.7",
+    version="0.1.8",
     description="A package to generate tests & write it into files using OpenAI's GPT-3",
     author="Maksymenkov Eugene",
     author_email="foatei@gmail.com",
     url="https://github.com/halalbooking/hb_test_generator",
     packages=['hb_test_generator'],
     install_requires=[
         "openai",
```

