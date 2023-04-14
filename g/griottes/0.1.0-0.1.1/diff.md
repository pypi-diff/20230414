# Comparing `tmp/griottes-0.1.0.tar.gz` & `tmp/griottes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griottes-0.1.0.tar", last modified: Mon Mar  6 16:12:16 2023, max compression
+gzip compressed data, was "griottes-0.1.1.tar", last modified: Fri Apr 14 14:10:44 2023, max compression
```

## Comparing `griottes-0.1.0.tar` & `griottes-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.046088 griottes-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.026088 griottes-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.034088 griottes-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-06 16:11:57.000000 griottes-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-06 16:11:57.000000 griottes-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-06 16:11:57.000000 griottes-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-06 16:11:57.000000 griottes-0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-06 16:11:57.000000 griottes-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-06 16:12:16.046088 griottes-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-03-06 16:11:57.000000 griottes-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.034088 griottes-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.038088 griottes-0.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.038088 griottes-0.1.0/docs/source/API/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/API/griottes.rst
--rw-r--r--   0 runner    (1001) docker     (123)   461609 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/Figure_2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   448994 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/Figure_3.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)   259728 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/Figure_4.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-06 16:11:57.000000 griottes-0.1.0/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-06 16:11:57.000000 griottes-0.1.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.038088 griottes-0.1.0/example_notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   461609 2023-03-06 16:11:57.000000 griottes-0.1.0/example_notebooks/Figure_2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   448994 2023-03-06 16:11:57.000000 griottes-0.1.0/example_notebooks/Figure_3.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)   259728 2023-03-06 16:11:57.000000 griottes-0.1.0/example_notebooks/Figure_4.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.038088 griottes-0.1.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   394043 2023-03-06 16:11:57.000000 griottes-0.1.0/images/griottes_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    69204 2023-03-06 16:11:57.000000 griottes-0.1.0/images/intro_graphs_construction.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.026088 griottes-0.1.0/pip-wheel-metadata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.042088 griottes-0.1.0/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-06 16:11:57.000000 griottes-0.1.0/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-06 16:11:57.000000 griottes-0.1.0/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/METADATA
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 16:11:57.000000 griottes-0.1.0/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-06 16:11:57.000000 griottes-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-06 16:11:57.000000 griottes-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-06 16:12:16.046088 griottes-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 16:11:57.000000 griottes-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.026088 griottes-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.042088 griottes-0.1.0/src/griottes/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-06 16:12:15.000000 griottes-0.1.0/src/griottes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.042088 griottes-0.1.0/src/griottes/analyse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/analyse/cell_property_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/analyse/voronoi_cell_property_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.046088 griottes-0.1.0/src/griottes/graphmaker/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/graphmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/graphmaker/graph_generation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/graphmaker/make_spheroids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.046088 griottes-0.1.0/src/griottes/graphplotter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/graphplotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/graphplotter/graph_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.046088 griottes-0.1.0/src/griottes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/tests/test_analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-03-06 16:11:57.000000 griottes-0.1.0/src/griottes/tests/test_graphmaker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 16:12:16.042088 griottes-0.1.0/src/griottes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-06 16:12:15.000000 griottes-0.1.0/src/griottes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-03-06 16:12:16.000000 griottes-0.1.0/src/griottes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 16:12:15.000000 griottes-0.1.0/src/griottes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-06 16:12:15.000000 griottes-0.1.0/src/griottes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 16:12:15.000000 griottes-0.1.0/src/griottes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-06 16:11:57.000000 griottes-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.719145 griottes-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.695143 griottes-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.703144 griottes-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-14 14:10:26.000000 griottes-0.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-14 14:10:26.000000 griottes-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 14:10:26.000000 griottes-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-14 14:10:26.000000 griottes-0.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 14:10:26.000000 griottes-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-14 14:10:44.719145 griottes-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-04-14 14:10:26.000000 griottes-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.703144 griottes-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.707144 griottes-0.1.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.707144 griottes-0.1.1/docs/source/API/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/API/griottes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   461609 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/Figure_2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   448994 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/Figure_3.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)   259728 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/Figure_4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 14:10:26.000000 griottes-0.1.1/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 14:10:26.000000 griottes-0.1.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.711144 griottes-0.1.1/example_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   461609 2023-04-14 14:10:26.000000 griottes-0.1.1/example_notebooks/Figure_2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   448994 2023-04-14 14:10:26.000000 griottes-0.1.1/example_notebooks/Figure_3.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)   259728 2023-04-14 14:10:26.000000 griottes-0.1.1/example_notebooks/Figure_4.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.711144 griottes-0.1.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   394043 2023-04-14 14:10:26.000000 griottes-0.1.1/images/griottes_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69204 2023-04-14 14:10:26.000000 griottes-0.1.1/images/intro_graphs_construction.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.699144 griottes-0.1.1/pip-wheel-metadata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.715144 griottes-0.1.1/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 14:10:26.000000 griottes-0.1.1/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-14 14:10:26.000000 griottes-0.1.1/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/METADATA
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 14:10:26.000000 griottes-0.1.1/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-14 14:10:26.000000 griottes-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 14:10:26.000000 griottes-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-14 14:10:44.719145 griottes-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:10:26.000000 griottes-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.699144 griottes-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.715144 griottes-0.1.1/src/griottes/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 14:10:44.000000 griottes-0.1.1/src/griottes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.715144 griottes-0.1.1/src/griottes/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/analyse/cell_property_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/analyse/voronoi_cell_property_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.719145 griottes-0.1.1/src/griottes/graphmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/graphmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19746 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/graphmaker/graph_generation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/graphmaker/make_spheroids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.719145 griottes-0.1.1/src/griottes/graphplotter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/graphplotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/graphplotter/graph_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.719145 griottes-0.1.1/src/griottes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/tests/test_analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-14 14:10:26.000000 griottes-0.1.1/src/griottes/tests/test_graphmaker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:10:44.715144 griottes-0.1.1/src/griottes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-14 14:10:44.000000 griottes-0.1.1/src/griottes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-14 14:10:44.000000 griottes-0.1.1/src/griottes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:10:44.000000 griottes-0.1.1/src/griottes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 14:10:44.000000 griottes-0.1.1/src/griottes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 14:10:44.000000 griottes-0.1.1/src/griottes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 14:10:26.000000 griottes-0.1.1/tox.ini
```

### Comparing `griottes-0.1.0/.github/workflows/main.yml` & `griottes-0.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/.gitignore` & `griottes-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/.readthedocs.yaml` & `griottes-0.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/LICENSE` & `griottes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/PKG-INFO` & `griottes-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griottes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python program to generate NetworkX graphs from segmented images
 Author: 
 Gustave Ronteix
 Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: MIT
 Project-URL: Source code, "https://github.com/BaroudLab/Griottes",
