# Comparing `tmp/turbo_docs-0.6.1.tar.gz` & `tmp/turbo_docs-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.6.1.tar", last modified: Fri Apr 14 15:15:06 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.6.2.tar", last modified: Fri Apr 14 16:56:06 2023, max compression
```

## Comparing `turbo_docs-0.6.1.tar` & `turbo_docs-0.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:15:06.422832 turbo_docs-0.6.1/
--rw-rw-rw-   0        0        0     1483 2023-04-14 15:15:06.420823 turbo_docs-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     1027 2023-04-14 15:13:09.000000 turbo_docs-0.6.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-14 15:15:06.422832 turbo_docs-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-04-14 15:03:54.000000 turbo_docs-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:15:06.401833 turbo_docs-0.6.1/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.1/turbo_docs/__init__.py
--rw-rw-rw-   0        0        0     3474 2023-04-14 14:56:25.000000 turbo_docs-0.6.1/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:15:06.418828 turbo_docs-0.6.1/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.1/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      893 2023-04-12 00:51:47.000000 turbo_docs-0.6.1/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1794 2023-04-11 19:29:42.000000 turbo_docs-0.6.1/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      687 2023-04-14 14:45:03.000000 turbo_docs-0.6.1/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:15:06.412826 turbo_docs-0.6.1/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     1483 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 16:56:06.139620 turbo_docs-0.6.2/
+-rw-rw-rw-   0        0        0     1483 2023-04-14 16:56:06.137857 turbo_docs-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1027 2023-04-14 16:55:11.000000 turbo_docs-0.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 16:56:06.139620 turbo_docs-0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-04-14 16:55:45.000000 turbo_docs-0.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:56:06.117796 turbo_docs-0.6.2/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.2/turbo_docs/__init__.py
+-rw-rw-rw-   0        0        0     3656 2023-04-14 16:49:36.000000 turbo_docs-0.6.2/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:56:06.135848 turbo_docs-0.6.2/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.2/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-12 00:51:47.000000 turbo_docs-0.6.2/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1794 2023-04-11 19:29:42.000000 turbo_docs-0.6.2/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      687 2023-04-14 14:45:03.000000 turbo_docs-0.6.2/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:56:06.129340 turbo_docs-0.6.2/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     1483 2023-04-14 16:56:06.000000 turbo_docs-0.6.2/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-14 16:56:06.000000 turbo_docs-0.6.2/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:56:06.000000 turbo_docs-0.6.2/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-14 16:56:06.000000 turbo_docs-0.6.2/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-04-14 16:56:06.000000 turbo_docs-0.6.2/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-14 16:56:06.000000 turbo_docs-0.6.2/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.6.1/PKG-INFO` & `turbo_docs-0.6.2/turbo_docs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: turbo_docs
-Version: 0.6.1
+Name: turbo-docs
+Version: 0.6.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `turbo_docs-0.6.1/README.md` & `turbo_docs-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.1/setup.py` & `turbo_docs-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="turbo_docs",
-    version="0.6.1",
+    version="0.6.2",
     packages=find_packages(),
     install_requires=[
         "requests",
         "openai",
         "click",
         "pyperclip",
     ],
```

### Comparing `turbo_docs-0.6.1/turbo_docs/generate.py` & `turbo_docs-0.6.2/turbo_docs/generate.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,33 +4,41 @@
 import pyperclip
 from turbo_docs.utils import directory, openai_api, cli_options
 
 
 def run_create_readme(text):
     """ Generate a formatted and user-friendly README.md file using the provided text.
     """
+    readme = "README.md"
     prompt = f"Create a formatted & user-friendly readme.md from the following:\n\n{text}"
     response = openai_api.gpt_completion_wrapper(prompt)
-    with open("README.md", "w") as readme_file:
-        readme_file.write(response)
+    try:
+        with open(readme, "w") as readme_file:
+            readme_file.write(response)
+    except PermissionError:
+        os.remove(readme)
+        with open(readme, "w") as readme_file:
+            readme_file.write(response)
     print(f"(--create_readme) Generated README.md")
 
 
+
+
 def run_create_readme_plus(files):
     """ Generate a README.md file with summarized code content from the provided files.
     """
     responses = {}
     for file_path, file_content in files.items():
         if os.stat(file_path).st_size and file_path.split(".")[1]:
             print(f"(--create_readme_plus) Summarizing {file_path}")
             prompt = f"Create a README summarizing the following code, especially maintaining key logic:\n{file_content}"
             responses[file_path] = openai_api.gpt_completion_wrapper(prompt)
 
-    psuedocode = "\n\n\n".join([f"{file_path}:\n{summary}" for file_path, summary in responses.items()])
-    run_create_readme(psuedocode)
+    flatmap = "\n\n\n".join([f"{file_path}:\n{summary}" for file_path, summary in responses.items()])
+    run_create_readme(flatmap)
     print(f"(--create_readme_plus) Generated README.md")
 
 
 def run_create_tests(test_file_path, file_content):
     """ Generate unit tests for the provided code file content and save them in a test file.
     """
     print(f"(--create_tests) Generating unit tests for {test_file_path}")
```

### Comparing `turbo_docs-0.6.1/turbo_docs/utils/cli_options.py` & `turbo_docs-0.6.2/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.1/turbo_docs/utils/directory.py` & `turbo_docs-0.6.2/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.1/turbo_docs/utils/openai_api.py` & `turbo_docs-0.6.2/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.1/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-0.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: turbo-docs
-Version: 0.6.1
+Name: turbo_docs
+Version: 0.6.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

