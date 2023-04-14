# Comparing `tmp/mosaic-clustering-0.4.0.tar.gz` & `tmp/mosaic-clustering-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaic-clustering-0.4.0.tar", last modified: Tue Mar 28 16:46:25 2023, max compression
+gzip compressed data, was "mosaic-clustering-0.4.1.tar", last modified: Fri Apr 14 09:13:50 2023, max compression
```

## Comparing `mosaic-clustering-0.4.0.tar` & `mosaic-clustering-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:46:25.095890 mosaic-clustering-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-03-28 16:46:25.095890 mosaic-clustering-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/extra-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-28 16:46:25.099890 mosaic-clustering-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:46:25.087890 mosaic-clustering-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:46:25.091890 mosaic-clustering-0.4.0/src/mosaic/
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/src/mosaic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/src/mosaic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/src/mosaic/_correlation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/src/mosaic/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/src/mosaic/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/src/mosaic/gridsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/src/mosaic/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/src/mosaic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:46:25.095890 mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8728 2023-03-28 16:46:25.000000 mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-28 16:46:25.000000 mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 16:46:25.000000 mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-28 16:46:25.000000 mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-28 16:46:25.000000 mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-28 16:46:25.000000 mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:46:25.095890 mosaic-clustering-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/tests/test___main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/tests/test__correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/tests/test_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/tests/test_gridsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/tests/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-28 16:46:10.000000 mosaic-clustering-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:13:50.776984 mosaic-clustering-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-04-14 09:13:50.776984 mosaic-clustering-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/extra-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-14 09:13:50.776984 mosaic-clustering-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:13:50.768984 mosaic-clustering-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:13:50.772984 mosaic-clustering-0.4.1/src/mosaic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/src/mosaic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/src/mosaic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/src/mosaic/_correlation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/src/mosaic/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/src/mosaic/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/src/mosaic/gridsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/src/mosaic/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/src/mosaic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:13:50.772984 mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-04-14 09:13:50.000000 mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 09:13:50.000000 mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:13:50.000000 mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 09:13:50.000000 mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-14 09:13:50.000000 mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 09:13:50.000000 mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:13:50.776984 mosaic-clustering-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/tests/test___main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/tests/test__correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/tests/test_gridsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/tests/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-14 09:13:39.000000 mosaic-clustering-0.4.1/tests/test_utils.py
```

### Comparing `mosaic-clustering-0.4.0/LICENSE` & `mosaic-clustering-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/PKG-INFO` & `mosaic-clustering-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaic-clustering
-Version: 0.4.0
+Version: 0.4.1
 Summary: Correlation based feature selection for MD data
 Home-page: https://github.com/moldyn/feature_selection
 Author: braniii
 License: BSD 3-Clause License
 Project-URL: Documentation, https://moldyn.github.io/MoSAIC
 Project-URL: Source Code, https://github.com/moldyn/MoSAIC
 Project-URL: Bug Tracker, https://github.com/moldyn/MoSAIC/issues
