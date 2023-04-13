# Comparing `tmp/sal-code-generator-0.0.3.tar.gz` & `tmp/sal-code-generator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sal-code-generator-0.0.3.tar", last modified: Mon Nov 14 01:53:25 2022, max compression
+gzip compressed data, was "sal-code-generator-0.0.5.tar", last modified: Mon Nov 14 02:14:46 2022, max compression
```

## Comparing `sal-code-generator-0.0.3.tar` & `sal-code-generator-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mg         (501) staff       (20)        0 2022-11-14 01:53:25.415656 sal-code-generator-0.0.3/
--rw-rw-r--   0 mg         (501) staff       (20)    11337 2022-09-05 16:31:43.000000 sal-code-generator-0.0.3/LICENSE
--rw-rw-r--   0 mg         (501) staff       (20)      111 2022-09-05 16:31:43.000000 sal-code-generator-0.0.3/MANIFEST.in
--rw-r--r--   0 mg         (501) staff       (20)     1247 2022-11-14 01:53:25.415526 sal-code-generator-0.0.3/PKG-INFO
--rw-r--r--   0 mg         (501) staff       (20)      421 2022-11-14 00:40:43.000000 sal-code-generator-0.0.3/README.md
--rw-r--r--   0 mg         (501) staff       (20)      553 2022-11-14 01:49:43.000000 sal-code-generator-0.0.3/pyproject.toml
-drwxr-xr-x   0 mg         (501) staff       (20)        0 2022-11-14 01:53:25.414387 sal-code-generator-0.0.3/sal/
--rw-r--r--   0 mg         (501) staff       (20)       22 2022-11-14 01:53:04.000000 sal-code-generator-0.0.3/sal/__init__.py
--rw-r--r--   0 mg         (501) staff       (20)     7751 2022-11-14 01:53:04.000000 sal-code-generator-0.0.3/sal/_modidx.py
--rw-r--r--   0 mg         (501) staff       (20)     1852 2022-11-14 01:53:04.000000 sal-code-generator-0.0.3/sal/cli.py
--rw-r--r--   0 mg         (501) staff       (20)     5683 2022-11-14 01:53:04.000000 sal-code-generator-0.0.3/sal/codegen.py
--rw-r--r--   0 mg         (501) staff       (20)     5617 2022-11-14 01:53:04.000000 sal-code-generator-0.0.3/sal/core.py
--rw-r--r--   0 mg         (501) staff       (20)     1548 2022-11-14 01:53:04.000000 sal-code-generator-0.0.3/sal/loaders.py
-drwxr-xr-x   0 mg         (501) staff       (20)        0 2022-11-14 01:53:25.415280 sal-code-generator-0.0.3/sal_code_generator.egg-info/
--rw-r--r--   0 mg         (501) staff       (20)     1247 2022-11-14 01:53:25.000000 sal-code-generator-0.0.3/sal_code_generator.egg-info/PKG-INFO
--rw-r--r--   0 mg         (501) staff       (20)      445 2022-11-14 01:53:25.000000 sal-code-generator-0.0.3/sal_code_generator.egg-info/SOURCES.txt
--rw-r--r--   0 mg         (501) staff       (20)        1 2022-11-14 01:53:25.000000 sal-code-generator-0.0.3/sal_code_generator.egg-info/dependency_links.txt
--rw-r--r--   0 mg         (501) staff       (20)       28 2022-11-14 01:53:25.000000 sal-code-generator-0.0.3/sal_code_generator.egg-info/entry_points.txt
--rw-r--r--   0 mg         (501) staff       (20)        1 2022-11-14 00:09:34.000000 sal-code-generator-0.0.3/sal_code_generator.egg-info/not-zip-safe
--rw-r--r--   0 mg         (501) staff       (20)        7 2022-11-14 01:53:25.000000 sal-code-generator-0.0.3/sal_code_generator.egg-info/requires.txt
--rw-r--r--   0 mg         (501) staff       (20)        4 2022-11-14 01:53:25.000000 sal-code-generator-0.0.3/sal_code_generator.egg-info/top_level.txt
--rw-r--r--   0 mg         (501) staff       (20)      838 2022-11-14 01:50:18.000000 sal-code-generator-0.0.3/settings.ini
--rw-r--r--   0 mg         (501) staff       (20)       38 2022-11-14 01:53:25.415701 sal-code-generator-0.0.3/setup.cfg
--rw-rw-r--   0 mg         (501) staff       (20)     2541 2022-09-05 16:31:43.000000 sal-code-generator-0.0.3/setup.py
+drwxr-xr-x   0 mg         (501) staff       (20)        0 2022-11-14 02:14:46.512771 sal-code-generator-0.0.5/
+-rw-rw-r--   0 mg         (501) staff       (20)    11337 2022-09-05 16:31:43.000000 sal-code-generator-0.0.5/LICENSE
+-rw-rw-r--   0 mg         (501) staff       (20)      111 2022-09-05 16:31:43.000000 sal-code-generator-0.0.5/MANIFEST.in
+-rw-r--r--   0 mg         (501) staff       (20)     1247 2022-11-14 02:14:46.512657 sal-code-generator-0.0.5/PKG-INFO
+-rw-r--r--   0 mg         (501) staff       (20)      421 2022-11-14 00:40:43.000000 sal-code-generator-0.0.5/README.md
+-rw-r--r--   0 mg         (501) staff       (20)      521 2022-11-14 02:14:25.000000 sal-code-generator-0.0.5/pyproject.toml
+drwxr-xr-x   0 mg         (501) staff       (20)        0 2022-11-14 02:14:46.511838 sal-code-generator-0.0.5/sal/
+-rw-r--r--   0 mg         (501) staff       (20)       22 2022-11-14 02:14:41.000000 sal-code-generator-0.0.5/sal/__init__.py
+-rw-r--r--   0 mg         (501) staff       (20)     7751 2022-11-14 02:14:41.000000 sal-code-generator-0.0.5/sal/_modidx.py
+-rw-r--r--   0 mg         (501) staff       (20)     1792 2022-11-14 02:14:41.000000 sal-code-generator-0.0.5/sal/cli.py
+-rw-r--r--   0 mg         (501) staff       (20)     5683 2022-11-14 02:14:41.000000 sal-code-generator-0.0.5/sal/codegen.py
+-rw-r--r--   0 mg         (501) staff       (20)     5617 2022-11-14 02:14:41.000000 sal-code-generator-0.0.5/sal/core.py
+-rw-r--r--   0 mg         (501) staff       (20)     1548 2022-11-14 02:14:41.000000 sal-code-generator-0.0.5/sal/loaders.py
+drwxr-xr-x   0 mg         (501) staff       (20)        0 2022-11-14 02:14:46.512507 sal-code-generator-0.0.5/sal_code_generator.egg-info/
+-rw-r--r--   0 mg         (501) staff       (20)     1247 2022-11-14 02:14:46.000000 sal-code-generator-0.0.5/sal_code_generator.egg-info/PKG-INFO
+-rw-r--r--   0 mg         (501) staff       (20)      445 2022-11-14 02:14:46.000000 sal-code-generator-0.0.5/sal_code_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 mg         (501) staff       (20)        1 2022-11-14 02:14:46.000000 sal-code-generator-0.0.5/sal_code_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 mg         (501) staff       (20)       28 2022-11-14 02:14:46.000000 sal-code-generator-0.0.5/sal_code_generator.egg-info/entry_points.txt
+-rw-r--r--   0 mg         (501) staff       (20)        1 2022-11-14 00:09:34.000000 sal-code-generator-0.0.5/sal_code_generator.egg-info/not-zip-safe
+-rw-r--r--   0 mg         (501) staff       (20)        7 2022-11-14 02:14:46.000000 sal-code-generator-0.0.5/sal_code_generator.egg-info/requires.txt
+-rw-r--r--   0 mg         (501) staff       (20)        4 2022-11-14 02:14:46.000000 sal-code-generator-0.0.5/sal_code_generator.egg-info/top_level.txt
+-rw-r--r--   0 mg         (501) staff       (20)      838 2022-11-14 02:14:25.000000 sal-code-generator-0.0.5/settings.ini
+-rw-r--r--   0 mg         (501) staff       (20)       38 2022-11-14 02:14:46.512805 sal-code-generator-0.0.5/setup.cfg
+-rw-rw-r--   0 mg         (501) staff       (20)     2541 2022-09-05 16:31:43.000000 sal-code-generator-0.0.5/setup.py
```

### Comparing `sal-code-generator-0.0.3/LICENSE` & `sal-code-generator-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sal-code-generator-0.0.3/PKG-INFO` & `sal-code-generator-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sal-code-generator
-Version: 0.0.3
+Version: 0.0.5
 Summary: A salty code generator to season your code with generated code
 Home-page: https://github.com/mintyPT/sal
 Author: mauro santos
 Author-email: mauro@scandit.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python codegen code generator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sal-code-generator-0.0.3/pyproject.toml` & `sal-code-generator-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 [tool.poetry]
 name = "sal"
