# Comparing `tmp/pylbm-0.8.0.tar.gz` & `tmp/pylbm-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylbm-0.8.0.tar", last modified: Wed Jan 19 16:27:26 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pylbm-0.8.0.tar` & `pylbm-0.9.0.tar`

### file list

```diff
@@ -1,82 +1,68 @@
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.282504 pylbm-0.8.0/
--rw-rw-r--   0 loic      (1001) loic      (1001)     4333 2022-01-19 16:27:26.282504 pylbm-0.8.0/PKG-INFO
--rw-rw-r--   0 loic      (1001) loic      (1001)     2251 2021-04-16 08:42:34.000000 pylbm-0.8.0/README.rst
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.278504 pylbm-0.8.0/pylbm/
--rw-rw-r--   0 loic      (1001) loic      (1001)     1957 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/__init__.py
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.278504 pylbm-0.8.0/pylbm/algorithm/
--rw-rw-r--   0 loic      (1001) loic      (1001)      210 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/algorithm/__init__.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    20483 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/algorithm/base.py
--rw-rw-r--   0 loic      (1001) loic      (1001)      322 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/algorithm/ode.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     1778 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/algorithm/pull.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     2801 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/algorithm/transform.py
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.282504 pylbm-0.8.0/pylbm/analysis/
--rw-rw-r--   0 loic      (1001) loic      (1001)      293 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/analysis/__init__.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     9967 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/analysis/equivalent_equation.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    11012 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/analysis/stability.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    24449 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/boundary.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     2612 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/container.py
--rw-rw-r--   0 loic      (1001) loic      (1001)      502 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/context.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    31179 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/domain.py
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.282504 pylbm-0.8.0/pylbm/elements/
--rw-rw-r--   0 loic      (1001) loic      (1001)      734 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/__init__.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    15977 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/base.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     4581 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/circle.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    17125 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/cylinder.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     5112 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/ellipse.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     5808 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/ellipsoid.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     5688 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/parallelogram.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     4714 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/sphere.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     7997 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/stl_element.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     4876 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/elements/triangle.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     8949 2021-06-12 08:52:25.000000 pylbm-0.8.0/pylbm/elements/utils.py
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.282504 pylbm-0.8.0/pylbm/generator/
--rw-rw-r--   0 loic      (1001) loic      (1001)      158 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/generator/__init__.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    57143 2021-06-11 15:23:51.000000 pylbm-0.8.0/pylbm/generator/ast.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     4723 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/generator/autowrap.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    57520 2021-06-11 15:23:51.000000 pylbm-0.8.0/pylbm/generator/codegen.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     1111 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/generator/generator.py
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.282504 pylbm-0.8.0/pylbm/generator/printing/
--rw-rw-r--   0 loic      (1001) loic      (1001)        0 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/generator/printing/__init__.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    15312 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/generator/printing/cython.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    14638 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/generator/printing/loopy.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    42288 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/generator/printing/pycode.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    11147 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/geometry.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     9119 2021-05-31 11:38:43.000000 pylbm-0.8.0/pylbm/hdf5.py
--rw-rw-r--   0 loic      (1001) loic      (1001)      176 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/jinja_env.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     3370 2022-01-19 16:21:02.000000 pylbm-0.8.0/pylbm/monitoring.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     6327 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/mpi_topology.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     1230 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/options.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    20148 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/scheme.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    12825 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/simulation.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    29021 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/stencil.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    13582 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/storage.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     9209 2022-01-19 16:21:02.000000 pylbm-0.8.0/pylbm/symbolic.py
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.282504 pylbm-0.8.0/pylbm/templates/
--rw-rw-r--   0 loic      (1001) loic      (1001)      161 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/circle.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      199 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/cylinder.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      420 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/domain.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      177 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/ellipse.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      201 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/ellipsoid.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      342 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/equivalent_equation.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      382 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/geometry.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      991 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/scheme.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      141 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/simulation.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      181 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/square.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      483 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/stencil.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)      320 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/stl.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)       53 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/templates/wrap.tpl
--rw-rw-r--   0 loic      (1001) loic      (1001)     5393 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/utils.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    13191 2022-01-19 08:12:10.000000 pylbm-0.8.0/pylbm/validator.py
--rw-rw-r--   0 loic      (1001) loic      (1001)       17 2022-01-19 16:27:26.000000 pylbm-0.8.0/pylbm/version.py
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.282504 pylbm-0.8.0/pylbm/viewer/
--rw-rw-r--   0 loic      (1001) loic      (1001)       59 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/viewer/__init__.py
--rw-rw-r--   0 loic      (1001) loic      (1001)     1099 2021-04-16 08:42:34.000000 pylbm-0.8.0/pylbm/viewer/base.py
--rw-rw-r--   0 loic      (1001) loic      (1001)    18895 2021-04-16 09:06:47.000000 pylbm-0.8.0/pylbm/viewer/matplotlib_viewer.py
-drwxrwxr-x   0 loic      (1001) loic      (1001)        0 2022-01-19 16:27:26.278504 pylbm-0.8.0/pylbm.egg-info/
--rw-rw-r--   0 loic      (1001) loic      (1001)     4333 2022-01-19 16:27:26.000000 pylbm-0.8.0/pylbm.egg-info/PKG-INFO
--rw-rw-r--   0 loic      (1001) loic      (1001)     1743 2022-01-19 16:27:26.000000 pylbm-0.8.0/pylbm.egg-info/SOURCES.txt
--rw-rw-r--   0 loic      (1001) loic      (1001)        1 2022-01-19 16:27:26.000000 pylbm-0.8.0/pylbm.egg-info/dependency_links.txt
--rw-rw-r--   0 loic      (1001) loic      (1001)      128 2022-01-19 16:27:26.000000 pylbm-0.8.0/pylbm.egg-info/requires.txt
--rw-rw-r--   0 loic      (1001) loic      (1001)        6 2022-01-19 16:27:26.000000 pylbm-0.8.0/pylbm.egg-info/top_level.txt
--rw-rw-r--   0 loic      (1001) loic      (1001)       38 2022-01-19 16:27:26.282504 pylbm-0.8.0/setup.cfg
--rw-rw-r--   0 loic      (1001) loic      (1001)     2479 2022-01-19 16:22:19.000000 pylbm-0.8.0/setup.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/__init__.py
+-rw-r--r--   0        0        0    24858 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/boundary.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/container.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/context.py
+-rw-r--r--   0        0        0    31179 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/domain.py
+-rw-r--r--   0        0        0    11147 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/geometry.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/hdf5.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/jinja_env.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/monitoring.py
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/mpi_topology.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/options.py
+-rw-r--r--   0        0        0    20148 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/scheme.py
+-rw-r--r--   0        0        0    12825 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/simulation.py
+-rw-r--r--   0        0        0    29021 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/stencil.py
+-rw-r--r--   0        0        0    13554 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/storage.py
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/symbolic.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/utils.py
+-rw-r--r--   0        0        0    13191 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/validator.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/algorithm/__init__.py
+-rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/algorithm/base.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/algorithm/ode.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/algorithm/pull.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/algorithm/transform.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/analysis/__init__.py
+-rw-r--r--   0        0        0     9967 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/analysis/equivalent_equation.py
+-rw-r--r--   0        0        0    11012 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/analysis/stability.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/__init__.py
+-rw-r--r--   0        0        0    15950 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/base.py
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/circle.py
+-rw-r--r--   0        0        0    17125 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/cylinder.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/ellipse.py
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/ellipsoid.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/parallelogram.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/sphere.py
+-rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/stl_element.py
+-rw-r--r--   0        0        0     4876 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/triangle.py
+-rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/elements/utils.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/__init__.py
+-rw-r--r--   0        0        0    56992 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/ast.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/autowrap.py
+-rw-r--r--   0        0        0    57521 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/codegen.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/printing/__init__.py
+-rw-r--r--   0        0        0    15312 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/printing/cython.py
+-rw-r--r--   0        0        0    14638 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/printing/loopy.py
+-rw-r--r--   0        0        0    42288 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/generator/printing/pycode.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/circle.tpl
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/cylinder.tpl
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/domain.tpl
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/ellipse.tpl
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/ellipsoid.tpl
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/equivalent_equation.tpl
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/geometry.tpl
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/scheme.tpl
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/simulation.tpl
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/square.tpl
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/stencil.tpl
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/stl.tpl
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/templates/wrap.tpl
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/viewer/__init__.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/viewer/base.py
+-rw-r--r--   0        0        0    18868 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/viewer/matplotlib_viewer.py
+-rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 pylbm-0.9.0/pylbm/viewer/vispyViewer.py_tofix
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pylbm-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 pylbm-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 pylbm-0.9.0/README.rst
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 pylbm-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 pylbm-0.9.0/PKG-INFO
```

