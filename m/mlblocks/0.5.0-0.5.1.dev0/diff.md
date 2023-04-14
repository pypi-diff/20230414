# Comparing `tmp/mlblocks-0.5.0.tar.gz` & `tmp/mlblocks-0.5.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mlblocks-0.5.0.tar", last modified: Sun Jan 22 21:26:07 2023, max compression
+gzip compressed data, was "mlblocks-0.5.1.dev0.tar", last modified: Fri Apr 14 18:27:51 2023, max compression
```

## Comparing `mlblocks-0.5.0.tar` & `mlblocks-0.5.1.dev0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/
--rw-r--r--   0 sarah      (501) staff       (20)    16621 2023-01-22 21:26:07.000000 mlblocks-0.5.0/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-01-22 21:08:36.000000 mlblocks-0.5.0/LICENSE
--rw-r--r--   0 sarah      (501) staff       (20)     7923 2023-01-22 21:08:36.000000 mlblocks-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 sarah      (501) staff       (20)     6951 2023-01-22 21:26:03.000000 mlblocks-0.5.0/HISTORY.md
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/tests/
--rw-r--r--   0 sarah      (501) staff       (20)    14919 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/test_mlblock.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/tests/features/
--rw-r--r--   0 sarah      (501) staff       (20)     4481 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/features/test_partial_outputs.py
--rw-r--r--   0 sarah      (501) staff       (20)     2977 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/features/test_pipeline_loading.py
--rw-r--r--   0 sarah      (501) staff       (20)      845 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/features/test_fit_predicr_args.py
--rw-r--r--   0 sarah      (501) staff       (20)    36889 2023-01-22 21:26:03.000000 mlblocks-0.5.0/tests/test_mlpipeline.py
--rw-r--r--   0 sarah      (501) staff       (20)        0 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)    10345 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/test_discovery.py
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/tests/data/
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/tests/data/diagrams/
--rw-r--r--   0 sarah      (501) staff       (20)     1440 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/data/diagrams/diagram_multiple_blocks.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/data/diagrams/diagram_fit.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-01-22 21:08:36.000000 mlblocks-0.5.0/tests/data/diagrams/diagram_simple.txt
--rw-r--r--   0 sarah      (501) staff       (20)      299 2023-01-22 21:08:36.000000 mlblocks-0.5.0/MANIFEST.in
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/mlblocks.egg-info/
--rw-r--r--   0 sarah      (501) staff       (20)    16621 2023-01-22 21:26:07.000000 mlblocks-0.5.0/mlblocks.egg-info/PKG-INFO
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-01-22 21:26:07.000000 mlblocks-0.5.0/mlblocks.egg-info/not-zip-safe
--rw-r--r--   0 sarah      (501) staff       (20)     1324 2023-01-22 21:26:07.000000 mlblocks-0.5.0/mlblocks.egg-info/SOURCES.txt
--rw-r--r--   0 sarah      (501) staff       (20)     1170 2023-01-22 21:26:07.000000 mlblocks-0.5.0/mlblocks.egg-info/requires.txt
--rw-r--r--   0 sarah      (501) staff       (20)        9 2023-01-22 21:26:07.000000 mlblocks-0.5.0/mlblocks.egg-info/top_level.txt
--rw-r--r--   0 sarah      (501) staff       (20)        1 2023-01-22 21:26:07.000000 mlblocks-0.5.0/mlblocks.egg-info/dependency_links.txt
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/docs/
--rw-r--r--   0 sarah      (501) staff       (20)     4317 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/index.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/docs/advanced_usage/
--rw-r--r--   0 sarah      (501) staff       (20)     4471 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/advanced_usage/adding_primitives.rst
--rw-r--r--   0 sarah      (501) staff       (20)    12082 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/advanced_usage/primitives.rst
--rw-r--r--   0 sarah      (501) staff       (20)     8503 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/advanced_usage/hyperparameters.rst
--rw-r--r--   0 sarah      (501) staff       (20)    17648 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/advanced_usage/pipelines.rst
--rw-r--r--   0 sarah      (501) staff       (20)       33 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/contributing.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/docs/images/
--rw-r--r--   0 sarah      (501) staff       (20)      437 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/images/mlblocks-icon.png
--rw-r--r--   0 sarah      (501) staff       (20)     3857 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/images/mlblocks-logo-small.png
--rw-r--r--   0 sarah      (501) staff       (20)    12140 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/images/mlblocks-logo.png
--rw-r--r--   0 sarah      (501) staff       (20)      609 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/Makefile
--rwxr-xr-x   0 sarah      (501) staff       (20)     6038 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/conf.py
--rw-r--r--   0 sarah      (501) staff       (20)      770 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/make.bat
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/docs/api/
--rw-r--r--   0 sarah      (501) staff       (20)       58 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/api/mlblocks.rst
--rw-r--r--   0 sarah      (501) staff       (20)       28 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/authors.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/docs/pipeline_examples/
--rw-r--r--   0 sarah      (501) staff       (20)     2889 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/pipeline_examples/single_table.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2038 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/pipeline_examples/multi_table.rst
--rw-r--r--   0 sarah      (501) staff       (20)     2967 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/pipeline_examples/graph.rst
--rw-r--r--   0 sarah      (501) staff       (20)     5191 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/pipeline_examples/text.rst
--rw-r--r--   0 sarah      (501) staff       (20)     4872 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/pipeline_examples/image.rst
--rw-r--r--   0 sarah      (501) staff       (20)       29 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/changelog.rst
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/docs/getting_started/
--rw-r--r--   0 sarah      (501) staff       (20)     1252 2023-01-22 21:08:36.000000 mlblocks-0.5.0/docs/getting_started/install.rst
--rw-r--r--   0 sarah      (501) staff       (20)     4535 2023-01-22 21:26:03.000000 mlblocks-0.5.0/docs/getting_started/quickstart.rst
--rw-r--r--   0 sarah      (501) staff       (20)     6112 2023-01-22 21:08:36.000000 mlblocks-0.5.0/README.md
--rw-r--r--   0 sarah      (501) staff       (20)     3030 2023-01-22 21:26:03.000000 mlblocks-0.5.0/setup.py
--rw-r--r--   0 sarah      (501) staff       (20)      268 2023-01-22 21:08:36.000000 mlblocks-0.5.0/AUTHORS.rst
--rw-r--r--   0 sarah      (501) staff       (20)     1150 2023-01-22 21:26:07.000000 mlblocks-0.5.0/setup.cfg
-drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-01-22 21:26:07.000000 mlblocks-0.5.0/mlblocks/
--rw-r--r--   0 sarah      (501) staff       (20)    11931 2023-01-22 21:08:36.000000 mlblocks-0.5.0/mlblocks/mlblock.py
--rw-r--r--   0 sarah      (501) staff       (20)    14156 2023-01-22 21:08:36.000000 mlblocks-0.5.0/mlblocks/discovery.py
--rw-r--r--   0 sarah      (501) staff       (20)     1009 2023-01-22 21:26:03.000000 mlblocks-0.5.0/mlblocks/__init__.py
--rw-r--r--   0 sarah      (501) staff       (20)    54563 2023-01-22 21:08:36.000000 mlblocks-0.5.0/mlblocks/mlpipeline.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.192095 mlblocks-0.5.1.dev0/
+-rw-r--r--   0 sarah      (501) staff       (20)      268 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/AUTHORS.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     7923 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/CONTRIBUTING.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     6951 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/HISTORY.md
+-rw-r--r--   0 sarah      (501) staff       (20)     1076 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/LICENSE
+-rw-r--r--   0 sarah      (501) staff       (20)      299 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/MANIFEST.in
+-rw-r--r--   0 sarah      (501) staff       (20)    14133 2023-04-14 18:27:51.192312 mlblocks-0.5.1.dev0/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     6124 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/README.md
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.166828 mlblocks-0.5.1.dev0/docs/
+-rw-r--r--   0 sarah      (501) staff       (20)      609 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/Makefile
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.168883 mlblocks-0.5.1.dev0/docs/advanced_usage/
+-rw-r--r--   0 sarah      (501) staff       (20)     4471 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/advanced_usage/adding_primitives.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     8503 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/advanced_usage/hyperparameters.rst
+-rw-r--r--   0 sarah      (501) staff       (20)    17648 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/advanced_usage/pipelines.rst
+-rw-r--r--   0 sarah      (501) staff       (20)    12082 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/advanced_usage/primitives.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.169324 mlblocks-0.5.1.dev0/docs/api/
+-rw-r--r--   0 sarah      (501) staff       (20)       58 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/api/mlblocks.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       28 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/authors.rst
+-rw-r--r--   0 sarah      (501) staff       (20)       29 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/changelog.rst
+-rwxr-xr-x   0 sarah      (501) staff       (20)     6038 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/conf.py
+-rw-r--r--   0 sarah      (501) staff       (20)       33 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/contributing.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.170321 mlblocks-0.5.1.dev0/docs/getting_started/
+-rw-r--r--   0 sarah      (501) staff       (20)     1252 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/getting_started/install.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     4535 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/getting_started/quickstart.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.171913 mlblocks-0.5.1.dev0/docs/images/
+-rw-r--r--   0 sarah      (501) staff       (20)      437 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/images/mlblocks-icon.png
+-rw-r--r--   0 sarah      (501) staff       (20)     3857 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/images/mlblocks-logo-small.png
+-rw-r--r--   0 sarah      (501) staff       (20)    12140 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/images/mlblocks-logo.png
+-rw-r--r--   0 sarah      (501) staff       (20)     4317 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/index.rst
+-rw-r--r--   0 sarah      (501) staff       (20)      770 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/make.bat
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.174364 mlblocks-0.5.1.dev0/docs/pipeline_examples/
+-rw-r--r--   0 sarah      (501) staff       (20)     2967 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/graph.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     4872 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/image.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2038 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/multi_table.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     2889 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/single_table.rst
+-rw-r--r--   0 sarah      (501) staff       (20)     5191 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/docs/pipeline_examples/text.rst
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.178181 mlblocks-0.5.1.dev0/mlblocks/
+-rw-r--r--   0 sarah      (501) staff       (20)     1014 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/mlblocks/__init__.py
+-rw-r--r--   0 sarah      (501) staff       (20)    14156 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/mlblocks/discovery.py
+-rw-r--r--   0 sarah      (501) staff       (20)    11931 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/mlblocks/mlblock.py
+-rw-r--r--   0 sarah      (501) staff       (20)    54563 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/mlblocks/mlpipeline.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.183275 mlblocks-0.5.1.dev0/mlblocks.egg-info/
+-rw-r--r--   0 sarah      (501) staff       (20)    14133 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/PKG-INFO
+-rw-r--r--   0 sarah      (501) staff       (20)     1324 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        1 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/not-zip-safe
+-rw-r--r--   0 sarah      (501) staff       (20)     1170 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/requires.txt
+-rw-r--r--   0 sarah      (501) staff       (20)        9 2023-04-14 18:27:51.000000 mlblocks-0.5.1.dev0/mlblocks.egg-info/top_level.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1155 2023-04-14 18:27:51.193296 mlblocks-0.5.1.dev0/setup.cfg
+-rw-r--r--   0 sarah      (501) staff       (20)     3135 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/setup.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.186418 mlblocks-0.5.1.dev0/tests/
+-rw-r--r--   0 sarah      (501) staff       (20)        0 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/__init__.py
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.160306 mlblocks-0.5.1.dev0/tests/data/
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.189514 mlblocks-0.5.1.dev0/tests/data/diagrams/
+-rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_fit.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1440 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_multiple_blocks.txt
+-rw-r--r--   0 sarah      (501) staff       (20)     1171 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_simple.txt
+drwxr-xr-x   0 sarah      (501) staff       (20)        0 2023-04-14 18:27:51.191636 mlblocks-0.5.1.dev0/tests/features/
+-rw-r--r--   0 sarah      (501) staff       (20)      845 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/features/test_fit_predicr_args.py
+-rw-r--r--   0 sarah      (501) staff       (20)     4481 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/features/test_partial_outputs.py
+-rw-r--r--   0 sarah      (501) staff       (20)     2977 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/features/test_pipeline_loading.py
+-rw-r--r--   0 sarah      (501) staff       (20)    10345 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/test_discovery.py
+-rw-r--r--   0 sarah      (501) staff       (20)    14919 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/test_mlblock.py
+-rw-r--r--   0 sarah      (501) staff       (20)    36889 2023-04-14 18:14:02.000000 mlblocks-0.5.1.dev0/tests/test_mlpipeline.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mlblocks-0.5.0/PKG-INFO` & `mlblocks-0.5.1.dev0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,354 +1,357 @@
 Metadata-Version: 2.1
 Name: mlblocks
