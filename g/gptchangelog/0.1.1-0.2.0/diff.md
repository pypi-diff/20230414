# Comparing `tmp/gptchangelog-0.1.1.tar.gz` & `tmp/gptchangelog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptchangelog-0.1.1.tar", last modified: Thu Apr 13 16:27:09 2023, max compression
+gzip compressed data, was "gptchangelog-0.2.0.tar", last modified: Fri Apr 14 18:40:34 2023, max compression
```

## Comparing `gptchangelog-0.1.1.tar` & `gptchangelog-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-13 16:27:09.701250 gptchangelog-0.1.1/
--rw-r--r--   0 xjodoin    (501) staff       (20)     1089 2023-04-13 15:28:44.000000 gptchangelog-0.1.1/LICENSE
--rw-r--r--   0 xjodoin    (501) staff       (20)     1861 2023-04-13 16:27:09.700988 gptchangelog-0.1.1/PKG-INFO
--rw-r--r--   0 xjodoin    (501) staff       (20)     1088 2023-04-13 15:56:57.000000 gptchangelog-0.1.1/README.md
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-13 16:27:09.698595 gptchangelog-0.1.1/gptchangelog/
--rw-r--r--   0 xjodoin    (501) staff       (20)     2939 2023-04-13 16:23:08.000000 gptchangelog-0.1.1/gptchangelog/__init__.py
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-13 16:27:09.700601 gptchangelog-0.1.1/gptchangelog.egg-info/
--rw-r--r--   0 xjodoin    (501) staff       (20)     1861 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/PKG-INFO
--rw-r--r--   0 xjodoin    (501) staff       (20)      269 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/SOURCES.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)        1 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/dependency_links.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       52 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/entry_points.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       30 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/requires.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       13 2023-04-13 16:27:09.000000 gptchangelog-0.1.1/gptchangelog.egg-info/top_level.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       38 2023-04-13 16:27:09.701347 gptchangelog-0.1.1/setup.cfg
--rw-r--r--   0 xjodoin    (501) staff       (20)     1173 2023-04-13 16:25:44.000000 gptchangelog-0.1.1/setup.py
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-14 18:40:34.389761 gptchangelog-0.2.0/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1089 2023-04-13 15:28:44.000000 gptchangelog-0.2.0/LICENSE
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1861 2023-04-14 18:40:34.389456 gptchangelog-0.2.0/PKG-INFO
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1088 2023-04-13 15:56:57.000000 gptchangelog-0.2.0/README.md
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-14 18:40:34.385204 gptchangelog-0.2.0/gptchangelog/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     3132 2023-04-14 18:26:04.000000 gptchangelog-0.2.0/gptchangelog/__init__.py
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-14 18:40:34.388493 gptchangelog-0.2.0/gptchangelog/templates/
+-rw-r--r--   0 xjodoin    (501) staff       (20)      317 2023-04-14 18:33:21.000000 gptchangelog-0.2.0/gptchangelog/templates/changelog_prompt.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)      549 2023-04-14 18:10:00.000000 gptchangelog-0.2.0/gptchangelog/templates/version_prompt.txt
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-04-14 18:40:34.387632 gptchangelog-0.2.0/gptchangelog.egg-info/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1861 2023-04-14 18:40:34.000000 gptchangelog-0.2.0/gptchangelog.egg-info/PKG-INFO
+-rw-r--r--   0 xjodoin    (501) staff       (20)      355 2023-04-14 18:40:34.000000 gptchangelog-0.2.0/gptchangelog.egg-info/SOURCES.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)        1 2023-04-14 18:40:34.000000 gptchangelog-0.2.0/gptchangelog.egg-info/dependency_links.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       52 2023-04-14 18:40:34.000000 gptchangelog-0.2.0/gptchangelog.egg-info/entry_points.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       30 2023-04-14 18:40:34.000000 gptchangelog-0.2.0/gptchangelog.egg-info/requires.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       13 2023-04-14 18:40:34.000000 gptchangelog-0.2.0/gptchangelog.egg-info/top_level.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       38 2023-04-14 18:40:34.389868 gptchangelog-0.2.0/setup.cfg
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1229 2023-04-14 18:39:44.000000 gptchangelog-0.2.0/setup.py
```

### Comparing `gptchangelog-0.1.1/LICENSE` & `gptchangelog-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gptchangelog-0.1.1/PKG-INFO` & `gptchangelog-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptchangelog
-Version: 0.1.1
+Version: 0.2.0
 Summary: Automatically generate a changelog using GPT-3
 Home-page: https://github.com/xjodoin/gptchangelog
 Author: Xavier Jodoin
 Author-email: xavier@jodoin.me
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gptchangelog-0.1.1/README.md` & `gptchangelog-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gptchangelog-0.1.1/gptchangelog/__init__.py` & `gptchangelog-0.2.0/gptchangelog/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import configparser
 import os
+from datetime import datetime
+from string import Template
 
 import git
 import openai
 
 
+def render_prompt(template_path, context):
+    script_dir = os.path.dirname(os.path.abspath(__file__))
+    full_template_path = os.path.join(script_dir, template_path)
+    with open(full_template_path, 'r') as template_file:
+        template_content = template_file.read()
+
+    template = Template(template_content)
+    return template.safe_substitute(context)
+
+
 def generate_changelog_and_next_version(commit_messages, latest_version):
-    prompt = (
-        f"Based on the following commit messages and the latest version {latest_version}, "
-        f"determine the next version using semantic versioning:\n\n{commit_messages}\n\n"
-        f"Just the next version: "
-    )
+    prompt = render_prompt('templates/version_prompt.txt', {'commit_messages': commit_messages, 'latest_version': latest_version})
+
     response = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=[
             {"role": "system", "content": "You are a helpful assistant."},
             {"role": "user", "content": prompt, }
         ],
     )
     next_version = response.choices[0].message['content'].strip()
 
     print(f"Next version: {next_version}")
 
-    prompt = (
-        f"Generate a well-formatted changelog in markdown format for a software project "
-        f"with the following commit messages:\n\n{commit_messages}\n\n"
-        f"Please exclude empty sections in the changelog. The next version is {next_version}.\n\n"
-        f"Changelog:\n"
-    )
+    prompt = render_prompt('templates/changelog_prompt.txt', {'commit_messages': commit_messages, 'next_version': next_version, 'current_date': datetime.today().strftime('%Y-%m-%d')})
     response = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         messages=[
             {"role": "system", "content": "You are a helpful assistant."},
             {"role": "user", "content": prompt, }
         ],
     )
```

### Comparing `gptchangelog-0.1.1/gptchangelog.egg-info/PKG-INFO` & `gptchangelog-0.2.0/gptchangelog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptchangelog
-Version: 0.1.1
+Version: 0.2.0
 Summary: Automatically generate a changelog using GPT-3
 Home-page: https://github.com/xjodoin/gptchangelog
 Author: Xavier Jodoin
 Author-email: xavier@jodoin.me
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gptchangelog-0.1.1/setup.py` & `gptchangelog-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gptchangelog",
-    version="0.1.1",
+    version="0.2.0",
     author="Xavier Jodoin",
     author_email="xavier@jodoin.me",
     description="Automatically generate a changelog using GPT-3",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xjodoin/gptchangelog",
     packages=find_packages(),
+    package_data={"gptchangelog": ["templates/*.txt"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
```

