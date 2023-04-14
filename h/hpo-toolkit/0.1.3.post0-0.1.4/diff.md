# Comparing `tmp/hpo-toolkit-0.1.3.post0.tar.gz` & `tmp/hpo-toolkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hpo-toolkit-0.1.3.post0.tar", last modified: Fri Mar 10 15:26:25 2023, max compression
+gzip compressed data, was "hpo-toolkit-0.1.4.tar", last modified: Fri Apr 14 16:17:45 2023, max compression
```

## Comparing `hpo-toolkit-0.1.3.post0.tar` & `hpo-toolkit-0.1.4.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.636278 hpo-toolkit-0.1.3.post0/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    35149 2022-12-16 17:20:05.000000 hpo-toolkit-0.1.3.post0/LICENSE
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    41601 2023-03-10 15:26:25.636278 hpo-toolkit-0.1.3.post0/PKG-INFO
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      549 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/README.md
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      809 2023-03-03 16:00:11.000000 hpo-toolkit-0.1.3.post0/pyproject.toml
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       38 2023-03-10 15:26:25.636278 hpo-toolkit-0.1.3.post0/setup.cfg
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.620278 hpo-toolkit-0.1.3.post0/src/
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.624278 hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)    41601 2023-03-10 15:26:25.000000 hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1822 2023-03-10 15:26:25.000000 hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-03-10 15:26:25.000000 hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-02-27 14:40:18.000000 hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       12 2023-03-10 15:26:25.000000 hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/requires.txt
--rw-rw-r--   0 ielis     (1000) ielis     (1000)        6 2023-03-10 15:26:25.000000 hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/top_level.txt
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.624278 hpo-toolkit-0.1.3.post0/src/hpotk/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      207 2023-03-10 15:24:33.000000 hpo-toolkit-0.1.3.post0/src/hpotk/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.624278 hpo-toolkit-0.1.3.post0/src/hpotk/algorithm/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      158 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/src/hpotk/algorithm/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6912 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/src/hpotk/algorithm/_traversal.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.628278 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      267 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     9105 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/_base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2577 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/_simple.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.628278 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/load/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       54 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/load/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      307 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/load/_api.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.628278 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/load/hpoa/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       43 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/load/hpoa/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     8380 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/annotations/load/hpoa/_impl.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.628278 hpo-toolkit-0.1.3.post0/src/hpotk/constants/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       18 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/constants/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.628278 hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      139 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      452 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2428 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/frequency.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1925 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/inheritance.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1419 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/onset.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1989 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/organ_system.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      376 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/severity.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.632278 hpo-toolkit-0.1.3.post0/src/hpotk/graph/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      154 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/graph/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1289 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/graph/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1625 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/graph/_csr_graph.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4741 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/src/hpotk/graph/_factory.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.632278 hpo-toolkit-0.1.3.post0/src/hpotk/graph/csr/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       55 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/graph/csr/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     7494 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/graph/csr/_csr.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     5587 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/graph/csr/test__csr.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.632278 hpo-toolkit-0.1.3.post0/src/hpotk/model/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      326 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/model/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      887 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/model/_base.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4985 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/model/_term.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2821 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/model/_term_id.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.632278 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      126 2022-12-22 14:58:29.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2003 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/_api.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      238 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/_attrs.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4567 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/_default.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.632278 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)       24 2023-02-27 15:19:11.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/__init__.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.636278 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      110 2023-02-27 15:20:14.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2197 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/_factory.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     6859 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/_load.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     8317 2022-12-20 22:42:27.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/_model.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      828 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/test_load.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3432 2023-02-28 13:59:18.000000 hpo-toolkit-0.1.3.post0/src/hpotk/util.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.636278 hpo-toolkit-0.1.3.post0/src/hpotk/validate/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)      213 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/src/hpotk/validate/__init__.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4412 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/src/hpotk/validate/_hpo.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     1756 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/src/hpotk/validate/_model.py
-drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-03-10 15:26:25.636278 hpo-toolkit-0.1.3.post0/tests/
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3052 2023-02-27 17:09:23.000000 hpo-toolkit-0.1.3.post0/tests/test_algorithm.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2400 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.3.post0/tests/test_disease.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4219 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/tests/test_obographs.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     3133 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/tests/test_term.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     2070 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.3.post0/tests/test_term_id.py
--rw-rw-r--   0 ielis     (1000) ielis     (1000)     4962 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.3.post0/tests/test_validate.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    35149 2022-12-16 17:20:05.000000 hpo-toolkit-0.1.4/LICENSE
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    41595 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/PKG-INFO
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      549 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/README.md
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      809 2023-03-03 16:00:11.000000 hpo-toolkit-0.1.4/pyproject.toml
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       38 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/setup.cfg
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.601534 hpo-toolkit-0.1.4/src/
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    41595 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1847 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        1 2023-02-27 14:40:18.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/not-zip-safe
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       12 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)        6 2023-04-14 16:17:45.000000 hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      202 2023-04-14 16:09:26.000000 hpo-toolkit-0.1.4/src/hpotk/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/algorithm/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      158 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/algorithm/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6912 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/algorithm/_traversal.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/annotations/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      267 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     9105 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/_base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2577 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/_simple.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/annotations/load/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       54 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/load/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      307 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/load/_api.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/annotations/load/hpoa/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       43 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/load/hpoa/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     8861 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/annotations/load/hpoa/_impl.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/constants/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       18 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.605534 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      139 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      452 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2428 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/frequency.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1925 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/inheritance.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1419 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/onset.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1989 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/organ_system.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      376 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/constants/hpo/severity.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/graph/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      154 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1289 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1625 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/_csr_graph.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4741 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/graph/_factory.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/graph/csr/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       55 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/csr/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7494 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/csr/_csr.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5587 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/graph/csr/test__csr.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/model/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      365 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/model/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      887 2023-04-13 21:02:33.000000 hpo-toolkit-0.1.4/src/hpotk/model/_base.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)    10107 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/model/_term.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2821 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/model/_term_id.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      856 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/model/_util.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/ontology/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      126 2022-12-22 14:58:29.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2003 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/_api.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      238 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/_attrs.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4567 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/_default.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/ontology/load/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)       24 2023-02-27 15:19:11.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/__init__.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.609534 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      110 2023-02-27 15:20:14.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     5930 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_factory.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     6859 2023-03-14 15:54:53.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_load.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     9853 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_model.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      828 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/test_load.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3432 2023-02-28 13:59:18.000000 hpo-toolkit-0.1.4/src/hpotk/util.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/src/hpotk/validate/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)      213 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/validate/__init__.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4412 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/validate/_hpo.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     1756 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/src/hpotk/validate/_model.py
+drwxrwxr-x   0 ielis     (1000) ielis     (1000)        0 2023-04-14 16:17:45.613534 hpo-toolkit-0.1.4/tests/
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     3052 2023-02-27 17:09:23.000000 hpo-toolkit-0.1.4/tests/test_algorithm.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2400 2023-03-08 21:00:13.000000 hpo-toolkit-0.1.4/tests/test_disease.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     7087 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/tests/test_obographs.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4681 2023-04-14 14:23:26.000000 hpo-toolkit-0.1.4/tests/test_term.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     2070 2022-12-28 21:43:07.000000 hpo-toolkit-0.1.4/tests/test_term_id.py
+-rw-rw-r--   0 ielis     (1000) ielis     (1000)     4962 2023-02-28 16:13:00.000000 hpo-toolkit-0.1.4/tests/test_validate.py
```

### Comparing `hpo-toolkit-0.1.3.post0/LICENSE` & `hpo-toolkit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/PKG-INFO` & `hpo-toolkit-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo-toolkit
-Version: 0.1.3.post0
+Version: 0.1.4
 Summary: A toolkit for working with Human Phenotype Ontology in Python
 Author-email: Daniel Danis <daniel.gordon.danis@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpo-toolkit-0.1.3.post0/README.md` & `hpo-toolkit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/pyproject.toml` & `hpo-toolkit-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/PKG-INFO` & `hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hpo-toolkit
