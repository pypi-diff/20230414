# Comparing `tmp/symbolic-learn-0.1.1.tar.gz` & `tmp/symbolic-learn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolic-learn-0.1.1.tar", last modified: Fri Apr 14 14:44:22 2023, max compression
+gzip compressed data, was "symbolic-learn-0.1.2.tar", last modified: Fri Apr 14 14:50:53 2023, max compression
```

## Comparing `symbolic-learn-0.1.1.tar` & `symbolic-learn-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:44:22.498807 symbolic-learn-0.1.1/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1072 2023-04-13 10:14:20.000000 symbolic-learn-0.1.1/LICENSE.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2378 2023-04-14 14:44:22.498807 symbolic-learn-0.1.1/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1804 2023-04-14 14:42:16.000000 symbolic-learn-0.1.1/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      783 2023-04-14 14:43:49.000000 symbolic-learn-0.1.1/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:44:22.494807 symbolic-learn-0.1.1/sblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-03-17 10:13:18.000000 symbolic-learn-0.1.1/sblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   348239 2023-04-14 13:33:26.000000 symbolic-learn-0.1.1/sblearn/compute.c
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    15924 2023-04-14 14:17:57.000000 symbolic-learn-0.1.1/sblearn/models.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)   855277 2023-04-14 13:33:26.000000 symbolic-learn-0.1.1/sblearn/trees.c
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-14 14:44:22.498807 symbolic-learn-0.1.1/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1401 2023-04-14 14:11:48.000000 symbolic-learn-0.1.1/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:44:22.498807 symbolic-learn-0.1.1/symbolic_learn.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2378 2023-04-14 14:44:22.000000 symbolic-learn-0.1.1/symbolic_learn.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      307 2023-04-14 14:44:22.000000 symbolic-learn-0.1.1/symbolic_learn.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-14 14:44:22.000000 symbolic-learn-0.1.1/symbolic_learn.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       57 2023-04-14 14:44:22.000000 symbolic-learn-0.1.1/symbolic_learn.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-14 14:44:22.000000 symbolic-learn-0.1.1/symbolic_learn.egg-info/top_level.txt
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:50:53.506961 symbolic-learn-0.1.2/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1072 2023-04-13 10:14:20.000000 symbolic-learn-0.1.2/LICENSE.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2388 2023-04-14 14:50:53.506961 symbolic-learn-0.1.2/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1814 2023-04-14 14:49:49.000000 symbolic-learn-0.1.2/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      783 2023-04-14 14:50:36.000000 symbolic-learn-0.1.2/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:50:53.502961 symbolic-learn-0.1.2/sblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-03-17 10:13:18.000000 symbolic-learn-0.1.2/sblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   348239 2023-04-14 13:33:26.000000 symbolic-learn-0.1.2/sblearn/compute.c
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    15924 2023-04-14 14:17:57.000000 symbolic-learn-0.1.2/sblearn/models.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)   855277 2023-04-14 13:33:26.000000 symbolic-learn-0.1.2/sblearn/trees.c
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-04-14 14:50:53.506961 symbolic-learn-0.1.2/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1401 2023-04-14 14:11:48.000000 symbolic-learn-0.1.2/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-04-14 14:50:53.506961 symbolic-learn-0.1.2/symbolic_learn.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2388 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      307 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       57 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        8 2023-04-14 14:50:53.000000 symbolic-learn-0.1.2/symbolic_learn.egg-info/top_level.txt
```

### Comparing `symbolic-learn-0.1.1/LICENSE.txt` & `symbolic-learn-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.1/PKG-INFO` & `symbolic-learn-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolic-learn
-Version: 0.1.1
+Version: 0.1.2
 Summary: A sklearn-compatible package that implements a symbolic regression model
 Author-email: Vincent Papelard <papelardvincent@gmail.com>
 Project-URL: Homepage, https://github.com/vinpap/symbolic-learn
 Project-URL: Documentation, https://symbolic-learn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 
 
 What is symbolic regression?
 ------------------------------
 
 Symbolic regression is a type of regression model that combines mathematical blocks to find the function that best fits the data. Here each function is represented as a binary tree like this one:
 
