# Comparing `tmp/mlblocks-0.5.1.dev0.tar.gz` & `tmp/mlblocks-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlblocks-0.5.1.dev0.tar", last modified: Fri Apr 14 18:27:51 2023, max compression
+gzip compressed data, was "mlblocks-0.6.0.tar", last modified: Fri Apr 14 19:21:35 2023, max compression
```

## Comparing `mlblocks-0.5.1.dev0.tar` & `mlblocks-0.6.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.192095 mlblocks-0.5.1.dev0/
--rw-r--r--   0 sarah      (501) staff       (20)      268 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/AUTHORS.rst
--rw-r--r--   0 sarah      (501) staff       (20)     7923 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)     6951 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/HISTORY.md
--rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)      299 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/MANIFEST.in
--rw-r--r--   0 sarah      (501) staff       (20)    14133 2023-04-14 18:27:51.192312 mlblocks-0.5.1.dev0/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     6124 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/README.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.166828 mlblocks-0.5.1.dev0/docs/
--rw-r--r--   0 sarah      (501) staff       (20)      609 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/Makefile
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.168883 mlblocks-0.5.1.dev0/docs/advanced_usage/
--rw-r--r--   0 sarah      (501) staff       (20)     4471 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/advanced_usage/adding_primitives.rst
--rw-r--r--   0 sarah      (501) staff       (20)     8503 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/advanced_usage/hyperparameters.rst
--rw-r--r--   0 sarah      (501) staff       (20)    17648 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/advanced_usage/pipelines.rst
--rw-r--r--   0 sarah      (501) staff       (20)    12082 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/advanced_usage/primitives.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.169324 mlblocks-0.5.1.dev0/docs/api/
--rw-r--r--   0 sarah      (501) staff       (20)       58 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/api/mlblocks.rst
--rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/authors.rst
--rw-r--r--   0 sarah      (501) staff       (20)       29 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/changelog.rst
--rwxr-xr-x   0 sarah      (501) staff       (20)     6038 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/conf.py
--rw-r--r--   0 sarah      (501) staff       (20)       33 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/contributing.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.170321 mlblocks-0.5.1.dev0/docs/getting_started/
--rw-r--r--   0 sarah      (501) staff       (20)     1252 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/getting_started/install.rst
--rw-r--r--   0 sarah      (501) staff       (20)     4535 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/getting_started/quickstart.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.171913 mlblocks-0.5.1.dev0/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)      437 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/images/mlblocks-icon.png
--rw-r--r--   0 sarah      (501) staff       (20)     3857 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/images/mlblocks-logo-small.png
--rw-r--r--   0 sarah      (501) staff       (20)    12140 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/images/mlblocks-logo.png
--rw-r--r--   0 sarah      (501) staff       (20)     4317 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/index.rst
--rw-r--r--   0 sarah      (501) staff       (20)      770 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/make.bat
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.174364 mlblocks-0.5.1.dev0/docs/pipeline_examples/
--rw-r--r--   0 sarah      (501) staff       (20)     2967 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/graph.rst
--rw-r--r--   0 sarah      (501) staff       (20)     4872 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/image.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2038 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/multi_table.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2889 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/single_table.rst
--rw-r--r--   0 sarah      (501) staff       (20)     5191 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/text.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.178181 mlblocks-0.5.1.dev0/mlblocks/
--rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/mlblocks/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)    14156 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/mlblocks/discovery.py
--rw-r--r--   0 sarah      (501) staff       (20)    11931 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/mlblocks/mlblock.py
--rw-r--r--   0 sarah      (501) staff       (20)    54563 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/mlblocks/mlpipeline.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.183275 mlblocks-0.5.1.dev0/mlblocks.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)    14133 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     1324 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/dependency_links.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)     1170 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)        9 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/top_level.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1155 2023-04-14 18:27:51.193296 mlblocks-0.5.1.dev0/setup.cfg
--rw-r--r--   0 sarah      (501) staff       (20)     3135 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/setup.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.186418 mlblocks-0.5.1.dev0/tests/
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/__init__.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.160306 mlblocks-0.5.1.dev0/tests/data/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.189514 mlblocks-0.5.1.dev0/tests/data/diagrams/
--rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_fit.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1440 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_multiple_blocks.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_simple.txt
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.191636 mlblocks-0.5.1.dev0/tests/features/
--rw-r--r--   0 sarah      (501) staff       (20)      845 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/features/test_fit_predicr_args.py
--rw-r--r--   0 sarah      (501) staff       (20)     4481 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/features/test_partial_outputs.py
--rw-r--r--   0 sarah      (501) staff       (20)     2977 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/features/test_pipeline_loading.py
--rw-r--r--   0 sarah      (501) staff       (20)    10345 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/test_discovery.py
--rw-r--r--   0 sarah      (501) staff       (20)    14919 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/test_mlblock.py
--rw-r--r--   0 sarah      (501) staff       (20)    36889 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/test_mlpipeline.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.697346 mlblocks-0.6.0/
+-rw-r--r--   0 sarah      (501) staff       (20)      268 2023-04-14 18:14:02.000000 mlblocks-0.6.0/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7923 2023-04-14 18:14:02.000000 mlblocks-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7099 2023-04-14 19:21:31.000000 mlblocks-0.6.0/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-04-14 18:14:02.000000 mlblocks-0.6.0/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      299 2023-04-14 18:14:02.000000 mlblocks-0.6.0/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)    14276 2023-04-14 19:21:35.697638 mlblocks-0.6.0/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     6124 2023-04-14 19:21:31.000000 mlblocks-0.6.0/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.664322 mlblocks-0.6.0/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      609 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/Makefile
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.667280 mlblocks-0.6.0/docs/advanced_usage/
+-rw-r--r--   0 sarah      (501) staff       (20)     4471 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/advanced_usage/adding_primitives.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     8503 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/advanced_usage/hyperparameters.rst
+-rw-r--r--   0 sarah      (501) staff       (20)    17648 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/advanced_usage/pipelines.rst
+-rw-r--r--   0 sarah      (501) staff       (20)    12082 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/advanced_usage/primitives.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.667850 mlblocks-0.6.0/docs/api/
+-rw-r--r--   0 sarah      (501) staff       (20)       58 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/api/mlblocks.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/authors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/changelog.rst
+-rwxr-xr-x   0 sarah      (501) staff       (20)     6038 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/conf.py
+-rw-r--r--   0 sarah      (501) staff       (20)       33 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/contributing.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.669236 mlblocks-0.6.0/docs/getting_started/
+-rw-r--r--   0 sarah      (501) staff       (20)     1252 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/getting_started/install.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     4535 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/getting_started/quickstart.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.671821 mlblocks-0.6.0/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)      437 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/images/mlblocks-icon.png
+-rw-r--r--   0 sarah      (501) staff       (20)     3857 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/images/mlblocks-logo-small.png
+-rw-r--r--   0 sarah      (501) staff       (20)    12140 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/images/mlblocks-logo.png
+-rw-r--r--   0 sarah      (501) staff       (20)     4317 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      770 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/make.bat
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.676525 mlblocks-0.6.0/docs/pipeline_examples/
+-rw-r--r--   0 sarah      (501) staff       (20)     2967 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/pipeline_examples/graph.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     4872 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/pipeline_examples/image.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2038 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/pipeline_examples/multi_table.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2889 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/pipeline_examples/single_table.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5191 2023-04-14 18:14:02.000000 mlblocks-0.6.0/docs/pipeline_examples/text.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.680279 mlblocks-0.6.0/mlblocks/
+-rw-r--r--   0 sarah      (501) staff       (20)     1009 2023-04-14 19:21:31.000000 mlblocks-0.6.0/mlblocks/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)    14156 2023-04-14 18:14:02.000000 mlblocks-0.6.0/mlblocks/discovery.py
+-rw-r--r--   0 sarah      (501) staff       (20)    11931 2023-04-14 18:14:02.000000 mlblocks-0.6.0/mlblocks/mlblock.py
+-rw-r--r--   0 sarah      (501) staff       (20)    54563 2023-04-14 18:14:02.000000 mlblocks-0.6.0/mlblocks/mlpipeline.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.685156 mlblocks-0.6.0/mlblocks.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)    14276 2023-04-14 19:21:35.000000 mlblocks-0.6.0/mlblocks.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     1324 2023-04-14 19:21:35.000000 mlblocks-0.6.0/mlblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-14 19:21:35.000000 mlblocks-0.6.0/mlblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-14 19:21:35.000000 mlblocks-0.6.0/mlblocks.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)     1170 2023-04-14 19:21:35.000000 mlblocks-0.6.0/mlblocks.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        9 2023-04-14 19:21:35.000000 mlblocks-0.6.0/mlblocks.egg-info/top_level.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1150 2023-04-14 19:21:35.699074 mlblocks-0.6.0/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     3130 2023-04-14 19:21:31.000000 mlblocks-0.6.0/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.688841 mlblocks-0.6.0/tests/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.654357 mlblocks-0.6.0/tests/data/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.692726 mlblocks-0.6.0/tests/data/diagrams/
+-rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/data/diagrams/diagram_fit.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1440 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/data/diagrams/diagram_multiple_blocks.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/data/diagrams/diagram_simple.txt
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 19:21:35.696628 mlblocks-0.6.0/tests/features/
+-rw-r--r--   0 sarah      (501) staff       (20)      845 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/features/test_fit_predicr_args.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4481 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/features/test_partial_outputs.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2977 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/features/test_pipeline_loading.py
+-rw-r--r--   0 sarah      (501) staff       (20)    10345 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/test_discovery.py
+-rw-r--r--   0 sarah      (501) staff       (20)    14919 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/test_mlblock.py
+-rw-r--r--   0 sarah      (501) staff       (20)    36889 2023-04-14 18:14:02.000000 mlblocks-0.6.0/tests/test_mlpipeline.py
```

### Comparing `mlblocks-0.5.1.dev0/CONTRIBUTING.rst` & `mlblocks-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/HISTORY.md` & `mlblocks-0.6.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+0.6.0 - 2023-04-14
+------------------
+
+* Support python 3.9 and 3.10 - [Issue #141](https://github.com/MLBazaar/MLBlocks/issues/141) by @sarahmish
+
 0.5.0 - 2023-01-22
 ------------------
 
 * Update `numpy` dependency and isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by @sarahmish
 
 0.4.1 - 2021-10-08
 ------------------
```

### Comparing `mlblocks-0.5.1.dev0/LICENSE` & `mlblocks-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/PKG-INFO` & `mlblocks-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlblocks
-Version: 0.5.1.dev0
+Version: 0.6.0
 Summary: Pipelines and primitives for machine learning and data science.
 Home-page: https://github.com/MLBazaar/MLBlocks
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: auto machine learning classification regression data science pipeline
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -179,14 +179,19 @@
 them and expand the library to address other data types: images, text, graph, time series and
 integrate with deep learning libraries.
 
 
 Changelog
 =========
 
+0.6.0 - 2023-04-14
+------------------
+
+* Support python 3.9 and 3.10 - [Issue #141](https://github.com/MLBazaar/MLBlocks/issues/141) by @sarahmish
+
 0.5.0 - 2023-01-22
 ------------------
 
 * Update `numpy` dependency and isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by @sarahmish
 
 0.4.1 - 2021-10-08
 ------------------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlblocks Version: 0.5.1.dev0 Summary: Pipelines and
+Metadata-Version: 2.1 Name: mlblocks Version: 0.6.0 Summary: Pipelines and
 primitives for machine learning and data science. Home-page: https://
 github.com/MLBazaar/MLBlocks Author: MIT Data To AI Lab Author-email:
 dailabmit@gmail.com License: MIT license Keywords: auto machine learning
 classification regression data science pipeline Classifier: Development Status
 :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -86,17 +86,19 @@
 the first MLBlocks version from 2015, designed for only multi table, multi
 entity temporal data, please refer to Bryan Collazoâs thesis: * [Machine
 learning blocks](https://dai.lids.mit.edu/wp-content/uploads/2018/06/
 Mlblocks_Bryan.pdf). Bryan Collazo. Masters thesis, MIT EECS, 2015. With recent
 availability of a multitude of libraries and tools, we decided it was time to
 integrate them and expand the library to address other data types: images,
 text, graph, time series and integrate with deep learning libraries. Changelog
-========= 0.5.0 - 2023-01-22 ------------------ * Update `numpy` dependency and
-isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139)
-by @sarahmish 0.4.1 - 2021-10-08 ------------------ * Update NumPy dependency -
+========= 0.6.0 - 2023-04-14 ------------------ * Support python 3.9 and 3.10 -
+[Issue #141](https://github.com/MLBazaar/MLBlocks/issues/141) by @sarahmish
+0.5.0 - 2023-01-22 ------------------ * Update `numpy` dependency and isolate
+tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by
+@sarahmish 0.4.1 - 2021-10-08 ------------------ * Update NumPy dependency -
 [Issue #136](https://github.com/MLBazaar/MLBlocks/issues/136) by @sarahmish *
 Support dynamic inputs and outputs - [Issue #134](https://github.com/MLBazaar/
 MLBlocks/issues/134) by @pvk-developer 0.4.0 - 2021-01-09 ------------------ *
 Stop pipeline fitting after the last block - [Issue #131](https://github.com/
 MLBazaar/MLBlocks/issues/131) by @sarahmish * Add memory debug and profiling -
 [Issue #130](https://github.com/MLBazaar/MLBlocks/issues/130) by @pvk-developer
 * Update Python support - [Issue #129](https://github.com/MLBazaar/MLBlocks/
```

### Comparing `mlblocks-0.5.1.dev0/README.md` & `mlblocks-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/Makefile` & `mlblocks-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/advanced_usage/adding_primitives.rst` & `mlblocks-0.6.0/docs/advanced_usage/adding_primitives.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/advanced_usage/hyperparameters.rst` & `mlblocks-0.6.0/docs/advanced_usage/hyperparameters.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/advanced_usage/pipelines.rst` & `mlblocks-0.6.0/docs/advanced_usage/pipelines.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/advanced_usage/primitives.rst` & `mlblocks-0.6.0/docs/advanced_usage/primitives.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/conf.py` & `mlblocks-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/getting_started/install.rst` & `mlblocks-0.6.0/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/getting_started/quickstart.rst` & `mlblocks-0.6.0/docs/getting_started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/images/mlblocks-logo-small.png` & `mlblocks-0.6.0/docs/images/mlblocks-logo-small.png`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/images/mlblocks-logo.png` & `mlblocks-0.6.0/docs/images/mlblocks-logo.png`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/index.rst` & `mlblocks-0.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/make.bat` & `mlblocks-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/pipeline_examples/graph.rst` & `mlblocks-0.6.0/docs/pipeline_examples/graph.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/pipeline_examples/image.rst` & `mlblocks-0.6.0/docs/pipeline_examples/image.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/pipeline_examples/multi_table.rst` & `mlblocks-0.6.0/docs/pipeline_examples/multi_table.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/pipeline_examples/single_table.rst` & `mlblocks-0.6.0/docs/pipeline_examples/single_table.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/docs/pipeline_examples/text.rst` & `mlblocks-0.6.0/docs/pipeline_examples/text.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/mlblocks/__init__.py` & `mlblocks-0.6.0/mlblocks/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from mlblocks.mlblock import MLBlock
 from mlblocks.mlpipeline import MLPipeline
 
 __author__ = 'MIT Data To AI Lab'
 __copyright__ = 'Copyright (c) 2018, MIT Data To AI Lab'
 __email__ = 'dailabmit@gmail.com'
 __license__ = 'MIT'
-__version__ = '0.5.1.dev0'
+__version__ = '0.6.0'
 
 __all__ = [
     'MLBlock',
     'MLPipeline',
     'add_pipelines_path',
     'add_primitives_path',
     'find_pipelines',
```

### Comparing `mlblocks-0.5.1.dev0/mlblocks/discovery.py` & `mlblocks-0.6.0/mlblocks/discovery.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/mlblocks/mlblock.py` & `mlblocks-0.6.0/mlblocks/mlblock.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/mlblocks/mlpipeline.py` & `mlblocks-0.6.0/mlblocks/mlpipeline.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/mlblocks.egg-info/PKG-INFO` & `mlblocks-0.6.0/mlblocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlblocks
-Version: 0.5.1.dev0
+Version: 0.6.0
 Summary: Pipelines and primitives for machine learning and data science.
 Home-page: https://github.com/MLBazaar/MLBlocks
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
 Keywords: auto machine learning classification regression data science pipeline
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -179,14 +179,19 @@
 them and expand the library to address other data types: images, text, graph, time series and
 integrate with deep learning libraries.
 
 
 Changelog
 =========
 
+0.6.0 - 2023-04-14
+------------------
+
+* Support python 3.9 and 3.10 - [Issue #141](https://github.com/MLBazaar/MLBlocks/issues/141) by @sarahmish
+
 0.5.0 - 2023-01-22
 ------------------
 
 * Update `numpy` dependency and isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by @sarahmish
 
 0.4.1 - 2021-10-08
 ------------------
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlblocks Version: 0.5.1.dev0 Summary: Pipelines and
+Metadata-Version: 2.1 Name: mlblocks Version: 0.6.0 Summary: Pipelines and
 primitives for machine learning and data science. Home-page: https://
 github.com/MLBazaar/MLBlocks Author: MIT Data To AI Lab Author-email:
 dailabmit@gmail.com License: MIT license Keywords: auto machine learning
 classification regression data science pipeline Classifier: Development Status
 :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -86,17 +86,19 @@
 the first MLBlocks version from 2015, designed for only multi table, multi
 entity temporal data, please refer to Bryan Collazoâs thesis: * [Machine
 learning blocks](https://dai.lids.mit.edu/wp-content/uploads/2018/06/
 Mlblocks_Bryan.pdf). Bryan Collazo. Masters thesis, MIT EECS, 2015. With recent
 availability of a multitude of libraries and tools, we decided it was time to
 integrate them and expand the library to address other data types: images,
 text, graph, time series and integrate with deep learning libraries. Changelog
-========= 0.5.0 - 2023-01-22 ------------------ * Update `numpy` dependency and
-isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139)
-by @sarahmish 0.4.1 - 2021-10-08 ------------------ * Update NumPy dependency -
+========= 0.6.0 - 2023-04-14 ------------------ * Support python 3.9 and 3.10 -
+[Issue #141](https://github.com/MLBazaar/MLBlocks/issues/141) by @sarahmish
+0.5.0 - 2023-01-22 ------------------ * Update `numpy` dependency and isolate
+tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by
+@sarahmish 0.4.1 - 2021-10-08 ------------------ * Update NumPy dependency -
 [Issue #136](https://github.com/MLBazaar/MLBlocks/issues/136) by @sarahmish *
 Support dynamic inputs and outputs - [Issue #134](https://github.com/MLBazaar/
 MLBlocks/issues/134) by @pvk-developer 0.4.0 - 2021-01-09 ------------------ *
 Stop pipeline fitting after the last block - [Issue #131](https://github.com/
 MLBazaar/MLBlocks/issues/131) by @sarahmish * Add memory debug and profiling -
 [Issue #130](https://github.com/MLBazaar/MLBlocks/issues/130) by @pvk-developer
 * Update Python support - [Issue #129](https://github.com/MLBazaar/MLBlocks/
```

### Comparing `mlblocks-0.5.1.dev0/mlblocks.egg-info/SOURCES.txt` & `mlblocks-0.6.0/mlblocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/mlblocks.egg-info/requires.txt` & `mlblocks-0.6.0/mlblocks.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/setup.cfg` & `mlblocks-0.6.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.1.dev0
+current_version = 0.6.0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `mlblocks-0.5.1.dev0/setup.py` & `mlblocks-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,10 +116,10 @@
     name='mlblocks',
     packages=find_packages(include=['mlblocks', 'mlblocks.*']),
     python_requires='>=3.6,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/MLBazaar/MLBlocks',
-    version='0.5.1.dev0',
+    version='0.6.0',
     zip_safe=False,
 )
```

### Comparing `mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_fit.txt` & `mlblocks-0.6.0/tests/data/diagrams/diagram_fit.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_multiple_blocks.txt` & `mlblocks-0.6.0/tests/data/diagrams/diagram_multiple_blocks.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_simple.txt` & `mlblocks-0.6.0/tests/data/diagrams/diagram_simple.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/tests/features/test_fit_predicr_args.py` & `mlblocks-0.6.0/tests/features/test_fit_predicr_args.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/tests/features/test_partial_outputs.py` & `mlblocks-0.6.0/tests/features/test_partial_outputs.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/tests/features/test_pipeline_loading.py` & `mlblocks-0.6.0/tests/features/test_pipeline_loading.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/tests/test_discovery.py` & `mlblocks-0.6.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/tests/test_mlblock.py` & `mlblocks-0.6.0/tests/test_mlblock.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.1.dev0/tests/test_mlpipeline.py` & `mlblocks-0.6.0/tests/test_mlpipeline.py`

 * *Files identical despite different names*

