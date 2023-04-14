# Comparing `tmp/pyreason-1.2.9.tar.gz` & `tmp/pyreason-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreason-1.2.9.tar", last modified: Tue Mar 21 03:33:38 2023, max compression
+gzip compressed data, was "pyreason-1.3.0.tar", last modified: Fri Apr 14 12:16:43 2023, max compression
```

## Comparing `pyreason-1.2.9.tar` & `pyreason-1.3.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.679835 pyreason-1.2.9/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-03-21 03:33:24.000000 pyreason-1.2.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-21 03:33:24.000000 pyreason-1.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-03-21 03:33:38.679835 pyreason-1.2.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3132 2023-03-21 03:33:24.000000 pyreason-1.2.9/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.667835 pyreason-1.2.9/pyreason/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/.cache_status.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.671835 pyreason-1.2.9/pyreason/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.671835 pyreason-1.2.9/pyreason/examples/hello-world/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/examples/hello-world/facts.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/examples/hello-world/friends.graphml
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/examples/hello-world/ipl.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/examples/hello-world/labels.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/examples/hello-world/rules.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)    18900 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/pyreason.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.671835 pyreason-1.2.9/pyreason/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.671835 pyreason-1.2.9/pyreason/scripts/annotation_functions/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/annotation_functions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/annotation_functions/annotation_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.671835 pyreason-1.2.9/pyreason/scripts/components/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/components/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/components/label.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/components/world.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4649 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/diffuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.675835 pyreason-1.2.9/pyreason/scripts/facts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/facts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/facts/fact_edge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/facts/fact_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.675835 pyreason-1.2.9/pyreason/scripts/interpretation/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/interpretation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    64721 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/interpretation/interpretation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.675835 pyreason-1.2.9/pyreason/scripts/interval/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/interval/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1727 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/interval/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.675835 pyreason-1.2.9/pyreason/scripts/numba_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/numba_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.675835 pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/label_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/world_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.675835 pyreason-1.2.9/pyreason/scripts/program/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/program/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1464 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/program/program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.675835 pyreason-1.2.9/pyreason/scripts/rules/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/rules/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.679835 pyreason-1.2.9/pyreason/scripts/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3346 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/utils/filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/utils/graphml_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3187 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/utils/output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/utils/plotter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/utils/visuals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-03-21 03:33:24.000000 pyreason-1.2.9/pyreason/scripts/utils/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 03:33:38.671835 pyreason-1.2.9/pyreason.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-03-21 03:33:38.000000 pyreason-1.2.9/pyreason.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-21 03:33:38.000000 pyreason-1.2.9/pyreason.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 03:33:38.000000 pyreason-1.2.9/pyreason.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-21 03:33:38.000000 pyreason-1.2.9/pyreason.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-21 03:33:38.000000 pyreason-1.2.9/pyreason.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 03:33:38.679835 pyreason-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-03-21 03:33:24.000000 pyreason-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.054364 pyreason-1.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-04-14 12:16:29.000000 pyreason-1.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 12:16:29.000000 pyreason-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-14 12:16:43.054364 pyreason-1.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3261 2023-04-14 12:16:29.000000 pyreason-1.3.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       85 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.046363 pyreason-1.3.0/pyreason/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/.cache_status.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/examples/hello-world/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2646 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/facts.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/friends.graphml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/ipl.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/labels.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1048 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/examples/hello-world/rules.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21896 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/pyreason.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/annotation_functions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/annotation_functions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3398 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/annotation_functions/annotation_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6555 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/components/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/components/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/components/label.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1356 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/components/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4649 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/diffuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/facts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/facts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/facts/fact_edge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/facts/fact_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/interpretation/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/interpretation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65031 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/interpretation/interpretation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/interval/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/interval/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/interval/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/numba_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6220 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5992 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4186 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2933 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10162 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4779 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.054364 pyreason-1.3.0/pyreason/scripts/program/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/program/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1793 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/program/program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.054364 pyreason-1.3.0/pyreason/scripts/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/rules/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.054364 pyreason-1.3.0/pyreason/scripts/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3346 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4217 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/graphml_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3375 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2763 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/plotter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/visuals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-04-14 12:16:29.000000 pyreason-1.3.0/pyreason/scripts/utils/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:16:43.050364 pyreason-1.3.0/pyreason.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 12:16:43.000000 pyreason-1.3.0/pyreason.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:16:43.054364 pyreason-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-14 12:16:29.000000 pyreason-1.3.0/setup.py
```

### Comparing `pyreason-1.2.9/LICENSE.md` & `pyreason-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/PKG-INFO` & `pyreason-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.2.9
+Version: 1.3.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
@@ -24,15 +24,17 @@
 An explainable inference software supporting annotated, real valued, graph based and temporal logic.
 
 ## Links
 Paper: https://arxiv.org/abs/2302.13482
 
 Video: https://www.youtube.com/watch?v=E1PSl3KQCmo
 
