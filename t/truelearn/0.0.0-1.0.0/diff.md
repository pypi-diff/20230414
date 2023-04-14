# Comparing `tmp/truelearn-0.0.0.tar.gz` & `tmp/truelearn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truelearn-0.0.0.tar", last modified: Tue Jan 17 12:43:56 2023, max compression
+gzip compressed data, was "/home/runner/work/truelearn/truelearn/dist/.tmp-c7b6n0nu/truelearn-1.0.0.tar", last modified: Fri Apr 14 14:38:52 2023, max compression
```

## Comparing `truelearn-0.0.0.tar` & `truelearn-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 12:43:56.948912 truelearn-0.0.0/
--rw-rw-rw-   0        0        0      113 2023-01-17 12:43:56.948912 truelearn-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-01-17 12:41:42.000000 truelearn-0.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-17 12:43:56.911129 truelearn-0.0.0/models/
--rw-rw-rw-   0        0        0        0 2023-01-17 12:40:26.000000 truelearn-0.0.0/models/__init__.py
--rw-rw-rw-   0        0        0      115 2023-01-17 12:43:56.948912 truelearn-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      260 2023-01-17 12:43:51.000000 truelearn-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-17 12:43:56.917645 truelearn-0.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-01-17 12:35:36.000000 truelearn-0.0.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-17 12:43:56.933285 truelearn-0.0.0/truelearn.egg-info/
--rw-rw-rw-   0        0        0      113 2023-01-17 12:43:56.000000 truelearn-0.0.0/truelearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-01-17 12:43:56.000000 truelearn-0.0.0/truelearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 12:43:56.000000 truelearn-0.0.0/truelearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-01-17 12:43:56.000000 truelearn-0.0.0/truelearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-14 14:38:40.000000 truelearn-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-14 14:38:52.000000 truelearn-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-04-14 14:38:40.000000 truelearn-1.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-14 14:38:41.000000 truelearn-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:38:52.000000 truelearn-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/datasets/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/datasets/_peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn/learning/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17749 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/_engage_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/_ink_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/_interest_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/_knowledge_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/_majority_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/_novelty_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/learning/_persistent_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/models/_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/models/_knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/models/_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/preprocessing/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/preprocessing/_wikifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn/utils/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/metrics/_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn/utils/visualisations/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_bar_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_bubble_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_dot_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_line_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_pie_rose_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_radar_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_treemap_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-04-14 14:38:41.000000 truelearn-1.0.0/truelearn/utils/visualisations/_word_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 14:38:52.000000 truelearn-1.0.0/truelearn.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

