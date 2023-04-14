# Comparing `tmp/turbo_docs-0.6.0.tar.gz` & `tmp/turbo_docs-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-0.6.0.tar", last modified: Wed Apr 12 02:00:08 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.6.1.tar", last modified: Fri Apr 14 15:15:06 2023, max compression
```

## Comparing `turbo_docs-0.6.0.tar` & `turbo_docs-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 02:00:08.139047 turbo_docs-0.6.0/
--rw-rw-rw-   0        0        0      520 2023-04-12 02:00:08.138047 turbo_docs-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     1213 2023-04-12 01:09:37.000000 turbo_docs-0.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-12 02:00:08.140047 turbo_docs-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-04-12 02:00:02.000000 turbo_docs-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:00:08.118048 turbo_docs-0.6.0/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.0/turbo_docs/__init__.py
--rw-rw-rw-   0        0        0     3456 2023-04-12 01:08:34.000000 turbo_docs-0.6.0/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:00:08.136051 turbo_docs-0.6.0/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.0/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      893 2023-04-12 00:51:47.000000 turbo_docs-0.6.0/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1794 2023-04-11 19:29:42.000000 turbo_docs-0.6.0/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      566 2023-04-10 22:51:04.000000 turbo_docs-0.6.0/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-12 02:00:08.129049 turbo_docs-0.6.0/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0      520 2023-04-12 02:00:07.000000 turbo_docs-0.6.0/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-04-12 02:00:08.000000 turbo_docs-0.6.0/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 02:00:07.000000 turbo_docs-0.6.0/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-12 02:00:07.000000 turbo_docs-0.6.0/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-04-12 02:00:07.000000 turbo_docs-0.6.0/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-12 02:00:08.000000 turbo_docs-0.6.0/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 15:15:06.422832 turbo_docs-0.6.1/
+-rw-rw-rw-   0        0        0     1483 2023-04-14 15:15:06.420823 turbo_docs-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1027 2023-04-14 15:13:09.000000 turbo_docs-0.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 15:15:06.422832 turbo_docs-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-04-14 15:03:54.000000 turbo_docs-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:15:06.401833 turbo_docs-0.6.1/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.1/turbo_docs/__init__.py
+-rw-rw-rw-   0        0        0     3474 2023-04-14 14:56:25.000000 turbo_docs-0.6.1/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:15:06.418828 turbo_docs-0.6.1/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.6.1/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      893 2023-04-12 00:51:47.000000 turbo_docs-0.6.1/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1794 2023-04-11 19:29:42.000000 turbo_docs-0.6.1/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      687 2023-04-14 14:45:03.000000 turbo_docs-0.6.1/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-14 15:15:06.412826 turbo_docs-0.6.1/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     1483 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-14 15:15:06.000000 turbo_docs-0.6.1/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.6.0/setup.py` & `turbo_docs-0.6.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="turbo_docs",
-    version="0.6.0",
+    version="0.6.1",
     packages=find_packages(),
     install_requires=[
         "requests",
         "openai",
         "click",
         "pyperclip",
     ],
@@ -21,8 +21,9 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
+    long_description=open("README.md", encoding="utf-8").read()
 )
```

### Comparing `turbo_docs-0.6.0/turbo_docs/generate.py` & `turbo_docs-0.6.1/turbo_docs/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def run_create_readme_plus(files):
     """ Generate a README.md file with summarized code content from the provided files.
     """
     responses = {}
     for file_path, file_content in files.items():
         if os.stat(file_path).st_size and file_path.split(".")[1]:
             print(f"(--create_readme_plus) Summarizing {file_path}")
-            prompt = f"Summarize the following code, especially maintaining key logic:\n{file_content}"
+            prompt = f"Create a README summarizing the following code, especially maintaining key logic:\n{file_content}"
             responses[file_path] = openai_api.gpt_completion_wrapper(prompt)
 
     psuedocode = "\n\n\n".join([f"{file_path}:\n{summary}" for file_path, summary in responses.items()])
     run_create_readme(psuedocode)
     print(f"(--create_readme_plus) Generated README.md")
```

### Comparing `turbo_docs-0.6.0/turbo_docs/utils/cli_options.py` & `turbo_docs-0.6.1/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.0/turbo_docs/utils/directory.py` & `turbo_docs-0.6.1/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.6.0/turbo_docs/utils/openai_api.py` & `turbo_docs-0.6.1/turbo_docs/utils/openai_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import json
 import os
-import openai
 
-openai.api_key = os.environ.get('OPENAI_API_KEY')
-if not openai.api_key:
-    raise ValueError("Cannot find API key. Run the following command: export OPENAI_API_KEY=<your_api_key>")
+
+def openai_init():
+    """
+    """
+    import openai
+    openai.api_key = os.environ.get('OPENAI_API_KEY')
+
+    if not openai.api_key:
+        raise ValueError("Cannot find API key. Run the following command: export OPENAI_API_KEY=<your_api_key>")
+    return openai
 
 
 def gpt_completion_wrapper(prompt):
     """ Send a prompt to the OpenAI GPT-3 API and receive a completion.
     """
-    completions = openai.Completion.create(
+    openai_package = openai_init()
+    completions = openai_package.Completion.create(
         engine="text-davinci-003",
         prompt=prompt,
         max_tokens=2048,
         n=1,
         stop=None,
     )
     return completions.choices[0]['text']
```