### Comparing `pylbm-0.8.0/README.rst` & `pylbm-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/__init__.py` & `pylbm-0.9.0/pylbm/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 from colorama import init
 init()
 
 # pylint: disable=wrong-import-position
 # pylint: disable=wildcard-import
 # pylint: disable=invalid-name
 
-from .version import version as __version__  # noqa: E402
+__version__ = "0.9.0"
+
 from .domain import Domain                   # noqa: E402
 from .stencil import Stencil                 # noqa: E402
 from .simulation import Simulation           # noqa: E402
 from . import boundary as bc                 # noqa: E402
 from .scheme import Scheme                   # noqa: E402
 from .elements import *                      # noqa: E402
 from .geometry import Geometry               # noqa: E402
```

### Comparing `pylbm-0.8.0/pylbm/algorithm/base.py` & `pylbm-0.9.0/pylbm/algorithm/base.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/algorithm/pull.py` & `pylbm-0.9.0/pylbm/algorithm/pull.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/algorithm/transform.py` & `pylbm-0.9.0/pylbm/algorithm/transform.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/analysis/equivalent_equation.py` & `pylbm-0.9.0/pylbm/analysis/equivalent_equation.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/analysis/stability.py` & `pylbm-0.9.0/pylbm/analysis/stability.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/boundary.py` & `pylbm-0.9.0/pylbm/boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         num = domain.stencil.unum2index[v.num]
 
         ind = np.where(domain.flag[num] == self.label)
         self.indices = np.array(ind)
         if self.indices.size != 0:
             self.indices += np.asarray(v.v)[:, np.newaxis]
         self.distance = np.array(domain.distance[(num,) + ind])