-Version: 0.1.3.post0
+Version: 0.1.4
 Summary: A toolkit for working with Human Phenotype Ontology in Python
 Author-email: Daniel Danis <daniel.gordon.danis@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hpo-toolkit-0.1.3.post0/src/hpo_toolkit.egg-info/SOURCES.txt` & `hpo-toolkit-0.1.4/src/hpo_toolkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 src/hpotk/graph/csr/__init__.py
 src/hpotk/graph/csr/_csr.py
 src/hpotk/graph/csr/test__csr.py
 src/hpotk/model/__init__.py
 src/hpotk/model/_base.py
 src/hpotk/model/_term.py
 src/hpotk/model/_term_id.py
+src/hpotk/model/_util.py
 src/hpotk/ontology/__init__.py
 src/hpotk/ontology/_api.py
 src/hpotk/ontology/_attrs.py
 src/hpotk/ontology/_default.py
 src/hpotk/ontology/load/__init__.py
 src/hpotk/ontology/load/obographs/__init__.py
 src/hpotk/ontology/load/obographs/_factory.py
```

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/algorithm/_traversal.py` & `hpo-toolkit-0.1.4/src/hpotk/algorithm/_traversal.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/annotations/_base.py` & `hpo-toolkit-0.1.4/src/hpotk/annotations/_base.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/annotations/_simple.py` & `hpo-toolkit-0.1.4/src/hpotk/annotations/_simple.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/annotations/load/hpoa/_impl.py` & `hpo-toolkit-0.1.4/src/hpotk/annotations/load/hpoa/_impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,21 +38,30 @@
         self._hpo = hpo
         self._cohort_size = cohort_size
         self._salvage_negated_frequencies = salvage_negated_frequencies
 
     def load(self, file: typing.Union[typing.IO, str]) -> HpoDiseases:
         data = defaultdict(list)
         version = None
+        expecting_to_see_header_line = True
         with open_text_io_handle(file) as fh:
             for line in fh:
-                if line.startswith('#'):
-                    # header
-                    version_matcher = HPOA_VERSION_PATTERN.match(line)
-                    if version_matcher:
-                        version = version_matcher.group('version')
+                if expecting_to_see_header_line:
+                    if line.startswith('#'):
+                        # header
+                        if line.startswith('#DatabaseID'):
+                            # The older HPOA format
+                            expecting_to_see_header_line = False
+                        else:
+                            version_matcher = HPOA_VERSION_PATTERN.match(line)
+                            if version_matcher:
+                                version = version_matcher.group('version')
+                    else:
+                        if line.startswith('database_id'):
+                            expecting_to_see_header_line = False
                     continue
                 else:
                     # corpus
                     hpoa = _parse_hpoa_line(line)
                     if hpoa:
                         data[hpoa.disease_id].append(hpoa)
```

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/frequency.py` & `hpo-toolkit-0.1.4/src/hpotk/constants/hpo/frequency.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/inheritance.py` & `hpo-toolkit-0.1.4/src/hpotk/constants/hpo/inheritance.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/onset.py` & `hpo-toolkit-0.1.4/src/hpotk/constants/hpo/onset.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/constants/hpo/organ_system.py` & `hpo-toolkit-0.1.4/src/hpotk/constants/hpo/organ_system.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/graph/_api.py` & `hpo-toolkit-0.1.4/src/hpotk/graph/_api.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/graph/_csr_graph.py` & `hpo-toolkit-0.1.4/src/hpotk/graph/_csr_graph.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/graph/_factory.py` & `hpo-toolkit-0.1.4/src/hpotk/graph/_factory.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/graph/csr/_csr.py` & `hpo-toolkit-0.1.4/src/hpotk/graph/csr/_csr.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/graph/csr/test__csr.py` & `hpo-toolkit-0.1.4/src/hpotk/graph/csr/test__csr.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/model/_base.py` & `hpo-toolkit-0.1.4/src/hpotk/model/_base.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/model/_term_id.py` & `hpo-toolkit-0.1.4/src/hpotk/model/_term_id.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/ontology/_api.py` & `hpo-toolkit-0.1.4/src/hpotk/ontology/_api.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/ontology/_default.py` & `hpo-toolkit-0.1.4/src/hpotk/ontology/_default.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/_load.py` & `hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_load.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/_model.py` & `hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,32 +12,38 @@
     PROPERTY = 3
 
 
 def create_property_value(cls, data: typing.Dict):
     if cls == PropertyValue:
         return PropertyValue(pred=get_attr_or_none(data, 'pred'),
                              val=get_attr_or_none(data, 'val'),
-                             xrefs=[xref for xref in data['xrefs']] if 'xrefs' in data else [],
+                             xrefs=data['xrefs'] if 'xrefs' in data else [],
                              meta=create_meta(data['meta']) if 'meta' in data else None)
     elif cls == DefinitionPropertyValue:
         return DefinitionPropertyValue(pred=get_attr_or_none(data, 'pred'),
                                        val=get_attr_or_none(data, 'val'),
-                                       xrefs=[xref for xref in data['xrefs']] if 'xrefs' in data else [],
+                                       xrefs=data['xrefs'] if 'xrefs' in data else [],
                                        meta=create_meta(data['meta']) if 'meta' in data else None)
     elif cls == BasicPropertyValue:
         return BasicPropertyValue(pred=get_attr_or_none(data, 'pred'),
                                   val=get_attr_or_none(data, 'val'),
-                                  xrefs=[xref for xref in data['xrefs']] if 'xrefs' in data else [],
+                                  xrefs=data['xrefs'] if 'xrefs' in data else [],
                                   meta=create_meta(data['meta']) if 'meta' in data else None)
     elif cls == XrefPropertyValue:
         return XrefPropertyValue(lbl=get_attr_or_none(data, 'lbl'),
                                  pred=get_attr_or_none(data, 'pred'),
                                  val=get_attr_or_none(data, 'val'),
-                                 xrefs=[xref for xref in data['xrefs']] if 'xrefs' in data else [],
+                                 xrefs=data['xrefs'] if 'xrefs' in data else [],
                                  meta=create_meta(data['meta']) if 'meta' in data else None)
