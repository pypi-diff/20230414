# Comparing `tmp/nnogada-0.9.1.tar.gz` & `tmp/nnogada-0.9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnogada-0.9.1.tar", last modified: Thu Apr 13 21:49:07 2023, max compression
+gzip compressed data, was "nnogada-0.9.1.1.tar", last modified: Thu Apr 13 22:18:51 2023, max compression
```

## Comparing `nnogada-0.9.1.tar` & `nnogada-0.9.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-04-13 21:49:07.564420 nnogada-0.9.1/
--rw-rw-r--   0 isidro    (1000) isidro    (1000)     1077 2023-01-17 20:47:14.000000 nnogada-0.9.1/LICENSE
--rw-rw-r--   0 isidro    (1000) isidro    (1000)     2795 2023-04-13 21:49:07.564420 nnogada-0.9.1/PKG-INFO
--rw-rw-r--   0 isidro    (1000) isidro    (1000)     1957 2023-04-13 21:46:45.000000 nnogada-0.9.1/README.md
-drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-04-13 21:49:07.564420 nnogada-0.9.1/nnogada.egg-info/
--rw-rw-r--   0 isidro    (1000) isidro    (1000)     2795 2023-04-13 21:49:07.000000 nnogada-0.9.1/nnogada.egg-info/PKG-INFO
--rw-rw-r--   0 isidro    (1000) isidro    (1000)      190 2023-04-13 21:49:07.000000 nnogada-0.9.1/nnogada.egg-info/SOURCES.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)        1 2023-04-13 21:49:07.000000 nnogada-0.9.1/nnogada.egg-info/dependency_links.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)       90 2023-04-13 21:49:07.000000 nnogada-0.9.1/nnogada.egg-info/requires.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)        1 2023-04-13 21:49:07.000000 nnogada-0.9.1/nnogada.egg-info/top_level.txt
--rw-rw-r--   0 isidro    (1000) isidro    (1000)       79 2023-04-13 21:49:07.564420 nnogada-0.9.1/setup.cfg
--rw-rw-r--   0 isidro    (1000) isidro    (1000)     1281 2023-04-10 15:22:58.000000 nnogada-0.9.1/setup.py
+drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-04-13 22:18:51.823639 nnogada-0.9.1.1/
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)     1077 2023-01-17 20:47:14.000000 nnogada-0.9.1.1/LICENSE
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)     1990 2023-04-13 22:18:51.823639 nnogada-0.9.1.1/PKG-INFO
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)     1150 2023-04-13 22:05:14.000000 nnogada-0.9.1.1/README.md
+drwxrwxr-x   0 isidro    (1000) isidro    (1000)        0 2023-04-13 22:18:51.823639 nnogada-0.9.1.1/nnogada.egg-info/
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)     1990 2023-04-13 22:18:51.000000 nnogada-0.9.1.1/nnogada.egg-info/PKG-INFO
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)      190 2023-04-13 22:18:51.000000 nnogada-0.9.1.1/nnogada.egg-info/SOURCES.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)        1 2023-04-13 22:18:51.000000 nnogada-0.9.1.1/nnogada.egg-info/dependency_links.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)       90 2023-04-13 22:18:51.000000 nnogada-0.9.1.1/nnogada.egg-info/requires.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)        1 2023-04-13 22:18:51.000000 nnogada-0.9.1.1/nnogada.egg-info/top_level.txt
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)       79 2023-04-13 22:18:51.823639 nnogada-0.9.1.1/setup.cfg
+-rw-rw-r--   0 isidro    (1000) isidro    (1000)     1283 2023-04-13 22:18:15.000000 nnogada-0.9.1.1/setup.py
```

### Comparing `nnogada-0.9.1/LICENSE` & `nnogada-0.9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nnogada-0.9.1/PKG-INFO` & `nnogada-0.9.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnogada
-Version: 0.9.1
+Version: 0.9.1.1
 Summary: Genetic hyperparameter tuning for neural nets
 Home-page: https://github.com/igomezv/nnogada
 Author: I Gomez-Vargas
 Author-email: igomez@icf.unam.mx
 License: MIT
 Keywords: Hyperparameter,optimization,machine learning,deep learning,genetic algorithms
 Platform: UNKNOWN
@@ -16,23 +16,21 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 License-File: LICENSE
 
