# Comparing `tmp/pysmells-1.0.8.tar.gz` & `tmp/pysmells-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmells-1.0.8.tar", last modified: Mon Apr 10 10:47:00 2023, max compression
+gzip compressed data, was "pysmells-1.0.9.tar", last modified: Tue Apr 11 21:14:10 2023, max compression
```

## Comparing `pysmells-1.0.8.tar` & `pysmells-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 10:47:00.670003 pysmells-1.0.8/
--rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.8/LICENSE
--rw-r--r--   0 marcossousa   (501) staff       (20)     2077 2023-04-10 10:47:00.668395 pysmells-1.0.8/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)     1131 2023-04-07 23:28:38.000000 pysmells-1.0.8/README.md
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 10:47:00.653426 pysmells-1.0.8/pysmells/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.8/pysmells/__init__.py
--rw-r--r--   0 marcossousa   (501) staff       (20)     4162 2023-04-10 10:39:40.000000 pysmells-1.0.8/pysmells/pysmells.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 10:47:00.665753 pysmells-1.0.8/pysmells.egg-info/
--rw-r--r--   0 marcossousa   (501) staff       (20)     2077 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/PKG-INFO
--rw-r--r--   0 marcossousa   (501) staff       (20)      279 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/SOURCES.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/dependency_links.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/entry_points.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       21 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/requires.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       14 2023-04-10 10:47:00.000000 pysmells-1.0.8/pysmells.egg-info/top_level.txt
--rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-10 10:47:00.670644 pysmells-1.0.8/setup.cfg
--rw-r--r--   0 marcossousa   (501) staff       (20)     1332 2023-04-10 10:45:40.000000 pysmells-1.0.8/setup.py
-drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-10 10:47:00.666605 pysmells-1.0.8/test/
--rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-09 23:44:38.000000 pysmells-1.0.8/test/__init__.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-11 21:14:10.666354 pysmells-1.0.9/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1115 2023-04-07 23:01:55.000000 pysmells-1.0.9/LICENSE
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1946 2023-04-11 21:14:10.664584 pysmells-1.0.9/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      930 2023-04-11 21:13:08.000000 pysmells-1.0.9/README.md
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-11 21:14:10.645025 pysmells-1.0.9/pysmells/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-07 22:10:03.000000 pysmells-1.0.9/pysmells/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)     5916 2023-04-11 20:54:07.000000 pysmells-1.0.9/pysmells/pysmells.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-11 21:14:10.654991 pysmells-1.0.9/pysmells.egg-info/
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1946 2023-04-11 21:14:10.000000 pysmells-1.0.9/pysmells.egg-info/PKG-INFO
+-rw-r--r--   0 marcossousa   (501) staff       (20)      387 2023-04-11 21:14:10.000000 pysmells-1.0.9/pysmells.egg-info/SOURCES.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)        1 2023-04-11 21:14:10.000000 pysmells-1.0.9/pysmells.egg-info/dependency_links.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       44 2023-04-11 21:14:10.000000 pysmells-1.0.9/pysmells.egg-info/entry_points.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       16 2023-04-11 21:14:10.000000 pysmells-1.0.9/pysmells.egg-info/requires.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       14 2023-04-11 21:14:10.000000 pysmells-1.0.9/pysmells.egg-info/top_level.txt
+-rw-r--r--   0 marcossousa   (501) staff       (20)       38 2023-04-11 21:14:10.666988 pysmells-1.0.9/setup.cfg
+-rw-r--r--   0 marcossousa   (501) staff       (20)     1386 2023-04-11 21:13:08.000000 pysmells-1.0.9/setup.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-11 21:14:10.656066 pysmells-1.0.9/test/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-09 23:44:38.000000 pysmells-1.0.9/test/__init__.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-11 21:14:10.658101 pysmells-1.0.9/test/programa1/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-10 20:11:29.000000 pysmells-1.0.9/test/programa1/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)       55 2023-04-11 20:53:24.000000 pysmells-1.0.9/test/programa1/badcode1.py
+drwxr-xr-x   0 marcossousa   (501) staff       (20)        0 2023-04-11 21:14:10.662251 pysmells-1.0.9/test/programa2/
+-rw-r--r--   0 marcossousa   (501) staff       (20)        0 2023-04-10 20:11:42.000000 pysmells-1.0.9/test/programa2/__init__.py
+-rw-r--r--   0 marcossousa   (501) staff       (20)       32 2023-04-11 20:53:24.000000 pysmells-1.0.9/test/programa2/badcode2.py
```

### Comparing `pysmells-1.0.8/LICENSE` & `pysmells-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmells-1.0.8/PKG-INFO` & `pysmells-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.8
-Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
+Version: 1.0.9
+Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. It will then generate a report detailing the results of the analysis. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 Home-page: https://github.com/pysmells/pysmells
 Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,37 +16,36 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pysmells
 
