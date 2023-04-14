# Comparing `tmp/catprompt-0.0.1.tar.gz` & `tmp/catprompt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catprompt-0.0.1.tar", last modified: Fri Apr 14 09:25:02 2023, max compression
+gzip compressed data, was "catprompt-0.0.2.tar", last modified: Fri Apr 14 09:32:06 2023, max compression
```

## Comparing `catprompt-0.0.1.tar` & `catprompt-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:25:02.782674 catprompt-0.0.1/
--rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-14 07:06:27.000000 catprompt-0.0.1/LICENSE
--rw-r--r--   0 juanre     (501) staff       (20)     5762 2023-04-14 09:25:02.782063 catprompt-0.0.1/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)     4135 2023-04-14 08:41:24.000000 catprompt-0.0.1/README.md
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:25:02.778733 catprompt-0.0.1/catprompt/
--rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-14 09:14:16.000000 catprompt-0.0.1/catprompt/__init__.py
--rw-r--r--   0 juanre     (501) staff       (20)     1619 2023-04-14 09:20:30.000000 catprompt-0.0.1/catprompt/prompter.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:25:02.780736 catprompt-0.0.1/catprompt.egg-info/
--rw-r--r--   0 juanre     (501) staff       (20)     5762 2023-04-14 09:25:02.000000 catprompt-0.0.1/catprompt.egg-info/PKG-INFO
--rw-r--r--   0 juanre     (501) staff       (20)      307 2023-04-14 09:25:02.000000 catprompt-0.0.1/catprompt.egg-info/SOURCES.txt
--rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-14 09:25:02.000000 catprompt-0.0.1/catprompt.egg-info/dependency_links.txt
--rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-14 09:25:02.000000 catprompt-0.0.1/catprompt.egg-info/entry_points.txt
--rw-r--r--   0 juanre     (501) staff       (20)       72 2023-04-14 09:25:02.000000 catprompt-0.0.1/catprompt.egg-info/requires.txt
--rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-14 09:25:02.000000 catprompt-0.0.1/catprompt.egg-info/top_level.txt
--rw-r--r--   0 juanre     (501) staff       (20)      790 2023-04-14 09:11:25.000000 catprompt-0.0.1/pyproject.toml
--rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-14 09:25:02.782821 catprompt-0.0.1/setup.cfg
--rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-14 09:15:34.000000 catprompt-0.0.1/setup.py
-drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:25:02.781236 catprompt-0.0.1/test/
--rw-r--r--   0 juanre     (501) staff       (20)     1458 2023-04-14 09:14:49.000000 catprompt-0.0.1/test/test_prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:32:06.576426 catprompt-0.0.2/
+-rw-r--r--   0 juanre     (501) staff       (20)     1074 2023-04-14 07:06:27.000000 catprompt-0.0.2/LICENSE
+-rw-r--r--   0 juanre     (501) staff       (20)     5768 2023-04-14 09:32:06.575907 catprompt-0.0.2/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)     4141 2023-04-14 09:29:01.000000 catprompt-0.0.2/README.md
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:32:06.573114 catprompt-0.0.2/catprompt/
+-rw-r--r--   0 juanre     (501) staff       (20)        0 2023-04-14 09:14:16.000000 catprompt-0.0.2/catprompt/__init__.py
+-rw-r--r--   0 juanre     (501) staff       (20)     1619 2023-04-14 09:20:30.000000 catprompt-0.0.2/catprompt/prompter.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:32:06.574849 catprompt-0.0.2/catprompt.egg-info/
+-rw-r--r--   0 juanre     (501) staff       (20)     5768 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/PKG-INFO
+-rw-r--r--   0 juanre     (501) staff       (20)      307 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 juanre     (501) staff       (20)        1 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       54 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/entry_points.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       72 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/requires.txt
+-rw-r--r--   0 juanre     (501) staff       (20)       10 2023-04-14 09:32:06.000000 catprompt-0.0.2/catprompt.egg-info/top_level.txt
+-rw-r--r--   0 juanre     (501) staff       (20)      790 2023-04-14 09:31:11.000000 catprompt-0.0.2/pyproject.toml
+-rw-r--r--   0 juanre     (501) staff       (20)       38 2023-04-14 09:32:06.576608 catprompt-0.0.2/setup.cfg
+-rw-r--r--   0 juanre     (501) staff       (20)       93 2023-04-14 09:15:34.000000 catprompt-0.0.2/setup.py
+drwxr-xr-x   0 juanre     (501) staff       (20)        0 2023-04-14 09:32:06.575211 catprompt-0.0.2/test/
+-rw-r--r--   0 juanre     (501) staff       (20)     1458 2023-04-14 09:14:49.000000 catprompt-0.0.2/test/test_prompter.py
```

### Comparing `catprompt-0.0.1/LICENSE` & `catprompt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `catprompt-0.0.1/PKG-INFO` & `catprompt-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -55,15 +55,17 @@
 
 `catprompt path/to/prompt.txt`
 
 4. Use the processed content from the clipboard
 
 ## Installation
 
-To install catprompt:
+`pip install catprompt`
+
+or
 
 1. Visit the homepage at https://github.com/juanre/catprompt
 2. Download the package as a ZIP file or clone the repository using git
 3. Navigate to the downloaded folder in your command-line interface
 4. Run `pip install .` to install the package
 
 Make sure you have `pip` installed on your system. If not, you can find instructions on how to install pip here: https://pip.pypa.io/en/stable/installation/
```