-[<img src="https://img.shields.io/badge/astro--ph.IM-%20%09arXiv%3A2209.02685-green.svg">](https://arxiv.org/abs/2209.02685)
-
 # Neural Networks Optimized by Genetic Algorithms for Data Analysis (NNOGADA) 
 
 **nnogada** is a Python package that performs hyperparemeter tuning for artificial neural networks, particularly for Multi Layer Perceptrons, using simple genetic algorithms. Useful for generate better neural network models for data analysis. Currently, only works with feedforward neural networks in tensorflow.keras (classification and regression) and torch (regression at this moment).
 
 Before use the code, please install the requirements:
 
-    $ pip3 install -r requiriments.txt
+    $ pip3 install nnogada
  
 Or you can try to install nnogada in your computer:
 
      $ git clone https://github.com/igomezv/nnogada
 
      $ cd nnogada
 
@@ -40,27 +38,13 @@
 
 then you can delete the cloned repo because you must have nnogada installed locally.
 
 Other way to install nnogada (without clonning) is:
 
     $ pip3 install -e git+https://github.com/igomezv/nnogada#egg=nnogada
 
-
 If you use the code, please cite the paper *Gómez-Vargas, I., Andrade, J. B., & Vázquez, J. A. (2023). Neural networks optimized by genetic algorithms in cosmology. Physical Review D, 107(4), 043509.*
 
 Contributions are welcome!
 
-![](https://raw.githubusercontent.com/igomezv/igomezv.github.io/master/assets/img/nnogada_output.png)
-
-## Description of this repository
-
-- nnogada folder has the source code of the neural approximator with genetic algorithms.
-- In data folder we have some data used in tests. 
-- example_1.py is a classification task of galaxies, quasars and stars from SDSS using a keras neural model.
-- example_2.py is a regression task with SNeIa using a keras neural model.
-- example_3.py is the same as example_2.py but with a torch neural model.
-
-## TODO 
 
-- Include convolutional, recurrent neural networks and other architectures.
-- To allow pytorch models for classification.
```

### Comparing `nnogada-0.9.1/nnogada.egg-info/PKG-INFO` & `nnogada-0.9.1.1/nnogada.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnogada
-Version: 0.9.1
+Version: 0.9.1.1
 Summary: Genetic hyperparameter tuning for neural nets
 Home-page: https://github.com/igomezv/nnogada
 Author: I Gomez-Vargas
 Author-email: igomez@icf.unam.mx
 License: MIT
 Keywords: Hyperparameter,optimization,machine learning,deep learning,genetic algorithms
 Platform: UNKNOWN
@@ -16,23 +16,21 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English
 License-File: LICENSE
 
-[<img src="https://img.shields.io/badge/astro--ph.IM-%20%09arXiv%3A2209.02685-green.svg">](https://arxiv.org/abs/2209.02685)
-
 # Neural Networks Optimized by Genetic Algorithms for Data Analysis (NNOGADA) 
 
 **nnogada** is a Python package that performs hyperparemeter tuning for artificial neural networks, particularly for Multi Layer Perceptrons, using simple genetic algorithms. Useful for generate better neural network models for data analysis. Currently, only works with feedforward neural networks in tensorflow.keras (classification and regression) and torch (regression at this moment).
 
 Before use the code, please install the requirements:
 
-    $ pip3 install -r requiriments.txt
+    $ pip3 install nnogada
  
 Or you can try to install nnogada in your computer:
 
      $ git clone https://github.com/igomezv/nnogada
 
      $ cd nnogada
 
@@ -40,27 +38,13 @@
 
 then you can delete the cloned repo because you must have nnogada installed locally.
 
 Other way to install nnogada (without clonning) is:
 
     $ pip3 install -e git+https://github.com/igomezv/nnogada#egg=nnogada
 
-
 If you use the code, please cite the paper *Gómez-Vargas, I., Andrade, J. B., & Vázquez, J. A. (2023). Neural networks optimized by genetic algorithms in cosmology. Physical Review D, 107(4), 043509.*
 
 Contributions are welcome!
 
-![](https://raw.githubusercontent.com/igomezv/igomezv.github.io/master/assets/img/nnogada_output.png)
-
-## Description of this repository
-
-- nnogada folder has the source code of the neural approximator with genetic algorithms.
-- In data folder we have some data used in tests. 
-- example_1.py is a classification task of galaxies, quasars and stars from SDSS using a keras neural model.
-- example_2.py is a regression task with SNeIa using a keras neural model.
-- example_3.py is the same as example_2.py but with a torch neural model.
-
-## TODO 
 
-- Include convolutional, recurrent neural networks and other architectures.
-- To allow pytorch models for classification.
```

### Comparing `nnogada-0.9.1/setup.py` & `nnogada-0.9.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     desc = fh.read()
 
 required = ["numpy", "scipy", "sklearn", "tensorflow", "deap", "bitstring", "pandas",
             "torch", "torchinfo", "torch_optimizer", "tqdm"]
 
 setup(
     name="nnogada",
-    version='0.9.1',
+    version='0.9.1.1',
     author='I Gomez-Vargas',
     author_email="igomez@icf.unam.mx",
     url="https://github.com/igomezv/nnogada",
     license="MIT",
     description="Genetic hyperparameter tuning for neural nets",
     long_description=desc,
     install_requires=required,
```

