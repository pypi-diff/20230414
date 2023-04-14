# Comparing `tmp/opta-0.3.0.tar.gz` & `tmp/opta-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opta-0.3.0.tar", max compression
+gzip compressed data, was "opta-0.3.1.tar", max compression
```

## Comparing `opta-0.3.0.tar` & `opta-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1075 2022-06-07 07:37:58.992410 opta-0.3.0/LICENSE
--rw-r--r--   0        0        0     1091 2022-06-07 07:37:58.992410 opta-0.3.0/opta/algorithms/abstract.py
--rw-r--r--   0        0        0     1982 2022-06-07 07:37:58.992410 opta-0.3.0/opta/algorithms/black_hole_optimization.py
--rw-r--r--   0        0        0      777 2022-06-07 07:37:58.992410 opta-0.3.0/opta/algorithms/random_search.py
--rw-r--r--   0        0        0      698 2022-06-07 07:37:58.992410 opta-0.3.0/opta/tools/coding.py
--rw-r--r--   0        0        0      379 2022-06-07 07:37:58.992410 opta-0.3.0/opta/tools/testing.py
--rw-r--r--   0        0        0      601 2022-06-07 07:37:58.992410 opta-0.3.0/opta/tools/vectors.py
--rw-r--r--   0        0        0      427 2022-06-07 07:37:58.992410 opta-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      610 2022-06-07 07:38:39.871440 opta-0.3.0/setup.py
--rw-r--r--   0        0        0      443 2022-06-07 07:38:39.871685 opta-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-14 19:53:21.311162 opta-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1091 2023-04-14 19:53:21.311162 opta-0.3.1/opta/algorithms/abstract.py
+-rw-r--r--   0        0        0     1982 2023-04-14 19:53:21.311162 opta-0.3.1/opta/algorithms/black_hole_optimization.py
+-rw-r--r--   0        0        0      777 2023-04-14 19:53:21.311162 opta-0.3.1/opta/algorithms/random_search.py
+-rw-r--r--   0        0        0      698 2023-04-14 19:53:21.311162 opta-0.3.1/opta/tools/coding.py
+-rw-r--r--   0        0        0      379 2023-04-14 19:53:21.311162 opta-0.3.1/opta/tools/testing.py
+-rw-r--r--   0        0        0      601 2023-04-14 19:53:21.311162 opta-0.3.1/opta/tools/vectors.py
+-rw-r--r--   0        0        0      433 2023-04-14 19:53:21.311162 opta-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 opta-0.3.1/PKG-INFO
```

### Comparing `opta-0.3.0/LICENSE` & `opta-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opta-0.3.0/opta/algorithms/abstract.py` & `opta-0.3.1/opta/algorithms/abstract.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.0/opta/algorithms/black_hole_optimization.py` & `opta-0.3.1/opta/algorithms/black_hole_optimization.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.0/opta/algorithms/random_search.py` & `opta-0.3.1/opta/algorithms/random_search.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.0/opta/tools/coding.py` & `opta-0.3.1/opta/tools/coding.py`

 * *Files identical despite different names*

### Comparing `opta-0.3.0/opta/tools/vectors.py` & `opta-0.3.1/opta/tools/vectors.py`

 * *Files identical despite different names*

