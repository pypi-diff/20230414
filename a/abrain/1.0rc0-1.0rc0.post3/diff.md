# Comparing `tmp/abrain-1.0rc0.tar.gz` & `tmp/abrain-1.0rc0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abrain-1.0rc0.tar", last modified: Fri Jan 20 09:54:48 2023, max compression
+gzip compressed data, was "abrain-1.0rc0.post3.tar", last modified: Fri Apr 14 12:04:34 2023, max compression
```

## Comparing `abrain-1.0rc0.tar` & `abrain-1.0rc0.post3.tar`

### file list

```diff
@@ -1,63 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.875040 abrain-1.0rc0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8835 2023-01-20 09:54:38.000000 abrain-1.0rc0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-20 09:54:38.000000 abrain-1.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-20 09:54:38.000000 abrain-1.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-01-20 09:54:48.875040 abrain-1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-01-20 09:54:38.000000 abrain-1.0rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-01-20 09:54:38.000000 abrain-1.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 09:54:48.875040 abrain-1.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-01-20 09:54:38.000000 abrain-1.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.867040 abrain-1.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.871040 abrain-1.0rc0/src/abrain/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.871040 abrain-1.0rc0/src/abrain/_bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_bindings/config.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_bindings/genotype.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_bindings/module.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.871040 abrain-1.0rc0/src/abrain/_bindings/phenotype/
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_bindings/phenotype/ann.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_bindings/phenotype/cppn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_bindings/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.871040 abrain-1.0rc0/src/abrain/_cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/config.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/config.h
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/genotype.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.871040 abrain-1.0rc0/src/abrain/_cpp/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/misc/constants_template.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/misc/point.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.871040 abrain-1.0rc0/src/abrain/_cpp/phenotype/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/phenotype/ann.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     3710 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/phenotype/ann.h
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/phenotype/cppn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/phenotype/cppn.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    14903 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/phenotype/eshn.cpp
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/_cpp/phenotype/eshn.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.871040 abrain-1.0rc0/src/abrain/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/ann.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.875040 abrain-1.0rc0/src/abrain/core/functions/
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/abs.png
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/abs.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/bsgm.png
--rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/bsgm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/gaus.png
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/gaus.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/id.png
--rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/id.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/plotter.sh
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/sin.png
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/sin.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/ssgm.png
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/ssgm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/ssgn.png
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/ssgn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/step.png
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/step.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/functions/template.tex
--rw-r--r--   0 runner    (1001) docker     (123)    17775 2023-01-20 09:54:38.000000 abrain-1.0rc0/src/abrain/core/genome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:54:48.871040 abrain-1.0rc0/src/abrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-01-20 09:54:48.000000 abrain-1.0rc0/src/abrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-01-20 09:54:48.000000 abrain-1.0rc0/src/abrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 09:54:48.000000 abrain-1.0rc0/src/abrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-20 09:54:48.000000 abrain-1.0rc0/src/abrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-20 09:54:48.000000 abrain-1.0rc0/src/abrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.741765 abrain-1.0rc0.post3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8861 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-14 12:04:34.741765 abrain-1.0rc0.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:04:34.741765 abrain-1.0rc0.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.733764 abrain-1.0rc0.post3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.733764 abrain-1.0rc0.post3/src/abrain/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.733764 abrain-1.0rc0.post3/src/abrain/_bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_bindings/config.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_bindings/genotype.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_bindings/module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.733764 abrain-1.0rc0.post3/src/abrain/_bindings/phenotype/
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_bindings/phenotype/ann.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_bindings/phenotype/cppn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_bindings/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.737764 abrain-1.0rc0.post3/src/abrain/_cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/config.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/genotype.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.737764 abrain-1.0rc0.post3/src/abrain/_cpp/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/misc/constants_template.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3548 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/misc/point.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.737764 abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6331 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/ann.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3795 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/ann.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/cppn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/cppn.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15579 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/eshn.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/eshn.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.737764 abrain-1.0rc0.post3/src/abrain/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/ann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.741765 abrain-1.0rc0.post3/src/abrain/core/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/abs.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/abs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/bsgm.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/bsgm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/gaus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/gaus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8964 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/id.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/id.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/plotter.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/sin.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/sin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/ssgm.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/ssgm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/ssgn.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/ssgn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/step.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/step.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/functions/template.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/src/abrain/core/genome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.733764 abrain-1.0rc0.post3/src/abrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-14 12:04:34.000000 abrain-1.0rc0.post3/src/abrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-14 12:04:34.000000 abrain-1.0rc0.post3/src/abrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:04:34.000000 abrain-1.0rc0.post3/src/abrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-14 12:04:34.000000 abrain-1.0rc0.post3/src/abrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 12:04:34.000000 abrain-1.0rc0.post3/src/abrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:04:34.741765 abrain-1.0rc0.post3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/tests/test_ann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/tests/test_cppn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/tests/test_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-04-14 12:04:25.000000 abrain-1.0rc0.post3/tests/test_genome.py
```

### Comparing `abrain-1.0rc0/CMakeLists.txt` & `abrain-1.0rc0.post3/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,18 +63,19 @@
 pybind11_add_module(${LIB_CPP} ${CPP_SRC} ${PYBIND_SRC})
 target_compile_definitions(${LIB_CPP}
                            PRIVATE VERSION_INFO=${EXAMPLE_VERSION_INFO})
 
 ################################################################################
 ## C++ Coverage
 ################################################################################
+message("> With coverage ${WITH_COVERAGE}")
 if(WITH_COVERAGE)
     message("#### Searching for packages")