+    elif cls == SynonymPropertyValue:
+        return SynonymPropertyValue(synonym_type=get_attr_or_none(data, 'synonymType'),
+                                    pred=get_attr_or_none(data, 'pred'),
+                                    val=get_attr_or_none(data, 'val'),
+                                    xrefs=data['xrefs'] if 'xrefs' in data else [],
+                                    meta=create_meta(data['meta']) if 'meta' in data else None)
     else:
         return None
 
 
 class PropertyValue:
 
     def __init__(self, pred: typing.Optional[str],
@@ -88,18 +94,14 @@
 
     def __repr__(self):
         return str(self)
 
 
 class XrefPropertyValue(PropertyValue):
 
-    @staticmethod
-    def create_xref_property_value(data: typing.Dict):
-        return
-
     def __init__(self, lbl: typing.Optional[str],
                  pred: typing.Optional[str],
                  val: typing.Optional[str],
                  xrefs: typing.Sequence[str],
                  meta):
         super().__init__(pred, val, xrefs, meta)
         self._lbl = lbl
@@ -111,32 +113,64 @@
     def __str__(self):
         return f'XrefPropertyValue(lbl={self.lbl}, pred={self.pred}, val={self.val}, xrefs={self.xrefs}, meta={self.meta})'
 
     def __repr__(self):
         return str(self)
 
 
+class SynonymPropertyValue(PropertyValue):
+
+    def __init__(self, synonym_type: typing.Optional[str],
+                 pred: typing.Optional[str],
+                 val: typing.Optional[str],
+                 xrefs: typing.Sequence[str],
+                 meta):
+        super().__init__(pred, val, xrefs, meta)
+        self._synonym_type = synonym_type
+
+    @property
+    def synonym_type(self) -> typing.Optional[str]:
+        return self._synonym_type
+
+    def __str__(self):
+        return f'SynonymPropertyValue(' \
+               f'synonym_type={self.synonym_type},' \
+               f' pred={self.pred},' \
+               f' val={self.val},' \
+               f' xrefs={self.xrefs},' \
+               f' meta={self.meta})'
+
+    def __repr__(self):
+        return str(self)
+
+
 class Meta:
 
     def __init__(self, definition: typing.Optional[DefinitionPropertyValue],
+                 synonyms: typing.Sequence[SynonymPropertyValue],
                  comments: typing.Sequence[str],
                  basic_property_values: typing.Sequence[BasicPropertyValue],
                  xrefs: typing.Sequence[XrefPropertyValue],
                  is_deprecated: bool):
         self._definition = definition
+        self._synonyms = synonyms
         self._comments = comments
         self._property_values = basic_property_values
         self._xrefs = xrefs
         self._is_deprecated = is_deprecated
 
     @property
     def definition(self) -> typing.Optional[DefinitionPropertyValue]:
         return self._definition
 
     @property
+    def synonyms(self) -> typing.Sequence[SynonymPropertyValue]:
+        return self._synonyms
+
+    @property
     def comments(self) -> typing.Sequence[str]:
         return self._comments
 
     @property
     def basic_property_values(self) -> typing.Sequence[BasicPropertyValue]:
         return self._property_values
 
@@ -145,15 +179,20 @@
         return self._xrefs
 
     @property
     def is_deprecated(self) -> bool:
         return self._is_deprecated
 
     def __str__(self):
-        return f'Meta(definition={self.definition}, comments={self.comments}, basic_property_values={self.basic_property_values}, xrefs={self.xrefs}, is_deprecated={self.is_deprecated})'
+        return f'Meta(definition={self.definition},' \
+               f' synonyms={self.synonyms},' \
+               f' comments={self.comments},' \
+               f' basic_property_values={self.basic_property_values},' \
+               f' xrefs={self.xrefs},' \
+               f' is_deprecated={self.is_deprecated})'
 
     def __repr__(self):
         return str(self)
 
 
 class NodeOrEdge(metaclass=abc.ABCMeta):
 
@@ -236,18 +275,19 @@
 
 
 def create_meta(data) -> typing.Optional[Meta]:
     definition = create_property_value(DefinitionPropertyValue, data['definition']) if 'definition' in data else None
     comments = data['comments'] if 'comments' in data else []
     basic_property_values = [create_property_value(BasicPropertyValue, d) for d in
                              data['basicPropertyValues']] if 'basicPropertyValues' in data else []
+    synonyms = [create_property_value(SynonymPropertyValue, x) for x in data['synonyms']] if 'synonyms' in data else []
     xrefs = [create_property_value(XrefPropertyValue, x) for x in data['xrefs']] if 'xrefs' in data else []
     is_deprecated = 'deprecated' in data
 
-    return Meta(definition, comments, basic_property_values, xrefs, is_deprecated)
+    return Meta(definition, synonyms, comments, basic_property_values, xrefs, is_deprecated)
 
 
 def create_node(data) -> typing.Optional[Node]:
     identifier = data['id']
     lbl = data['lbl'] if 'lbl' in data else None
 
     if 'type' not in data:
```

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/ontology/load/obographs/test_load.py` & `hpo-toolkit-0.1.4/src/hpotk/ontology/load/obographs/test_load.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/util.py` & `hpo-toolkit-0.1.4/src/hpotk/util.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/validate/_hpo.py` & `hpo-toolkit-0.1.4/src/hpotk/validate/_hpo.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/src/hpotk/validate/_model.py` & `hpo-toolkit-0.1.4/src/hpotk/validate/_model.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/tests/test_algorithm.py` & `hpo-toolkit-0.1.4/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/tests/test_disease.py` & `hpo-toolkit-0.1.4/tests/test_disease.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/tests/test_obographs.py` & `hpo-toolkit-0.1.4/tests/test_obographs.py`

 * *Files 27% similar despite different names*

```diff
@@ -51,14 +51,19 @@
         self.assertIsNotNone(o, "Ontology must not be None")
 
         arachnodactyly = TermId.from_curie("HP:0001166")
         assert all([val.value in {"HP:0001238", "HP:0100807"} for val in (o.graph.get_parents(arachnodactyly))])
         assert len(list(o.graph.get_children(arachnodactyly))) == 0
 
     @unittest.skip
+    def test_real_life(self):
+        o: hp.ontology.Ontology = load_ontology('/home/ielis/data/ontologies/hpo/2023-01-27/hp.json')
+        self.assertIsNotNone(o, "Ontology must not be None")
+
+    @unittest.skip
     def test_print_stats(self):
         import json
         with open(TOY_HPO) as fh:
             graphs = json.load(fh)
 
         graph = graphs['graphs'][0]
         all_nodes = graph['nodes']
@@ -78,7 +83,65 @@
                 if 'deprecated' in meta:
                     deprecated = meta['deprecated']
                     if not deprecated:
                         result.append(node)
                 else:
                     result.append(node)
         return result
+
+
+class TestTerms(unittest.TestCase):
+    """
+    We only load the ontology once, and we test the properties of the loaded data.
+    """
+
+    ONTOLOGY: hp.ontology.Ontology = None
+
+    @classmethod
+    def setUpClass(cls) -> None:
+        cls.ONTOLOGY = load_ontology(TOY_HPO)
+
+    def test_term_properties(self):
+        # Test properties of a Term
+        term = TestTerms.ONTOLOGY.get_term('HP:0001626')
+
+        self.assertEqual(term.identifier.value, 'HP:0001626')
+        self.assertEqual(term.name, 'Abnormality of the cardiovascular system')
+        self.assertEqual(term.definition, 'Any abnormality of the cardiovascular system.')
+        self.assertEqual(term.comment, 'The cardiovascular system consists of the heart, vasculature, and the '
+                                       'lymphatic system.')
+        self.assertEqual(term.is_obsolete, False)
+        self.assertListEqual(term.alt_term_ids, [TermId.from_curie('HP:0003116')])
+
+        synonyms = term.synonyms
+        self.assertEqual(len(synonyms), 3)
+
+        one = synonyms[0]
+        self.assertEqual(one.name, 'Cardiovascular disease')
+        self.assertEqual(one.category, hp.model.SynonymCategory.RELATED)
+        self.assertEqual(one.synonym_type, hp.model.SynonymType.LAYPERSON_TERM)
+        self.assertIsNone(one.xrefs)
+
+        two = synonyms[1]
+        self.assertEqual(two.name, 'Cardiovascular abnormality')
+        self.assertEqual(two.category, hp.model.SynonymCategory.EXACT)
+        self.assertEqual(two.synonym_type, hp.model.SynonymType.LAYPERSON_TERM)
+        self.assertIsNone(two.xrefs)
+
+        three = synonyms[2]
+        self.assertEqual(three.name, 'Abnormality of the cardiovascular system')
+        self.assertEqual(three.category, hp.model.SynonymCategory.EXACT)
+        self.assertEqual(three.synonym_type, hp.model.SynonymType.LAYPERSON_TERM)
+        self.assertIsNone(three.xrefs)
+
+        self.assertEqual(term.xrefs, [TermId.from_curie(curie) for curie in ('UMLS:C0243050', 'UMLS:C0007222',
+                                                                             'MSH:D018376', 'SNOMEDCT_US:49601007',
+                                                                             'MSH:D002318')])
+
+    def test_synonym_properties(self):
+        term = TestTerms.ONTOLOGY.get_term('HP:0001627')
+        synonym = term.synonyms[7]
+        self.assertEqual(synonym.name, 'Abnormally shaped heart')
+        self.assertEqual(synonym.category, hp.model.SynonymCategory.EXACT)
+        self.assertEqual(synonym.synonym_type, hp.model.SynonymType.LAYPERSON_TERM)
+        self.assertEqual(synonym.xrefs, [TermId.from_curie('ORCID:0000-0001-5208-3432')])
+
```

### Comparing `hpo-toolkit-0.1.3.post0/tests/test_term_id.py` & `hpo-toolkit-0.1.4/tests/test_term_id.py`

 * *Files identical despite different names*

### Comparing `hpo-toolkit-0.1.3.post0/tests/test_validate.py` & `hpo-toolkit-0.1.4/tests/test_validate.py`

 * *Files identical despite different names*