+        self.normal = np.array(domain.normal[(num,) + ind])  #
 
 class Boundary:
     """
     Construct the boundary problem by defining the list of indices on the border and the methods used on each label.
 
     Parameters
     ----------
@@ -88,14 +89,16 @@
         stencil = self.domain.stencil
 
         istore = collections.OrderedDict() # important to set the boundary conditions always in the same way !!!
         ilabel = {}
         distance = {}
         value_bc = {}
         time_bc = {}
+        normal = {}
+
 
         #pylint: disable=too-many-nested-blocks
         for label in self.domain.list_of_labels():
             if label in [-1, -2]: # periodic or interface conditions
                 continue
 
             value_bc[label] = dico_bound[label].get('value', None)
@@ -104,30 +107,34 @@
             # for each method get the list of points, the labels and the distances
             # where the distribution function must be updated on the boundary
             for k, v in methods.items():
                 for inumk, numk in enumerate(stencil.num[k]):
                     if self.bv_per_label[label][stencil.unum2index[numk]].indices.size != 0:
                         indices = self.bv_per_label[label][stencil.unum2index[numk]].indices
                         distance_tmp = self.bv_per_label[label][stencil.unum2index[numk]].distance
+                        normal_tmp = self.bv_per_label[label][stencil.unum2index[numk]].normal
                         velocity = (inumk + stencil.nv_ptr[k])*np.ones(indices.shape[1], dtype=np.int32)[np.newaxis, :]
                         ilabel_tmp = label*np.ones(indices.shape[1], dtype=np.int32)
                         istore_tmp = np.concatenate([velocity, indices])
                         if istore.get(v, None) is None:
                             istore[v] = istore_tmp.copy()
                             ilabel[v] = ilabel_tmp.copy()
                             distance[v] = distance_tmp.copy()
+                            normal[v] = normal_tmp.copy()
                         else:
                             istore[v] = np.concatenate([istore[v], istore_tmp], axis=1)
                             ilabel[v] = np.concatenate([ilabel[v], ilabel_tmp])
                             distance[v] = np.concatenate([distance[v], distance_tmp])
+                            normal[v] = np.concatenate([normal[v], normal_tmp])  #
 
         # for each method create the instance associated
         self.methods = []
         for k in list(istore.keys()):
-            self.methods.append(k(istore[k], ilabel[k], distance[k], stencil,
+            print(k)
+            self.methods.append(k(istore[k], ilabel[k], distance[k], normal[k], stencil,
                                   value_bc, time_bc, domain.distance.shape, generator))
 
 
 #pylint: disable=protected-access
 class BoundaryMethod:
     """
     Set boundary method.