-version = "0.1.0"
+version = "0.0.5"
 description = ""
 authors = ["mauro santos <mauro.goncalo@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fastcore = "^1.5.27"
 python-frontmatter = "^1.0.0"
 click = "^8.1.3"
 black = "^22.10.0"
-
-[tool.poetry.dev-dependencies]
 notebook = "^6.5.1"
 nbdev = "^2.3.7"
 twine = "^4.0.1"
 jupyterlab = "^3.5.0"
 pre-commit = "^2.20.0"
 jupyter-black = "^0.3.1"
```

### Comparing `sal-code-generator-0.0.3/sal/_modidx.py` & `sal-code-generator-0.0.5/sal/_modidx.py`

 * *Files identical despite different names*

### Comparing `sal-code-generator-0.0.3/sal/cli.py` & `sal-code-generator-0.0.5/sal/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,27 +35,23 @@
 @click.option("--count", default=1, help="Number of greetings.")
 @click.option("--name", prompt="Your name")
 def hello(count, name):
     """Simple program that greets NAME for a total of COUNT times."""
     for x in range(count):
         click.echo(f"Hello {name}!")
 
-# %% ../nbs/03_cli.ipynb 13
+# %% ../nbs/03_cli.ipynb 14
 def is_notebook() -> bool:
     try:
         shell = get_ipython().__class__.__name__
         if shell == "ZMQInteractiveShell" or shell == "CaptureShell":
             return True  # Jupyter notebook or qtconsole
         elif shell == "TerminalInteractiveShell":
             return False  # Terminal running IPython
         else:
             return False  # Other type (?)
     except NameError:
         return False  # Probably standard Python interpreter
 
-# %% ../nbs/03_cli.ipynb 14
-print('='*120)
-print('='*120)
-print('='*120)
-print('='*120)
+# %% ../nbs/03_cli.ipynb 15
 if __name__ == "__main__" and not is_notebook():
     hello()
```

### Comparing `sal-code-generator-0.0.3/sal/codegen.py` & `sal-code-generator-0.0.5/sal/codegen.py`

 * *Files identical despite different names*

### Comparing `sal-code-generator-0.0.3/sal/core.py` & `sal-code-generator-0.0.5/sal/core.py`

 * *Files identical despite different names*

### Comparing `sal-code-generator-0.0.3/sal/loaders.py` & `sal-code-generator-0.0.5/sal/loaders.py`

 * *Files identical despite different names*

### Comparing `sal-code-generator-0.0.3/sal_code_generator.egg-info/PKG-INFO` & `sal-code-generator-0.0.5/sal_code_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sal-code-generator
-Version: 0.0.3
+Version: 0.0.5
 Summary: A salty code generator to season your code with generated code
 Home-page: https://github.com/mintyPT/sal
 Author: mauro santos
 Author-email: mauro@scandit.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python codegen code generator
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sal-code-generator-0.0.3/settings.ini` & `sal-code-generator-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = sal
 lib_name = sal-code-generator
-version = 0.0.3
+version = 0.0.5
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = sal
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `sal-code-generator-0.0.3/setup.py` & `sal-code-generator-0.0.5/setup.py`

 * *Files identical despite different names*