-Website: https://neurosymoblic.asu.edu/pyreason/
+Website: https://neurosymbolic.asu.edu/pyreason/
+
+PyReason Gym: https://github.com/lab-v2/pyreason-gym
 
 Check out the [PyReason Hello World](https://github.com/lab-v2/pyreason/blob/main/docs/hello-world.md) program if you're new, or want get get a feel for the software.
 
 
 ## Table of Contents
   
 1. [Introduction](#1-introduction)
@@ -56,17 +58,19 @@
 
 The format of these files is very important. Please refer to the [example YAML files provided](https://github.com/lab-v2/pyreason/blob/main/pyreason/examples/example_yamls) when making your own rules/facts/labels/ipl. TODO: make doc for each format.
 
 ## 2. Install
 PyReason can be installed as a python library (recommended) or as a command line tool
 
 ## 2.1 Install as a Python Library
-This might take a minute or two
+We import pyreason to initialize it for the first time, this may take a few minutes
 ```bash
 pip install pyreason
+python
+import pyreason
 ```
 
 ## 2.2 Install as a Command Line Tool
 
 ```bash
 git clone https://github.com/lab-v2/pyreason
 cd pyreason
```

### Comparing `pyreason-1.2.9/README.md` & `pyreason-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 An explainable inference software supporting annotated, real valued, graph based and temporal logic.
 
 ## Links
 Paper: https://arxiv.org/abs/2302.13482
 
 Video: https://www.youtube.com/watch?v=E1PSl3KQCmo
 
-Website: https://neurosymoblic.asu.edu/pyreason/
+Website: https://neurosymbolic.asu.edu/pyreason/
+
+PyReason Gym: https://github.com/lab-v2/pyreason-gym
 
 Check out the [PyReason Hello World](https://github.com/lab-v2/pyreason/blob/main/docs/hello-world.md) program if you're new, or want get get a feel for the software.
 
 
 ## Table of Contents
   
 1. [Introduction](#1-introduction)
@@ -39,17 +41,19 @@
 
 The format of these files is very important. Please refer to the [example YAML files provided](https://github.com/lab-v2/pyreason/blob/main/pyreason/examples/example_yamls) when making your own rules/facts/labels/ipl. TODO: make doc for each format.
 
 ## 2. Install
 PyReason can be installed as a python library (recommended) or as a command line tool
 
 ## 2.1 Install as a Python Library
-This might take a minute or two
+We import pyreason to initialize it for the first time, this may take a few minutes
 ```bash
 pip install pyreason
+python
+import pyreason
 ```
 
 ## 2.2 Install as a Command Line Tool
 
 ```bash
 git clone https://github.com/lab-v2/pyreason
 cd pyreason
```

### Comparing `pyreason-1.2.9/pyreason/__init__.py` & `pyreason-1.3.0/pyreason/__init__.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/examples/hello-world/facts.yaml` & `pyreason-1.3.0/pyreason/examples/hello-world/facts.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/examples/hello-world/friends.graphml` & `pyreason-1.3.0/pyreason/examples/hello-world/friends.graphml`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/examples/hello-world/rules.yaml` & `pyreason-1.3.0/pyreason/examples/hello-world/rules.yaml`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/pyreason.py` & `pyreason-1.3.0/pyreason/pyreason.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # This is the file that will be imported when "import pyreason" is called. All content will be run automatically
 import numba
 import time
 import sys
 import warnings
 import memory_profiler as mp
-from typing import List
+from typing import List, Type
 
 from pyreason.scripts.utils.output import Output
 from pyreason.scripts.utils.filter import Filter
 from pyreason.scripts.program.program import Program
+from pyreason.scripts.interpretation.interpretation import Interpretation
 from pyreason.scripts.utils.graphml_parser import GraphmlParser
 import pyreason.scripts.utils.yaml_parser as yaml_parser
 import pyreason.scripts.numba_wrapper.numba_types.label_type as label
 import pyreason.scripts.numba_wrapper.numba_types.fact_node_type as fact_node
 import pyreason.scripts.numba_wrapper.numba_types.fact_edge_type as fact_edge
 import pyreason.scripts.numba_wrapper.numba_types.interval_type as interval
 
@@ -32,106 +33,106 @@
         self.__save_graph_attributes_to_trace = False
         self.__canonical = False
         self.__inconsistency_check = True
         self.__static_graph_facts = True
 
     @property
     def verbose(self) -> bool:
-        """Returns whether verbose mode is on or not
+        """Returns whether verbose mode is on or not. Default is True
 
         :return: bool
         """
         return self.__verbose
     
     @property
     def output_to_file(self) -> bool:
-        """Returns whether output is going to be printed to file or not
+        """Returns whether output is going to be printed to file or not. Default is False
 
         :return: bool
         """
         return self.__output_to_file
 
     @property
     def output_file_name(self) -> str:
-        """Returns whether name of the file output will be saved in. Only applicable if `output_to_file` is true
+        """Returns whether name of the file output will be saved in. Only applicable if `output_to_file` is true. Default is pyreason_output
 
         :return: str
         """
         return self.__output_file_name
 
     @property
     def graph_attribute_parsing(self) -> bool:
-        """Returns whether graph will be parsed for attributes or not
+        """Returns whether graph will be parsed for attributes or not. Default is True
 
         :return: bool
         """
         return self.__graph_attribute_parsing
 
     @property
     def abort_on_inconsistency(self) -> bool:
-        """Returns whether program will abort when it encounters an inconsistency in the interpretation or not
+        """Returns whether program will abort when it encounters an inconsistency in the interpretation or not. Default is False
 
         :return: bool
         """
         return self.__abort_on_inconsistency
 
     @property
     def memory_profile(self) -> bool:
-        """Returns whether program will profile maximum memory usage or not
+        """Returns whether program will profile maximum memory usage or not. Default is False
 
         :return: bool
         """
         return self.__memory_profile
 
     @property
     def reverse_digraph(self) -> bool:
         """Returns whether graph will be reversed or not.
-        If graph is reversed, an edge a->b will become b->a
+        If graph is reversed, an edge a->b will become b->a. Default is False
 
         :return: bool
         """
         return self.__reverse_digraph
 
     @property
     def atom_trace(self) -> bool:
         """Returns whether to keep track of all atoms that are responsible for the firing of rules or not.
-        NOTE: Turning this on may increase memory usage
+        NOTE: Turning this on may increase memory usage. Default is False
 
         :return: bool
         """
         return self.__atom_trace   
 
     @property
     def save_graph_attributes_to_trace(self) -> bool:
         """Returns whether to save the graph attribute facts to the rule trace. Graphs are large and turning this on can result in more memory usage.
-        NOTE: Turning this on may increase memory usage
+        NOTE: Turning this on may increase memory usage. Default is False
 
         :return: bool
         """
         return self.__save_graph_attributes_to_trace        
     
     @property
     def canonical(self) -> bool:
-        """Returns whether the interpretation is canonical or non-canonical
+        """Returns whether the interpretation is canonical or non-canonical. Default is False
 
         :return: bool
         """
         return self.__canonical
    
     @property
     def inconsistency_check(self) -> bool:
-        """Returns whether to check for inconsistencies in the interpretation or not
+        """Returns whether to check for inconsistencies in the interpretation or not. Default is True
 
         :return: bool
         """
         return self.__inconsistency_check
     
     @property
     def static_graph_facts(self) -> bool:
-        """Returns whether to make graph facts static or not
+        """Returns whether to make graph facts static or not. Default is True
 
         :return: bool
         """
         return self.__static_graph_facts
 
     @verbose.setter
     def verbose(self, value: bool) -> None:
@@ -294,14 +295,15 @@
 
 __non_fluent_graph_facts_node = None
 __non_fluent_graph_facts_edge = None
 __specific_graph_node_labels = None
 __specific_graph_edge_labels = None
 
 __timestamp = ''
+__program = None
 
 __graphml_parser = GraphmlParser()
 settings = _Settings()
 
 
 # FUNCTIONS
 def load_graph(path: str) -> None:
@@ -353,72 +355,86 @@
 
     :param path: Path for the YAML IPL file
     """
     global __ipl
     __ipl = yaml_parser.parse_ipl(path)
 
 
-def reason(timesteps: int=-1, convergence_threshold: int=-1, convergence_bound_threshold: float=-1):
+def reason(timesteps: int=-1, convergence_threshold: int=-1, convergence_bound_threshold: float=-1, again: bool=False, node_facts: List[Type[fact_node.Fact]]=None, edge_facts: List[Type[fact_edge.Fact]]=None, include_graph_facts: bool=True):
     """Function to start the main reasoning process. Graph and rules must already be loaded.
 
     :param timesteps: Max number of timesteps to run. -1 specifies run till convergence, defaults to -1
     :param convergence_threshold: Maximim number of interpretations that have changed between timesteps or fixed point operations until considered convergent. Program will end at convergence. -1 => no changes, perfect convergence, defaults to -1
     :param convergence_bound_threshold: Maximum change in any interpretation (bounds) between timesteps or fixed point operations until considered convergent, defaults to -1
+    :param again: Whether to reason again on an existing interpretation, defaults to False
+    :param node_facts: New node facts to use during the next reasoning process. Other facts from file will be discarded, defaults to None
+    :param edge_facts: New edge facts to use during the next reasoning process. Other facts from file will be discarded, defaults to None
+    :param include_graph_facts: Whether to add the graph facts to the facts supplied through `node_facts`, defaults to True
     :return: The final interpretation after reasoning.
     """
     global settings, __timestamp
 
     # Timestamp for saving files
     __timestamp = time.strftime('%Y%m%d-%H%M%S')
 
     if settings.output_to_file:
         sys.stdout = open(f"./{settings.output_file_name}_{__timestamp}.txt", "a")
 
-    if settings.memory_profile:
-        start_mem = mp.memory_usage(max_usage=True)
-        mem_usage, interpretation = mp.memory_usage((_reason, [timesteps, convergence_threshold, convergence_bound_threshold]), max_usage=True, retval=True)
-        print(f"\nProgram used {mem_usage-start_mem} MB of memory")
+    if not again or __program is None:
+        if settings.memory_profile:
+            start_mem = mp.memory_usage(max_usage=True)
+            mem_usage, interp = mp.memory_usage((_reason, [timesteps, convergence_threshold, convergence_bound_threshold]), max_usage=True, retval=True)
+            print(f"\nProgram used {mem_usage-start_mem} MB of memory")
+        else:
+            interp = _reason(timesteps, convergence_threshold, convergence_bound_threshold)
     else:
-        interpretation = _reason(timesteps, convergence_threshold, convergence_bound_threshold)
-
-    return interpretation
-
+        if settings.memory_profile:
+            start_mem = mp.memory_usage(max_usage=True)
+            mem_usage, interp = mp.memory_usage((_reason_again, [timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts, include_graph_facts]), max_usage=True, retval=True)
+            print(f"\nProgram used {mem_usage-start_mem} MB of memory")
+        else:
+            interp = _reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts, include_graph_facts)
+        
+    return interp
 
 
 def _reason(timesteps, convergence_threshold, convergence_bound_threshold):
     # Globals
     global __graph, __rules, __node_facts, __edge_facts, __ipl, __node_labels, __edge_labels, __specific_node_labels, __specific_edge_labels, __graphml_parser
-    global settings, __timestamp
+    global settings, __timestamp, __program
 
     # Assert variables are of correct type
 
     if settings.output_to_file:
         sys.stdout = open(f"./{settings.output_file_name}_{__timestamp}.txt", "a")
 
     # Check variables that HAVE to be set. Exceptions
     if __graph is None:
         raise Exception('Graph not loaded. Use `load_graph` to load the graphml file')
     if __rules is None:
         raise Exception('Rules not loaded. Use `load_rules` to load the rules yaml file')
 
     # Check variables that are highly recommended. Warnings
     if __node_labels is None and __edge_labels is None:
-        warnings.warn('Labels yaml file has not been loaded. Use `load_labels`. Only graph attributes will be used as labels\n')
+        if settings.verbose:
+            warnings.warn('Labels yaml file has not been loaded. Use `load_labels`. Only graph attributes will be used as labels\n')
         __node_labels = numba.typed.List.empty_list(label.label_type)
         __edge_labels = numba.typed.List.empty_list(label.label_type)
         __specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.string))
         __specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(numba.types.Tuple((numba.types.string, numba.types.string))))
 
     if __node_facts is None and __edge_facts is None:
-        warnings.warn('Facts yaml file has not been loaded. Use `load_facts`. Only graph attributes will be used as facts\n')
+        if settings.verbose:
+            warnings.warn('Facts yaml file has not been loaded. Use `load_facts`. Only graph attributes will be used as facts\n')
         __node_facts = numba.typed.List.empty_list(fact_node.fact_type)
         __edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
 
     if __ipl is None:
-        warnings.warn('Inconsistent Predicate List yaml file has not been loaded. Use `load_ipl`. Loading IPL is optional\n')
+        if settings.verbose:
+            warnings.warn('Inconsistent Predicate List yaml file has not been loaded. Use `load_ipl`. Loading IPL is optional\n')
         __ipl = numba.typed.List.empty_list(numba.types.Tuple((label.label_type, label.label_type)))
 
     
     # If graph attribute parsing, add results to existing specific labels and facts
     for label_name, nodes in __specific_graph_node_labels.items():
         if label_name in __specific_node_labels:
             __specific_node_labels[label_name].extend(nodes)
@@ -430,22 +446,52 @@
             __specific_edge_labels[label_name].extend(edges)
         else:
             __specific_edge_labels[label_name] = edges
     __node_facts.extend(__non_fluent_graph_facts_node)
     __edge_facts.extend(__non_fluent_graph_facts_edge)   
 
     # Setup logical program
-    program = Program(__graph, timesteps, __node_facts, __edge_facts, __rules, __ipl, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check)
-    program.available_labels_node = __node_labels
-    program.available_labels_edge = __edge_labels
-    program.specific_node_labels = __specific_node_labels
-    program.specific_edge_labels = __specific_edge_labels
+    __program = Program(__graph, __node_facts, __edge_facts, __rules, __ipl, settings.reverse_digraph, settings.atom_trace, settings.save_graph_attributes_to_trace, settings.canonical, settings.inconsistency_check)
+    __program.available_labels_node = __node_labels
+    __program.available_labels_edge = __edge_labels
+    __program.specific_node_labels = __specific_node_labels
+    __program.specific_edge_labels = __specific_edge_labels
+
+    # Run Program and get final interpretation
+    interpretation = __program.reason(timesteps, convergence_threshold, convergence_bound_threshold, settings.verbose)
+
+    return interpretation
+
+
+def _reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts, include_graph_facts):
+    # Globals
+    global __graph, __rules, __node_facts, __edge_facts, __ipl, __node_labels, __edge_labels, __specific_node_labels, __specific_edge_labels, __graphml_parser
+    global settings, __timestamp, __program
+
+    assert __program is not None, 'To run `reason_again` you need to have reasoned once before'
+
+    # If facts have not been inputted, use the old facts
+    __program.interp.facts_to_be_applied_node.clear()
+    __program.interp.facts_to_be_applied_edge.clear()
+    if node_facts is not None:
+        node_facts = numba.typed.List(node_facts)
+        if include_graph_facts:
+            node_facts.extend(__non_fluent_graph_facts_node)
+    else:
+        node_facts = numba.typed.List.empty_list(fact_node.fact_type)
+
+    if edge_facts is not None:
+        edge_facts = numba.typed.List(edge_facts)
+        if include_graph_facts:
+            edge_facts.extend(__non_fluent_graph_facts_edge)
+    else:
+        edge_facts = numba.typed.List.empty_list(fact_edge.fact_type)
 
     # Run Program and get final interpretation
-    interpretation = program.reason(convergence_threshold, convergence_bound_threshold, settings.verbose)
+    interpretation = __program.reason_again(timesteps, convergence_threshold, convergence_bound_threshold, node_facts, edge_facts, settings.verbose)
 
     return interpretation
 
 
 def save_rule_trace(interpretation, folder: str='./'):
     """Saves the trace of the program. This includes every change that has occured to the interpretation. If `atom_trace` was set to true
     this gives us full explainability of why interpretations changed
```

### Comparing `pyreason-1.2.9/pyreason/scripts/annotation_functions/annotation_functions.py` & `pyreason-1.3.0/pyreason/scripts/annotation_functions/annotation_functions.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/args.py` & `pyreason-1.3.0/pyreason/scripts/args.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/components/world.py` & `pyreason-1.3.0/pyreason/scripts/components/world.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,18 @@
     
     def __init__(self, labels):
         self._labels = labels
         self._world = numba.typed.Dict.empty(key_type=label.label_type, value_type=interval.interval_type)
         for l in labels:
             self._world[l] = interval.closed(0.0, 1.0)
 
+    @property
+    def world(self):
+        return self._world
+
     def make_world(labels, world):
         w = World(labels)
         w._world = world
         return w
 
     def is_satisfied(self, label, interval):
         result = False
```

### Comparing `pyreason-1.2.9/pyreason/scripts/diffuse.py` & `pyreason-1.3.0/pyreason/scripts/diffuse.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/facts/fact_edge.py` & `pyreason-1.3.0/pyreason/scripts/facts/fact_edge.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/facts/fact_node.py` & `pyreason-1.3.0/pyreason/scripts/facts/fact_node.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/interpretation/interpretation.py` & `pyreason-1.3.0/pyreason/scripts/interpretation/interpretation.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,36 +18,24 @@
 
 class Interpretation:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(node_type))
 	specific_edge_labels = numba.typed.Dict.empty(key_type=label.label_type, value_type=numba.types.ListType(edge_type))
 
-	def __init__(self, graph, tmax, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check, convergence_threshold, convergence_bound_threshold):
-		self.tmax = tmax
+	def __init__(self, graph, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check):
 		self.graph = graph
 		self.ipl = ipl
 		self.reverse_graph = reverse_graph
 		self.atom_trace = atom_trace
 		self.save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self.canonical = canonical
 		self.inconsistency_check = inconsistency_check
 		self.time = 0
 
-		# Set up convergence criteria
-		if convergence_bound_threshold==-1 and convergence_threshold==-1:
-			self._convergence_mode = 'perfect_convergence'
-			self._convergence_delta = 0
-		elif convergence_bound_threshold==-1:
-			self._convergence_mode = 'delta_interpretation'
-			self._convergence_delta = convergence_threshold
-		else:
-			self._convergence_mode = 'delta_bound'
-			self._convergence_delta = convergence_bound_threshold
-
 		# Initialize list of tuples for rules/facts to be applied, along with all the ground atoms that fired the rule. One to One correspondence between rules_to_be_applied_node and rules_to_be_applied_node_trace if atom_trace is true
 		self.rules_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.rules_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), numba.types.string)))
 		self.facts_to_be_applied_node_trace = numba.typed.List.empty_list(numba.types.string)
 		self.facts_to_be_applied_edge_trace = numba.typed.List.empty_list(numba.types.string)
 		self.rules_to_be_applied_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, node_type, label.label_type, interval.interval_type)))
 		self.rules_to_be_applied_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, edge_type, label.label_type, interval.interval_type)))
@@ -58,14 +46,18 @@
 
 		# Keep track of all the rules that have affeceted each node/edge at each timestep/fp operation, and all ground atoms that have affected the rules as well. Keep track of previous bounds and name of the rule/fact here
 		self.rule_trace_node_atoms = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), interval.interval_type, numba.types.string)))
 		self.rule_trace_edge_atoms = numba.typed.List.empty_list(numba.types.Tuple((numba.types.ListType(numba.types.ListType(node_type)), numba.types.ListType(numba.types.ListType(edge_type)), interval.interval_type, numba.types.string)))
 		self.rule_trace_node = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, numba.types.int8, node_type, label.label_type, interval.interval_type)))
 		self.rule_trace_edge = numba.typed.List.empty_list(numba.types.Tuple((numba.types.int8, numba.types.int8, edge_type, label.label_type, interval.interval_type)))
 
+		# Nodes and edges of the graph
+		self.nodes = numba.typed.List(self.graph.nodes())
+		self.edges = numba.typed.List(self.graph.edges())
+
 		# Make sure they are correct type
 		if len(self.available_labels_node)==0:
 			self.available_labels_node = numba.typed.List.empty_list(label.label_type)
 		else:
 			self.available_labels_node = numba.typed.List(self.available_labels_node)
 		if len(self.available_labels_edge)==0:
 			self.available_labels_edge = numba.typed.List.empty_list(label.label_type)
@@ -107,16 +99,33 @@
 			interpretations[e] = world.World(available_labels)
 		# Specific labels
 		for l, es in specific_labels.items():
 			for e in es:
 				interpretations[e].world[l] = interval.closed(0.0, 1.0)
 
 		return interpretations
+	
+	@staticmethod
+	@numba.njit(cache=True)
+	def _init_convergence(convergence_bound_threshold, convergence_threshold):
+		if convergence_bound_threshold==-1 and convergence_threshold==-1:
+			convergence_mode = 'perfect_convergence'
+			convergence_delta = 0
+		elif convergence_bound_threshold==-1:
+			convergence_mode = 'delta_interpretation'
+			convergence_delta = convergence_threshold
+		else:
+			convergence_mode = 'delta_bound'
+			convergence_delta = convergence_bound_threshold
+		return convergence_mode, convergence_delta
+		
 
-	def start_fp(self, facts_node, facts_edge, rules, verbose):
+	def start_fp(self, tmax, facts_node, facts_edge, rules, verbose, convergence_threshold, convergence_bound_threshold):
+		self.tmax = tmax
+		self._convergence_mode, self._convergence_delta = self._init_convergence(convergence_bound_threshold, convergence_threshold)
 		max_facts_time = self._init_facts(facts_node, facts_edge, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.atom_trace)
 		self._start_fp(rules, max_facts_time, verbose)
 
 
 	@staticmethod
 	@numba.njit(cache=True)
 	def _init_facts(facts_node, facts_edge, facts_to_be_applied_node, facts_to_be_applied_edge, facts_to_be_applied_node_trace, facts_to_be_applied_edge_trace, atom_trace):
@@ -137,15 +146,15 @@
 				facts_to_be_applied_edge.append((numba.types.int8(t), fact.get_component(), fact.get_label(), fact.get_bound(), fact.static, graph_attribute))
 				if atom_trace:
 					facts_to_be_applied_edge_trace.append(fact.get_name())
 		return max_time
 
 		
 	def _start_fp(self, rules, max_facts_time, verbose):
-		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, rules, numba.typed.List(self.graph.nodes()), numba.typed.List(self.graph.edges()), self.neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.available_labels_node, self.available_labels_edge, self.specific_node_labels, self.specific_edge_labels, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
+		fp_cnt, t = self.reason(self.interpretations_node, self.interpretations_edge, self.tmax, rules, self.nodes, self.edges, self.neighbors, self.rules_to_be_applied_node, self.rules_to_be_applied_edge, self.edges_to_be_added_node_rule, self.edges_to_be_added_edge_rule, self.rules_to_be_applied_node_trace, self.rules_to_be_applied_edge_trace, self.facts_to_be_applied_node, self.facts_to_be_applied_edge, self.facts_to_be_applied_node_trace, self.facts_to_be_applied_edge_trace, self.available_labels_node, self.available_labels_edge, self.specific_node_labels, self.specific_edge_labels, self.ipl, self.rule_trace_node, self.rule_trace_edge, self.rule_trace_node_atoms, self.rule_trace_edge_atoms, self.reverse_graph, self.atom_trace, self.save_graph_attributes_to_rule_trace, self.canonical, self.inconsistency_check, max_facts_time, self._convergence_mode, self._convergence_delta, verbose)
 		self.time = t
 		if verbose:
 			print('Fixed Point iterations:', fp_cnt)
 
 
 	@staticmethod
 	@numba.njit(cache=True)
```

### Comparing `pyreason-1.2.9/pyreason/scripts/interval/interval.py` & `pyreason-1.3.0/pyreason/scripts/interval/interval.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,20 @@
         if lower > upper:
             lower = np.float32(0)
             upper = np.float32(1)
         return Interval(lower, upper, False, self.lower, self.upper)
 
     def to_str(self):
         return self.__repr__()
+    
+    def __eq__(self, interval):
+        if interval.lower==self.lower and interval.upper==self.upper:
+            return True
+        else:
+            return False
 
     def __repr__(self):
         return f'[{self.lower},{self.upper}]'
 
     def __contains__(self, item):
         if self.lower <= item.lower and self.upper >= item.upper:
             return True
```

### Comparing `pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py` & `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_edge_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py` & `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/fact_node_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/interval_type.py` & `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/interval_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/label_type.py` & `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/label_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/rule_type.py` & `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/rule_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/numba_wrapper/numba_types/world_type.py` & `pyreason-1.3.0/pyreason/scripts/numba_wrapper/numba_types/world_type.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/program/program.py` & `pyreason-1.3.0/pyreason/scripts/program/program.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,31 +3,39 @@
 
 class Program:
 	available_labels_node = []
 	available_labels_edge = []
 	specific_node_labels = []
 	specific_edge_labels = []
 
-	def __init__(self, graph, tmax, facts_node, facts_edge, rules, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check):
+	def __init__(self, graph, facts_node, facts_edge, rules, ipl, reverse_graph, atom_trace, save_graph_attributes_to_rule_trace, canonical, inconsistency_check):
 		self._graph = graph
-		self._tmax = tmax
 		self._facts_node = facts_node
 		self._facts_edge = facts_edge
 		self._rules = rules
 		self._ipl = ipl
 		self._reverse_graph = reverse_graph
 		self._atom_trace = atom_trace
 		self._save_graph_attributes_to_rule_trace = save_graph_attributes_to_rule_trace
 		self._canonical = canonical
 		self._inconsistency_check = inconsistency_check
+		self.interp = None
 
-	def reason(self, convergence_threshold, convergence_bound_threshold, verbose=True):
+	def reason(self, tmax, convergence_threshold, convergence_bound_threshold, verbose=True):
+		self._tmax = tmax
 		# Set up available labels
 		Interpretation.available_labels_node = self.available_labels_node
 		Interpretation.available_labels_edge = self.available_labels_edge
 		Interpretation.specific_node_labels = self.specific_node_labels
 		Interpretation.specific_edge_labels = self.specific_edge_labels
 
-		interp = Interpretation(self._graph, self._tmax, self._ipl, self._reverse_graph, self._atom_trace, self._save_graph_attributes_to_rule_trace, self._canonical, self._inconsistency_check, convergence_threshold, convergence_bound_threshold)
-		interp.start_fp(self._facts_node, self._facts_edge, self._rules, verbose)
+		self.interp = Interpretation(self._graph, self._ipl, self._reverse_graph, self._atom_trace, self._save_graph_attributes_to_rule_trace, self._canonical, self._inconsistency_check)
+		self.interp.start_fp(self._tmax, self._facts_node, self._facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
+
+		return self.interp
+	
+	def reason_again(self, tmax, convergence_threshold, convergence_bound_threshold, facts_node, facts_edge, verbose=True):
+		self._tmax = tmax
+		self.interp.start_fp(tmax, facts_node, facts_edge, self._rules, verbose, convergence_threshold, convergence_bound_threshold)
 
-		return interp		
+		return self.interp
+
```

### Comparing `pyreason-1.2.9/pyreason/scripts/rules/rule.py` & `pyreason-1.3.0/pyreason/scripts/rules/rule.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/utils/filter.py` & `pyreason-1.3.0/pyreason/scripts/utils/filter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/utils/graphml_parser.py` & `pyreason-1.3.0/pyreason/scripts/utils/graphml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/utils/output.py` & `pyreason-1.3.0/pyreason/scripts/utils/output.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,16 +62,20 @@
                     # Go through all the changes in the rule trace
                     # len(qn) = num of clauses in rule that was used
                     row[6] = name
 
                     # Go through each clause
                     for j in range(len(qn)):
                         max_j = max(j, max_j)
-                        # Node clause
-                        row.append(list(qn[j]))
+                        if len(qe[j])==0:
+                            # Node clause
+                            row.append(list(qn[j]))
+                        elif len(qn[j])==0:
+                            # Edge clause
+                            row.append(list(qe[j]))
 
 
                 data.append(row)
 
             # Add Clause-num to header
             if interpretation.atom_trace and max_j!=-1:
                 for i in range(1, max_j+2):
```

### Comparing `pyreason-1.2.9/pyreason/scripts/utils/plotter.py` & `pyreason-1.3.0/pyreason/scripts/utils/plotter.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/utils/visuals.py` & `pyreason-1.3.0/pyreason/scripts/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason/scripts/utils/yaml_parser.py` & `pyreason-1.3.0/pyreason/scripts/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/pyreason.egg-info/PKG-INFO` & `pyreason-1.3.0/pyreason.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreason
-Version: 1.2.9
+Version: 1.3.0
 Summary: An explainable inference software supporting annotated, real valued, graph based and temporal logic
 Home-page: https://github.com/lab-v2/pyreason
 Author: Dyuman Aditya
 Author-email: dyuman.aditya@gmail.com
 License: BSD 3-clause
 Project-URL: Bug Tracker, https://github.com/lab-v2/pyreason/issues
 Project-URL: Repository, https://github.com/lab-v2/pyreason
@@ -24,15 +24,17 @@
 An explainable inference software supporting annotated, real valued, graph based and temporal logic.
 
 ## Links
 Paper: https://arxiv.org/abs/2302.13482
 
 Video: https://www.youtube.com/watch?v=E1PSl3KQCmo
 
-Website: https://neurosymoblic.asu.edu/pyreason/
+Website: https://neurosymbolic.asu.edu/pyreason/
+
+PyReason Gym: https://github.com/lab-v2/pyreason-gym
 
 Check out the [PyReason Hello World](https://github.com/lab-v2/pyreason/blob/main/docs/hello-world.md) program if you're new, or want get get a feel for the software.
 
 
 ## Table of Contents
   
 1. [Introduction](#1-introduction)
@@ -56,17 +58,19 @@
 
 The format of these files is very important. Please refer to the [example YAML files provided](https://github.com/lab-v2/pyreason/blob/main/pyreason/examples/example_yamls) when making your own rules/facts/labels/ipl. TODO: make doc for each format.
 
 ## 2. Install
 PyReason can be installed as a python library (recommended) or as a command line tool
 
 ## 2.1 Install as a Python Library
-This might take a minute or two
+We import pyreason to initialize it for the first time, this may take a few minutes
 ```bash
 pip install pyreason
+python
+import pyreason
 ```
 
 ## 2.2 Install as a Command Line Tool
 
 ```bash
 git clone https://github.com/lab-v2/pyreason
 cd pyreason
```

### Comparing `pyreason-1.2.9/pyreason.egg-info/SOURCES.txt` & `pyreason-1.3.0/pyreason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyreason-1.2.9/setup.py` & `pyreason-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name = 'pyreason',
-    version = '1.2.9',
+    version = '1.3.0',
     author = 'Dyuman Aditya',
     author_email = 'dyuman.aditya@gmail.com',
     description = 'An explainable inference software supporting annotated, real valued, graph based and temporal logic',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/lab-v2/pyreason',
     license = 'BSD 3-clause',
```