@@ -150,20 +157,21 @@
         label of the boundary
     iload : list
         indices of points needed to compute the boundary condition
     value_bc : dictionnary
        the prescribed values on the border
 
     """
-    def __init__(self, istore, ilabel, distance, stencil, value_bc, time_bc, nspace, generator):
+    def __init__(self, istore, ilabel, distance, normal, stencil, value_bc, time_bc, nspace, generator):
         self.istore = istore
         self.feq = np.zeros((stencil.nv_ptr[-1], istore.shape[1]))
         self.rhs = np.zeros(istore.shape[1])
         self.ilabel = ilabel
         self.distance = distance
+        self.normal = normal
         self.stencil = stencil
         self.time_bc = {}
         self.value_bc = {}
         for k in np.unique(self.ilabel):
             self.value_bc[k] = value_bc[k]
             self.time_bc[k] = time_bc[k]
         self.iload = []
@@ -409,28 +417,28 @@
 
     Notes
     ------
 
     .. plot:: codes/Bouzidi.py
 
     """
-    def __init__(self, istore, ilabel, distance, stencil, value_bc, time_bc, nspace, generator):
-        super(BouzidiBounceBack, self).__init__(istore, ilabel, distance, stencil, value_bc, time_bc, nspace, generator)
+    def __init__(self, istore, ilabel, distance, normal, stencil, value_bc, time_bc, nspace, generator):
+        super(BouzidiBounceBack, self).__init__(istore, ilabel, distance, normal, stencil, value_bc, time_bc, nspace, generator)
         self.s = np.empty(self.istore.shape[1])
 
     def set_iload(self):
         """
         Compute the indices that are needed (symmertic velocities and space indices).
         """
         k = self.istore[0]
         ksym = self.stencil.get_symmetric()[k]
         v = self.stencil.get_all_velocities()
 
-        iload1 = np.zeros(self.istore.shape, dtype=np.int)
-        iload2 = np.zeros(self.istore.shape, dtype=np.int)
+        iload1 = np.zeros(self.istore.shape, dtype=np.int32)
+        iload2 = np.zeros(self.istore.shape, dtype=np.int32)
 
         mask = self.distance < .5
         iload1[0, mask] = ksym[mask]
         iload2[0, mask] = ksym[mask]
         iload1[1:, mask] = self.istore[1:, mask] + v[k[mask]].T
         iload2[1:, mask] = self.istore[1:, mask] + 2*v[k[mask]].T
         self.s[mask] = 2.*self.distance[mask]
