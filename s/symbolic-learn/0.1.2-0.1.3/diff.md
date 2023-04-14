# Comparing `tmp/symbolic-learn-0.1.2.tar.gz` & `tmp/symbolic-learn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolic-learn-0.1.2.tar", last modified: Fri Apr 14 14:50:53 2023, max compression
+gzip compressed data, was "symbolic-learn-0.1.3.tar", last modified: Fri Apr 14 19:41:15 2023, max compression
```

## Comparing `symbolic-learn-0.1.2.tar` & `symbolic-learn-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:50:53.506961 symbolic-learn-0.1.2/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1072 2023-04-13 10:14:20.000000 symbolic-learn-0.1.2/LICENSE.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2388 2023-04-14 14:50:53.506961 symbolic-learn-0.1.2/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1814 2023-04-14 14:49:49.000000 symbolic-learn-0.1.2/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      783 2023-04-14 14:50:36.000000 symbolic-learn-0.1.2/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:50:53.502961 symbolic-learn-0.1.2/sblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-03-17 10:13:18.000000 symbolic-learn-0.1.2/sblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   348239 2023-04-14 13:33:26.000000 symbolic-learn-0.1.2/sblearn/compute.c
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    15924 2023-04-14 14:17:57.000000 symbolic-learn-0.1.2/sblearn/models.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   855277 2023-04-14 13:33:26.000000 symbolic-learn-0.1.2/sblearn/trees.c
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-14 14:50:53.506961 symbolic-learn-0.1.2/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1401 2023-04-14 14:11:48.000000 symbolic-learn-0.1.2/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:50:53.506961 symbolic-learn-0.1.2/symbolic_learn.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2388 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      307 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       57 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/top_level.txt
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 19:41:15.399092 symbolic-learn-0.1.3/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1072 2023-04-13 10:14:20.000000 symbolic-learn-0.1.3/LICENSE.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2591 2023-04-14 19:41:15.399092 symbolic-learn-0.1.3/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2017 2023-04-14 19:35:51.000000 symbolic-learn-0.1.3/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      783 2023-04-14 19:39:23.000000 symbolic-learn-0.1.3/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 19:41:15.395092 symbolic-learn-0.1.3/sblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-03-17 10:13:18.000000 symbolic-learn-0.1.3/sblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   348239 2023-04-14 13:33:26.000000 symbolic-learn-0.1.3/sblearn/compute.c
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    15924 2023-04-14 16:14:25.000000 symbolic-learn-0.1.3/sblearn/models.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   855277 2023-04-14 13:33:26.000000 symbolic-learn-0.1.3/sblearn/trees.c
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-14 19:41:15.399092 symbolic-learn-0.1.3/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-04-14 18:18:13.000000 symbolic-learn-0.1.3/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 19:41:15.399092 symbolic-learn-0.1.3/symbolic_learn.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2591 2023-04-14 19:41:15.000000 symbolic-learn-0.1.3/symbolic_learn.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      307 2023-04-14 19:41:15.000000 symbolic-learn-0.1.3/symbolic_learn.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-14 19:41:15.000000 symbolic-learn-0.1.3/symbolic_learn.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       57 2023-04-14 19:41:15.000000 symbolic-learn-0.1.3/symbolic_learn.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-14 19:41:15.000000 symbolic-learn-0.1.3/symbolic_learn.egg-info/top_level.txt
```

### Comparing `symbolic-learn-0.1.2/LICENSE.txt` & `symbolic-learn-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.2/PKG-INFO` & `symbolic-learn-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolic-learn
-Version: 0.1.2
+Version: 0.1.3
 Summary: A sklearn-compatible package that implements a symbolic regression model
 Author-email: Vincent Papelard <papelardvincent@gmail.com>
 Project-URL: Homepage, https://github.com/vinpap/symbolic-learn
 Project-URL: Documentation, https://symbolic-learn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,7 +38,17 @@
 Here is how to instantiate and train a symbolic regression model::
 
     from sblearn.models import SymbolicRegressor
     model = SymbolicRegressor()
     model.fit(X_train, y_train)
 
 After training your model, you can use access the fitted function's formula and function tree through the model's attributes `formulas` and `trees`. `Read the doc <https://symbolic-learn.readthedocs.io/en/latest/>`_ for more information.
+
+
+Installation
+---------------------------
+
+In order to install the package, use this command::
+
+   pip install symbolic-learn
+
+*Note for Windows users*: Microsoft Visual C++ 2014 or higher is required!
```

### Comparing `symbolic-learn-0.1.2/README.rst` & `symbolic-learn-0.1.3/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -23,8 +23,18 @@
 
 Here is how to instantiate and train a symbolic regression model::
 
     from sblearn.models import SymbolicRegressor
     model = SymbolicRegressor()
     model.fit(X_train, y_train)
 
-After training your model, you can use access the fitted function's formula and function tree through the model's attributes `formulas` and `trees`. `Read the doc <https://symbolic-learn.readthedocs.io/en/latest/>`_ for more information.
+After training your model, you can use access the fitted function's formula and function tree through the model's attributes `formulas` and `trees`. `Read the doc <https://symbolic-learn.readthedocs.io/en/latest/>`_ for more information.
+
+
+Installation
+---------------------------
+
+In order to install the package, use this command::
+
+   pip install symbolic-learn
+
+*Note for Windows users*: Microsoft Visual C++ 2014 or higher is required!
```

### Comparing `symbolic-learn-0.1.2/pyproject.toml` & `symbolic-learn-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "Cython", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symbolic-learn"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Vincent Papelard", email="papelardvincent@gmail.com" },
 ]
 description = "A sklearn-compatible package that implements a symbolic regression model"
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `symbolic-learn-0.1.2/sblearn/compute.c` & `symbolic-learn-0.1.3/sblearn/compute.c`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.2/sblearn/models.py` & `symbolic-learn-0.1.3/sblearn/models.py`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.2/sblearn/trees.c` & `symbolic-learn-0.1.3/sblearn/trees.c`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.2/symbolic_learn.egg-info/PKG-INFO` & `symbolic-learn-0.1.3/symbolic_learn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolic-learn
-Version: 0.1.2
+Version: 0.1.3
 Summary: A sklearn-compatible package that implements a symbolic regression model
 Author-email: Vincent Papelard <papelardvincent@gmail.com>
 Project-URL: Homepage, https://github.com/vinpap/symbolic-learn
 Project-URL: Documentation, https://symbolic-learn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -38,7 +38,17 @@
 Here is how to instantiate and train a symbolic regression model::
 
     from sblearn.models import SymbolicRegressor
     model = SymbolicRegressor()
     model.fit(X_train, y_train)
 
 After training your model, you can use access the fitted function's formula and function tree through the model's attributes `formulas` and `trees`. `Read the doc <https://symbolic-learn.readthedocs.io/en/latest/>`_ for more information.
+
+
+Installation
+---------------------------
+
+In order to install the package, use this command::
+
+   pip install symbolic-learn
+
+*Note for Windows users*: Microsoft Visual C++ 2014 or higher is required!
```