```

### Comparing `griottes-0.1.0/README.md` & `griottes-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/Makefile` & `griottes-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/make.bat` & `griottes-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/source/API/griottes.rst` & `griottes-0.1.1/docs/source/API/griottes.rst`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/source/Figure_2.ipynb` & `griottes-0.1.1/docs/source/Figure_2.ipynb`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/source/Figure_3.ipynb` & `griottes-0.1.1/docs/source/Figure_3.ipynb`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/source/Figure_4.ipynb` & `griottes-0.1.1/docs/source/Figure_4.ipynb`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/source/conf.py` & `griottes-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/source/index.rst` & `griottes-0.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/docs/source/installation.rst` & `griottes-0.1.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/example_notebooks/Figure_2.ipynb` & `griottes-0.1.1/example_notebooks/Figure_2.ipynb`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/example_notebooks/Figure_3.ipynb` & `griottes-0.1.1/example_notebooks/Figure_3.ipynb`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/example_notebooks/Figure_4.ipynb` & `griottes-0.1.1/example_notebooks/Figure_4.ipynb`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/images/griottes_example.png` & `griottes-0.1.1/images/griottes_example.png`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/images/intro_graphs_construction.png` & `griottes-0.1.1/images/intro_graphs_construction.png`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/LICENSE` & `griottes-0.1.1/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/METADATA` & `griottes-0.1.1/pip-wheel-metadata/griottes-0.0.6.dev18+g284644c.d20230306.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/setup.cfg` & `griottes-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/src/griottes/analyse/voronoi_cell_property_analysis.py` & `griottes-0.1.1/src/griottes/analyse/voronoi_cell_property_analysis.py`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/src/griottes/graphmaker/graph_generation_func.py` & `griottes-0.1.1/src/griottes/graphmaker/graph_generation_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     mask_channel=None,
     min_area=0,
     analyze_fluo_channels=True,
     image_is_2D=True,
     fluo_channel_analysis_method="basic",
     descriptors=[],
     radius=30,
+    **kwargs
 ):
     """
     Creates a contact graph.
     This function creates a contact graph from an
     image. The contact graph is a graph where each node
     represents a region and each edge represents a contact
     between two adjascent regions.
```

### Comparing `griottes-0.1.0/src/griottes/graphmaker/make_spheroids.py` & `griottes-0.1.1/src/griottes/graphmaker/make_spheroids.py`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/src/griottes/graphplotter/graph_plot.py` & `griottes-0.1.1/src/griottes/graphplotter/graph_plot.py`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/src/griottes/tests/test_analyse.py` & `griottes-0.1.1/src/griottes/tests/test_analyse.py`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/src/griottes/tests/test_graphmaker.py` & `griottes-0.1.1/src/griottes/tests/test_graphmaker.py`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/src/griottes.egg-info/PKG-INFO` & `griottes-0.1.1/src/griottes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griottes
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python program to generate NetworkX graphs from segmented images
 Author: 
 Gustave Ronteix
 Andrey Aristov
 Author-email: aaristov@pasteur.fr
 License: MIT
 Project-URL: Source code, "https://github.com/BaroudLab/Griottes",
```

### Comparing `griottes-0.1.0/src/griottes.egg-info/SOURCES.txt` & `griottes-0.1.1/src/griottes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `griottes-0.1.0/tox.ini` & `griottes-0.1.1/tox.ini`

 * *Files identical despite different names*