```

### Comparing `pylbm-0.8.0/pylbm/container.py` & `pylbm-0.9.0/pylbm/container.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/domain.py` & `pylbm-0.9.0/pylbm/domain.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/__init__.py` & `pylbm-0.9.0/pylbm/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/base.py` & `pylbm-0.9.0/pylbm/elements/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Base element
 """
 
 # pylint: disable=invalid-name
 
 import logging
 from abc import ABC, abstractmethod
-from six.moves import range
+
 import numpy as np
 
 from .utils import distance_lines, distance_ellipse
 
 __all__ = ['Element', 'BaseCircle', 'BaseEllipse',
            'BaseTriangle', 'BaseParallelogram']
```

### Comparing `pylbm-0.8.0/pylbm/elements/circle.py` & `pylbm-0.9.0/pylbm/elements/circle.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/cylinder.py` & `pylbm-0.9.0/pylbm/elements/cylinder.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/ellipse.py` & `pylbm-0.9.0/pylbm/elements/ellipse.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/ellipsoid.py` & `pylbm-0.9.0/pylbm/elements/ellipsoid.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/parallelogram.py` & `pylbm-0.9.0/pylbm/elements/parallelogram.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/sphere.py` & `pylbm-0.9.0/pylbm/elements/sphere.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/stl_element.py` & `pylbm-0.9.0/pylbm/elements/stl_element.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/triangle.py` & `pylbm-0.9.0/pylbm/elements/triangle.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/elements/utils.py` & `pylbm-0.9.0/pylbm/elements/utils.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/generator/ast.py` & `pylbm-0.9.0/pylbm/generator/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,20 +129,19 @@
 
 from typing import Any, Dict, List
 
 from collections import defaultdict
 
 from sympy import Lt, Le, Ge, Gt
 from sympy.core import Symbol, Tuple, Dummy
-from sympy.core.compatibility import is_sequence
 from sympy.core.basic import Basic
 from sympy.core.expr import Expr
 from sympy.core.numbers import Float, Integer, oo
 from sympy.core.sympify import _sympify, sympify, SympifyError
-from sympy.utilities.iterables import iterable
+from sympy.utilities.iterables import iterable, is_sequence
 
 
 def _mk_Tuple(args):
     """
     Create a Sympy Tuple object from an iterable, converting Python strings to
     AST strings.
 
@@ -855,27 +854,24 @@
     ))
     """
     __slots__ = ('target', 'body')
     # _construct_target = staticmethod(_sympify)
 
     @classmethod
     def _construct_body(cls, itr):
-        from sympy.core.compatibility import is_sequence
-
         if isinstance(itr, CodeBlock):
             return itr
         elif is_sequence(itr):
             return CodeBlock(*itr)
         else:
             return CodeBlock(itr)
 
     @classmethod
     def _construct_target(cls, itr):
         from sympy.tensor import Idx
-        from sympy.core.compatibility import is_sequence
         if isinstance(itr, Idx):
             return Tuple(itr)
         elif is_sequence(itr):
             # return (*itr,)
             return Tuple(*itr)
         else:
             raise TypeError("Loop object requires an Idx or a list of Idx.")
```

### Comparing `pylbm-0.8.0/pylbm/generator/autowrap.py` & `pylbm-0.9.0/pylbm/generator/autowrap.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/generator/codegen.py` & `pylbm-0.9.0/pylbm/generator/codegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 import textwrap
 from io import StringIO
 
 from sympy import __version__ as sympy_version
 from .ast import Assignment, For, If, WithBody
 # from sympy.codegen import Assignment
 from sympy.core import Symbol, S, Tuple, Equality, Function, Basic
-from sympy.core.compatibility import is_sequence
+from sympy.utilities.iterables import is_sequence
 from sympy.tensor import Idx, Indexed, IndexedBase
 from sympy.matrices import (MatrixSymbol, ImmutableMatrix, MatrixBase,
                             MatrixExpr, MatrixSlice)
 
 from .printing.pycode import NumPyPrinter
 from .printing.cython import CythonCodePrinter
 from .printing.loopy import LoopyCodePrinter
```

### Comparing `pylbm-0.8.0/pylbm/generator/generator.py` & `pylbm-0.9.0/pylbm/generator/generator.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/generator/printing/cython.py` & `pylbm-0.9.0/pylbm/generator/printing/cython.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/generator/printing/loopy.py` & `pylbm-0.9.0/pylbm/generator/printing/loopy.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/generator/printing/pycode.py` & `pylbm-0.9.0/pylbm/generator/printing/pycode.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/geometry.py` & `pylbm-0.9.0/pylbm/geometry.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/hdf5.py` & `pylbm-0.9.0/pylbm/hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # License: BSD 3 clause
 
 """
 HDF5 module
 """
 import os
 import logging
-from six.moves import range
 import numpy as np
 import h5py
 import mpi4py.MPI as mpi
 
 log = logging.getLogger(__name__) #pylint: disable=invalid-name
 
 class H5File:
@@ -106,16 +105,16 @@
             comm.Free()
 
         if mpi.COMM_WORLD.Get_rank() == 0:
             for i in range(len(self.region)):
                 self.region[i].insert(0, 0)
                 for j in range(1, len(self.region[i])):
                     self.region[i][j] += self.region[i][j-1]
-            #self.region = np.asarray(self.region, dtype=np.int)
-            #self.region = np.concatenate((np.zeros((self.dim, 1), dtype=np.int), np.cumsum(self.region, axis=1)), axis=1)
+            #self.region = np.asarray(self.region, dtype=np.int32)
+            #self.region = np.concatenate((np.zeros((self.dim, 1), dtype=np.int32), np.cumsum(self.region, axis=1)), axis=1)
             #print(self.region)
             for i in range(self.dim):
                 dset = self.h5file.create_dataset("x_{}".format(i), [self.global_size[i]], dtype=np.double)
                 dset[:] = np.concatenate(coords[i])
 
     def _get_slice(self, rank):
         """