-Version: 0.5.0
+Version: 0.5.1.dev0
 Summary: Pipelines and primitives for machine learning and data science.
 Home-page: https://github.com/MLBazaar/MLBlocks
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
-Description: <p align="left">
-          <a href="https://dai.lids.mit.edu">
-            <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
-          </a>
-          <i>An Open Source Project from the <a href="https://dai.lids.mit.edu">Data to AI Lab, at MIT</a></i>
-        </p>
-        
-        <p align="left">
-        <img width=20% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/mlblocks-icon.png" alt=“MLBlocks” />
-        </p>
-        
-        <p align="left">
-        Pipelines and Primitives for Machine Learning and Data Science.
-        </p>
-        
-        [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-        [![PyPi](https://img.shields.io/pypi/v/mlblocks.svg)](https://pypi.python.org/pypi/mlblocks)
-        [![Tests](https://github.com/MLBazaar/MLBlocks/workflows/Run%20Tests/badge.svg)](https://github.com/MLBazaar/MLBlocks/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
-        [![CodeCov](https://codecov.io/gh/MLBazaar/MLBlocks/branch/master/graph/badge.svg)](https://codecov.io/gh/MLBazaar/MLBlocks)
-        [![Downloads](https://pepy.tech/badge/mlblocks)](https://pepy.tech/project/mlblocks)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MLBazaar/MLBlocks/master?filepath=examples/tutorials)
-        
-        <br>
-        
-        # MLBlocks
-        
-        * Documentation: https://mlbazaar.github.io/MLBlocks
-        * Github: https://github.com/MLBazaar/MLBlocks
-        * License: [MIT](https://github.com/MLBazaar/MLBlocks/blob/master/LICENSE)
-        * Development Status: [Pre-Alpha](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-        
-        ## Overview
-        
-        MLBlocks is a simple framework for composing end-to-end tunable Machine Learning Pipelines by
-        seamlessly combining tools from any python library with a simple, common and uniform interface.
-        
-        Features include:
-        
-        * Build Machine Learning Pipelines combining **any Machine Learning Library in Python**.
-        * Access a repository with hundreds of primitives and pipelines ready to be used with little to
-          no python code to write, carefully curated by Machine Learning and Domain experts.
-        * Extract machine-readable information about which hyperparameters can be tuned and within
-          which ranges, allowing automated integration with Hyperparameter Optimization tools like
-          [BTB](https://github.com/MLBazaar/BTB).
-        * Complex multi-branch pipelines and DAG configurations, with unlimited number of inputs and
-          outputs per primitive.
-        * Easy save and load Pipelines using JSON Annotations.
-        
-        # Install
-        
-        ## Requirements
-        
-        **MLBlocks** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
-        
-        ## Install with `pip`
-        
-        The easiest and recommended way to install **MLBlocks** is using [pip](
-        https://pip.pypa.io/en/stable/):
-        
-        ```bash
-        pip install mlblocks
-        ```
-        
-        This will pull and install the latest stable release from [PyPi](https://pypi.org/).
-        
-        If you want to install from source or contribute to the project please read the
-        [Contributing Guide](https://mlbazaar.github.io/MLBlocks/contributing.html#get-started).
-        
-        ## MLPrimitives
-        
-        In order to be usable, MLBlocks requires a compatible primitives library.
-        
-        The official library, required in order to follow the following MLBlocks tutorial,
-        is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), which you can install
-        with this command:
-        
-        ```bash
-        pip install mlprimitives
-        ```
-        
-        # Quickstart
-        
-        Below there is a short example about how to use **MLBlocks** to solve the [Adult Census
-        Dataset](https://archive.ics.uci.edu/ml/datasets/Adult) classification problem using a
-        pipeline which combines primitives from [MLPrimitives](https://github.com/MLBazaar/MLPrimitives),
-        [scikit-learn](https://scikit-learn.org/) and [xgboost](https://xgboost.readthedocs.io/).
-        
-        ```python3
-        from mlblocks import MLPipeline
-        from mlprimitives.datasets import load_dataset
-        
-        dataset = load_dataset('census')
-        X_train, X_test, y_train, y_test = dataset.get_splits(1)
-        
-        primitives = [
-            'mlprimitives.custom.preprocessing.ClassEncoder',
-            'mlprimitives.custom.feature_extraction.CategoricalEncoder',
-            'sklearn.impute.SimpleImputer',
-            'xgboost.XGBClassifier',
-            'mlprimitives.custom.preprocessing.ClassDecoder'
-        ]
-        pipeline = MLPipeline(primitives)
-        
-        pipeline.fit(X_train, y_train)
-        predictions = pipeline.predict(X_test)
-        
-        dataset.score(y_test, predictions)
-        ```
-        
-        # What's Next?
-        
-        If you want to learn more about how to tune the pipeline hyperparameters, save and load
-        the pipelines using JSON annotations or build complex multi-branched pipelines, please
-        check our [documentation site](https://mlbazaar.github.io/MLBlocks).
-        
-        Also do not forget to have a look at the [notebook tutorials](
-        https://github.com/MLBazaar/MLBlocks/tree/master/examples/tutorials)!
-        
-        # Citing MLBlocks
-        
-        If you use MLBlocks for your research, please consider citing our related papers.
-        
-        For the current design of MLBlocks and its usage within the larger *Machine Learning Bazaar* project at
-        the MIT Data To AI Lab, please see:
-        
-        Micah J. Smith, Carles Sala, James Max Kanter, and Kalyan Veeramachaneni. ["The Machine Learning Bazaar:
-        Harnessing the ML Ecosystem for Effective System Development."](https://arxiv.org/abs/1905.08942) arXiv
-        Preprint 1905.08942. 2019.
-        
-        ```bibtex
-        @article{smith2019mlbazaar,
-          author = {Smith, Micah J. and Sala, Carles and Kanter, James Max and Veeramachaneni, Kalyan},
-          title = {The Machine Learning Bazaar: Harnessing the ML Ecosystem for Effective System Development},
-          journal = {arXiv e-prints},
-          year = {2019},
-          eid = {arXiv:1905.08942},
-          pages = {arXiv:1905.08942},
-          archivePrefix = {arXiv},
-          eprint = {1905.08942},
-        }
-        ```
-        
-        For the first MLBlocks version from 2015, designed for only multi table, multi entity temporal data, please
-        refer to Bryan Collazo’s thesis:
-        
-        * [Machine learning blocks](https://dai.lids.mit.edu/wp-content/uploads/2018/06/Mlblocks_Bryan.pdf).
-          Bryan Collazo. Masters thesis, MIT EECS, 2015.
-        
-        With recent availability of a multitude of libraries and tools, we decided it was time to integrate
-        them and expand the library to address other data types: images, text, graph, time series and
-        integrate with deep learning libraries.
-        
-        
-        Changelog
-        =========
-        
-        0.5.0 - 2023-01-22
-        ------------------
-        
-        * Update `numpy` dependency and isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by @sarahmish
-        
-        0.4.1 - 2021-10-08
-        ------------------
-        
-        * Update NumPy dependency - [Issue #136](https://github.com/MLBazaar/MLBlocks/issues/136) by @sarahmish
-        * Support dynamic inputs and outputs - [Issue #134](https://github.com/MLBazaar/MLBlocks/issues/134) by @pvk-developer
-        
-        0.4.0 - 2021-01-09
-        ------------------
-        
-        * Stop pipeline fitting after the last block - [Issue #131](https://github.com/MLBazaar/MLBlocks/issues/131) by @sarahmish
-        * Add memory debug and profiling - [Issue #130](https://github.com/MLBazaar/MLBlocks/issues/130) by @pvk-developer
-        * Update Python support - [Issue #129](https://github.com/MLBazaar/MLBlocks/issues/129) by @csala
-        * Get execution time for each block - [Issue #127](https://github.com/MLBazaar/MLBlocks/issues/127) by @sarahmish
-        * Allow loading a primitive or pipeline directly from the JSON path - [Issue #114](https://github.com/MLBazaar/MLBlocks/issues/114) by @csala
-        * Pipeline Diagrams - [Issue #113](https://github.com/MLBazaar/MLBlocks/issues/113) by @erica-chiu
-        * Get Pipeline Inputs - [Issue #112](https://github.com/MLBazaar/MLBlocks/issues/112) by @erica-chiu
-        
-        0.3.4 - 2019-11-01
-        ------------------
-        
-        * Ability to return intermediate context - [Issue #110](https://github.com/MLBazaar/MLBlocks/issues/110) by @csala
-        * Support for static or class methods - [Issue #107](https://github.com/MLBazaar/MLBlocks/issues/107) by @csala
-        
-        0.3.3 - 2019-09-09
-        ------------------
-        
-        * Improved intermediate outputs management - [Issue #105](https://github.com/MLBazaar/MLBlocks/issues/105) by @csala
-        
-        0.3.2 - 2019-08-12
-        ------------------
-        
-        * Allow passing fit and produce arguments as `init_params` - [Issue #96](https://github.com/MLBazaar/MLBlocks/issues/96) by @csala
-        * Support optional fit and produce args and arg defaults - [Issue #95](https://github.com/MLBazaar/MLBlocks/issues/95) by @csala
-        * Isolate primitives from their hyperparameters dictionary - [Issue #94](https://github.com/MLBazaar/MLBlocks/issues/94) by @csala
-        * Add functions to explore the available primitives and pipelines - [Issue #90](https://github.com/MLBazaar/MLBlocks/issues/90) by @csala
-        * Add primitive caching - [Issue #22](https://github.com/MLBazaar/MLBlocks/issues/22) by @csala
-        
-        0.3.1 - Pipelines Discovery
-        ---------------------------
-        
-        * Support flat hyperparameter dictionaries - [Issue #92](https://github.com/MLBazaar/MLBlocks/issues/92) by @csala
-        * Load pipelines by name and register them as `entry_points` - [Issue #88](https://github.com/MLBazaar/MLBlocks/issues/88) by @csala
-        * Implement partial re-fit -[Issue #61](https://github.com/MLBazaar/MLBlocks/issues/61) by @csala
-        * Move argument parsing to MLBlock - [Issue #86](https://github.com/MLBazaar/MLBlocks/issues/86) by @csala
-        * Allow getting intermediate outputs - [Issue #58](https://github.com/MLBazaar/MLBlocks/issues/58) by @csala
-        
-        0.3.0 - New Primitives Discovery
-        --------------------------------
-        
-        * New primitives discovery system based on `entry_points`.
-        * Conditional Hyperparameters filtering in MLBlock initialization.
-        * Improved logging and exception reporting.
-        
-        0.2.4 - New Datasets and Unit Tests
-        -----------------------------------
-        
-        * Add a new multi-table dataset.
-        * Add Unit Tests up to 50% coverage.
-        * Improve documentation.
-        * Fix minor bug in newsgroups dataset.
-        
-        0.2.3 - Demo Datasets
-        ---------------------
-        
-        * Add new methods to Dataset class.
-        * Add documentation for the datasets module.
-        
-        0.2.2 - MLPipeline Load/Save
-        ----------------------------
-        
-        * Implement save and load methods for MLPipelines
-        * Add more datasets
-        
-        0.2.1 - New Documentation
-        -------------------------
-        
-        * Add mlblocks.datasets module with demo data download functions.
-        * Extensive documentation, including multiple pipeline examples.
-        
-        0.2.0 - New MLBlocks API
-        ------------------------
-        
-        A new MLBlocks API and Primitive format.
-        
-        This is a summary of the changes:
-        
-        * Primitives JSONs and Python code has been moved to a different repository, called MLPrimitives
-        * Optional usage of multiple JSON primitive folders.
-        * JSON format has been changed to allow more flexibility and features:
-            * input and output arguments, as well as argument types, can be specified for each method
-            * both classes and function as primitives are supported
-            * multitype and conditional hyperparameters fully supported
-            * data modalities and primitive classifiers introduced
-            * metadata such as documentation, description and author fields added
-        * Parsers are removed, and now the MLBlock class is responsible for loading and reading the
-          JSON primitive.
-        * Multiple blocks of the same primitive are supported within the same pipeline.
-        * Arbitrary inputs and outputs for both pipelines and blocks are allowed.
-        * Shared variables during pipeline execution, usable by multiple blocks.
-        
-        0.1.9 - Bugfix Release
-        ----------------------
-        
-        * Disable some NetworkX functions for incompatibilities with some types of graphs.
-        
-        0.1.8 - New primitives and some improvements
-        --------------------------------------------
-        
-        * Improve the NetworkX primitives.
-        * Add String Vectorization and Datetime Featurization primitives.
-        * Refactor some Keras primitives to work with single dimension `y` arrays and be compatible with `pickle`.
-        * Add XGBClassifier and XGBRegressor primitives.
-        * Add some `keras.applications` pretrained networks as preprocessing primitives.
-        * Add helper class to allow function primitives.
-        
-        0.1.7 - Nested hyperparams dicts
-        --------------------------------
-        
-        * Support passing hyperparams as nested dicts.
-        
-        0.1.6 - Text and Graph Pipelines
-        --------------------------------
-        
-        * Add LSTM classifier and regressor primitives.
-        * Add OneHotEncoder and MultiLabelEncoder primitives.
-        * Add several NetworkX graph featurization primitives.
-        * Add `community.best_partition` primitive.
-        
-        0.1.5 - Collaborative Filtering Pipelines
-        -----------------------------------------
-        
-        * Add LightFM primitive.
-        
-        0.1.4 - Image pipelines improved
-        --------------------------------
-        
-        * Allow passing `init_params` on `MLPipeline` creation.
-        * Fix bug with MLHyperparam types and Keras.
-        * Rename `produce_params` as `predict_params`.
-        * Add SingleCNN Classifier and Regressor primitives.
-        * Simplify and improve Trivial Predictor
-        
-        0.1.3 - Multi Table pipelines improved
-        --------------------------------------
-        
-        * Improve RandomForest primitive ranges
-        * Improve DFS primitive
-        * Add Tree Based Feature Selection primitives
-        * Fix bugs in TrivialPredictor
-        * Improved documentation
-        
-        0.1.2 - Bugfix release
-        ----------------------
-        
-        * Fix bug in TrivialMedianPredictor
-        * Fix bug in OneHotLabelEncoder
-        
-        0.1.1 - Single Table pipelines improved
-        ---------------------------------------
-        
-        * New project structure and primitives for integration into MIT-TA2.
-        * MIT-TA2 default pipelines and single table pipelines fully working.
-        
-        0.1.0
-        -----
-        
-        * First release on PyPI.
-        
 Keywords: auto machine learning classification regression data science pipeline
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6,<3.9
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: unit
 Provides-Extra: test
 Provides-Extra: examples
 Provides-Extra: mlprimitives
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+<p align="left">
+  <a href="https://dai.lids.mit.edu">
+    <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
+  </a>
+  <i>An Open Source Project from the <a href="https://dai.lids.mit.edu">Data to AI Lab, at MIT</a></i>
+</p>
+
+<p align="left">
+<img width=20% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/mlblocks-icon.png" alt=“MLBlocks” />
+</p>
+
+<p align="left">
+Pipelines and Primitives for Machine Learning and Data Science.
+</p>
+
+[![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+[![PyPi](https://img.shields.io/pypi/v/mlblocks.svg)](https://pypi.python.org/pypi/mlblocks)
+[![Tests](https://github.com/MLBazaar/MLBlocks/workflows/Run%20Tests/badge.svg)](https://github.com/MLBazaar/MLBlocks/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
+[![CodeCov](https://codecov.io/gh/MLBazaar/MLBlocks/branch/master/graph/badge.svg)](https://codecov.io/gh/MLBazaar/MLBlocks)
+[![Downloads](https://pepy.tech/badge/mlblocks)](https://pepy.tech/project/mlblocks)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MLBazaar/MLBlocks/master?filepath=examples/tutorials)
+
+<br>
+
+# MLBlocks
+
+* Documentation: https://mlbazaar.github.io/MLBlocks
+* Github: https://github.com/MLBazaar/MLBlocks
+* License: [MIT](https://github.com/MLBazaar/MLBlocks/blob/master/LICENSE)
+* Development Status: [Pre-Alpha](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+
+## Overview
+
+MLBlocks is a simple framework for composing end-to-end tunable Machine Learning Pipelines by
+seamlessly combining tools from any python library with a simple, common and uniform interface.
+
+Features include:
+
+* Build Machine Learning Pipelines combining **any Machine Learning Library in Python**.
+* Access a repository with hundreds of primitives and pipelines ready to be used with little to
+  no python code to write, carefully curated by Machine Learning and Domain experts.
+* Extract machine-readable information about which hyperparameters can be tuned and within
+  which ranges, allowing automated integration with Hyperparameter Optimization tools like
+  [BTB](https://github.com/MLBazaar/BTB).
+* Complex multi-branch pipelines and DAG configurations, with unlimited number of inputs and
+  outputs per primitive.
+* Easy save and load Pipelines using JSON Annotations.
+
+# Install
+
+## Requirements
+
+**MLBlocks** has been developed and tested on [Python 3.6, 3.7, 3.8, 3.9, and 3.10](https://www.python.org/downloads/)
+
+## Install with `pip`
+
+The easiest and recommended way to install **MLBlocks** is using [pip](
+https://pip.pypa.io/en/stable/):
+
+```bash
+pip install mlblocks
+```
+
+This will pull and install the latest stable release from [PyPi](https://pypi.org/).
+
+If you want to install from source or contribute to the project please read the
+[Contributing Guide](https://mlbazaar.github.io/MLBlocks/contributing.html#get-started).
+
+## MLPrimitives
+
+In order to be usable, MLBlocks requires a compatible primitives library.
+
+The official library, required in order to follow the following MLBlocks tutorial,
+is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), which you can install
+with this command:
+
+```bash
+pip install mlprimitives
+```
+
+# Quickstart
+
+Below there is a short example about how to use **MLBlocks** to solve the [Adult Census
+Dataset](https://archive.ics.uci.edu/ml/datasets/Adult) classification problem using a
+pipeline which combines primitives from [MLPrimitives](https://github.com/MLBazaar/MLPrimitives),
+[scikit-learn](https://scikit-learn.org/) and [xgboost](https://xgboost.readthedocs.io/).
+
+```python3
+from mlblocks import MLPipeline
+from mlprimitives.datasets import load_dataset
+
+dataset = load_dataset('census')
+X_train, X_test, y_train, y_test = dataset.get_splits(1)
+
+primitives = [
+    'mlprimitives.custom.preprocessing.ClassEncoder',
+    'mlprimitives.custom.feature_extraction.CategoricalEncoder',
+    'sklearn.impute.SimpleImputer',
+    'xgboost.XGBClassifier',
+    'mlprimitives.custom.preprocessing.ClassDecoder'
+]
+pipeline = MLPipeline(primitives)
+
+pipeline.fit(X_train, y_train)
+predictions = pipeline.predict(X_test)
+
+dataset.score(y_test, predictions)
+```
+
+# What's Next?
+
+If you want to learn more about how to tune the pipeline hyperparameters, save and load
+the pipelines using JSON annotations or build complex multi-branched pipelines, please
+check our [documentation site](https://mlbazaar.github.io/MLBlocks).
+
+Also do not forget to have a look at the [notebook tutorials](
+https://github.com/MLBazaar/MLBlocks/tree/master/examples/tutorials)!
+
+# Citing MLBlocks
+
+If you use MLBlocks for your research, please consider citing our related papers.
+
+For the current design of MLBlocks and its usage within the larger *Machine Learning Bazaar* project at
+the MIT Data To AI Lab, please see:
+
+Micah J. Smith, Carles Sala, James Max Kanter, and Kalyan Veeramachaneni. ["The Machine Learning Bazaar:
+Harnessing the ML Ecosystem for Effective System Development."](https://arxiv.org/abs/1905.08942) arXiv
+Preprint 1905.08942. 2019.
+
+```bibtex
+@article{smith2019mlbazaar,
+  author = {Smith, Micah J. and Sala, Carles and Kanter, James Max and Veeramachaneni, Kalyan},
+  title = {The Machine Learning Bazaar: Harnessing the ML Ecosystem for Effective System Development},
+  journal = {arXiv e-prints},
+  year = {2019},
+  eid = {arXiv:1905.08942},
+  pages = {arXiv:1905.08942},
+  archivePrefix = {arXiv},
+  eprint = {1905.08942},
+}
+```
+
+For the first MLBlocks version from 2015, designed for only multi table, multi entity temporal data, please
+refer to Bryan Collazo’s thesis:
+
+* [Machine learning blocks](https://dai.lids.mit.edu/wp-content/uploads/2018/06/Mlblocks_Bryan.pdf).
+  Bryan Collazo. Masters thesis, MIT EECS, 2015.
+
+With recent availability of a multitude of libraries and tools, we decided it was time to integrate
+them and expand the library to address other data types: images, text, graph, time series and
+integrate with deep learning libraries.
+
+
+Changelog
+=========
+
+0.5.0 - 2023-01-22
+------------------
+
+* Update `numpy` dependency and isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by @sarahmish
+
+0.4.1 - 2021-10-08
+------------------
+
+* Update NumPy dependency - [Issue #136](https://github.com/MLBazaar/MLBlocks/issues/136) by @sarahmish
+* Support dynamic inputs and outputs - [Issue #134](https://github.com/MLBazaar/MLBlocks/issues/134) by @pvk-developer
+
+0.4.0 - 2021-01-09
+------------------
+
+* Stop pipeline fitting after the last block - [Issue #131](https://github.com/MLBazaar/MLBlocks/issues/131) by @sarahmish
+* Add memory debug and profiling - [Issue #130](https://github.com/MLBazaar/MLBlocks/issues/130) by @pvk-developer
+* Update Python support - [Issue #129](https://github.com/MLBazaar/MLBlocks/issues/129) by @csala
+* Get execution time for each block - [Issue #127](https://github.com/MLBazaar/MLBlocks/issues/127) by @sarahmish
+* Allow loading a primitive or pipeline directly from the JSON path - [Issue #114](https://github.com/MLBazaar/MLBlocks/issues/114) by @csala
+* Pipeline Diagrams - [Issue #113](https://github.com/MLBazaar/MLBlocks/issues/113) by @erica-chiu
+* Get Pipeline Inputs - [Issue #112](https://github.com/MLBazaar/MLBlocks/issues/112) by @erica-chiu
+
+0.3.4 - 2019-11-01
+------------------
+
+* Ability to return intermediate context - [Issue #110](https://github.com/MLBazaar/MLBlocks/issues/110) by @csala
+* Support for static or class methods - [Issue #107](https://github.com/MLBazaar/MLBlocks/issues/107) by @csala
+
+0.3.3 - 2019-09-09
+------------------
+
+* Improved intermediate outputs management - [Issue #105](https://github.com/MLBazaar/MLBlocks/issues/105) by @csala
+
+0.3.2 - 2019-08-12
+------------------
+
+* Allow passing fit and produce arguments as `init_params` - [Issue #96](https://github.com/MLBazaar/MLBlocks/issues/96) by @csala
+* Support optional fit and produce args and arg defaults - [Issue #95](https://github.com/MLBazaar/MLBlocks/issues/95) by @csala
+* Isolate primitives from their hyperparameters dictionary - [Issue #94](https://github.com/MLBazaar/MLBlocks/issues/94) by @csala
+* Add functions to explore the available primitives and pipelines - [Issue #90](https://github.com/MLBazaar/MLBlocks/issues/90) by @csala
+* Add primitive caching - [Issue #22](https://github.com/MLBazaar/MLBlocks/issues/22) by @csala
+
+0.3.1 - Pipelines Discovery
+---------------------------
+
+* Support flat hyperparameter dictionaries - [Issue #92](https://github.com/MLBazaar/MLBlocks/issues/92) by @csala
+* Load pipelines by name and register them as `entry_points` - [Issue #88](https://github.com/MLBazaar/MLBlocks/issues/88) by @csala
+* Implement partial re-fit -[Issue #61](https://github.com/MLBazaar/MLBlocks/issues/61) by @csala
+* Move argument parsing to MLBlock - [Issue #86](https://github.com/MLBazaar/MLBlocks/issues/86) by @csala
+* Allow getting intermediate outputs - [Issue #58](https://github.com/MLBazaar/MLBlocks/issues/58) by @csala
+
+0.3.0 - New Primitives Discovery
+--------------------------------
+
+* New primitives discovery system based on `entry_points`.
+* Conditional Hyperparameters filtering in MLBlock initialization.
+* Improved logging and exception reporting.
+
+0.2.4 - New Datasets and Unit Tests
+-----------------------------------
+
+* Add a new multi-table dataset.
+* Add Unit Tests up to 50% coverage.
+* Improve documentation.
+* Fix minor bug in newsgroups dataset.
+
+0.2.3 - Demo Datasets
+---------------------
+
+* Add new methods to Dataset class.
+* Add documentation for the datasets module.
+
+0.2.2 - MLPipeline Load/Save
+----------------------------
+
+* Implement save and load methods for MLPipelines
+* Add more datasets
+
+0.2.1 - New Documentation
+-------------------------
+
+* Add mlblocks.datasets module with demo data download functions.
+* Extensive documentation, including multiple pipeline examples.
+
+0.2.0 - New MLBlocks API
+------------------------
+
+A new MLBlocks API and Primitive format.
+
+This is a summary of the changes:
+
+* Primitives JSONs and Python code has been moved to a different repository, called MLPrimitives
+* Optional usage of multiple JSON primitive folders.
+* JSON format has been changed to allow more flexibility and features:
+    * input and output arguments, as well as argument types, can be specified for each method
+    * both classes and function as primitives are supported
+    * multitype and conditional hyperparameters fully supported
+    * data modalities and primitive classifiers introduced
+    * metadata such as documentation, description and author fields added
+* Parsers are removed, and now the MLBlock class is responsible for loading and reading the
+  JSON primitive.
+* Multiple blocks of the same primitive are supported within the same pipeline.
+* Arbitrary inputs and outputs for both pipelines and blocks are allowed.
+* Shared variables during pipeline execution, usable by multiple blocks.
+
+0.1.9 - Bugfix Release
+----------------------
+
+* Disable some NetworkX functions for incompatibilities with some types of graphs.
+
+0.1.8 - New primitives and some improvements
+--------------------------------------------
+
+* Improve the NetworkX primitives.
+* Add String Vectorization and Datetime Featurization primitives.
+* Refactor some Keras primitives to work with single dimension `y` arrays and be compatible with `pickle`.
+* Add XGBClassifier and XGBRegressor primitives.
+* Add some `keras.applications` pretrained networks as preprocessing primitives.
+* Add helper class to allow function primitives.
+
+0.1.7 - Nested hyperparams dicts
+--------------------------------
+
+* Support passing hyperparams as nested dicts.
+
+0.1.6 - Text and Graph Pipelines
+--------------------------------
+
+* Add LSTM classifier and regressor primitives.
+* Add OneHotEncoder and MultiLabelEncoder primitives.
+* Add several NetworkX graph featurization primitives.
+* Add `community.best_partition` primitive.
+
+0.1.5 - Collaborative Filtering Pipelines
+-----------------------------------------
+
+* Add LightFM primitive.
+
+0.1.4 - Image pipelines improved
+--------------------------------
+
+* Allow passing `init_params` on `MLPipeline` creation.
+* Fix bug with MLHyperparam types and Keras.
+* Rename `produce_params` as `predict_params`.
+* Add SingleCNN Classifier and Regressor primitives.
+* Simplify and improve Trivial Predictor
+
+0.1.3 - Multi Table pipelines improved
+--------------------------------------
+
+* Improve RandomForest primitive ranges
+* Improve DFS primitive
+* Add Tree Based Feature Selection primitives
+* Fix bugs in TrivialPredictor
+* Improved documentation
+
+0.1.2 - Bugfix release
+----------------------
+
+* Fix bug in TrivialMedianPredictor
+* Fix bug in OneHotLabelEncoder
+
+0.1.1 - Single Table pipelines improved
+---------------------------------------
+
+* New project structure and primitives for integration into MIT-TA2.
+* MIT-TA2 default pipelines and single table pipelines fully working.
+
+0.1.0
+-----
+
+* First release on PyPI.
```

#### html2text {}

```diff
@@ -1,11 +1,21 @@
-Metadata-Version: 2.1 Name: mlblocks Version: 0.5.0 Summary: Pipelines and
+Metadata-Version: 2.1 Name: mlblocks Version: 0.5.1.dev0 Summary: Pipelines and
 primitives for machine learning and data science. Home-page: https://
 github.com/MLBazaar/MLBlocks Author: MIT Data To AI Lab Author-email:
-dailabmit@gmail.com License: MIT license Description:
+dailabmit@gmail.com License: MIT license Keywords: auto machine learning
+classification regression data science pipeline Classifier: Development Status
+:: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6,<3.11 Description-Content-Type: text/markdown Provides-
+Extra: dev Provides-Extra: unit Provides-Extra: test Provides-Extra: examples
+Provides-Extra: mlprimitives License-File: LICENSE License-File: AUTHORS.rst
 [DAI-Lab] An Open Source Project from the Data_to_AI_Lab,_at_MIT
 [âMLBlocksâ]
 Pipelines and Primitives for Machine Learning and Data Science.
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi](https://img.shields.io/pypi/v/mlblocks.svg)](https://
 pypi.python.org/pypi/mlblocks) [![Tests](https://github.com/MLBazaar/MLBlocks/
@@ -28,27 +38,27 @@
 with little to no python code to write, carefully curated by Machine Learning
 and Domain experts. * Extract machine-readable information about which
 hyperparameters can be tuned and within which ranges, allowing automated
 integration with Hyperparameter Optimization tools like [BTB](https://
 github.com/MLBazaar/BTB). * Complex multi-branch pipelines and DAG
 configurations, with unlimited number of inputs and outputs per primitive. *
 Easy save and load Pipelines using JSON Annotations. # Install ## Requirements
-**MLBlocks** has been developed and tested on [Python 3.6, 3.7 and 3.8](https:/
-/www.python.org/downloads/) ## Install with `pip` The easiest and recommended
-way to install **MLBlocks** is using [pip]( https://pip.pypa.io/en/stable/):
-```bash pip install mlblocks ``` This will pull and install the latest stable
-release from [PyPi](https://pypi.org/). If you want to install from source or
-contribute to the project please read the [Contributing Guide](https://
-mlbazaar.github.io/MLBlocks/contributing.html#get-started). ## MLPrimitives In
-order to be usable, MLBlocks requires a compatible primitives library. The
-official library, required in order to follow the following MLBlocks tutorial,
-is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), which you can
-install with this command: ```bash pip install mlprimitives ``` # Quickstart
-Below there is a short example about how to use **MLBlocks** to solve the
-[Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/Adult)
+**MLBlocks** has been developed and tested on [Python 3.6, 3.7, 3.8, 3.9, and
+3.10](https://www.python.org/downloads/) ## Install with `pip` The easiest and
+recommended way to install **MLBlocks** is using [pip]( https://pip.pypa.io/en/
+stable/): ```bash pip install mlblocks ``` This will pull and install the
+latest stable release from [PyPi](https://pypi.org/). If you want to install
+from source or contribute to the project please read the [Contributing Guide]
+(https://mlbazaar.github.io/MLBlocks/contributing.html#get-started). ##
+MLPrimitives In order to be usable, MLBlocks requires a compatible primitives
+library. The official library, required in order to follow the following
+MLBlocks tutorial, is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives),
+which you can install with this command: ```bash pip install mlprimitives ``` #
+Quickstart Below there is a short example about how to use **MLBlocks** to
+solve the [Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/Adult)
 classification problem using a pipeline which combines primitives from
 [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), [scikit-learn](https:
 //scikit-learn.org/) and [xgboost](https://xgboost.readthedocs.io/). ```python3
 from mlblocks import MLPipeline from mlprimitives.datasets import load_dataset
 dataset = load_dataset('census') X_train, X_test, y_train, y_test =
 dataset.get_splits(1) primitives =
 [ 'mlprimitives.custom.preprocessing.ClassEncoder',
@@ -165,16 +175,8 @@
 ------------------------------------- * Improve RandomForest primitive ranges *
 Improve DFS primitive * Add Tree Based Feature Selection primitives * Fix bugs
 in TrivialPredictor * Improved documentation 0.1.2 - Bugfix release -----------
 ----------- * Fix bug in TrivialMedianPredictor * Fix bug in OneHotLabelEncoder
 0.1.1 - Single Table pipelines improved --------------------------------------
 - * New project structure and primitives for integration into MIT-TA2. * MIT-
 TA2 default pipelines and single table pipelines fully working. 0.1.0 ----- *
-First release on PyPI. Keywords: auto machine learning classification
-regression data science pipeline Platform: UNKNOWN Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3.6,<3.9
-Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-unit Provides-Extra: test Provides-Extra: examples Provides-Extra: mlprimitives
+First release on PyPI.
```

### Comparing `mlblocks-0.5.0/LICENSE` & `mlblocks-0.5.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/CONTRIBUTING.rst` & `mlblocks-0.5.1.dev0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/HISTORY.md` & `mlblocks-0.5.1.dev0/HISTORY.md`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/test_mlblock.py` & `mlblocks-0.5.1.dev0/tests/test_mlblock.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/features/test_partial_outputs.py` & `mlblocks-0.5.1.dev0/tests/features/test_partial_outputs.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/features/test_pipeline_loading.py` & `mlblocks-0.5.1.dev0/tests/features/test_pipeline_loading.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/features/test_fit_predicr_args.py` & `mlblocks-0.5.1.dev0/tests/features/test_fit_predicr_args.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/test_mlpipeline.py` & `mlblocks-0.5.1.dev0/tests/test_mlpipeline.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/test_discovery.py` & `mlblocks-0.5.1.dev0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/data/diagrams/diagram_multiple_blocks.txt` & `mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_multiple_blocks.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/data/diagrams/diagram_fit.txt` & `mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_fit.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/tests/data/diagrams/diagram_simple.txt` & `mlblocks-0.5.1.dev0/tests/data/diagrams/diagram_simple.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/mlblocks.egg-info/PKG-INFO` & `mlblocks-0.5.1.dev0/mlblocks.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,354 +1,357 @@
 Metadata-Version: 2.1
 Name: mlblocks
-Version: 0.5.0
+Version: 0.5.1.dev0
 Summary: Pipelines and primitives for machine learning and data science.
 Home-page: https://github.com/MLBazaar/MLBlocks
 Author: MIT Data To AI Lab
 Author-email: dailabmit@gmail.com
 License: MIT license
-Description: <p align="left">
-          <a href="https://dai.lids.mit.edu">
-            <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
-          </a>
-          <i>An Open Source Project from the <a href="https://dai.lids.mit.edu">Data to AI Lab, at MIT</a></i>
-        </p>
-        
-        <p align="left">
-        <img width=20% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/mlblocks-icon.png" alt=“MLBlocks” />
-        </p>
-        
-        <p align="left">
-        Pipelines and Primitives for Machine Learning and Data Science.
-        </p>
-        
-        [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-        [![PyPi](https://img.shields.io/pypi/v/mlblocks.svg)](https://pypi.python.org/pypi/mlblocks)
-        [![Tests](https://github.com/MLBazaar/MLBlocks/workflows/Run%20Tests/badge.svg)](https://github.com/MLBazaar/MLBlocks/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
-        [![CodeCov](https://codecov.io/gh/MLBazaar/MLBlocks/branch/master/graph/badge.svg)](https://codecov.io/gh/MLBazaar/MLBlocks)
-        [![Downloads](https://pepy.tech/badge/mlblocks)](https://pepy.tech/project/mlblocks)
-        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MLBazaar/MLBlocks/master?filepath=examples/tutorials)
-        
-        <br>
-        
-        # MLBlocks
-        
-        * Documentation: https://mlbazaar.github.io/MLBlocks
-        * Github: https://github.com/MLBazaar/MLBlocks
-        * License: [MIT](https://github.com/MLBazaar/MLBlocks/blob/master/LICENSE)
-        * Development Status: [Pre-Alpha](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
-        
-        ## Overview
-        
-        MLBlocks is a simple framework for composing end-to-end tunable Machine Learning Pipelines by
-        seamlessly combining tools from any python library with a simple, common and uniform interface.
-        
-        Features include:
-        
-        * Build Machine Learning Pipelines combining **any Machine Learning Library in Python**.
-        * Access a repository with hundreds of primitives and pipelines ready to be used with little to
-          no python code to write, carefully curated by Machine Learning and Domain experts.
-        * Extract machine-readable information about which hyperparameters can be tuned and within
-          which ranges, allowing automated integration with Hyperparameter Optimization tools like
-          [BTB](https://github.com/MLBazaar/BTB).
-        * Complex multi-branch pipelines and DAG configurations, with unlimited number of inputs and
-          outputs per primitive.
-        * Easy save and load Pipelines using JSON Annotations.
-        
-        # Install
-        
-        ## Requirements
-        
-        **MLBlocks** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
-        
-        ## Install with `pip`
-        
-        The easiest and recommended way to install **MLBlocks** is using [pip](
-        https://pip.pypa.io/en/stable/):
-        
-        ```bash
-        pip install mlblocks
-        ```
-        
-        This will pull and install the latest stable release from [PyPi](https://pypi.org/).
-        
-        If you want to install from source or contribute to the project please read the
-        [Contributing Guide](https://mlbazaar.github.io/MLBlocks/contributing.html#get-started).
-        
-        ## MLPrimitives
-        
-        In order to be usable, MLBlocks requires a compatible primitives library.
-        
-        The official library, required in order to follow the following MLBlocks tutorial,
-        is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), which you can install
-        with this command:
-        
-        ```bash
-        pip install mlprimitives
-        ```
-        
-        # Quickstart
-        
-        Below there is a short example about how to use **MLBlocks** to solve the [Adult Census
-        Dataset](https://archive.ics.uci.edu/ml/datasets/Adult) classification problem using a
-        pipeline which combines primitives from [MLPrimitives](https://github.com/MLBazaar/MLPrimitives),
-        [scikit-learn](https://scikit-learn.org/) and [xgboost](https://xgboost.readthedocs.io/).
-        
-        ```python3
-        from mlblocks import MLPipeline
-        from mlprimitives.datasets import load_dataset
-        
-        dataset = load_dataset('census')
-        X_train, X_test, y_train, y_test = dataset.get_splits(1)
-        
-        primitives = [
-            'mlprimitives.custom.preprocessing.ClassEncoder',
-            'mlprimitives.custom.feature_extraction.CategoricalEncoder',
-            'sklearn.impute.SimpleImputer',
-            'xgboost.XGBClassifier',
-            'mlprimitives.custom.preprocessing.ClassDecoder'
-        ]
-        pipeline = MLPipeline(primitives)
-        
-        pipeline.fit(X_train, y_train)
-        predictions = pipeline.predict(X_test)
-        
-        dataset.score(y_test, predictions)
-        ```
-        
-        # What's Next?
-        
-        If you want to learn more about how to tune the pipeline hyperparameters, save and load
-        the pipelines using JSON annotations or build complex multi-branched pipelines, please
-        check our [documentation site](https://mlbazaar.github.io/MLBlocks).
-        
-        Also do not forget to have a look at the [notebook tutorials](
-        https://github.com/MLBazaar/MLBlocks/tree/master/examples/tutorials)!
-        
-        # Citing MLBlocks
-        
-        If you use MLBlocks for your research, please consider citing our related papers.
-        
-        For the current design of MLBlocks and its usage within the larger *Machine Learning Bazaar* project at
-        the MIT Data To AI Lab, please see:
-        
-        Micah J. Smith, Carles Sala, James Max Kanter, and Kalyan Veeramachaneni. ["The Machine Learning Bazaar:
-        Harnessing the ML Ecosystem for Effective System Development."](https://arxiv.org/abs/1905.08942) arXiv
-        Preprint 1905.08942. 2019.
-        
-        ```bibtex
-        @article{smith2019mlbazaar,
-          author = {Smith, Micah J. and Sala, Carles and Kanter, James Max and Veeramachaneni, Kalyan},
-          title = {The Machine Learning Bazaar: Harnessing the ML Ecosystem for Effective System Development},
-          journal = {arXiv e-prints},
-          year = {2019},
-          eid = {arXiv:1905.08942},
-          pages = {arXiv:1905.08942},
-          archivePrefix = {arXiv},
-          eprint = {1905.08942},
-        }
-        ```
-        
-        For the first MLBlocks version from 2015, designed for only multi table, multi entity temporal data, please
-        refer to Bryan Collazo’s thesis:
-        
-        * [Machine learning blocks](https://dai.lids.mit.edu/wp-content/uploads/2018/06/Mlblocks_Bryan.pdf).
-          Bryan Collazo. Masters thesis, MIT EECS, 2015.
-        
-        With recent availability of a multitude of libraries and tools, we decided it was time to integrate
-        them and expand the library to address other data types: images, text, graph, time series and
-        integrate with deep learning libraries.
-        
-        
-        Changelog
-        =========
-        
-        0.5.0 - 2023-01-22
-        ------------------
-        
-        * Update `numpy` dependency and isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by @sarahmish
-        
-        0.4.1 - 2021-10-08
-        ------------------
-        
-        * Update NumPy dependency - [Issue #136](https://github.com/MLBazaar/MLBlocks/issues/136) by @sarahmish
-        * Support dynamic inputs and outputs - [Issue #134](https://github.com/MLBazaar/MLBlocks/issues/134) by @pvk-developer
-        
-        0.4.0 - 2021-01-09
-        ------------------
-        
-        * Stop pipeline fitting after the last block - [Issue #131](https://github.com/MLBazaar/MLBlocks/issues/131) by @sarahmish
-        * Add memory debug and profiling - [Issue #130](https://github.com/MLBazaar/MLBlocks/issues/130) by @pvk-developer
-        * Update Python support - [Issue #129](https://github.com/MLBazaar/MLBlocks/issues/129) by @csala
-        * Get execution time for each block - [Issue #127](https://github.com/MLBazaar/MLBlocks/issues/127) by @sarahmish
-        * Allow loading a primitive or pipeline directly from the JSON path - [Issue #114](https://github.com/MLBazaar/MLBlocks/issues/114) by @csala
-        * Pipeline Diagrams - [Issue #113](https://github.com/MLBazaar/MLBlocks/issues/113) by @erica-chiu
-        * Get Pipeline Inputs - [Issue #112](https://github.com/MLBazaar/MLBlocks/issues/112) by @erica-chiu
-        
-        0.3.4 - 2019-11-01
-        ------------------
-        
-        * Ability to return intermediate context - [Issue #110](https://github.com/MLBazaar/MLBlocks/issues/110) by @csala
-        * Support for static or class methods - [Issue #107](https://github.com/MLBazaar/MLBlocks/issues/107) by @csala
-        
-        0.3.3 - 2019-09-09
-        ------------------
-        
-        * Improved intermediate outputs management - [Issue #105](https://github.com/MLBazaar/MLBlocks/issues/105) by @csala
-        
-        0.3.2 - 2019-08-12
-        ------------------
-        
-        * Allow passing fit and produce arguments as `init_params` - [Issue #96](https://github.com/MLBazaar/MLBlocks/issues/96) by @csala
-        * Support optional fit and produce args and arg defaults - [Issue #95](https://github.com/MLBazaar/MLBlocks/issues/95) by @csala
-        * Isolate primitives from their hyperparameters dictionary - [Issue #94](https://github.com/MLBazaar/MLBlocks/issues/94) by @csala
-        * Add functions to explore the available primitives and pipelines - [Issue #90](https://github.com/MLBazaar/MLBlocks/issues/90) by @csala
-        * Add primitive caching - [Issue #22](https://github.com/MLBazaar/MLBlocks/issues/22) by @csala
-        
-        0.3.1 - Pipelines Discovery
-        ---------------------------
-        
-        * Support flat hyperparameter dictionaries - [Issue #92](https://github.com/MLBazaar/MLBlocks/issues/92) by @csala
-        * Load pipelines by name and register them as `entry_points` - [Issue #88](https://github.com/MLBazaar/MLBlocks/issues/88) by @csala
-        * Implement partial re-fit -[Issue #61](https://github.com/MLBazaar/MLBlocks/issues/61) by @csala
-        * Move argument parsing to MLBlock - [Issue #86](https://github.com/MLBazaar/MLBlocks/issues/86) by @csala
-        * Allow getting intermediate outputs - [Issue #58](https://github.com/MLBazaar/MLBlocks/issues/58) by @csala
-        
-        0.3.0 - New Primitives Discovery
-        --------------------------------
-        
-        * New primitives discovery system based on `entry_points`.
-        * Conditional Hyperparameters filtering in MLBlock initialization.
-        * Improved logging and exception reporting.
-        
-        0.2.4 - New Datasets and Unit Tests
-        -----------------------------------
-        
-        * Add a new multi-table dataset.
-        * Add Unit Tests up to 50% coverage.
-        * Improve documentation.
-        * Fix minor bug in newsgroups dataset.
-        
-        0.2.3 - Demo Datasets
-        ---------------------
-        
-        * Add new methods to Dataset class.
-        * Add documentation for the datasets module.
-        
-        0.2.2 - MLPipeline Load/Save
-        ----------------------------
-        
-        * Implement save and load methods for MLPipelines
-        * Add more datasets
-        
-        0.2.1 - New Documentation
-        -------------------------
-        
-        * Add mlblocks.datasets module with demo data download functions.
-        * Extensive documentation, including multiple pipeline examples.
-        
-        0.2.0 - New MLBlocks API
-        ------------------------
-        
-        A new MLBlocks API and Primitive format.
-        
-        This is a summary of the changes:
-        
-        * Primitives JSONs and Python code has been moved to a different repository, called MLPrimitives
-        * Optional usage of multiple JSON primitive folders.
-        * JSON format has been changed to allow more flexibility and features:
-            * input and output arguments, as well as argument types, can be specified for each method
-            * both classes and function as primitives are supported
-            * multitype and conditional hyperparameters fully supported
-            * data modalities and primitive classifiers introduced
-            * metadata such as documentation, description and author fields added
-        * Parsers are removed, and now the MLBlock class is responsible for loading and reading the
-          JSON primitive.
-        * Multiple blocks of the same primitive are supported within the same pipeline.
-        * Arbitrary inputs and outputs for both pipelines and blocks are allowed.
-        * Shared variables during pipeline execution, usable by multiple blocks.
-        
-        0.1.9 - Bugfix Release
-        ----------------------
-        
-        * Disable some NetworkX functions for incompatibilities with some types of graphs.
-        
-        0.1.8 - New primitives and some improvements
-        --------------------------------------------
-        
-        * Improve the NetworkX primitives.
-        * Add String Vectorization and Datetime Featurization primitives.
-        * Refactor some Keras primitives to work with single dimension `y` arrays and be compatible with `pickle`.
-        * Add XGBClassifier and XGBRegressor primitives.
-        * Add some `keras.applications` pretrained networks as preprocessing primitives.
-        * Add helper class to allow function primitives.
-        
-        0.1.7 - Nested hyperparams dicts
-        --------------------------------
-        
-        * Support passing hyperparams as nested dicts.
-        
-        0.1.6 - Text and Graph Pipelines
-        --------------------------------
-        
-        * Add LSTM classifier and regressor primitives.
-        * Add OneHotEncoder and MultiLabelEncoder primitives.
-        * Add several NetworkX graph featurization primitives.
-        * Add `community.best_partition` primitive.
-        
-        0.1.5 - Collaborative Filtering Pipelines
-        -----------------------------------------
-        
-        * Add LightFM primitive.
-        
-        0.1.4 - Image pipelines improved
-        --------------------------------
-        
-        * Allow passing `init_params` on `MLPipeline` creation.
-        * Fix bug with MLHyperparam types and Keras.
-        * Rename `produce_params` as `predict_params`.
-        * Add SingleCNN Classifier and Regressor primitives.
-        * Simplify and improve Trivial Predictor
-        
-        0.1.3 - Multi Table pipelines improved
-        --------------------------------------
-        
-        * Improve RandomForest primitive ranges
-        * Improve DFS primitive
-        * Add Tree Based Feature Selection primitives
-        * Fix bugs in TrivialPredictor
-        * Improved documentation
-        
-        0.1.2 - Bugfix release
-        ----------------------
-        
-        * Fix bug in TrivialMedianPredictor
-        * Fix bug in OneHotLabelEncoder
-        
-        0.1.1 - Single Table pipelines improved
-        ---------------------------------------
-        
-        * New project structure and primitives for integration into MIT-TA2.
-        * MIT-TA2 default pipelines and single table pipelines fully working.
-        
-        0.1.0
-        -----
-        
-        * First release on PyPI.
-        
 Keywords: auto machine learning classification regression data science pipeline
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6,<3.9
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6,<3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: unit
 Provides-Extra: test
 Provides-Extra: examples
 Provides-Extra: mlprimitives
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+<p align="left">
+  <a href="https://dai.lids.mit.edu">
+    <img width=15% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/Logo_DAI_highres.png" alt="DAI-Lab" />
+  </a>
+  <i>An Open Source Project from the <a href="https://dai.lids.mit.edu">Data to AI Lab, at MIT</a></i>
+</p>
+
+<p align="left">
+<img width=20% src="https://dai.lids.mit.edu/wp-content/uploads/2018/06/mlblocks-icon.png" alt=“MLBlocks” />
+</p>
+
+<p align="left">
+Pipelines and Primitives for Machine Learning and Data Science.
+</p>
+
+[![Development Status](https://img.shields.io/badge/Development%20Status-2%20--%20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+[![PyPi](https://img.shields.io/pypi/v/mlblocks.svg)](https://pypi.python.org/pypi/mlblocks)
+[![Tests](https://github.com/MLBazaar/MLBlocks/workflows/Run%20Tests/badge.svg)](https://github.com/MLBazaar/MLBlocks/actions?query=workflow%3A%22Run+Tests%22+branch%3Amaster)
+[![CodeCov](https://codecov.io/gh/MLBazaar/MLBlocks/branch/master/graph/badge.svg)](https://codecov.io/gh/MLBazaar/MLBlocks)
+[![Downloads](https://pepy.tech/badge/mlblocks)](https://pepy.tech/project/mlblocks)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/MLBazaar/MLBlocks/master?filepath=examples/tutorials)
+
+<br>
+
+# MLBlocks
+
+* Documentation: https://mlbazaar.github.io/MLBlocks
+* Github: https://github.com/MLBazaar/MLBlocks
+* License: [MIT](https://github.com/MLBazaar/MLBlocks/blob/master/LICENSE)
+* Development Status: [Pre-Alpha](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-+Pre-Alpha)
+
+## Overview
+
+MLBlocks is a simple framework for composing end-to-end tunable Machine Learning Pipelines by
+seamlessly combining tools from any python library with a simple, common and uniform interface.
+
+Features include:
+
+* Build Machine Learning Pipelines combining **any Machine Learning Library in Python**.
+* Access a repository with hundreds of primitives and pipelines ready to be used with little to
+  no python code to write, carefully curated by Machine Learning and Domain experts.
+* Extract machine-readable information about which hyperparameters can be tuned and within
+  which ranges, allowing automated integration with Hyperparameter Optimization tools like
+  [BTB](https://github.com/MLBazaar/BTB).
+* Complex multi-branch pipelines and DAG configurations, with unlimited number of inputs and
+  outputs per primitive.
+* Easy save and load Pipelines using JSON Annotations.
+
+# Install
+
+## Requirements
+
+**MLBlocks** has been developed and tested on [Python 3.6, 3.7, 3.8, 3.9, and 3.10](https://www.python.org/downloads/)
+
+## Install with `pip`
+
+The easiest and recommended way to install **MLBlocks** is using [pip](
+https://pip.pypa.io/en/stable/):
+
+```bash
+pip install mlblocks
+```
+
+This will pull and install the latest stable release from [PyPi](https://pypi.org/).
+
+If you want to install from source or contribute to the project please read the
+[Contributing Guide](https://mlbazaar.github.io/MLBlocks/contributing.html#get-started).
+
+## MLPrimitives
+
+In order to be usable, MLBlocks requires a compatible primitives library.
+
+The official library, required in order to follow the following MLBlocks tutorial,
+is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), which you can install
+with this command:
+
+```bash
+pip install mlprimitives
+```
+
+# Quickstart
+
+Below there is a short example about how to use **MLBlocks** to solve the [Adult Census
+Dataset](https://archive.ics.uci.edu/ml/datasets/Adult) classification problem using a
+pipeline which combines primitives from [MLPrimitives](https://github.com/MLBazaar/MLPrimitives),
+[scikit-learn](https://scikit-learn.org/) and [xgboost](https://xgboost.readthedocs.io/).
+
+```python3
+from mlblocks import MLPipeline
+from mlprimitives.datasets import load_dataset
+
+dataset = load_dataset('census')
+X_train, X_test, y_train, y_test = dataset.get_splits(1)
+
+primitives = [
+    'mlprimitives.custom.preprocessing.ClassEncoder',
+    'mlprimitives.custom.feature_extraction.CategoricalEncoder',
+    'sklearn.impute.SimpleImputer',
+    'xgboost.XGBClassifier',
+    'mlprimitives.custom.preprocessing.ClassDecoder'
+]
+pipeline = MLPipeline(primitives)
+
+pipeline.fit(X_train, y_train)
+predictions = pipeline.predict(X_test)
+
+dataset.score(y_test, predictions)
+```
+
+# What's Next?
+
+If you want to learn more about how to tune the pipeline hyperparameters, save and load
+the pipelines using JSON annotations or build complex multi-branched pipelines, please
+check our [documentation site](https://mlbazaar.github.io/MLBlocks).
+
+Also do not forget to have a look at the [notebook tutorials](
+https://github.com/MLBazaar/MLBlocks/tree/master/examples/tutorials)!
+
+# Citing MLBlocks
+
+If you use MLBlocks for your research, please consider citing our related papers.
+
+For the current design of MLBlocks and its usage within the larger *Machine Learning Bazaar* project at
+the MIT Data To AI Lab, please see:
+
+Micah J. Smith, Carles Sala, James Max Kanter, and Kalyan Veeramachaneni. ["The Machine Learning Bazaar:
+Harnessing the ML Ecosystem for Effective System Development."](https://arxiv.org/abs/1905.08942) arXiv
+Preprint 1905.08942. 2019.
+
+```bibtex
+@article{smith2019mlbazaar,
+  author = {Smith, Micah J. and Sala, Carles and Kanter, James Max and Veeramachaneni, Kalyan},
+  title = {The Machine Learning Bazaar: Harnessing the ML Ecosystem for Effective System Development},
+  journal = {arXiv e-prints},
+  year = {2019},
+  eid = {arXiv:1905.08942},
+  pages = {arXiv:1905.08942},
+  archivePrefix = {arXiv},
+  eprint = {1905.08942},
+}
+```
+
+For the first MLBlocks version from 2015, designed for only multi table, multi entity temporal data, please
+refer to Bryan Collazo’s thesis:
+
+* [Machine learning blocks](https://dai.lids.mit.edu/wp-content/uploads/2018/06/Mlblocks_Bryan.pdf).
+  Bryan Collazo. Masters thesis, MIT EECS, 2015.
+
+With recent availability of a multitude of libraries and tools, we decided it was time to integrate
+them and expand the library to address other data types: images, text, graph, time series and
+integrate with deep learning libraries.
+
+
+Changelog
+=========
+
+0.5.0 - 2023-01-22
+------------------
+
+* Update `numpy` dependency and isolate tests - [Issue #139](https://github.com/MLBazaar/MLBlocks/issues/139) by @sarahmish
+
+0.4.1 - 2021-10-08
+------------------
+
+* Update NumPy dependency - [Issue #136](https://github.com/MLBazaar/MLBlocks/issues/136) by @sarahmish
+* Support dynamic inputs and outputs - [Issue #134](https://github.com/MLBazaar/MLBlocks/issues/134) by @pvk-developer
+
+0.4.0 - 2021-01-09
+------------------
+
+* Stop pipeline fitting after the last block - [Issue #131](https://github.com/MLBazaar/MLBlocks/issues/131) by @sarahmish
+* Add memory debug and profiling - [Issue #130](https://github.com/MLBazaar/MLBlocks/issues/130) by @pvk-developer
+* Update Python support - [Issue #129](https://github.com/MLBazaar/MLBlocks/issues/129) by @csala
+* Get execution time for each block - [Issue #127](https://github.com/MLBazaar/MLBlocks/issues/127) by @sarahmish
+* Allow loading a primitive or pipeline directly from the JSON path - [Issue #114](https://github.com/MLBazaar/MLBlocks/issues/114) by @csala
+* Pipeline Diagrams - [Issue #113](https://github.com/MLBazaar/MLBlocks/issues/113) by @erica-chiu
+* Get Pipeline Inputs - [Issue #112](https://github.com/MLBazaar/MLBlocks/issues/112) by @erica-chiu
+
+0.3.4 - 2019-11-01
+------------------
+
+* Ability to return intermediate context - [Issue #110](https://github.com/MLBazaar/MLBlocks/issues/110) by @csala
+* Support for static or class methods - [Issue #107](https://github.com/MLBazaar/MLBlocks/issues/107) by @csala
+
+0.3.3 - 2019-09-09
+------------------
+
+* Improved intermediate outputs management - [Issue #105](https://github.com/MLBazaar/MLBlocks/issues/105) by @csala
+
+0.3.2 - 2019-08-12
+------------------
+
+* Allow passing fit and produce arguments as `init_params` - [Issue #96](https://github.com/MLBazaar/MLBlocks/issues/96) by @csala
+* Support optional fit and produce args and arg defaults - [Issue #95](https://github.com/MLBazaar/MLBlocks/issues/95) by @csala
+* Isolate primitives from their hyperparameters dictionary - [Issue #94](https://github.com/MLBazaar/MLBlocks/issues/94) by @csala
+* Add functions to explore the available primitives and pipelines - [Issue #90](https://github.com/MLBazaar/MLBlocks/issues/90) by @csala
+* Add primitive caching - [Issue #22](https://github.com/MLBazaar/MLBlocks/issues/22) by @csala
+
+0.3.1 - Pipelines Discovery
+---------------------------
+
+* Support flat hyperparameter dictionaries - [Issue #92](https://github.com/MLBazaar/MLBlocks/issues/92) by @csala
+* Load pipelines by name and register them as `entry_points` - [Issue #88](https://github.com/MLBazaar/MLBlocks/issues/88) by @csala
+* Implement partial re-fit -[Issue #61](https://github.com/MLBazaar/MLBlocks/issues/61) by @csala
+* Move argument parsing to MLBlock - [Issue #86](https://github.com/MLBazaar/MLBlocks/issues/86) by @csala
+* Allow getting intermediate outputs - [Issue #58](https://github.com/MLBazaar/MLBlocks/issues/58) by @csala
+
+0.3.0 - New Primitives Discovery
+--------------------------------
+
+* New primitives discovery system based on `entry_points`.
+* Conditional Hyperparameters filtering in MLBlock initialization.
+* Improved logging and exception reporting.
+
+0.2.4 - New Datasets and Unit Tests
+-----------------------------------
+
+* Add a new multi-table dataset.
+* Add Unit Tests up to 50% coverage.
+* Improve documentation.
+* Fix minor bug in newsgroups dataset.
+
+0.2.3 - Demo Datasets
+---------------------
+
+* Add new methods to Dataset class.
+* Add documentation for the datasets module.
+
+0.2.2 - MLPipeline Load/Save
+----------------------------
+
+* Implement save and load methods for MLPipelines
+* Add more datasets
+
+0.2.1 - New Documentation
+-------------------------
+
+* Add mlblocks.datasets module with demo data download functions.
+* Extensive documentation, including multiple pipeline examples.
+
+0.2.0 - New MLBlocks API
+------------------------
+
+A new MLBlocks API and Primitive format.
+
+This is a summary of the changes:
+
+* Primitives JSONs and Python code has been moved to a different repository, called MLPrimitives
+* Optional usage of multiple JSON primitive folders.
+* JSON format has been changed to allow more flexibility and features:
+    * input and output arguments, as well as argument types, can be specified for each method
+    * both classes and function as primitives are supported
+    * multitype and conditional hyperparameters fully supported
+    * data modalities and primitive classifiers introduced
+    * metadata such as documentation, description and author fields added
+* Parsers are removed, and now the MLBlock class is responsible for loading and reading the
+  JSON primitive.
+* Multiple blocks of the same primitive are supported within the same pipeline.
+* Arbitrary inputs and outputs for both pipelines and blocks are allowed.
+* Shared variables during pipeline execution, usable by multiple blocks.
+
+0.1.9 - Bugfix Release
+----------------------
+
+* Disable some NetworkX functions for incompatibilities with some types of graphs.
+
+0.1.8 - New primitives and some improvements
+--------------------------------------------
+
+* Improve the NetworkX primitives.
+* Add String Vectorization and Datetime Featurization primitives.
+* Refactor some Keras primitives to work with single dimension `y` arrays and be compatible with `pickle`.
+* Add XGBClassifier and XGBRegressor primitives.
+* Add some `keras.applications` pretrained networks as preprocessing primitives.
+* Add helper class to allow function primitives.
+
+0.1.7 - Nested hyperparams dicts
+--------------------------------
+
+* Support passing hyperparams as nested dicts.
+
+0.1.6 - Text and Graph Pipelines
+--------------------------------
+
+* Add LSTM classifier and regressor primitives.
+* Add OneHotEncoder and MultiLabelEncoder primitives.
+* Add several NetworkX graph featurization primitives.
+* Add `community.best_partition` primitive.
+
+0.1.5 - Collaborative Filtering Pipelines
+-----------------------------------------
+
+* Add LightFM primitive.
+
+0.1.4 - Image pipelines improved
+--------------------------------
+
+* Allow passing `init_params` on `MLPipeline` creation.
+* Fix bug with MLHyperparam types and Keras.
+* Rename `produce_params` as `predict_params`.
+* Add SingleCNN Classifier and Regressor primitives.
+* Simplify and improve Trivial Predictor
+
+0.1.3 - Multi Table pipelines improved
+--------------------------------------
+
+* Improve RandomForest primitive ranges
+* Improve DFS primitive
+* Add Tree Based Feature Selection primitives
+* Fix bugs in TrivialPredictor
+* Improved documentation
+
+0.1.2 - Bugfix release
+----------------------
+
+* Fix bug in TrivialMedianPredictor
+* Fix bug in OneHotLabelEncoder
+
+0.1.1 - Single Table pipelines improved
+---------------------------------------
+
+* New project structure and primitives for integration into MIT-TA2.
+* MIT-TA2 default pipelines and single table pipelines fully working.
+
+0.1.0
+-----
+
+* First release on PyPI.
```

#### html2text {}

```diff
@@ -1,11 +1,21 @@
-Metadata-Version: 2.1 Name: mlblocks Version: 0.5.0 Summary: Pipelines and
+Metadata-Version: 2.1 Name: mlblocks Version: 0.5.1.dev0 Summary: Pipelines and
 primitives for machine learning and data science. Home-page: https://
 github.com/MLBazaar/MLBlocks Author: MIT Data To AI Lab Author-email:
-dailabmit@gmail.com License: MIT license Description:
+dailabmit@gmail.com License: MIT license Keywords: auto machine learning
+classification regression data science pipeline Classifier: Development Status
+:: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6,<3.11 Description-Content-Type: text/markdown Provides-
+Extra: dev Provides-Extra: unit Provides-Extra: test Provides-Extra: examples
+Provides-Extra: mlprimitives License-File: LICENSE License-File: AUTHORS.rst
 [DAI-Lab] An Open Source Project from the Data_to_AI_Lab,_at_MIT
 [âMLBlocksâ]
 Pipelines and Primitives for Machine Learning and Data Science.
 [![Development Status](https://img.shields.io/badge/Development%20Status-2%20--
 %20Pre--Alpha-yellow)](https://pypi.org/search/?c=Development+Status+%3A%3A+2+-
 +Pre-Alpha) [![PyPi](https://img.shields.io/pypi/v/mlblocks.svg)](https://
 pypi.python.org/pypi/mlblocks) [![Tests](https://github.com/MLBazaar/MLBlocks/
@@ -28,27 +38,27 @@
 with little to no python code to write, carefully curated by Machine Learning
 and Domain experts. * Extract machine-readable information about which
 hyperparameters can be tuned and within which ranges, allowing automated
 integration with Hyperparameter Optimization tools like [BTB](https://
 github.com/MLBazaar/BTB). * Complex multi-branch pipelines and DAG
 configurations, with unlimited number of inputs and outputs per primitive. *
 Easy save and load Pipelines using JSON Annotations. # Install ## Requirements
-**MLBlocks** has been developed and tested on [Python 3.6, 3.7 and 3.8](https:/
-/www.python.org/downloads/) ## Install with `pip` The easiest and recommended
-way to install **MLBlocks** is using [pip]( https://pip.pypa.io/en/stable/):
-```bash pip install mlblocks ``` This will pull and install the latest stable
-release from [PyPi](https://pypi.org/). If you want to install from source or
-contribute to the project please read the [Contributing Guide](https://
-mlbazaar.github.io/MLBlocks/contributing.html#get-started). ## MLPrimitives In
-order to be usable, MLBlocks requires a compatible primitives library. The
-official library, required in order to follow the following MLBlocks tutorial,
-is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), which you can
-install with this command: ```bash pip install mlprimitives ``` # Quickstart
-Below there is a short example about how to use **MLBlocks** to solve the
-[Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/Adult)
+**MLBlocks** has been developed and tested on [Python 3.6, 3.7, 3.8, 3.9, and
+3.10](https://www.python.org/downloads/) ## Install with `pip` The easiest and
+recommended way to install **MLBlocks** is using [pip]( https://pip.pypa.io/en/
+stable/): ```bash pip install mlblocks ``` This will pull and install the
+latest stable release from [PyPi](https://pypi.org/). If you want to install
+from source or contribute to the project please read the [Contributing Guide]
+(https://mlbazaar.github.io/MLBlocks/contributing.html#get-started). ##
+MLPrimitives In order to be usable, MLBlocks requires a compatible primitives
+library. The official library, required in order to follow the following
+MLBlocks tutorial, is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives),
+which you can install with this command: ```bash pip install mlprimitives ``` #
+Quickstart Below there is a short example about how to use **MLBlocks** to
+solve the [Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/Adult)
 classification problem using a pipeline which combines primitives from
 [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), [scikit-learn](https:
 //scikit-learn.org/) and [xgboost](https://xgboost.readthedocs.io/). ```python3
 from mlblocks import MLPipeline from mlprimitives.datasets import load_dataset
 dataset = load_dataset('census') X_train, X_test, y_train, y_test =
 dataset.get_splits(1) primitives =
 [ 'mlprimitives.custom.preprocessing.ClassEncoder',
@@ -165,16 +175,8 @@
 ------------------------------------- * Improve RandomForest primitive ranges *
 Improve DFS primitive * Add Tree Based Feature Selection primitives * Fix bugs
 in TrivialPredictor * Improved documentation 0.1.2 - Bugfix release -----------
 ----------- * Fix bug in TrivialMedianPredictor * Fix bug in OneHotLabelEncoder
 0.1.1 - Single Table pipelines improved --------------------------------------
 - * New project structure and primitives for integration into MIT-TA2. * MIT-
 TA2 default pipelines and single table pipelines fully working. 0.1.0 ----- *
-First release on PyPI. Keywords: auto machine learning classification
-regression data science pipeline Platform: UNKNOWN Classifier: Development
-Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Requires-Python: >=3.6,<3.9
-Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-unit Provides-Extra: test Provides-Extra: examples Provides-Extra: mlprimitives
+First release on PyPI.
```

### Comparing `mlblocks-0.5.0/mlblocks.egg-info/SOURCES.txt` & `mlblocks-0.5.1.dev0/mlblocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/mlblocks.egg-info/requires.txt` & `mlblocks-0.5.1.dev0/mlblocks.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/index.rst` & `mlblocks-0.5.1.dev0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/advanced_usage/adding_primitives.rst` & `mlblocks-0.5.1.dev0/docs/advanced_usage/adding_primitives.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/advanced_usage/primitives.rst` & `mlblocks-0.5.1.dev0/docs/advanced_usage/primitives.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/advanced_usage/hyperparameters.rst` & `mlblocks-0.5.1.dev0/docs/advanced_usage/hyperparameters.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/advanced_usage/pipelines.rst` & `mlblocks-0.5.1.dev0/docs/advanced_usage/pipelines.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/images/mlblocks-logo-small.png` & `mlblocks-0.5.1.dev0/docs/images/mlblocks-logo-small.png`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/images/mlblocks-logo.png` & `mlblocks-0.5.1.dev0/docs/images/mlblocks-logo.png`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/Makefile` & `mlblocks-0.5.1.dev0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/conf.py` & `mlblocks-0.5.1.dev0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/make.bat` & `mlblocks-0.5.1.dev0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/pipeline_examples/single_table.rst` & `mlblocks-0.5.1.dev0/docs/pipeline_examples/single_table.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/pipeline_examples/multi_table.rst` & `mlblocks-0.5.1.dev0/docs/pipeline_examples/multi_table.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/pipeline_examples/graph.rst` & `mlblocks-0.5.1.dev0/docs/pipeline_examples/graph.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/pipeline_examples/text.rst` & `mlblocks-0.5.1.dev0/docs/pipeline_examples/text.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/pipeline_examples/image.rst` & `mlblocks-0.5.1.dev0/docs/pipeline_examples/image.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/getting_started/install.rst` & `mlblocks-0.5.1.dev0/docs/getting_started/install.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/docs/getting_started/quickstart.rst` & `mlblocks-0.5.1.dev0/docs/getting_started/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/README.md` & `mlblocks-0.5.1.dev0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
   outputs per primitive.
 * Easy save and load Pipelines using JSON Annotations.
 
 # Install
 
 ## Requirements
 
-**MLBlocks** has been developed and tested on [Python 3.6, 3.7 and 3.8](https://www.python.org/downloads/)
+**MLBlocks** has been developed and tested on [Python 3.6, 3.7, 3.8, 3.9, and 3.10](https://www.python.org/downloads/)
 
 ## Install with `pip`
 
 The easiest and recommended way to install **MLBlocks** is using [pip](
 https://pip.pypa.io/en/stable/):
 
 ```bash
```

#### html2text {}

```diff
@@ -24,27 +24,27 @@
 with little to no python code to write, carefully curated by Machine Learning
 and Domain experts. * Extract machine-readable information about which
 hyperparameters can be tuned and within which ranges, allowing automated
 integration with Hyperparameter Optimization tools like [BTB](https://
 github.com/MLBazaar/BTB). * Complex multi-branch pipelines and DAG
 configurations, with unlimited number of inputs and outputs per primitive. *
 Easy save and load Pipelines using JSON Annotations. # Install ## Requirements
-**MLBlocks** has been developed and tested on [Python 3.6, 3.7 and 3.8](https:/
-/www.python.org/downloads/) ## Install with `pip` The easiest and recommended
-way to install **MLBlocks** is using [pip]( https://pip.pypa.io/en/stable/):
-```bash pip install mlblocks ``` This will pull and install the latest stable
-release from [PyPi](https://pypi.org/). If you want to install from source or
-contribute to the project please read the [Contributing Guide](https://
-mlbazaar.github.io/MLBlocks/contributing.html#get-started). ## MLPrimitives In
-order to be usable, MLBlocks requires a compatible primitives library. The
-official library, required in order to follow the following MLBlocks tutorial,
-is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), which you can
-install with this command: ```bash pip install mlprimitives ``` # Quickstart
-Below there is a short example about how to use **MLBlocks** to solve the
-[Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/Adult)
+**MLBlocks** has been developed and tested on [Python 3.6, 3.7, 3.8, 3.9, and
+3.10](https://www.python.org/downloads/) ## Install with `pip` The easiest and
+recommended way to install **MLBlocks** is using [pip]( https://pip.pypa.io/en/
+stable/): ```bash pip install mlblocks ``` This will pull and install the
+latest stable release from [PyPi](https://pypi.org/). If you want to install
+from source or contribute to the project please read the [Contributing Guide]
+(https://mlbazaar.github.io/MLBlocks/contributing.html#get-started). ##
+MLPrimitives In order to be usable, MLBlocks requires a compatible primitives
+library. The official library, required in order to follow the following
+MLBlocks tutorial, is [MLPrimitives](https://github.com/MLBazaar/MLPrimitives),
+which you can install with this command: ```bash pip install mlprimitives ``` #
+Quickstart Below there is a short example about how to use **MLBlocks** to
+solve the [Adult Census Dataset](https://archive.ics.uci.edu/ml/datasets/Adult)
 classification problem using a pipeline which combines primitives from
 [MLPrimitives](https://github.com/MLBazaar/MLPrimitives), [scikit-learn](https:
 //scikit-learn.org/) and [xgboost](https://xgboost.readthedocs.io/). ```python3
 from mlblocks import MLPipeline from mlprimitives.datasets import load_dataset
 dataset = load_dataset('census') X_train, X_test, y_train, y_test =
 dataset.get_splits(1) primitives =
 [ 'mlprimitives.custom.preprocessing.ClassEncoder',
```

### Comparing `mlblocks-0.5.0/setup.py` & `mlblocks-0.5.1.dev0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     description='Pipelines and primitives for machine learning and data science.',
     extras_require={
         'dev': development_requires + tests_require + examples_require,
         'unit': tests_require,
         'test': tests_require + examples_require,
         'examples': examples_require,
@@ -109,15 +111,15 @@
     install_requires=install_requires,
     keywords='auto machine learning classification regression data science pipeline',
     license='MIT license',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     name='mlblocks',
     packages=find_packages(include=['mlblocks', 'mlblocks.*']),
-    python_requires='>=3.6,<3.9',
+    python_requires='>=3.6,<3.11',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/MLBazaar/MLBlocks',
-    version='0.5.0',
+    version='0.5.1.dev0',
     zip_safe=False,
 )
```

### Comparing `mlblocks-0.5.0/setup.cfg` & `mlblocks-0.5.1.dev0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.0
+current_version = 0.5.1.dev0
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `mlblocks-0.5.0/mlblocks/mlblock.py` & `mlblocks-0.5.1.dev0/mlblocks/mlblock.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/mlblocks/discovery.py` & `mlblocks-0.5.1.dev0/mlblocks/discovery.py`

 * *Files identical despite different names*

### Comparing `mlblocks-0.5.0/mlblocks/__init__.py` & `mlblocks-0.5.1.dev0/mlblocks/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from mlblocks.mlblock import MLBlock
 from mlblocks.mlpipeline import MLPipeline
 
 __author__ = 'MIT Data To AI Lab'
 __copyright__ = 'Copyright (c) 2018, MIT Data To AI Lab'
 __email__ = 'dailabmit@gmail.com'
 __license__ = 'MIT'
-__version__ = '0.5.0'
+__version__ = '0.5.1.dev0'
 
 __all__ = [
     'MLBlock',
     'MLPipeline',
     'add_pipelines_path',
     'add_primitives_path',
     'find_pipelines',
```

### Comparing `mlblocks-0.5.0/mlblocks/mlpipeline.py` & `mlblocks-0.5.1.dev0/mlblocks/mlpipeline.py`

 * *Files identical despite different names*