-.. image:: https://github.com/vinpap/symbolic-learn/blob/master/docs/_static/genetic_program_tree.png
+.. image:: https://raw.githubusercontent.com/vinpap/symbolic-learn/master/docs/_static/genetic_program_tree.png
    :alt: Function tree representation : image not found
    :align: center
 
 The model initially generates a random population of such functions. It then uses genetic programming techniques on it to find out the function that best fits our dataset.
 As this model is based on `scikit-learn's <http://scikit-learn.org>`_ base estimator, it can be used the same way you would use any sklearn model. Thus, you can use it in pipelines or apply fine-tuning techniques such as GridSearchCV on it.
 
 Symbolic regression is best used when you want to take a naive approach to solving a regression problem. Unlike most existing models, it does not come with an **a priori** specification of a model. Therefore it is a good idea to use it when you want to find out and understand the mathematical structures in your data.
```

### Comparing `symbolic-learn-0.1.1/README.rst` & `symbolic-learn-0.1.2/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 What is symbolic regression?
 ------------------------------
 
 Symbolic regression is a type of regression model that combines mathematical blocks to find the function that best fits the data. Here each function is represented as a binary tree like this one:
 
-.. image:: https://github.com/vinpap/symbolic-learn/blob/master/docs/_static/genetic_program_tree.png
+.. image:: https://raw.githubusercontent.com/vinpap/symbolic-learn/master/docs/_static/genetic_program_tree.png
    :alt: Function tree representation : image not found
    :align: center
 
 The model initially generates a random population of such functions. It then uses genetic programming techniques on it to find out the function that best fits our dataset.
 As this model is based on `scikit-learn's <http://scikit-learn.org>`_ base estimator, it can be used the same way you would use any sklearn model. Thus, you can use it in pipelines or apply fine-tuning techniques such as GridSearchCV on it.
 
 Symbolic regression is best used when you want to take a naive approach to solving a regression problem. Unlike most existing models, it does not come with an **a priori** specification of a model. Therefore it is a good idea to use it when you want to find out and understand the mathematical structures in your data.
```

### Comparing `symbolic-learn-0.1.1/pyproject.toml` & `symbolic-learn-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "Cython", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "symbolic-learn"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Vincent Papelard", email="papelardvincent@gmail.com" },
 ]
 description = "A sklearn-compatible package that implements a symbolic regression model"
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `symbolic-learn-0.1.1/sblearn/compute.c` & `symbolic-learn-0.1.2/sblearn/compute.c`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.1/sblearn/models.py` & `symbolic-learn-0.1.2/sblearn/models.py`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.1/sblearn/trees.c` & `symbolic-learn-0.1.2/sblearn/trees.c`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.1/setup.py` & `symbolic-learn-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `symbolic-learn-0.1.1/symbolic_learn.egg-info/PKG-INFO` & `symbolic-learn-0.1.2/symbolic_learn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolic-learn
-Version: 0.1.1
+Version: 0.1.2
 Summary: A sklearn-compatible package that implements a symbolic regression model
 Author-email: Vincent Papelard <papelardvincent@gmail.com>
 Project-URL: Homepage, https://github.com/vinpap/symbolic-learn
 Project-URL: Documentation, https://symbolic-learn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 
 
 What is symbolic regression?
 ------------------------------
 
 Symbolic regression is a type of regression model that combines mathematical blocks to find the function that best fits the data. Here each function is represented as a binary tree like this one:
 
-.. image:: https://github.com/vinpap/symbolic-learn/blob/master/docs/_static/genetic_program_tree.png
+.. image:: https://raw.githubusercontent.com/vinpap/symbolic-learn/master/docs/_static/genetic_program_tree.png
    :alt: Function tree representation : image not found
    :align: center
 
 The model initially generates a random population of such functions. It then uses genetic programming techniques on it to find out the function that best fits our dataset.
 As this model is based on `scikit-learn's <http://scikit-learn.org>`_ base estimator, it can be used the same way you would use any sklearn model. Thus, you can use it in pipelines or apply fine-tuning techniques such as GridSearchCV on it.
 
 Symbolic regression is best used when you want to take a naive approach to solving a regression problem. Unlike most existing models, it does not come with an **a priori** specification of a model. Therefore it is a good idea to use it when you want to find out and understand the mathematical structures in your data.
```