### Comparing `catprompt-0.0.1/README.md` & `catprompt-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 
 `catprompt path/to/prompt.txt`
 
 4. Use the processed content from the clipboard
 
 ## Installation
 
-To install catprompt:
+`pip install catprompt`
+
+or
 
 1. Visit the homepage at https://github.com/juanre/catprompt
 2. Download the package as a ZIP file or clone the repository using git
 3. Navigate to the downloaded folder in your command-line interface
 4. Run `pip install .` to install the package
 
 Make sure you have `pip` installed on your system. If not, you can find instructions on how to install pip here: https://pip.pypa.io/en/stable/installation/
```

### Comparing `catprompt-0.0.1/catprompt/prompter.py` & `catprompt-0.0.2/catprompt/prompter.py`

 * *Files identical despite different names*

### Comparing `catprompt-0.0.1/catprompt.egg-info/PKG-INFO` & `catprompt-0.0.2/catprompt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catprompt
-Version: 0.0.1
+Version: 0.0.2
 Summary: Combine prompts for chatgpt.
 Author-email: Juan Reyero <juan@juanreyero.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -55,15 +55,17 @@
 
 `catprompt path/to/prompt.txt`
 
 4. Use the processed content from the clipboard
 
 ## Installation
 
-To install catprompt:
+`pip install catprompt`
+
+or
 
 1. Visit the homepage at https://github.com/juanre/catprompt
 2. Download the package as a ZIP file or clone the repository using git
 3. Navigate to the downloaded folder in your command-line interface
 4. Run `pip install .` to install the package
 
 Make sure you have `pip` installed on your system. If not, you can find instructions on how to install pip here: https://pip.pypa.io/en/stable/installation/
```

### Comparing `catprompt-0.0.1/pyproject.toml` & `catprompt-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "catprompt"
-version = "0.0.1"
+version = "0.0.2"
 description = "Combine prompts for chatgpt."
 readme = "README.md"
 authors = [
     { name = "Juan Reyero", email="juan@juanreyero.com" }
 ]
 requires-python = ">=3.8"
 license = { file="LICENSE" }
```

### Comparing `catprompt-0.0.1/test/test_prompter.py` & `catprompt-0.0.2/test/test_prompter.py`

 * *Files identical despite different names*