-A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
+Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. It will then generate a report detailing the results of the analysis. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 
 ## Installation
 
 You can install pysmells using pip:
 
 `pip install pysmells`
 
-## Usage
+Clone this repository:
 
-To use pysmells, navigate to the directory containing the Python files you want to analyze and run the following command:
+bash `git clone https://github.com/pysmells/pysmells.git`
 
-`pysmells`
+## Usage
 
+To use pysmells, navigate to the directory containing the Python files you want to analyze and run the following command:
 
-pysmells will analyze the Python files in the current directory, checking for programming errors, inconsistencies, programming style violations, and the correctness of type annotations in programs. It will then generate a report detailing the results of the analysis.
 
 ## Dependencies
 
 pysmells requires the following packages:
 
 - tabulate
-- mypy
 - pylint
 
 These dependencies will be automatically installed when you install pysmells using pip.
 
 ## License
 
 pysmells is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
```

### Comparing `pysmells-1.0.8/README.md` & `pysmells-1.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # Pysmells
 
-A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
+Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. It will then generate a report detailing the results of the analysis. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 
 ## Installation
 
 You can install pysmells using pip:
 
 `pip install pysmells`
 
-## Usage
+Clone this repository:
 
-To use pysmells, navigate to the directory containing the Python files you want to analyze and run the following command:
+bash `git clone https://github.com/pysmells/pysmells.git`
 
-`pysmells`
+## Usage
 
+To use pysmells, navigate to the directory containing the Python files you want to analyze and run the following command:
 
-pysmells will analyze the Python files in the current directory, checking for programming errors, inconsistencies, programming style violations, and the correctness of type annotations in programs. It will then generate a report detailing the results of the analysis.
 
 ## Dependencies
 
 pysmells requires the following packages:
 
 - tabulate
-- mypy
 - pylint
 
 These dependencies will be automatically installed when you install pysmells using pip.
 
 ## License
 
 pysmells is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
```

### Comparing `pysmells-1.0.8/pysmells.egg-info/PKG-INFO` & `pysmells-1.0.9/pysmells.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pysmells
-Version: 1.0.8
-Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
+Version: 1.0.9
+Summary: Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. It will then generate a report detailing the results of the analysis. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 Home-page: https://github.com/pysmells/pysmells
 Author: Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto
 Author-email: msousa@museu-goeldi.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -16,37 +16,36 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pysmells
 
-A Python code analysis tool that checks for programming errors, inconsistencies, and programming style violations, as well as the correctness of type annotations in programs. The pysmells tool is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 20, PEP 257, PEP 484, PEP 526, PEP 544, PEP 561, PEP 563, and PEP 589.
+Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. It will then generate a report detailing the results of the analysis. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.
 
 ## Installation
 
 You can install pysmells using pip:
 
 `pip install pysmells`
 
-## Usage
+Clone this repository:
 
-To use pysmells, navigate to the directory containing the Python files you want to analyze and run the following command:
+bash `git clone https://github.com/pysmells/pysmells.git`
 
-`pysmells`
+## Usage
 
+To use pysmells, navigate to the directory containing the Python files you want to analyze and run the following command:
 
-pysmells will analyze the Python files in the current directory, checking for programming errors, inconsistencies, programming style violations, and the correctness of type annotations in programs. It will then generate a report detailing the results of the analysis.
 
 ## Dependencies
 
 pysmells requires the following packages:
 
 - tabulate
-- mypy
 - pylint
 
 These dependencies will be automatically installed when you install pysmells using pip.
 
 ## License
 
 pysmells is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
```

### Comparing `pysmells-1.0.8/setup.py` & `pysmells-1.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pysmells",
-    version="1.0.8",
+    version="1.0.9",
     author="Marcos Paulo Alves de Sousa and Marco Aurélio Proença Neto",
     author_email="msousa@museu-goeldi.br",
-    description="Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.",
+    description="Pysmells is a tool that identifies when something doesn't 'smell right' in a python code, checking for programming errors, inconsistencies and programming style violations. It will then generate a report detailing the results of the analysis. Pysmells is based on the following Python Enhancement Proposals (PEPs): PEP 8, PEP 257 and PEP 20.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pysmells/pysmells",
     packages=find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
@@ -21,15 +21,14 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     python_requires='>=3.7',
     install_requires=[
         'tabulate',
-        'mypy',
         'pylint',
     ],
     entry_points={
         'console_scripts': [
             'pysmells=pysmells:main',
         ],
     },
```