@@ -239,15 +238,15 @@
         comm = self.mpi_topo.cartcomm
         if comm.Get_rank() == 0:
             self.h5file.close()
             self.xdmf_file = open(self.path + '/' + self.filename + '.xdmf', "w")
             self.xdmf_file.write("""<?xml version="1.0" ?>
 <!DOCTYPE Xdmf SYSTEM "Xdmf.dtd" []>
 <Xdmf>
- <Domain>           
+ <Domain>
             """)
             if self.dim == 2:
                 self.xdmf_file.write("""
                 <Grid Name="Structured Grid" GridType="Uniform">
                     <Topology TopologyType="2DRectMesh" NumberOfElements="{0}"/>
                     <Geometry GeometryType="VXVY">
                 """.format(' '.join(map(str, self.global_size))))
@@ -256,33 +255,33 @@
                 <Grid Name="Structured Grid" GridType="Uniform">
                     <Topology TopologyType="3DRectMesh" NumberOfElements="{0}"/>
                     <Geometry GeometryType="VXVYVZ">
                 """.format(' '.join(map(str, self.global_size))))
             for i in range(self.dim):
                 self.xdmf_file.write("""
                 <DataItem Format="HDF" Dimensions="{0}">
-                    {1}:/x_{2} 
+                    {1}:/x_{2}
                 </DataItem>
                 """.format(self.global_size[i], self.filename + '.h5', i))
 
             self.xdmf_file.write("</Geometry>\n")
 
             for k, v in self.scalars.items():
                 self.xdmf_file.write("""
                 <Attribute Name="{0}" AttributeType="Scalar" Center="Node">
                 <DataItem Format="HDF" Dimensions="{1}">
-                {2} 
+                {2}
                 </DataItem>
                 </Attribute>
                 """.format(k, ' '.join(map(str, self.global_size[::-1])), v))
 
             for k, v in self.vectors.items():
                 self.xdmf_file.write("""
                 <Attribute Name="{0}" AttributeType="Vector" Center="Node">
                 <DataItem Format="HDF" Dimensions="{1} {2}">