-    find_program(LCOV lcov REQUIRED)
-    find_program(GENHTML genhtml REQUIRED)
+    find_program(LCOV lcov)
+    find_program(GENHTML genhtml)
     if(NOT LCOV OR NOT GENHTML)
         message(SEND_ERROR "Could not find lcov/genhtml program(s). "
             "Either install missing components or run without coverage tests ("
             "${LCOV} & ${GENHTML})")
     endif()
 
     add_custom_target(coverage
```

### Comparing `abrain-1.0rc0/LICENSE` & `abrain-1.0rc0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/PKG-INFO` & `abrain-1.0rc0.post3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abrain
-Version: 1.0rc0
+Version: 1.0rc0.post3
 Summary: NeuroEvolution in Python backed by C++ computations
 Author-email: Kevin Godin-Dubois <k.j.m.godin-dubois@vu.nl>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -17,75 +17,64 @@
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: kaleido
 License-File: LICENSE
 
 # Artificial Brains (ABrain) for Python
 
+C++/Python implementation of fully evolvable Artificial Neural Networks.
+Uses the ES-HyperNEAT algorithms to *indirectly* encode ANNs with bio-mimetic
+patterns (repetitions, symmetry...), large number of neurons and relative
+robustness to input/output variations between generations.
+The API is served in Python and computations are performed in C++.
+
 [![Documentation Status](https://readthedocs.org/projects/abrain/badge/?version=latest)](https://abrain.readthedocs.io/en/latest/?badge=latest)
-![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-flake.md)
+![PEP8](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-flake.md)
+[![PyPI version](https://badge.fury.io/py/abrain.svg)](https://badge.fury.io/py/abrain)
+[![Downloads](https://static.pepy.tech/badge/abrain)](https://pepy.tech/project/abrain)
 
-### Release
-![](https://img.shields.io/badge/on-!-900?logo=pypi)
+#### tested on latest
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-manylinux.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-musllinux.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-macosx.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-win.md)
 
 ### Development
-![](https://img.shields.io/badge/version-!-900)
+![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-version.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-tests.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-cov.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-pcov.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-ccov.md)
 
-
-C++/Python implementation of the genotype/phenotype components of Evolvable Substrate HyperNEAT (read without evolution and speciation).
-
 ## Optional dependencies:
 
 ### Graphviz (dot)
 
-To generate directed graphs for the genomes
-Can only be fetched by system installer (apt-get, yum, ...)
+To generate directed graphs for the genomes.
+Can only be fetched by system installer (apt-get, yum, ...).
 See https://graphviz.org/download/ for instructions
 
 ### Kaleido
 
-To generate non-interactive images of ANN (through plotly)
-Due to inconsistent support, left as an optional dependency
+To generate non-interactive images of ANN (through plotly).
+Due to inconsistent support, left as an optional dependency.
 Use `pip install abrain[...,kaleido]` to get it
 
 ## Todo list:
- - Functionalities:
-   - Order-independent ANN evaluation (with back buffer)?
-   - Crossover / historical markings
-     - Actually needed?
-   - MANN Integration
-     - Easy extraction
-     - built-in testing
-     - C++ wrapper
-     - Visu
+- [ ] Functionalities:
+   - [ ] Order-independent ANN evaluation (with back buffer)?
+   - [ ] Crossover / historical markings
+     - [ ] Actually needed?
+   - [ ] MANN Integration
+     - [ ] Easy extraction
+     - [ ] built-in testing
+     - [ ] C++ wrapper
+     - [ ] Visu
      
-  - Misc:
-    - Documentation
-      - Usage
+  - [ ] Misc:
+    - [ ] Documentation
+      - [ ] Advanced usage
       
-    - Continuous integration
-      - build / tests
-      - Badges
-      
-    - Packaging:
-      - include c++ stubs?
-      - move to scikit/poetry/... ?
-      
-    - Installation errors:
-      - cp38,...,311-manylinux_i686 fail because cppn outputs diverge between manual and subset/all
-        > Caused by unmatched image/host platforms?
-        > Heisenbug, printing an FNode value before returning it makes it work
-        > Also disapears in when compiling in debug mode
-      - pp38,39-manylinux_i686,x86_64; pp38,39-macosx_x86_64; pp38,39-win_amd64 fail because of strange import error in numpy
-        > Solved by removing numpy dependency
-      - cp38,...,311-musllinux_i686 fail because pillow needs a jpeg library
-        > Solved? Added libjpeg to the apk (musllinux) install
-        > Removed pillow dependency
-      - cp38,..,311-win32,amd64 fail because of encoding error in ANN rendering
+      - [ ] move to scikit/poetry/... ?
+
+  - [ ] CI/CD
+    - [ ] Recent install gives `no loadimage plugion for "svg:cairo"` for pdf output
```

### Comparing `abrain-1.0rc0/README.md` & `abrain-1.0rc0.post3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,59 @@
 # Artificial Brains (ABrain) for Python
 
+C++/Python implementation of fully evolvable Artificial Neural Networks.
+Uses the ES-HyperNEAT algorithms to *indirectly* encode ANNs with bio-mimetic
+patterns (repetitions, symmetry...), large number of neurons and relative
+robustness to input/output variations between generations.
+The API is served in Python and computations are performed in C++.
+
 [![Documentation Status](https://readthedocs.org/projects/abrain/badge/?version=latest)](https://abrain.readthedocs.io/en/latest/?badge=latest)
-![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-flake.md)
+![PEP8](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-flake.md)
+[![PyPI version](https://badge.fury.io/py/abrain.svg)](https://badge.fury.io/py/abrain)
+[![Downloads](https://static.pepy.tech/badge/abrain)](https://pepy.tech/project/abrain)
 
-### Release
-![](https://img.shields.io/badge/on-!-900?logo=pypi)
+#### tested on latest
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-manylinux.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-musllinux.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-macosx.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-win.md)
 
 ### Development
-![](https://img.shields.io/badge/version-!-900)
+![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-version.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-tests.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-cov.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-pcov.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-ccov.md)
 
-
-C++/Python implementation of the genotype/phenotype components of Evolvable Substrate HyperNEAT (read without evolution and speciation).
-
 ## Optional dependencies:
 
 ### Graphviz (dot)
 
-To generate directed graphs for the genomes
-Can only be fetched by system installer (apt-get, yum, ...)
+To generate directed graphs for the genomes.
+Can only be fetched by system installer (apt-get, yum, ...).
 See https://graphviz.org/download/ for instructions
 
 ### Kaleido
 
-To generate non-interactive images of ANN (through plotly)
-Due to inconsistent support, left as an optional dependency
+To generate non-interactive images of ANN (through plotly).
+Due to inconsistent support, left as an optional dependency.
 Use `pip install abrain[...,kaleido]` to get it
 
 ## Todo list:
- - Functionalities:
-   - Order-independent ANN evaluation (with back buffer)?
-   - Crossover / historical markings
-     - Actually needed?
-   - MANN Integration
-     - Easy extraction
-     - built-in testing
-     - C++ wrapper
-     - Visu
+- [ ] Functionalities:
+   - [ ] Order-independent ANN evaluation (with back buffer)?
+   - [ ] Crossover / historical markings
+     - [ ] Actually needed?
+   - [ ] MANN Integration
+     - [ ] Easy extraction
+     - [ ] built-in testing
+     - [ ] C++ wrapper
+     - [ ] Visu
      
-  - Misc:
-    - Documentation
-      - Usage
+  - [ ] Misc:
+    - [ ] Documentation
+      - [ ] Advanced usage
       
-    - Continuous integration
-      - build / tests
-      - Badges
-      
-    - Packaging:
-      - include c++ stubs?
-      - move to scikit/poetry/... ?
-      
-    - Installation errors:
-      - cp38,...,311-manylinux_i686 fail because cppn outputs diverge between manual and subset/all
-        > Caused by unmatched image/host platforms?
-        > Heisenbug, printing an FNode value before returning it makes it work
-        > Also disapears in when compiling in debug mode
-      - pp38,39-manylinux_i686,x86_64; pp38,39-macosx_x86_64; pp38,39-win_amd64 fail because of strange import error in numpy
-        > Solved by removing numpy dependency
-      - cp38,...,311-musllinux_i686 fail because pillow needs a jpeg library
-        > Solved? Added libjpeg to the apk (musllinux) install
-        > Removed pillow dependency
-      - cp38,..,311-win32,amd64 fail because of encoding error in ANN rendering
+      - [ ] move to scikit/poetry/... ?
+
+  - [ ] CI/CD
+    - [ ] Recent install gives `no loadimage plugion for "svg:cairo"` for pdf output
```

### Comparing `abrain-1.0rc0/pyproject.toml` & `abrain-1.0rc0.post3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "abrain"
-version = "1.0rc"
+version = "1.0rc-post3"
 authors = [{ name="Kevin Godin-Dubois", email="k.j.m.godin-dubois@vu.nl"}]
 description = "NeuroEvolution in Python backed by C++ computations"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Development Status :: 3 - Alpha",
   
@@ -18,15 +18,14 @@
 
   "Intended Audience :: Science/Research", 
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Scientific/Engineering :: Artificial Life",
 ]
 dependencies = [
   "plotly",
-  "configobj",
   "importlib_resources",
   "graphviz",
   "pyrecord",
 ]
 
 [projects.urls]
 "Homepage" = "https://github.com/kgd-al/abrain"
```

### Comparing `abrain-1.0rc0/setup.py` & `abrain-1.0rc0.post3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,17 +31,14 @@
     def build_extension(self, ext: CMakeExtension) -> None:
         # Must be in this form due to bug in .resolve() only fixed in
         #  Python 3.10+
         ext_fullpath = Path.cwd() / self.get_ext_fullpath(ext.name) \
             # type: ignore[no-untyped-call]
         extdir = ext_fullpath.parent.resolve()
 
-        print(f"{ext_fullpath=}")
-        print(f"{extdir=}")
-
         # Using this requires trailing slash for auto-detection & inclusion of
         # auxiliary "native" libs
 
         # == kgd - Additions == #
         with_tests = bool(os.environ.get("TEST", 0))
         if with_tests:
             debug = True
@@ -65,15 +62,15 @@
             f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={extdir}{os.sep}",
             f"-DPYTHON_EXECUTABLE={sys.executable}",
             f"-DCMAKE_BUILD_TYPE={cfg}",  # not used on MSVC, but no harm
         ]
         build_args = []
         # Adding CMake arguments set as environment variable
         # (needed e.g. to build for ARM OSx on conda-forge)
-        
+
         if "CMAKE_ARGS" in os.environ:
             cmake_args += [item for item in os.environ["CMAKE_ARGS"].split(" ")
                            if item]
         print('[kgd-debug]', cmake_args)
 
         # Pass the version to C++ (why not?)
         cmake_args +=\
```

### Comparing `abrain-1.0rc0/src/abrain/__init__.py` & `abrain-1.0rc0.post3/src/abrain/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Docstring for abrain module/top-level package"""
 
-from .core.genome import Genome
 from .core.config import Config
+from .core.genome import Genome, GIDManager
 
 from .core.ann import ANN
 from .core.ann import plotly_render
 from ._cpp.phenotype import Point
 
 from ._cpp.phenotype import CPPN
 
 import importlib.metadata
 try:  # pragma: no cover
     # __package__ allows for the case where __name__ is "__main__"
     __version__ = importlib.metadata.version(__package__ or __name__)
-except importlib.metadata.PackageNotFoundError:
+except importlib.metadata.PackageNotFoundError:  # pragma: no cover
     __version__ = "0.0.0"
 
 
-__all__ = ['Genome', 'ANN', 'Config', 'Point', 'CPPN', 'plotly_render']
+__all__ = ['Genome', 'ANN', 'Config', 'Point', 'GIDManager', 'CPPN',
+           'plotly_render']
```

### Comparing `abrain-1.0rc0/src/abrain/_bindings/config.cpp` & `abrain-1.0rc0.post3/src/abrain/_bindings/config.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -33,34 +33,18 @@
   { "ESHN", {
     "initialDepth",
     "maxDepth",
     "iterations",
     "divThr",
     "varThr",
     "bndThr",
+    "allowPerceptrons"
   }}
 };
 
-using ParseInserter = std::function<void(const std::string&)>;
-bool do_parse_string (const std::string &s, ParseInserter inserter,
-                      const std::string &delims) {
-  auto l = s.find_first_of(delims[0]), r = s.find_last_of(delims[1]);
-  if (l != std::string::npos && r != std::string::npos) {
-    std::stringstream ss (s.substr(l+1, r-l-1));
-    std::string item;
-    while (std::getline(ss, item, ',')) {
-      if (item[0] == ' ') item = item.substr(1);
-      inserter(item);
-    }
-
-  } else
-    return false;
-  return true;
-}
-
 static utils::DocMap _docs {
   { "functionSet",
     "List of functions accessible to nodes via creation/mutation" },
 
   { "cppnWeightBounds",
     "Initial and maximal bounds for each of the CPPN's weights" },
 
@@ -108,14 +92,17 @@
     "Division threshold for a quad-/octtree cell/cube" },
 
   { "varThr",
     "Variance threshold for exploring a quad-/octtree cell/cube" },
 
   { "bndThr",
     "Minimal divergence threshold for discovering neurons" },
+
+  { "allowPerceptrons",
+    "Attempt to generate a perceptron if no hidden neurons were discovered" },
 };
 
 void init_config (py::module_ &m) {
   using Strings = std::vector<std::string>;
 
   auto strs = py::bind_vector<Strings>(m, "Strings");
   if (!std::is_same<Strings, Config::Functions>::value)
@@ -151,14 +138,19 @@
 
       .def_readwrite_static ID(initialDepth)
       .def_readwrite_static ID(maxDepth)
       .def_readwrite_static ID(iterations)
       .def_readwrite_static ID(divThr)
       .def_readwrite_static ID(varThr)
       .def_readwrite_static ID(bndThr)
+//       .def_readwrite_static ID(allowPerceptrons)
+      .def_property_static( // More verbose but prevents accidental conversions
+        "allowPerceptrons",
+        [](py::object) { return Config::allowPerceptrons; },
+        [](py::object, bool b) { Config::allowPerceptrons = b; })
 
       .def_readonly_static("_sections", &_sections)
       .def_readonly_static("_docstrings", &_docs)
 
       .def_static("known_function", [] (const phenotype::CPPN::FuncID &f) {
         static const auto &funcs = phenotype::CPPN::functions;
         return funcs.find(f) != funcs.end();
@@ -187,65 +179,53 @@
         std::ostringstream oss;
         oss << "Bounds(" << fb.min << ", " << fb.rndMin << ", " << fb.rndMax
             << ", " << fb.max << ", " << fb.stddev << ")";
         return oss.str();
       })
   ;
 
-  /// String parser methods (for config file reading)
-  fbnd.def_static("ccpParseString", [] (const std::string &s) {
-    Config::FBounds b {};
-    std::vector<float> values;
-    bool ok = do_parse_string(s, [&values] (auto item) {
-      std::istringstream iss (item);
-      float f;
-      iss >> f;
-      values.push_back(f);
-    }, "()");
-
-    ok &= (values.size() == 5);
-    if (ok) {
-      b.min = values[0], b.rndMin = values[1],
-      b.rndMax = values[2], b.max = values[3],
-      b.stddev = values[4];
-    }
-    return b;
-  }, "Try to parse the provided string into a mutation bounds object")
-      .def_static("isValid", [] (const Config::FBounds &b) {
+  // json converter (read/write to primitive python types)
+  fbnd.def("toJson", [] (const Config::FBounds &b) {
+      std::vector<float> v {{b.min, b.rndMin, b.rndMax, b.max, b.stddev}};
+        return py::list(py::cast(v));
+  }, "Convert to a python list of floats")
+      .def_static("fromJson", [] (const std::vector<float> &l) {
+        return Config::FBounds{l[0], l[1], l[2], l[3], l[4]};
+  }, "Convert from a python list of floats")
+      .def("isValid", [] (const Config::FBounds &b) {
     return b.min <= b.rndMin && b.rndMin <= b.rndMax && b.rndMax <= b.max
         && b.stddev > 0;
   }, "Whether this is a valid mutation bounds object");
 
-  strs.def_static("ccpParseString", [] (const std::string &s) {
-    Strings strs;
-    bool ok = do_parse_string(s, [&strs] (auto item) {
-      strs.push_back(item);
-    }, "[]");
-
-    if (ok) return strs;
-    else    return Strings{};
-  }, "Try to parse the provided string into a strings collection")
-      .def_static("isValid", [] (const Strings &s) {
+  strs.def("toJson", [] (const Strings &s) {
+      return py::list(py::cast(s));
+  }, "Convert to a python list of strings")
+      .def_static("fromJson", [] (const py::list &l) {
+        Strings s;
+        for (auto item: l)  s.push_back(item.cast<std::string>());
+        return s;
+  }, "Convert from a python list of strings")
+      .def("isValid", [] (const Strings &s) {
     return !s.empty();
   }, "Whether this is a valid strings colleciton (not empty)");
 
-  mutr.def_static("ccpParseString", [] (const std::string &s) {
-    Config::MutationRates mr;
-    bool ok = do_parse_string(s, [&mr] (auto item) {
-      auto d = item.find_first_of(':');
-      auto key = item.substr(0, d), value = item.substr(d+2);
-
-      std::istringstream iss (value);
-      float f;
-      iss >> f;
-      mr[key] = f;
-    }, "{}");
-
-    if (ok) return mr;
-    else    return Config::MutationRates{};
-  }, "Try to parse the provided string into a dictionary of mutation rates")
-      .def_static("isValid", [] (const Config::MutationRates &r) {
-    return !r.empty();
+
+  mutr.def("toJson", [] (const Config::MutationRates &s) {
+      return py::dict(py::cast(s));
+  }, "Convert to a python map of strings/float")
+      .def_static("fromJson", [] (const py::dict &d) {
+        Config::MutationRates r;
+        for (auto pair: d)
+          r[pair.first.cast<std::string>()] = pair.second.cast<float>();
+        return r;
+  }, "Convert from a python map of strings/floats")
+      .def("isValid", [] (const Config::MutationRates &r) {
+    float sum = 0;
+    for (const auto &p: r) {
+      if (p.second < 0) return false;
+      sum += p.second;
+    }
+    return sum > 0;
   }, "Whether this is a valid dictionary of mutation rates");
 }
 
 } // end of namespace kgd::eshn::pybind
```

### Comparing `abrain-1.0rc0/src/abrain/_bindings/genotype.cpp` & `abrain-1.0rc0.post3/src/abrain/_bindings/genotype.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,62 @@
 #include <sstream>
 
 #include "../_cpp/genotype.h"
 #include "utils.hpp"
 
 #include "pybind11/pybind11.h"
 namespace py = pybind11;
+using namespace pybind11::literals;
 
 #include "pybind11/stl_bind.h"
 PYBIND11_MAKE_OPAQUE(std::vector<kgd::eshn::genotype::CPPNData::Node>)
 PYBIND11_MAKE_OPAQUE(std::vector<kgd::eshn::genotype::CPPNData::Link>)
 
 using namespace kgd::eshn::genotype;
 namespace kgd::eshn::pybind {
 
 static const utils::DocMap _cppn_doc {
   { "INPUTS",  "Number of inputs for the CPPN"  },
   { "OUTPUTS", "Number of outputs for the CPPN" },
 };
 
-void init_genotype (py::module_ &m) {
-  using Node = CPPNData::Node;
-  using Link = CPPNData::Link;
+py::dict to_json (const CPPNData &d) {
+  py::dict dict;
+  py::list nodes, links;
+  for (auto &n: d.nodes)  nodes.append(py::make_tuple(n.id, n.func));
+  for (auto &l: d.links)
+    links.append(py::make_tuple(l.id, l.src, l.dst, l.weight));
+  dict["nodes"] = nodes;
+  dict["links"] = links;
+  dict["nextNodeID"] = d.nextNodeID;
+  dict["nextLinkID"] = d.nextLinkID;
+  return dict;
+}
+
+using Node = CPPNData::Node;
+using Link = CPPNData::Link;
+
+CPPNData from_json (py::dict dict) {
+  CPPNData d;
+  d.nextNodeID = dict["nextNodeID"].cast<int>();
+  d.nextLinkID = dict["nextLinkID"].cast<int>();
+  for (const py::handle &h: dict["nodes"]) {
+    py::tuple t = h.cast<py::tuple>();
+    d.nodes.push_back(Node{t[0].cast<int>(), t[1].cast<std::string>()});
+  }
+  for (const py::handle &h: dict["links"]) {
+    py::tuple t = h.cast<py::tuple>();
+    d.links.push_back(Link{t[0].cast<int>(),
+                            t[1].cast<uint>(), t[2].cast<uint>(),
+                            t[3].cast<float>()});
+  }
+  return d;
+}
 
+void init_genotype (py::module_ &m) {
   auto cppn = py::class_<CPPNData>(m, "CPPNData");
   auto node = py::class_<Node>(cppn, "Node");
   auto link = py::class_<Link>(cppn, "Link");
 
   py::bind_vector<std::vector<Node>>(cppn, "Nodes", "Collection of Nodes");
   py::bind_vector<std::vector<Link>>(cppn, "Links", "Collection of Links");
 
@@ -36,14 +67,21 @@
       .def_readonly_static ID(INPUTS, "")
       .def_readonly_static ID(OUTPUTS)
       .def_readonly_static("_docstrings", &_cppn_doc)
       .def_readwrite ID(nodes, "The collection of computing nodes")
       .def_readwrite ID(links, "The collection of inter-node relationships")
       .def_readwrite ID(nextNodeID, "ID for the next random node (monotonic)")
       .def_readwrite ID(nextLinkID, "ID for the next random link (monotonic")
+      .def("to_json", to_json, "Convert to a json-compliant Python dictionary")
+      .def_static("from_json", from_json, "j"_a,
+                  "Convert from the json-compliant Python dictionary `j`")
+      .def(py::pickle(
+        [] (const CLASS &d) { return to_json(d); },
+        [](py::dict d) {      return from_json(d);  }
+      ))
       ;
 
 #undef CLASS
 #define CLASS Node
   node.doc() = "Computational node of a CPPN";
   node.def(py::init<int, const Node::FuncID &>())
       .def("__repr__", [] (const Node &n) {
```

### Comparing `abrain-1.0rc0/src/abrain/_bindings/module.cpp` & `abrain-1.0rc0.post3/src/abrain/_bindings/module.cpp`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/_bindings/phenotype/ann.cpp` & `abrain-1.0rc0.post3/src/abrain/_bindings/phenotype/ann.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -76,15 +76,22 @@
 :param outputs: computed analog values for the output neurons
 :param substeps: number of sequential executions
 
 .. seealso:: :ref:`usage-basics-ann`
            )", "inputs"_a, "outputs"_a, "substeps"_a = 1)
 
       .def ID(empty,
-              "Whether the ANN contains neurons/connections")
+              R"(
+Whether the ANN contains neurons/connections
+
+:param strict: whether perceptrons count as empty (true) or not (false)
+
+.. seealso:: `Config::allowPerceptrons`
+              )", py::arg("strict") = false)
+      .def ID(perceptron, "Whether this ANN is a perceptron")
       .def ID(stats, "Return associated stats (connections, depth...)")
       .def("neurons", py::overload_cast<>(&ANN::neurons, py::const_),
            "Provide read-only access to the underlying neurons")
       .def ID(neuronAt, "Query an individual neuron", "pos"_a)
 
       .def_static("build", &ANN::build, R"(
 Create an ANN via ES-HyperNEAT
@@ -198,14 +205,25 @@
       .value("H", Type::H, "Hidden (processing data)")
       .value("O", Type::O, "Output (producing data)")
   ;
 
 #undef CLASS
 #define CLASS ANN::Stats
   stts.doc() = "Contains various statistics about an ANN";
-  stts.def_readonly ID(depth, "Maximal depth of the neural network")
+  stts.def_readonly ID(hidden, "Number of hidden neurons")
+      .def_readonly ID(depth, "Maximal depth of the neural network")
       .def_readonly ID(edges, "Number of connections")
       .def_readonly ID(axons, "Total length of the connections")
+      .def_readonly ID(iterations, "H -> H iterations before convergence")
+      .def("dict", [] (const CLASS &stats) {
+        return py::dict (
+#define PAIR(X) #X##_a=stats.X
+          PAIR(depth), PAIR(iterations),
+          PAIR(hidden),
+          PAIR(edges), PAIR(axons)
+#undef PAIR
+        );
+      }, "Return the stats as Python dictionary")
       ;
 }
 
 } // namespace kgd::eshn::pybind
```

### Comparing `abrain-1.0rc0/src/abrain/_bindings/phenotype/cppn.cpp` & `abrain-1.0rc0.post3/src/abrain/_bindings/phenotype/cppn.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #include <functional>
 
 #include "pybind11/pybind11.h"
 namespace py = pybind11;
 
 #include "pybind11/stl_bind.h"
 #include "pybind11/functional.h"
+#include "pybind11/operators.h"
 using namespace pybind11::literals;
 
 using namespace kgd::eshn::phenotype;
 PYBIND11_MAKE_OPAQUE(CPPN::Outputs)
 
 namespace kgd::eshn::pybind {
 
@@ -48,14 +49,21 @@
       .def(py::init([] (float x, float y, float z) { return Point({x,y,z}); }),
            "Create a point with the specified coordinates\n\n"
            "Args:\n"
            "  x, y, z (float): x, y, z coordinate",
            "x"_a, "y"_a, "z"_a)
 #endif
       .def("__repr__", [] (const Point &p) { return utils::mergeToString(p); })
+      .def(pybind11::self == pybind11::self)
+      .def(pybind11::self != pybind11::self)
+      .def("__hash__", [] (const Point &p) { // Bad hash
+        int sum = 0;
+        for (int i: p.data()) sum += i;
+        return sum;
+      })
       .def("tuple", [] (const Point &p) {
 #if ESHN_SUBSTRATE_DIMENSION == 3
         return std::tuple(p.x(), p.y(), p.z());
 #else
         return std::tuple(p.x(), p.y());
 #endif
       }, "Return a tuple for easy unpacking in python")
```

### Comparing `abrain-1.0rc0/src/abrain/_bindings/utils.hpp` & `abrain-1.0rc0.post3/src/abrain/_bindings/utils.hpp`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/_cpp/config.cpp` & `abrain-1.0rc0.post3/src/abrain/_cpp/config.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -47,8 +47,10 @@
 uint Config::maxDepth = 3;
 uint Config::iterations = 10;
 
 float Config::divThr = .3f;
 float Config::varThr = .3f;
 float Config::bndThr = .15f;
 
+bool Config::allowPerceptrons = true;
+
 } // end of namespace kgd::eshn
```

### Comparing `abrain-1.0rc0/src/abrain/_cpp/config.h` & `abrain-1.0rc0.post3/src/abrain/_cpp/config.h`

 * *Files 16% similar despite different names*

```diff
@@ -30,20 +30,21 @@
   using MutationRates = std::map<std::string, float>;
   static MutationRates mutationRates;
 
   using FBounds = Bounds<float>;
   static FBounds cppnWeightBounds;
 
   /// ================================================
-  /// ANN parameters (none?)
+  /// ANN parameters
   static float annWeightsRange;
   static FID activationFunc;
 
   /// ================================================
   /// ES-HyperNEAT parameters
   static uint initialDepth, maxDepth, iterations;
   static float divThr, varThr, bndThr;
+  static bool allowPerceptrons;
 };
 
 } // end of namespace kgd::eshn
 
 #endif // KGD_GENOTYPE_CONFIG_H
```

### Comparing `abrain-1.0rc0/src/abrain/_cpp/genotype.h` & `abrain-1.0rc0.post3/src/abrain/_cpp/genotype.h`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/_cpp/misc/constants_template.h` & `abrain-1.0rc0.post3/src/abrain/_cpp/misc/constants_template.h`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/_cpp/misc/point.hpp` & `abrain-1.0rc0.post3/src/abrain/_cpp/misc/point.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -60,21 +60,25 @@
   }
 
   float get (uint i) const {
     return _data[i] / float(RATIO);
   }
 
   void set (uint i, float v) {
-    _data[i] = std::round(RATIO * v);
+    _data[i] = int(std::round(RATIO * v));
   }
 
   void set (float v) {
     for (uint i=0; i<DIMENSIONS; i++) set(i, v);
   }
 
+  const auto& data (void) const {
+    return _data;
+  }
+
   Point_t& operator+= (const Point_t &that) {
     for (uint i=0; i<DIMENSIONS; i++) set(i, get(i) + that.get(i));
     return *this;
   }
 
   Point_t& operator-= (const Point_t &that) {
     for (uint i=0; i<DIMENSIONS; i++) set(i, get(i) - that.get(i));
```

### Comparing `abrain-1.0rc0/src/abrain/_cpp/phenotype/ann.cpp` & `abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/ann.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 #ifndef NDEBUG
 //#define DEBUG_COMPUTE 1
 #endif
 
 using Output = CPPN::Output;
 using Point = es::Point;
 
-bool ANN::empty(void) const {
-  return stats().edges == 0;
+bool ANN::empty(bool strict) const {
+  return strict ? (stats().hidden == 0) : (stats().edges == 0);
+}
+
+bool ANN::perceptron(void) const {
+  return (stats().hidden == 0) && stats().edges > 0;
 }
 
 ANN ANN::build (const Coordinates &inputs,
                 const Coordinates &outputs,
                 const genotype::CPPNData &genome) {
 
   static const auto& weightRange = Config::annWeightsRange;
@@ -44,16 +48,17 @@
   i = 0;
   ann._outputs.resize(outputs.size());
   ann._obuffer.resize(outputs.size());
   for (auto &p: outputs) neurons.insert(ann._outputs[i++] = add(p, Neuron::O));
 
   Coordinates hidden;
   evolvable_substrate::Connections connections;
-  if (evolvable_substrate::connect(cppn, inputs, outputs, hidden,
-                                   connections)) {
+  if (evolvable_substrate::connect(cppn, inputs, outputs,
+                                   hidden, connections,
+                                   ann._stats.iterations)) {
     for (auto &p: hidden) neurons.insert(add(p, Neuron::H));
     for (auto &c: connections)
       ann.neuronAt(c.to)->addLink(c.weight * weightRange, ann.neuronAt(c.from));
   }
 
   ann.computeStats();
 
@@ -143,29 +148,27 @@
     d = std::max(d, p.second->n.depth);
     delete p.second;
   }
   return d;
 }
 
 void ANN::computeStats(void) {
-  if (_neurons.size() == _inputs.size() + _outputs.size()) {
+  _stats.hidden = uint(_neurons.size() - _inputs.size() - _outputs.size());
+  if (_stats.hidden == 0) {
     for (Neuron::ptr &n: _inputs)   n->depth = 0;
     for (Neuron::ptr &n: _outputs)  n->depth = 1;
     _stats.depth = 1;
-    _stats.edges = 0;
-    _stats.axons = 0;
-    return;
-  }
 
-  _stats.depth = computeDepth(*this);
+  } else
+    _stats.depth = computeDepth(*this);
 
   auto &e = _stats.edges = 0;
   float &l = _stats.axons = 0;
   for (const Neuron::ptr &n: _neurons) {
-    e += n->links().size();
+    e += uint(n->links().size());
     for (const Neuron::Link &link: n->links())
       l += (n->pos - link.in.lock()->pos).length();
   }
 }
 
 ANN::Neuron::ptr ANN::addNeuron(const Point &p, Neuron::Type t, float bias) {
   return std::make_shared<Neuron>(p, t, bias);
```

### Comparing `abrain-1.0rc0/src/abrain/_cpp/phenotype/ann.h` & `abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/ann.h`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,18 @@
 
   private:
     Links _ilinks;
   };
 
   struct Stats {
     uint depth;
+    uint hidden;
     uint edges;
     float axons;  // total length
+    uint iterations;
   };
 
   ANN(void) = default;
 
   const auto& neurons (void) const {  return _neurons;  }
   auto& neurons (void) {  return _neurons;  }
 
@@ -85,15 +87,16 @@
 
 //  void reset (void);
 
   /// TODO Modify with buffer-based eval. Maybe
   /// .. todo:: Modify with buffer-based eval. Maybe
   void operator() (const IBuffer &inputs, OBuffer &outputs, uint substeps = 1);
 
-  bool empty (void) const;
+  bool empty (bool strict = false) const;
+  bool perceptron (void) const;
 
   void computeStats (void);
   const auto& stats (void) const {
     return _stats;
   }
 
   // Deepcopy for develop once / use many
```

### Comparing `abrain-1.0rc0/src/abrain/_cpp/phenotype/cppn.cpp` & `abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/cppn.cpp`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/_cpp/phenotype/cppn.h` & `abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/cppn.h`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   struct Range { float min, max; };
   static const std::map<FuncID, Range> functionRanges;
 
 private:
   struct Node_base {
     float data;
     
-    virtual ~Node_base(void) = default;
+    virtual ~Node_base(void) = default; // LCOVR_EXCL_LINE
 
     virtual float value (void) = 0;
   };
   using Node_ptr = std::shared_ptr<Node_base>;
   using Node_wptr = std::weak_ptr<Node_base>;
 
   struct INode final : public Node_base {
```

### Comparing `abrain-1.0rc0/src/abrain/_cpp/phenotype/eshn.cpp` & `abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/eshn.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
   float variance (void) const {
     if (cs.empty()) return 0;
     float mean = 0;
     for (auto &c: cs) mean += c->weight;
     mean /= cs.size();
     float var = 0;
-    for (auto &c: cs) var += std::pow(c->weight - mean, 2);
+    for (auto &c: cs) var += float(std::pow(c->weight - mean, 2));
     return var / cs.size();
   }
 
 #if DEBUG_ES_QUADTREE
   friend std::ostream& operator<< (std::ostream &os, const QuadTreeNode &n) {
     utils::IndentingOStreambuf indent (os);
     os << "QTN " << n.center << " " << n.radius << " " << n.level << " "
@@ -115,15 +115,15 @@
     q.pop();
 
     float cx = n.center.x(), cy = n.center.y();
 #if ESHN_SUBSTRATE_DIMENSION == 3
     float cz = n.center.z();
 #endif
     float hr = .5 * n.radius;
-    float nl = n.level + 1;
+    float nl = float(n.level) + 1;
 
     n.cs.resize(1 << ESHN_SUBSTRATE_DIMENSION);
     uint i=0;
     for (int x: {-1,1})
       for (int y: {-1, 1})
 #if ESHN_SUBSTRATE_DIMENSION == 2
         n.cs[i++] = node(cx + x * hr, cy + y * hr, hr, nl);
@@ -367,19 +367,36 @@
   for (auto &c: newConnections) {
     auto r = hiddens.insert(c.to);
     if (r.second) newHiddens.insert(c.to);
   }
   connections.insert(newConnections.begin(), newConnections.end());
 }
 
+/// Query for direct input-output connections
+void generatePerceptron(CPPN &cppn,
+                        const Coordinates &inputs, const Coordinates &outputs,
+                        Connections &connections) {
+
+  CPPN::OutputSubset wl {{ Output::Weight, Output::LEO }};
+  CPPN::Outputs res;
+
+  for (const Point &i: inputs) {
+    for (const Point &o: outputs) {
+      cppn(i, o, res, wl);
+      if (res[uint(Output::LEO)])
+        connections.insert({i, o, res[uint(Output::Weight)]});
+    }
+  }
+}
+
 bool connect (CPPN &cppn,
               const Coordinates &inputs, const Coordinates &outputs,
-              Coordinates &hidden, Connections &connections) {
+              Coordinates &hidden, Connections &connections, uint &iterations) {
 
-  static const auto &iterations = Config::iterations;
+  static const auto &max_iterations = Config::iterations;
 
   Coordinates_s sio;  // All fixed positions
   for (const auto &vec: {inputs, outputs}) {
     for (Point p: vec) {
       auto r = sio.insert(p);
       if (!r.second) {
         std::cerr << "inputs: " << inputs << "\noutputs: " << outputs
@@ -420,15 +437,15 @@
   n_hidden = shidden.size();
   n_connections = connections.size();
   oss << "\n";
 #endif
 
   bool converged = false;
   Coordinates_s unexploredHidden = shidden;
-  for (uint i=0; i<iterations && !converged; i++) {
+  for (iterations = 0; iterations<max_iterations && !converged; iterations++) {
 
     Coordinates_s newHiddens;
     for (const Point &p: unexploredHidden) {
       Connections tmpConnections;
       auto t = divisionAndInitialisation(cppn, p, true);
       pruneAndExtract(cppn, p, tmpConnections, t, true);
       collect(tmpConnections, connections, shidden, newHiddens);
@@ -500,14 +517,17 @@
   showConnections(oss, connections);
   oss << "\n";
 #endif
 #endif
 
   std::copy(shidden2.begin(), shidden2.end(), std::back_inserter(hidden));
 
+  if (hidden.empty() && Config::allowPerceptrons)
+    generatePerceptron(cppn, inputs, outputs, connections);
+
 #if DEBUG_ES
   std::cerr << oss.str() << std::endl;
 #endif
 
   return true;
 }
```

### Comparing `abrain-1.0rc0/src/abrain/_cpp/phenotype/eshn.h` & `abrain-1.0rc0.post3/src/abrain/_cpp/phenotype/eshn.h`

 * *Files 4% similar despite different names*

```diff
@@ -45,12 +45,13 @@
 
 using CPPN = kgd::eshn::phenotype::CPPN;
 using Point = CPPN::Point;
 using Coordinates = std::vector<Point>;
 
 bool connect (CPPN &cppn,
               const Coordinates &inputs, const Coordinates &outputs,
-              Coordinates &hidden, Connections &connections);
+              Coordinates &hidden, Connections &connections,
+              uint &iterations);
 
 } // end of namespace kgd::eshn::evolvable_substrate
 
 #endif // KGD_EVOLV_SUBSTRATE_H
```

### Comparing `abrain-1.0rc0/src/abrain/core/functions/abs.png` & `abrain-1.0rc0.post3/src/abrain/core/functions/abs.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/abs.svg` & `abrain-1.0rc0.post3/src/abrain/core/functions/abs.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/bsgm.png` & `abrain-1.0rc0.post3/src/abrain/core/functions/bsgm.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/bsgm.svg` & `abrain-1.0rc0.post3/src/abrain/core/functions/bsgm.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/gaus.png` & `abrain-1.0rc0.post3/src/abrain/core/functions/gaus.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/gaus.svg` & `abrain-1.0rc0.post3/src/abrain/core/functions/gaus.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/id.png` & `abrain-1.0rc0.post3/src/abrain/core/functions/id.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/id.svg` & `abrain-1.0rc0.post3/src/abrain/core/functions/id.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/plotter.sh` & `abrain-1.0rc0.post3/src/abrain/core/functions/plotter.sh`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/sin.png` & `abrain-1.0rc0.post3/src/abrain/core/functions/sin.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/sin.svg` & `abrain-1.0rc0.post3/src/abrain/core/functions/sin.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/ssgm.png` & `abrain-1.0rc0.post3/src/abrain/core/functions/ssgm.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/ssgm.svg` & `abrain-1.0rc0.post3/src/abrain/core/functions/ssgm.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/ssgn.png` & `abrain-1.0rc0.post3/src/abrain/core/functions/ssgn.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/ssgn.svg` & `abrain-1.0rc0.post3/src/abrain/core/functions/ssgn.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/step.png` & `abrain-1.0rc0.post3/src/abrain/core/functions/step.png`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/step.svg` & `abrain-1.0rc0.post3/src/abrain/core/functions/step.svg`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/functions/template.tex` & `abrain-1.0rc0.post3/src/abrain/core/functions/template.tex`

 * *Files identical despite different names*

### Comparing `abrain-1.0rc0/src/abrain/core/genome.py` & `abrain-1.0rc0.post3/src/abrain/core/genome.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,85 @@
 """
 Test documentation for genome file (module?)
 """
-import json
 import logging
 import pathlib
 from collections import namedtuple
 from collections.abc import Iterable
 from random import Random
 from shutil import which
-from typing import Dict, List
+from typing import Dict, List, Any, Optional
 
 from graphviz import Digraph
 from importlib_resources import files
 from pyrecord import Record
 
 from .._cpp.config import Config
 from .._cpp.genotype import CPPNData as _CPPNData
 
 logger = logging.getLogger(__name__ + ".mutations")
 
-
 dot_found = (which("dot") is not None)
 
 
+class GIDManager:
+    """Simple integer-producing class for unique genome identifier
+    """
+    def __init__(self):
+        """Assign 0 as the next value
+        """
+        self._next_value = 0
+
+    def __call__(self) -> int:
+        """Return a new value and increment internal counter
+        """
+        value = self._next_value
+        self._next_value += 1
+        return value
+
+
 class Genome(_CPPNData):
     """Genome class for ES-HyperNEAT.
 
     A simple collection of Node/Link.
     Can only be created via random init or copy
     """
 
     __private_key = object()
     """Private key for preventing default-constructed CPPNs
     """
 
+    __id_field = "_id"
+    """Name of the private field in which to store the optional identifier
+    """
+
+    __parents_field = "_parents"
+    """Name of the private field in which to store the optional genealogy
+    """
+
     def __init__(self, key=None):
         _CPPNData.__init__(self)
         assert (key == Genome.__private_key), \
             "Genome objects must be created via random, deepcopy or" \
             " reproduction methods"
 
     def __repr__(self):
         return f"CPPN:{Genome.INPUTS}:{Genome.OUTPUTS}([{len(self.nodes)}," \
                f" {self.nextNodeID}], [{len(self.links)},{self.nextLinkID}])"
 
-    @staticmethod
-    def _is_input(nid: int):
-        return nid < Genome.INPUTS
-
-    @staticmethod
-    def _is_output(nid: int):
-        return Genome.INPUTS <= nid < Genome.INPUTS + Genome.OUTPUTS
-
-    @staticmethod
-    def _is_hidden(nid: int):
-        return Genome.INPUTS + Genome.OUTPUTS <= nid
+    def id(self) -> Optional[int]:
+        """Return the genome id if one was generated"""
+        return getattr(self, self.__id_field, None)
+
+    def parents(self) -> Optional[int]:
+        """Return the genome's parent(s) if possible"""
+        return getattr(self, self.__parents_field, None)
 
     ###########################################################################
-    # Public mutation interface
+    # Public manipulation interface
     ###########################################################################
 
     def mutate(self, rng: Random) -> None:
         """Mutate (in-place) this genome
 
         :param rng: The source of randomness
         """
@@ -146,79 +164,147 @@
         }
 
         assert sum(rates.values()) > 0  # Should never occur outside tests
 
         choice = rng.choices(list(rates.keys()), list(rates.values()))[0]
         actions[choice][0](rng, *actions[choice][1:])
 
-    def mutated(self, rng: Random) -> 'Genome':
+    def mutated(self, rng: Random, id_manager: Optional[GIDManager] = None) \
+            -> 'Genome':
         """Return a mutated (copied) version of this genome
 
         :param rng: the source of randomness
+        :param id_manager: an optional manager providing unique identifiers
         """
         copy = self.copy()
         copy.mutate(rng)
-        return copy
-
-    def copy(self) -> 'Genome':
-        """Return a perfect (deep)copy of this genome"""
-        copy = Genome(Genome.__private_key)
-
-        copy.nodes = self.nodes
-        copy.links = self.links
-        copy.nextNodeID = self.nextNodeID
-        copy.nextLinkID = self.nextLinkID
-
+        assert hasattr(self, self.__id_field) == (id_manager is not None), \
+            "Current genome has an id, but no ID manager provided for child"
+        if id_manager is not None:
+            setattr(copy, self.__id_field, id_manager())
+            setattr(copy, self.__parents_field, [self.id()])
         return copy
 
     @staticmethod
-    def random(rng: Random) -> 'Genome':
+    def random(rng: Random, id_manager: Optional[GIDManager] = None) \
+            -> 'Genome':
         """Create a random CPPN with boolean initialization
 
         :param rng: The source of randomness
+        :param id_manager: an optional manager providing unique identifiers
+
         :return: A random CPPN genome
         """
         g = Genome(Genome.__private_key)
 
         for i in range(_CPPNData.INPUTS):
             for j in range(_CPPNData.OUTPUTS):
                 if rng.random() < .5:
                     g._add_link(i, j + _CPPNData.INPUTS,
                                 Genome.__random_link_weight(rng))
 
+        if id_manager is not None:
+            setattr(g, g.__id_field, id_manager())
+            setattr(g, g.__parents_field, [])
+
         return g
 
+    def copy(self) -> 'Genome':
+        """Return a perfect (deep)copy of this genome"""
+        copy = Genome(Genome.__private_key)
+
+        copy.nodes = self.nodes
+        copy.links = self.links
+        copy.nextNodeID = self.nextNodeID
+        copy.nextLinkID = self.nextLinkID
+
+        if hasattr(self, self.__id_field):
+            setattr(copy, copy.__id_field, self.id())
+            setattr(copy, copy.__parents_field, self.parents())
+
+        return copy
+
+    ###########################################################################
+    # Public copy/deepcopy interface
+    ###########################################################################
+
+    def __copy__(self):
+        """Return a perfect (deep)copy of this genome
+
+        Implements the shallow copy interface
+        """
+        return self.copy()
+
+    def __deepcopy__(self, _):
+        """Return a perfect (deep)copy of this genome
+
+        Implements the deep copy interface
+        """
+        return self.copy()
+
+    ###########################################################################
+    # Public pickle interface
+    ###########################################################################
+
+    def __getstate__(self):
+        """Pickle the genome
+
+        Also store the id/parents if present
+        """
+        dct = _CPPNData.__getstate__(self)
+        if hasattr(self, self.__id_field):
+            dct[self.__id_field] = self.id()
+            dct[self.__parents_field] = self.parents()
+        return dct
+
+    def __setstate__(self, state):
+        """Unpickle the genome
+
+        Also restore the id/parents if present
+        """
+        _CPPNData.__setstate__(self, state)
+        if self.__id_field in state:
+            setattr(self, self.__id_field, state[self.__id_field])
+            setattr(self, self.__parents_field, state[self.__parents_field])
+
     ###########################################################################
     # Public json/binary interface
     ###########################################################################
 
-    def to_json(self) -> str:
-        """Return a string json representation of this object"""
-        return json.dumps(dict(
+    def to_json(self) -> Dict[Any, Any]:
+        """Return a json (dict) representation of this object"""
+        dct = dict(
             nodes=[(n.id, n.func) for n in self.nodes],
             links=[(l_.id, l_.src, l_.dst, l_.weight) for l_ in self.links],
             NID=self.nextNodeID,
             LID=self.nextLinkID
-        ))
+        )
+        if (gid := self.id()) is not None:
+            dct[self.__id_field] = gid
+            dct[self.__parents_field] = self.parents()
+        return dct
 
     @staticmethod
-    def from_json(json_str: str) -> 'Genome':
+    def from_json(data: Dict[Any, Any]) -> 'Genome':
         """Recreate a Genome from a string json representation
         """
-        data = json.loads(json_str)
         g = Genome(Genome.__private_key)
         g.nodes = _CPPNData.Nodes([
             _CPPNData.Node(n[0], n[1]) for n in data["nodes"]
         ])
         g.links = _CPPNData.Links([
             _CPPNData.Link(*[d[0], d[1], d[2], d[3]]) for d in data["links"]
         ])
         g.nextNodeID = data["NID"]
         g.nextLinkID = data["LID"]
 
+        if (gid := data.get(g.__id_field, None)) is not None:
+            setattr(g, g.__id_field, gid)
+            setattr(g, g.__parents_field, data[g.__parents_field])
+
         return g
 
     ###########################################################################
     # Public graphviz/dot interface
     ###########################################################################
 
     @staticmethod
@@ -229,15 +315,16 @@
 
         :param path: the file to load
         :param rng: random pick unspecified functions
         :return: The user-specified CPPN
         """
         raise NotImplementedError  # pragma: no cover
 
-    def to_dot(self, path: str, ext: str = "pdf", title: str = None,
+    def to_dot(self, path: str, ext: str = "pdf",
+               title: Optional[str] = None,
                debug=None) -> str:
         """Produce a graphical representation of this genome
 
         .. note:: Missing functions images in nodes and/or lots of
             warning message are likely caused by misplaced image files.
             In doubt perform a full reinstall
 
@@ -250,20 +337,20 @@
 
                 - 'depth' will display every nodes' depth
 
         Raises:
             OSError: if the `dot` program is not available (not installed, on
                 the path and executable)
         """
-        if not dot_found:
+        if not dot_found:  # pragma: no cover
             raise OSError("""
                 dot program not found. Make sure it is installed before using
                  this function.
-                 
-                [ubuntu] sudo apt install graphviz 
+
+                [ubuntu] sudo apt install graphviz
             """)
 
         path = pathlib.Path(path)
         if path.suffix != "":
             ext = path.suffix.replace('.', '')
             path = path.with_suffix('')
 
@@ -362,14 +449,26 @@
         return dot.render(path, format=ext, cleanup=cleanup)
 
     ###########################################################################
     # Private mutation interface
     ###########################################################################
 
     @staticmethod
+    def _is_input(nid: int):
+        return nid < Genome.INPUTS
+
+    @staticmethod
+    def _is_output(nid: int):
+        return Genome.INPUTS <= nid < Genome.INPUTS + Genome.OUTPUTS
+
+    @staticmethod
+    def _is_hidden(nid: int):
+        return Genome.INPUTS + Genome.OUTPUTS <= nid
+
+    @staticmethod
     def __random_node_function(rng: Random):
         return rng.choice(Config.functionSet)
 
     def _add_node(self, func: str) -> int:
         nid = self.nextNodeID + self.INPUTS + self.OUTPUTS
         self.nodes.append(_CPPNData.Node(nid, func))
         self.nextNodeID += 1
@@ -396,34 +495,34 @@
 
     def __random_add_node(self, rng: Random) -> None:
         i = rng.randrange(0, len(self.links))
         link: _CPPNData.Link = self.links[i]
         nid = self._add_node(Genome.__random_node_function(rng))
 
         src, dst, weight = link.src, link.dst, link.weight
-        logger.info(f"[add_n] {src} -> {dst} >> {src} -> {nid} -> {dst}")
+        logger.debug(f"[add_n] {src} -> {dst} >> {src} -> {nid} -> {dst}")
 
         self._add_link(src, nid, 1)
         self._add_link(nid, dst, weight)
         self.links.pop(i)
 
     def __random_del_node(self, rng: Random, candidates) -> None:
         nid = rng.choice(candidates)
-        n_ix, n = next((n_ix, n) for n_ix, n in   # pragma: no branch
+        n_ix, n = next((n_ix, n) for n_ix, n in  # pragma: no branch
                        enumerate(self.nodes) if n.id == nid)
         i_links = [(j, link) for j, link in enumerate(self.links)
                    if link.dst == n.id]
         o_links = [(j, link) for j, link in enumerate(self.links)
                    if link.src == n.id]
         assert len(i_links) == 1 and len(o_links) == 1
 
         j_i, i_l = i_links[0][0], i_links[0][1]
         j_o, o_l = o_links[0][0], o_links[0][1]
-        logger.info(f"[del_n] {i_l.src} -> {n.id} -> {o_l.dst} >>"
-                    f" {i_l.src} -> {o_l.dst}")
+        logger.debug(f"[del_n] {i_l.src} -> {n.id} -> {o_l.dst} >>"
+                     f" {i_l.src} -> {o_l.dst}")
 
         if sum(li.src == i_l.src and li.dst == o_l.dst for li in
                self.links) == 0 \
                 and i_l.src != o_l.dst:
             # Link does not exist already and is not auto-recurrent -> add it
             self._add_link(i_l.src, o_l.dst, o_l.weight)
         self.nodes.pop(n_ix)
@@ -432,39 +531,40 @@
             j_o -= 1
         self.links.pop(j_o)
 
     def __random_add_link(self, rng: Random, candidates) -> None:
         link = rng.choice(list(candidates))
         weight = Genome.__random_link_weight(rng)
 
-        logger.info(f"[add_l] {link.src} -({weight})-> {link.dst}")
+        logger.debug(f"[add_l] {link.src} -({weight})-> {link.dst}")
 
         self._add_link(link.src, link.dst, weight)
 
     def __random_del_link(self, rng: Random, candidates) -> None:
         i = candidates[rng.randrange(0, len(candidates))]
-        logger.info(f"[del_l] {self.links[i].src} -> {self.links[i].dst}")
+        logger.debug(f"[del_l] {self.links[i].src} -> {self.links[i].dst}")
         self.links.pop(i)
 
     def __random_mutate_weight(self, rng: Random) -> None:
         link = rng.choice(self.links)
         bounds = Config.cppnWeightBounds
         delta = 0
         while delta == 0:
             delta = rng.gauss(0, bounds.stddev)
         w = max(bounds.min, min(link.weight + delta, bounds.max))
 
-        logger.info(f"[mut_w] {link.src} -({link.weight})-> {link.dst} >> {w}")
+        logger.debug(f"[mut_w] {link.src} -({link.weight})->"
+                     f" {link.dst} >> {w}")
 
         link.weight = w
 
     def __random_mutate_func(self, rng: Random) -> None:
         n = rng.choice(self.nodes)
         f = rng.choice([f for f in Config.functionSet if not f == n.func])
-        logger.info(f"[mut_f] N({n.id}, {n.func}) -> {f}")
+        logger.debug(f"[mut_f] N({n.id}, {n.func}) -> {f}")
         n.func = f
 
     @staticmethod
     def _compute_node_depths(links_original):
         depths = {}
         links = [l_ for l_ in links_original]
```

### Comparing `abrain-1.0rc0/src/abrain.egg-info/PKG-INFO` & `abrain-1.0rc0.post3/src/abrain.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abrain
-Version: 1.0rc0
+Version: 1.0rc0.post3
 Summary: NeuroEvolution in Python backed by C++ computations
 Author-email: Kevin Godin-Dubois <k.j.m.godin-dubois@vu.nl>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -17,75 +17,64 @@
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: kaleido
 License-File: LICENSE
 
 # Artificial Brains (ABrain) for Python
 
+C++/Python implementation of fully evolvable Artificial Neural Networks.
+Uses the ES-HyperNEAT algorithms to *indirectly* encode ANNs with bio-mimetic
+patterns (repetitions, symmetry...), large number of neurons and relative
+robustness to input/output variations between generations.
+The API is served in Python and computations are performed in C++.
+
 [![Documentation Status](https://readthedocs.org/projects/abrain/badge/?version=latest)](https://abrain.readthedocs.io/en/latest/?badge=latest)
-![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-flake.md)
+![PEP8](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-flake.md)
+[![PyPI version](https://badge.fury.io/py/abrain.svg)](https://badge.fury.io/py/abrain)
+[![Downloads](https://static.pepy.tech/badge/abrain)](https://pepy.tech/project/abrain)
 
-### Release
-![](https://img.shields.io/badge/on-!-900?logo=pypi)
+#### tested on latest
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-manylinux.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-musllinux.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-macosx.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-wheel-win.md)
 
 ### Development
-![](https://img.shields.io/badge/version-!-900)
+![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-version.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-tests.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-cov.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-pcov.md)
 ![](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/wiki/kgd-al/abrain/badge-ccov.md)
 
-
-C++/Python implementation of the genotype/phenotype components of Evolvable Substrate HyperNEAT (read without evolution and speciation).
-
 ## Optional dependencies:
 
 ### Graphviz (dot)
 
-To generate directed graphs for the genomes
-Can only be fetched by system installer (apt-get, yum, ...)
+To generate directed graphs for the genomes.
+Can only be fetched by system installer (apt-get, yum, ...).
 See https://graphviz.org/download/ for instructions
 
 ### Kaleido
 
-To generate non-interactive images of ANN (through plotly)
-Due to inconsistent support, left as an optional dependency
+To generate non-interactive images of ANN (through plotly).
+Due to inconsistent support, left as an optional dependency.
 Use `pip install abrain[...,kaleido]` to get it
 
 ## Todo list:
- - Functionalities:
-   - Order-independent ANN evaluation (with back buffer)?
-   - Crossover / historical markings
-     - Actually needed?
-   - MANN Integration
-     - Easy extraction
-     - built-in testing
-     - C++ wrapper
-     - Visu
+- [ ] Functionalities:
+   - [ ] Order-independent ANN evaluation (with back buffer)?
+   - [ ] Crossover / historical markings
+     - [ ] Actually needed?
+   - [ ] MANN Integration
+     - [ ] Easy extraction
+     - [ ] built-in testing
+     - [ ] C++ wrapper
+     - [ ] Visu
      
-  - Misc:
-    - Documentation
-      - Usage
+  - [ ] Misc:
+    - [ ] Documentation
+      - [ ] Advanced usage
       
-    - Continuous integration
-      - build / tests
-      - Badges
-      
-    - Packaging:
-      - include c++ stubs?
-      - move to scikit/poetry/... ?
-      
-    - Installation errors:
-      - cp38,...,311-manylinux_i686 fail because cppn outputs diverge between manual and subset/all
-        > Caused by unmatched image/host platforms?
-        > Heisenbug, printing an FNode value before returning it makes it work
-        > Also disapears in when compiling in debug mode
-      - pp38,39-manylinux_i686,x86_64; pp38,39-macosx_x86_64; pp38,39-win_amd64 fail because of strange import error in numpy
-        > Solved by removing numpy dependency
-      - cp38,...,311-musllinux_i686 fail because pillow needs a jpeg library
-        > Solved? Added libjpeg to the apk (musllinux) install
-        > Removed pillow dependency
-      - cp38,..,311-win32,amd64 fail because of encoding error in ANN rendering
+      - [ ] move to scikit/poetry/... ?
+
+  - [ ] CI/CD
+    - [ ] Recent install gives `no loadimage plugion for "svg:cairo"` for pdf output
```

### Comparing `abrain-1.0rc0/src/abrain.egg-info/SOURCES.txt` & `abrain-1.0rc0.post3/src/abrain.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -43,8 +43,13 @@
 src/abrain/core/functions/sin.svg
 src/abrain/core/functions/ssgm.png
 src/abrain/core/functions/ssgm.svg
 src/abrain/core/functions/ssgn.png
 src/abrain/core/functions/ssgn.svg
 src/abrain/core/functions/step.png
 src/abrain/core/functions/step.svg
-src/abrain/core/functions/template.tex
+src/abrain/core/functions/template.tex
+tests/test_ann.py
+tests/test_config.py
+tests/test_cppn.py
+tests/test_evolution.py
+tests/test_genome.py
```