@@ -125,36 +125,35 @@
 
 ### CI - Usage Directly from the Command Line
 The module brings a rich CI using [click](https://click.palletsprojects.com). Each module and submodule contains a detailed help, which can be accessed by
 ```bash
 $ python -m mosaic
 Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]...
 
-  MoSAIC motion v0.3.2
+  MoSAIC motion v0.4.1
 
   Molecular systems automated identification of collective motion, is
   a correlation based feature selection framework for MD data.
   Copyright (c) 2021-2023, Georg Diez and Daniel Nagel
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   clustering  Clustering similarity matrix of coordinates.
   similarity  Creating similarity matrix of coordinates.
-  umap        Embedd similarity matrix with UMAP.
 ```
 For more details on the submodule one needs to specify one of the three
 commands.
 
 A simple workflow example for clustering the input file `input_file` using
 correlation and Leiden with CPM and the default resolution parameter:
 ```bash
 # creating correlation matrix
-$ python -m mosaic similarity -i input_file -o output_similarity -metric correlation -v
+$ python -m mosaic similarity -i input_file -o output_similarity --metric correlation -v
 
 MoSAIC SIMILARITY
 ~~~ Initialize similarity class
 ~~~ Load file input_file
 ~~~ Fit input
 ~~~ Store similarity matrix in output_similarity
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaic-clustering Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: mosaic-clustering Version: 0.4.1 Summary:
 Correlation based feature selection for MD data Home-page: https://github.com/
 moldyn/feature_selection Author: braniii License: BSD 3-Clause License Project-
 URL: Documentation, https://moldyn.github.io/MoSAIC Project-URL: Source Code,
 https://github.com/moldyn/MoSAIC Project-URL: Bug Tracker, https://github.com/
 moldyn/MoSAIC/issues Keywords: feature selection,MD analysis Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Intended Audience :: Science/Research Classifier:
@@ -64,32 +64,32 @@
 (_MOSAIC_COMPLETE=bash_source mosaic)" ``` ## Usage In general one can call the
 module directly by its entry point `$ MoSAIC` or by calling the module `$
 python -m mosaic`. The latter method is preferred to ensure using the desired
 python environment. For enabling the shell completion, the entry point needs to
 be used. ### CI - Usage Directly from the Command Line The module brings a rich
 CI using [click](https://click.palletsprojects.com). Each module and submodule
 contains a detailed help, which can be accessed by ```bash $ python -m mosaic
-Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]... MoSAIC motion v0.3.2
+Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]... MoSAIC motion v0.4.1
 Molecular systems automated identification of collective motion, is a
 correlation based feature selection framework for MD data. Copyright (c) 2021-
 2023, Georg Diez and Daniel Nagel Options: --help Show this message and exit.
 Commands: clustering Clustering similarity matrix of coordinates. similarity
-Creating similarity matrix of coordinates. umap Embedd similarity matrix with
-UMAP. ``` For more details on the submodule one needs to specify one of the
-three commands. A simple workflow example for clustering the input file
-`input_file` using correlation and Leiden with CPM and the default resolution
-parameter: ```bash # creating correlation matrix $ python -m mosaic similarity
--i input_file -o output_similarity -metric correlation -v MoSAIC SIMILARITY ~~~
-Initialize similarity class ~~~ Load file input_file ~~~ Fit input ~~~ Store
-similarity matrix in output_similarity # clustering with CPM and default
-resolution parameter # the latter needs to be fine-tuned to each matrix $
-python -m mosaic clustering -i output_similarity -o output_clustering --plot -
-v MoSAIC CLUSTERING ~~~ Initialize clustering class ~~~ Load file
-output_similarity ~~~ Fit input ~~~ Store output ~~~ Plot matrix ``` This will
-generate the similarity matrix stored in `output_similarity`, the plotted
-result in `output_clustering.matrix.pdf`, the raw data of the matrix in
+Creating similarity matrix of coordinates. ``` For more details on the
+submodule one needs to specify one of the three commands. A simple workflow
+example for clustering the input file `input_file` using correlation and Leiden
+with CPM and the default resolution parameter: ```bash # creating correlation
+matrix $ python -m mosaic similarity -i input_file -o output_similarity --
+metric correlation -v MoSAIC SIMILARITY ~~~ Initialize similarity class ~~~
+Load file input_file ~~~ Fit input ~~~ Store similarity matrix in
+output_similarity # clustering with CPM and default resolution parameter # the
+latter needs to be fine-tuned to each matrix $ python -m mosaic clustering -
+i output_similarity -o output_clustering --plot -v MoSAIC CLUSTERING ~~~
+Initialize clustering class ~~~ Load file output_similarity ~~~ Fit input ~~~
+Store output ~~~ Plot matrix ``` This will generate the similarity matrix
+stored in `output_similarity`, the plotted result in
+`output_clustering.matrix.pdf`, the raw data of the matrix in
 `output_clustering.matrix` and a file containing in each row the indices of a
 cluster. ### Module - Inside a Python Script ```python import mosaic # Load
 file # X is np.ndarray of shape (n_samples, n_features) sim = mosaic.Similarity
 ( metric='correlation', # or 'NMI', 'GY', 'JSD' ) sim.fit(X) # Cluster matrix
 clust = mosaic.Clustering( mode='CPM', # or 'modularity ) clust.fit
 (sim.matrix_) clusters = clust.clusters_ clusterd_X = clust.matrix_ ... ```
```

### Comparing `mosaic-clustering-0.4.0/README.md` & `mosaic-clustering-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -95,36 +95,35 @@
 
 ### CI - Usage Directly from the Command Line
 The module brings a rich CI using [click](https://click.palletsprojects.com). Each module and submodule contains a detailed help, which can be accessed by
 ```bash
 $ python -m mosaic
 Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]...
 
-  MoSAIC motion v0.3.2
+  MoSAIC motion v0.4.1
 
   Molecular systems automated identification of collective motion, is
   a correlation based feature selection framework for MD data.
   Copyright (c) 2021-2023, Georg Diez and Daniel Nagel
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   clustering  Clustering similarity matrix of coordinates.
   similarity  Creating similarity matrix of coordinates.
-  umap        Embedd similarity matrix with UMAP.
 ```
 For more details on the submodule one needs to specify one of the three
 commands.
 
 A simple workflow example for clustering the input file `input_file` using
 correlation and Leiden with CPM and the default resolution parameter:
 ```bash
 # creating correlation matrix
-$ python -m mosaic similarity -i input_file -o output_similarity -metric correlation -v
+$ python -m mosaic similarity -i input_file -o output_similarity --metric correlation -v
 
 MoSAIC SIMILARITY
 ~~~ Initialize similarity class
 ~~~ Load file input_file
 ~~~ Fit input
 ~~~ Store similarity matrix in output_similarity
```

#### html2text {}

```diff
@@ -48,32 +48,32 @@
 (_MOSAIC_COMPLETE=bash_source mosaic)" ``` ## Usage In general one can call the
 module directly by its entry point `$ MoSAIC` or by calling the module `$
 python -m mosaic`. The latter method is preferred to ensure using the desired
 python environment. For enabling the shell completion, the entry point needs to
 be used. ### CI - Usage Directly from the Command Line The module brings a rich
 CI using [click](https://click.palletsprojects.com). Each module and submodule
 contains a detailed help, which can be accessed by ```bash $ python -m mosaic
-Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]... MoSAIC motion v0.3.2
+Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]... MoSAIC motion v0.4.1
 Molecular systems automated identification of collective motion, is a
 correlation based feature selection framework for MD data. Copyright (c) 2021-
 2023, Georg Diez and Daniel Nagel Options: --help Show this message and exit.
 Commands: clustering Clustering similarity matrix of coordinates. similarity
-Creating similarity matrix of coordinates. umap Embedd similarity matrix with
-UMAP. ``` For more details on the submodule one needs to specify one of the
-three commands. A simple workflow example for clustering the input file
-`input_file` using correlation and Leiden with CPM and the default resolution
-parameter: ```bash # creating correlation matrix $ python -m mosaic similarity
--i input_file -o output_similarity -metric correlation -v MoSAIC SIMILARITY ~~~
-Initialize similarity class ~~~ Load file input_file ~~~ Fit input ~~~ Store
-similarity matrix in output_similarity # clustering with CPM and default
-resolution parameter # the latter needs to be fine-tuned to each matrix $
-python -m mosaic clustering -i output_similarity -o output_clustering --plot -
-v MoSAIC CLUSTERING ~~~ Initialize clustering class ~~~ Load file
-output_similarity ~~~ Fit input ~~~ Store output ~~~ Plot matrix ``` This will
-generate the similarity matrix stored in `output_similarity`, the plotted
-result in `output_clustering.matrix.pdf`, the raw data of the matrix in
+Creating similarity matrix of coordinates. ``` For more details on the
+submodule one needs to specify one of the three commands. A simple workflow
+example for clustering the input file `input_file` using correlation and Leiden
+with CPM and the default resolution parameter: ```bash # creating correlation
+matrix $ python -m mosaic similarity -i input_file -o output_similarity --
+metric correlation -v MoSAIC SIMILARITY ~~~ Initialize similarity class ~~~
+Load file input_file ~~~ Fit input ~~~ Store similarity matrix in
+output_similarity # clustering with CPM and default resolution parameter # the
+latter needs to be fine-tuned to each matrix $ python -m mosaic clustering -
+i output_similarity -o output_clustering --plot -v MoSAIC CLUSTERING ~~~
+Initialize clustering class ~~~ Load file output_similarity ~~~ Fit input ~~~
+Store output ~~~ Plot matrix ``` This will generate the similarity matrix
+stored in `output_similarity`, the plotted result in
+`output_clustering.matrix.pdf`, the raw data of the matrix in
 `output_clustering.matrix` and a file containing in each row the indices of a
 cluster. ### Module - Inside a Python Script ```python import mosaic # Load
 file # X is np.ndarray of shape (n_samples, n_features) sim = mosaic.Similarity
 ( metric='correlation', # or 'NMI', 'GY', 'JSD' ) sim.fit(X) # Cluster matrix
 clust = mosaic.Clustering( mode='CPM', # or 'modularity ) clust.fit
 (sim.matrix_) clusters = clust.clusters_ clusterd_X = clust.matrix_ ... ```
```

### Comparing `mosaic-clustering-0.4.0/extra-requirements.txt` & `mosaic-clustering-0.4.1/extra-requirements.txt`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/setup.cfg` & `mosaic-clustering-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/setup.py` & `mosaic-clustering-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 README = remove_gh_dark_mode_only_tags(
     (HERE / 'README.md').read_text(),
 )
 
 # This call to setup() does all the work
 setuptools.setup(
     name='mosaic-clustering',
-    version='0.4.0',
+    version='0.4.1',
     description='Correlation based feature selection for MD data',
     long_description=README,
     long_description_content_type='text/markdown',
     keywords=[
         'feature selection',
         'MD analysis',
     ],
@@ -104,11 +104,11 @@
         'scipy',
         'scikit-learn',
         'scikit-learn-extra',
         'igraph',
         'leidenalg>=0.8.0',
         'click>=7.0.0',
         'typing_extensions>=3.9.0;python_version<"3.9"',
-        'prettypyplot',
+        'matplotlib>=3.5',
     ],
     extras_require=get_extra_requirements('extra-requirements.txt'),
 )
```

### Comparing `mosaic-clustering-0.4.0/src/mosaic/__init__.py` & `mosaic-clustering-0.4.1/src/mosaic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 
 import mosaic.utils  # noqa: F401
 from .clustering import Clustering
 from .gridsearch import GridSearchCV
 from .similarity import Similarity
 
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
```

### Comparing `mosaic-clustering-0.4.0/src/mosaic/__main__.py` & `mosaic-clustering-0.4.1/src/mosaic/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 Copyright (c) 2021-2022, Daniel Nagel
 All rights reserved.
 
 """
 import click
 import numpy as np
 import pandas as pd
-import prettypyplot as pplt
 from matplotlib import pyplot as plt
 
 import mosaic
 from mosaic.utils import save_clusters, savetxt
 
 # setup matplotlibs rcParam
-pplt.use_style(figsize=2, figratio=1, cmap='turbo')
 
 PRECISION = ['half', 'single', 'double']
 PRECISION_TO_DTYPE = {
     'half': np.float16,
     'single': np.float32,
     'double': np.float64,
 }
@@ -327,16 +325,16 @@
     if plot:
         if verbose:
             click.echo('~~~ Plot matrix')
 
         _, ax = plt.subplots()
         mat = clust.matrix_.astype(np.float64)
         mat[np.diag_indices_from(mat)] = np.nan
-        im = ax.imshow(
-            mat, aspect='equal', origin='upper', interpolation='none',
+        im = ax.pcolormesh(
+            mat, snap=True, vim=0, vmax=np.nanmax(mat),
         )
 
         ticks = np.array([0, *clust.ticks_[: -1]]) - 0.5
         major_mask = np.array([
             len(cluster) > 2 for cluster in clust.clusters_
         ])
         ticklabels = np.arange(len(ticks)) + 1
@@ -345,19 +343,19 @@
             (ax.set_yticks, ax.set_yticklabels),
         ):
             set_ticks(ticks[major_mask])
             set_ticklabels(ticklabels[major_mask])
             set_ticks(ticks[~major_mask], minor=True)
             set_ticklabels([], minor=True)
 
-        ax.grid(b=True, ls='-', lw=0.5)
-        ax.grid(b=True, ls='-', which='minor', lw=0.1)
+        ax.grid(True, ls='-', lw=0.5)
+        ax.grid(True, ls='-', which='minor', lw=0.1)
 
         ax.set_xlabel('clusters')
         ax.set_ylabel('clusters')
 
-        pplt.colorbar(im, width='3%')
-        pplt.savefig(f'{output_file}.matrix.pdf')
+        plt.colorbar(im, width='3%')
+        plt.savefig(f'{output_file}.matrix.pdf')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `mosaic-clustering-0.4.0/src/mosaic/_correlation_utils.py` & `mosaic-clustering-0.4.1/src/mosaic/_correlation_utils.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/src/mosaic/_typing.py` & `mosaic-clustering-0.4.1/src/mosaic/_typing.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/src/mosaic/clustering.py` & `mosaic-clustering-0.4.1/src/mosaic/clustering.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/src/mosaic/gridsearch.py` & `mosaic-clustering-0.4.1/src/mosaic/gridsearch.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/src/mosaic/similarity.py` & `mosaic-clustering-0.4.1/src/mosaic/similarity.py`

 * *Files 6% similar despite different names*

```diff
@@ -194,14 +194,22 @@
             raise TypeError('Using low_memory=True requires X:str')
         if X.ndim == 1:
             raise ValueError(
                 'Reshape your data either using array.reshape(-1, 1) if your '
                 'data has a single feature or array.reshape(1, -1) if it '
                 'contains a single sample.',
             )
+        std_devs = np.std(X, axis=0)
+        if np.any(std_devs == 0) or np.any(np.isnan(std_devs)):
+            raise ValueError(
+                'At lease one column has a zero or NaN standard deviation.'
+                'As the standard deviation for each feature should be non-zero'
+                'and finite delete this column or change the feature'
+                'accordingly.'
+            )
 
         n_samples, n_features = X.shape
         self._n_samples: int = n_samples
         self._n_features: int = n_features
 
         X: np.ndarray = _standard_scaler(X)
         if self.metric == 'correlation':
@@ -220,15 +228,15 @@
         """Dispatched for low_memory=True with string."""
         self._reset()
 
         corr: np.ndarray
         matrix_: np.ndarray
         # parse data
         if not self.low_memory:
-            raise TypeError('Mode low_memory=False reuqires X:np.ndarray.')
+            raise TypeError('Mode low_memory=False requires X:np.ndarray.')
 
         if self.metric == 'correlation':
             corr = self._online_correlation(X)
             matrix_ = np.abs(corr)
         else:
             raise NotImplementedError(
                 'Mode low_memory=True is only implemented for correlation.',
```

### Comparing `mosaic-clustering-0.4.0/src/mosaic/utils.py` & `mosaic-clustering-0.4.1/src/mosaic/utils.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/PKG-INFO` & `mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaic-clustering
-Version: 0.4.0
+Version: 0.4.1
 Summary: Correlation based feature selection for MD data
 Home-page: https://github.com/moldyn/feature_selection
 Author: braniii
 License: BSD 3-Clause License
 Project-URL: Documentation, https://moldyn.github.io/MoSAIC
 Project-URL: Source Code, https://github.com/moldyn/MoSAIC
 Project-URL: Bug Tracker, https://github.com/moldyn/MoSAIC/issues
@@ -125,36 +125,35 @@
 
 ### CI - Usage Directly from the Command Line
 The module brings a rich CI using [click](https://click.palletsprojects.com). Each module and submodule contains a detailed help, which can be accessed by
 ```bash
 $ python -m mosaic
 Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]...
 
-  MoSAIC motion v0.3.2
+  MoSAIC motion v0.4.1
 
   Molecular systems automated identification of collective motion, is
   a correlation based feature selection framework for MD data.
   Copyright (c) 2021-2023, Georg Diez and Daniel Nagel
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   clustering  Clustering similarity matrix of coordinates.
   similarity  Creating similarity matrix of coordinates.
-  umap        Embedd similarity matrix with UMAP.
 ```
 For more details on the submodule one needs to specify one of the three
 commands.
 
 A simple workflow example for clustering the input file `input_file` using
 correlation and Leiden with CPM and the default resolution parameter:
 ```bash
 # creating correlation matrix
-$ python -m mosaic similarity -i input_file -o output_similarity -metric correlation -v
+$ python -m mosaic similarity -i input_file -o output_similarity --metric correlation -v
 
 MoSAIC SIMILARITY
 ~~~ Initialize similarity class
 ~~~ Load file input_file
 ~~~ Fit input
 ~~~ Store similarity matrix in output_similarity
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaic-clustering Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: mosaic-clustering Version: 0.4.1 Summary:
 Correlation based feature selection for MD data Home-page: https://github.com/
 moldyn/feature_selection Author: braniii License: BSD 3-Clause License Project-
 URL: Documentation, https://moldyn.github.io/MoSAIC Project-URL: Source Code,
 https://github.com/moldyn/MoSAIC Project-URL: Bug Tracker, https://github.com/
 moldyn/MoSAIC/issues Keywords: feature selection,MD analysis Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Intended Audience :: Science/Research Classifier:
@@ -64,32 +64,32 @@
 (_MOSAIC_COMPLETE=bash_source mosaic)" ``` ## Usage In general one can call the
 module directly by its entry point `$ MoSAIC` or by calling the module `$
 python -m mosaic`. The latter method is preferred to ensure using the desired
 python environment. For enabling the shell completion, the entry point needs to
 be used. ### CI - Usage Directly from the Command Line The module brings a rich
 CI using [click](https://click.palletsprojects.com). Each module and submodule
 contains a detailed help, which can be accessed by ```bash $ python -m mosaic
-Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]... MoSAIC motion v0.3.2
+Usage: python -m mosaic [OPTIONS] COMMAND [ARGS]... MoSAIC motion v0.4.1
 Molecular systems automated identification of collective motion, is a
 correlation based feature selection framework for MD data. Copyright (c) 2021-
 2023, Georg Diez and Daniel Nagel Options: --help Show this message and exit.
 Commands: clustering Clustering similarity matrix of coordinates. similarity
-Creating similarity matrix of coordinates. umap Embedd similarity matrix with
-UMAP. ``` For more details on the submodule one needs to specify one of the
-three commands. A simple workflow example for clustering the input file
-`input_file` using correlation and Leiden with CPM and the default resolution
-parameter: ```bash # creating correlation matrix $ python -m mosaic similarity
--i input_file -o output_similarity -metric correlation -v MoSAIC SIMILARITY ~~~
-Initialize similarity class ~~~ Load file input_file ~~~ Fit input ~~~ Store
-similarity matrix in output_similarity # clustering with CPM and default
-resolution parameter # the latter needs to be fine-tuned to each matrix $
-python -m mosaic clustering -i output_similarity -o output_clustering --plot -
-v MoSAIC CLUSTERING ~~~ Initialize clustering class ~~~ Load file
-output_similarity ~~~ Fit input ~~~ Store output ~~~ Plot matrix ``` This will
-generate the similarity matrix stored in `output_similarity`, the plotted
-result in `output_clustering.matrix.pdf`, the raw data of the matrix in
+Creating similarity matrix of coordinates. ``` For more details on the
+submodule one needs to specify one of the three commands. A simple workflow
+example for clustering the input file `input_file` using correlation and Leiden
+with CPM and the default resolution parameter: ```bash # creating correlation
+matrix $ python -m mosaic similarity -i input_file -o output_similarity --
+metric correlation -v MoSAIC SIMILARITY ~~~ Initialize similarity class ~~~
+Load file input_file ~~~ Fit input ~~~ Store similarity matrix in
+output_similarity # clustering with CPM and default resolution parameter # the
+latter needs to be fine-tuned to each matrix $ python -m mosaic clustering -
+i output_similarity -o output_clustering --plot -v MoSAIC CLUSTERING ~~~
+Initialize clustering class ~~~ Load file output_similarity ~~~ Fit input ~~~
+Store output ~~~ Plot matrix ``` This will generate the similarity matrix
+stored in `output_similarity`, the plotted result in
+`output_clustering.matrix.pdf`, the raw data of the matrix in
 `output_clustering.matrix` and a file containing in each row the indices of a
 cluster. ### Module - Inside a Python Script ```python import mosaic # Load
 file # X is np.ndarray of shape (n_samples, n_features) sim = mosaic.Similarity
 ( metric='correlation', # or 'NMI', 'GY', 'JSD' ) sim.fit(X) # Cluster matrix
 clust = mosaic.Clustering( mode='CPM', # or 'modularity ) clust.fit
 (sim.matrix_) clusters = clust.clusters_ clusterd_X = clust.matrix_ ... ```
```

### Comparing `mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/SOURCES.txt` & `mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/src/mosaic_clustering.egg-info/requires.txt` & `mosaic-clustering-0.4.1/src/mosaic_clustering.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 beartype>=0.10.4
 scipy
 scikit-learn
 scikit-learn-extra
 igraph
 leidenalg>=0.8.0
 click>=7.0.0
-prettypyplot
+matplotlib>=3.5
 
 [:python_version < "3.9"]
 typing_extensions>=3.9.0
 
 [all]
-mkdocs-material
-mkdocs-literate-nav
-pytest
-mkdocs-gen-files
 pytest-cov
-mkdocs-click
+mkdocs-literate-nav
+mkdocs-material
 mkdocs-section-index
-mkdocstrings
-jupyter_contrib_nbextensions
+flake8
 pytest-rerunfailures
 mkdocs-jupyter
-flake8
 mkdocstrings-python
+mkdocs-click
+jupyter_contrib_nbextensions
+mkdocstrings
+pytest
+mkdocs-gen-files
 
 [docs]
-mkdocs-material
 mkdocs-literate-nav
-mkdocs-gen-files
+mkdocs-material
 mkdocs-section-index
-mkdocstrings
-jupyter_contrib_nbextensions
 mkdocs-jupyter
-mkdocs-click
 mkdocstrings-python
+mkdocs-click
+jupyter_contrib_nbextensions
+mkdocstrings
+mkdocs-gen-files
 
 [testing]
-pytest
-flake8
 pytest-cov
 pytest-rerunfailures
+pytest
+flake8
```

### Comparing `mosaic-clustering-0.4.0/tests/test___main__.py` & `mosaic-clustering-0.4.1/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/tests/test__correlation.py` & `mosaic-clustering-0.4.1/tests/test__correlation.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/tests/test_clustering.py` & `mosaic-clustering-0.4.1/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/tests/test_gridsearch.py` & `mosaic-clustering-0.4.1/tests/test_gridsearch.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/tests/test_similarity.py` & `mosaic-clustering-0.4.1/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `mosaic-clustering-0.4.0/tests/test_utils.py` & `mosaic-clustering-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