-                {3} 
+                {3}
                 </DataItem>
                 </Attribute>
                 """.format(k, ' '.join(map(str, self.global_size[::-1])), self.dim, v))
 
             self.xdmf_file.write("</Grid>\n</Domain>\n</Xdmf>\n")
             self.xdmf_file.close()
```

### Comparing `pylbm-0.8.0/pylbm/monitoring.py` & `pylbm-0.9.0/pylbm/monitoring.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/mpi_topology.py` & `pylbm-0.9.0/pylbm/mpi_topology.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/options.py` & `pylbm-0.9.0/pylbm/options.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/scheme.py` & `pylbm-0.9.0/pylbm/scheme.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/simulation.py` & `pylbm-0.9.0/pylbm/simulation.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/stencil.py` & `pylbm-0.9.0/pylbm/stencil.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/storage.py` & `pylbm-0.9.0/pylbm/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 """
 Storage module
 """
 
 import copy
 import logging
-from six.moves import range
 
 import numpy as np
 import sympy as sp
 import mpi4py.MPI as mpi
 
 from .generator import For
 from .monitoring import monitor
```

### Comparing `pylbm-0.8.0/pylbm/symbolic.py` & `pylbm-0.9.0/pylbm/symbolic.py`

 * *Files 15% similar despite different names*

```diff
@@ -254,52 +254,18 @@
         new_expr = expr.subs(replace)
         if new_expr == expr:
             return new_expr
         else:
             expr = new_expr
     return new_expr
 
-def getargspec_permissive(func):
-    """
-    find in https://github.com/neithere/argh/blob/master/argh/compat.py
-
-    An `inspect.getargspec` with a relaxed sanity check to support Cython.
-    Motivation:
-        A Cython-compiled function is *not* an instance of Python's
-        types.FunctionType.  That is the sanity check the standard Py2
-        library uses in `inspect.getargspec()`.  So, an exception is raised
-        when calling `argh.dispatch_command(cythonCompiledFunc)`.  However,
-        the CyFunctions do have perfectly usable `.func_code` and
-        `.func_defaults` which is all `inspect.getargspec` needs.
-        This function just copies `inspect.getargspec()` from the standard
-        library but relaxes the test to a more duck-typing one of having
-        both `.func_code` and `.func_defaults` attributes.
-    """
-    if inspect.ismethod(func):
-        func = func.im_func
-
-    # Py2 Stdlib uses isfunction(func) which is too strict for Cython-compiled
-    # functions though such have perfectly usable func_code, func_defaults.
-    if not (hasattr(func, "func_code") and hasattr(func, "func_defaults")):
-        raise TypeError('{!r} missing func_code or func_defaults'.format(func))
-
-    args, varargs, varkw = inspect.getargs(func.func_code)
-    return inspect.ArgSpec(args, varargs, varkw, func.func_defaults)
-
-PY3 = sys.version_info >= (3,)
-
-if PY3:
-    from inspect import getfullargspec as getargspec
-else:
-    getargspec = getargspec_permissive #pylint: disable=invalid-name
-
 def call_genfunction(function, args):
     from .monitoring import monitor
     from .context import queue
     try:
         func_args = function.arg_dict.keys()
         d = {k:args[k] for k in func_args} #pylint: disable=invalid-name
         d['queue'] = queue
     except: #pylint: disable=bare-except
-        func_args = getargspec(function).args
+        func_args = inspect.getfullargspec(function).args
         d = {k:args[k] for k in func_args} #pylint: disable=invalid-name
     monitor(function)(**d)
```

### Comparing `pylbm-0.8.0/pylbm/templates/scheme.tpl` & `pylbm-0.9.0/pylbm/templates/scheme.tpl`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/utils.py` & `pylbm-0.9.0/pylbm/utils.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/validator.py` & `pylbm-0.9.0/pylbm/validator.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/viewer/base.py` & `pylbm-0.9.0/pylbm/viewer/base.py`

 * *Files identical despite different names*

### Comparing `pylbm-0.8.0/pylbm/viewer/matplotlib_viewer.py` & `pylbm-0.9.0/pylbm/viewer/matplotlib_viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # License: BSD 3 clause
 # FIXME: write the documentation
 
 # pylint: disable=missing-docstring
 
 import logging
-from six.moves import range
+
 
 import matplotlib.pyplot as plt
 from matplotlib.patches import Ellipse, Polygon
 from matplotlib import animation
 from mpl_toolkits.mplot3d import Axes3D  # pylint: disable=unused-import
 
 import numpy as np
```

