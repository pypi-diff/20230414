# Comparing `tmp/hdmf-3.5.4.tar.gz` & `tmp/hdmf-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdmf-3.5.4.tar", last modified: Fri Apr  7 20:40:59 2023, max compression
+gzip compressed data, was "hdmf-3.5.5.tar", last modified: Thu Apr 13 23:52:54 2023, max compression
```

## Comparing `hdmf-3.5.4.tar` & `hdmf-3.5.5.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.680945 hdmf-3.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-07 20:39:25.000000 hdmf-3.5.4/Legal.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-07 20:39:25.000000 hdmf-3.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-07 20:40:59.680945 hdmf-3.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-07 20:39:25.000000 hdmf-3.5.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-07 20:39:25.000000 hdmf-3.5.4/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-07 20:39:25.000000 hdmf-3.5.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-07 20:39:25.000000 hdmf-3.5.4/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-07 20:39:25.000000 hdmf-3.5.4/requirements-min.txt
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-07 20:39:25.000000 hdmf-3.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-07 20:40:59.680945 hdmf-3.5.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2377 2023-04-07 20:39:25.000000 hdmf-3.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.660944 hdmf-3.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.680945 hdmf-3.5.4/src/hdmf/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/_due.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-07 20:40:59.680945 hdmf-3.5.4/src/hdmf/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.664944 hdmf-3.5.4/src/hdmf/backends/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/backends/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/hdf5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/hdf5/h5_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    72886 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/hdf5/h5tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/backends/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/build/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/classgenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    65654 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/objectmapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/build/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/common/
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/alignedtable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.660944 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/experimental.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/sparse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-07 20:39:26.000000 hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/hierarchicaltable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.668944 hdmf-3.5.4/src/hdmf/common/io/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/alignedtable.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/io/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    73532 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/common/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    47444 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    49701 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/src/hdmf/spec/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    24617 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)    60591 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/spec/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/src/hdmf/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/testing/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/testing/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1794 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/testing/validate_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    48832 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/src/hdmf/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/validate/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-04-07 20:39:25.000000 hdmf-3.5.4/src/hdmf/validate/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.664944 hdmf-3.5.4/src/hdmf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 20:39:53.000000 hdmf-3.5.4/src/hdmf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-07 20:40:59.000000 hdmf-3.5.4/src/hdmf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     5107 2023-04-07 20:39:25.000000 hdmf-3.5.4/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/unit/back_compat_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/back_compat_tests/1.0.5.h5
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/back_compat_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/back_compat_tests/test_1_1_0.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/unit/build_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.672944 hdmf-3.5.4/tests/unit/build_tests/mapper_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/mapper_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23395 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/mapper_tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    46424 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/mapper_tests/test_build_quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    48994 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_classgenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25679 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_convert_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_io_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_io_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/build_tests/test_io_map_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.676944 hdmf-3.5.4/tests/unit/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33128 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_alignedtable.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_common_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_generate_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_linkedtables.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)    36063 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)   110730 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/common/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.676944 hdmf-3.5.4/tests/unit/spec_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test-ext.base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test-ext.namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test.base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test.namespace.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_attribute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_dataset_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_dtype_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    32100 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_group_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_link_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_load_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_ref_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_spec_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/spec_tests/test_spec_write.py
--rw-r--r--   0 runner    (1001) docker     (123)    24297 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_io_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)   147101 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_io_hdf5_h5tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_multicontainerinterface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    21544 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.676944 hdmf-3.5.4/tests/unit/utils_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_DataChunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_DataChunkIterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_DataIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_GenericDataChunkIterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_core_ShapeValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)    49444 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_docval.py
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_labelleddict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/utils_test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 20:40:59.676944 hdmf-3.5.4/tests/unit/validator_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/validator_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/validator_tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    52983 2023-04-07 20:39:25.000000 hdmf-3.5.4/tests/unit/validator_tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-07 20:39:25.000000 hdmf-3.5.4/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-07 20:39:25.000000 hdmf-3.5.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.195384 hdmf-3.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-13 23:51:23.000000 hdmf-3.5.5/Legal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-13 23:51:23.000000 hdmf-3.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-13 23:52:54.195384 hdmf-3.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-04-13 23:51:23.000000 hdmf-3.5.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-13 23:51:23.000000 hdmf-3.5.5/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-13 23:51:23.000000 hdmf-3.5.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 23:51:23.000000 hdmf-3.5.5/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-13 23:51:23.000000 hdmf-3.5.5/requirements-min.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-13 23:51:23.000000 hdmf-3.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 23:52:54.195384 hdmf-3.5.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2377 2023-04-13 23:51:23.000000 hdmf-3.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.175384 hdmf-3.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.195384 hdmf-3.5.5/src/hdmf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/_due.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-13 23:52:54.195384 hdmf-3.5.5/src/hdmf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.183384 hdmf-3.5.5/src/hdmf/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/backends/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.183384 hdmf-3.5.5/src/hdmf/backends/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/backends/hdf5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/backends/hdf5/h5_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73154 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/backends/hdf5/h5tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/backends/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/backends/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/backends/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.183384 hdmf-3.5.5/src/hdmf/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/build/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20770 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/build/classgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/build/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39707 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/build/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/build/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65654 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/build/objectmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/build/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.183384 hdmf-3.5.5/src/hdmf/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/alignedtable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.175384 hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.183384 hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-13 23:51:24.000000 hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-13 23:51:24.000000 hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/experimental.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-13 23:51:24.000000 hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-13 23:51:24.000000 hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-13 23:51:24.000000 hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/sparse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-13 23:51:24.000000 hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/hierarchicaltable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.183384 hdmf-3.5.5/src/hdmf/common/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/io/alignedtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/io/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/io/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/io/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73532 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/common/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47444 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49701 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.187384 hdmf-3.5.5/src/hdmf/spec/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/spec/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24617 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/spec/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60591 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/spec/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/spec/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.187384 hdmf-3.5.5/src/hdmf/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/testing/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/testing/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1794 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/testing/validate_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48832 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.187384 hdmf-3.5.5/src/hdmf/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/validate/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28044 2023-04-13 23:51:23.000000 hdmf-3.5.5/src/hdmf/validate/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.179384 hdmf-3.5.5/src/hdmf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-04-13 23:52:54.000000 hdmf-3.5.5/src/hdmf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-13 23:52:54.000000 hdmf-3.5.5/src/hdmf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:52:54.000000 hdmf-3.5.5/src/hdmf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 23:52:54.000000 hdmf-3.5.5/src/hdmf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:51:49.000000 hdmf-3.5.5/src/hdmf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-13 23:52:54.000000 hdmf-3.5.5/src/hdmf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 23:52:54.000000 hdmf-3.5.5/src/hdmf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5107 2023-04-13 23:51:23.000000 hdmf-3.5.5/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.187384 hdmf-3.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.187384 hdmf-3.5.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.187384 hdmf-3.5.5/tests/unit/back_compat_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/back_compat_tests/1.0.5.h5
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/back_compat_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/back_compat_tests/test_1_1_0.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.187384 hdmf-3.5.5/tests/unit/build_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.191384 hdmf-3.5.5/tests/unit/build_tests/mapper_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/mapper_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23395 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/mapper_tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46424 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/mapper_tests/test_build_quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48994 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/test_classgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25679 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/test_convert_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14805 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/test_io_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/test_io_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/build_tests/test_io_map_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.191384 hdmf-3.5.5/tests/unit/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33128 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_alignedtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_common_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_generate_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48786 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_linkedtables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36063 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110730 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/common/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.191384 hdmf-3.5.5/tests/unit/spec_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test-ext.base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test-ext.namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test.base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test.namespace.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_attribute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11458 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_dataset_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_dtype_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32100 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_group_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_link_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_load_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_ref_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_spec_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/spec_tests/test_spec_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24297 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/test_io_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160105 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/test_io_hdf5_h5tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19807 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/test_multicontainerinterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21544 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.191384 hdmf-3.5.5/tests/unit/utils_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/test_core_DataChunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/test_core_DataChunkIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/test_core_DataIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/test_core_GenericDataChunkIterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/test_core_ShapeValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49444 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/test_docval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/test_labelleddict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/utils_test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:52:54.195384 hdmf-3.5.5/tests/unit/validator_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/validator_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/validator_tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52983 2023-04-13 23:51:23.000000 hdmf-3.5.5/tests/unit/validator_tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-04-13 23:51:23.000000 hdmf-3.5.5/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-13 23:51:23.000000 hdmf-3.5.5/versioneer.py
```

### Comparing `hdmf-3.5.4/Legal.txt` & `hdmf-3.5.5/Legal.txt`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/PKG-INFO` & `hdmf-3.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdmf
-Version: 3.5.4
+Version: 3.5.5
 Summary: A package for standardizing hierarchical object data
 Home-page: https://github.com/hdmf-dev/hdmf
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research
 Classifier: Programming Language :: Python
```

### Comparing `hdmf-3.5.4/README.rst` & `hdmf-3.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/license.txt` & `hdmf-3.5.5/license.txt`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/requirements-min.txt` & `hdmf-3.5.5/requirements-min.txt`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/requirements.txt` & `hdmf-3.5.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/setup.cfg` & `hdmf-3.5.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/setup.py` & `hdmf-3.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/__init__.py` & `hdmf-3.5.5/src/hdmf/__init__.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/_due.py` & `hdmf-3.5.5/src/hdmf/_due.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/array.py` & `hdmf-3.5.5/src/hdmf/array.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/backends/hdf5/h5_utils.py` & `hdmf-3.5.5/src/hdmf/backends/hdf5/h5_utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/backends/hdf5/h5tools.py` & `hdmf-3.5.5/src/hdmf/backends/hdf5/h5tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,14 +387,16 @@
          'doc': ('the Container object to export. If None, then the entire contents of the HDMFIO object will be '
                  'exported'),
          'default': None},
         {'name': 'write_args', 'type': dict, 'doc': 'arguments to pass to :py:meth:`write_builder`',
          'default': None},
         {'name': 'cache_spec', 'type': bool, 'doc': 'whether to cache the specification to file',
          'default': True}
+        # clear_cache is an arg on HDMFIO.export but it is intended for internal usage
+        # so it is not available on HDF5IO
     )
 
     @docval(*_export_args)
     def export(self, **kwargs):
         """Export data read from a file from any backend to HDF5.
 
         See :py:meth:`hdmf.backends.io.HDMFIO.export` for more details.
@@ -408,17 +410,19 @@
         if write_args is None:
             write_args = dict()
 
         if not isinstance(src_io, HDF5IO) and write_args.get('link_data', True):
             raise UnsupportedOperation("Cannot export from non-HDF5 backend %s to HDF5 with write argument "
                                        "link_data=True." % src_io.__class__.__name__)
 
-        write_args['export_source'] = src_io.source  # pass export_source=src_io.source to write_builder
+        write_args['export_source'] = os.path.abspath(src_io.source) if src_io.source is not None else None
         ckwargs = kwargs.copy()
         ckwargs['write_args'] = write_args
+        if not write_args.get('link_data', True):
+            ckwargs['clear_cache'] = True
         super().export(**ckwargs)
         if cache_spec:
             self.__cache_spec()
 
     @classmethod
     @docval({'name': 'path', 'type': str, 'doc': 'the path to the destination HDF5 file'},
             {'name': 'comm', 'type': 'Intracomm', 'doc': 'the MPI communicator to use for parallel I/O',
@@ -572,30 +576,30 @@
             name = str(os.path.basename(h5obj.name))
         for k in h5obj:
             sub_h5obj = h5obj.get(k)
             if not (sub_h5obj is None):
                 if sub_h5obj.name in ignore:
                     continue
                 link_type = h5obj.get(k, getlink=True)
-                if isinstance(link_type, SoftLink) or isinstance(link_type, ExternalLink):
+                if isinstance(link_type, (SoftLink, ExternalLink)):
                     # Reading links might be better suited in its own function
                     # get path of link (the key used for tracking what's been built)
                     target_path = link_type.path
                     target_obj = sub_h5obj.file[target_path]
                     builder_name = os.path.basename(target_path)
                     # get builder if already read, else build it
                     builder = self.__get_built(sub_h5obj.file.filename, target_obj.id)
                     if builder is None:
                         # NOTE: all links must have absolute paths
                         if isinstance(target_obj, Dataset):
                             builder = self.__read_dataset(target_obj, builder_name)
                         else:
                             builder = self.__read_group(target_obj, builder_name, ignore=ignore)
                         self.__set_built(sub_h5obj.file.filename,  target_obj.id, builder)
-                    link_builder = LinkBuilder(builder=builder, name=k, source=h5obj.file.filename)
+                    link_builder = LinkBuilder(builder=builder, name=k, source=os.path.abspath(h5obj.file.filename))
                     link_builder.location = h5obj.name
                     self.__set_written(link_builder)
                     kwargs['links'][builder_name] = link_builder
                     if isinstance(link_type, ExternalLink):
                         self.__open_links.append(sub_h5obj)
                 else:
                     builder = self.__get_built(sub_h5obj.file.filename, sub_h5obj.id)
@@ -611,15 +615,15 @@
                         builder = read_method(sub_h5obj)
                         self.__set_built(sub_h5obj.file.filename, sub_h5obj.id, builder)
                     obj_type[builder.name] = builder
             else:
                 warnings.warn('Path to Group altered/broken at ' + os.path.join(h5obj.name, k), BrokenLinkWarning)
                 kwargs['datasets'][k] = None
                 continue
-        kwargs['source'] = h5obj.file.filename
+        kwargs['source'] = os.path.abspath(h5obj.file.filename)
         ret = GroupBuilder(name, **kwargs)
         ret.location = os.path.dirname(h5obj.name)
         self.__set_written(ret)
         return ret
 
     def __read_dataset(self, h5obj, name=None):
         kwargs = {
@@ -629,15 +633,15 @@
         }
         for key, val in kwargs['attributes'].items():
             if isinstance(val, bytes):
                 kwargs['attributes'][key] = val.decode('UTF-8')
 
         if name is None:
             name = str(os.path.basename(h5obj.name))
-        kwargs['source'] = h5obj.file.filename
+        kwargs['source'] = os.path.abspath(h5obj.file.filename)
         ndims = len(h5obj.shape)
         if ndims == 0:                                       # read scalar
             scalar = h5obj[()]
             if isinstance(scalar, bytes):
                 scalar = scalar.decode('UTF-8')
 
             if isinstance(scalar, Reference):
@@ -1017,21 +1021,21 @@
         path = self.__get_path(target_builder)
         # source will indicate target_builder's location
         if export_source is None:
             write_source = builder.source
         else:
             write_source = export_source
 
-        if write_source == target_builder.source:
+        parent_filename = os.path.abspath(parent.file.filename)
+        if target_builder.source in (write_source, parent_filename):
             link_obj = SoftLink(path)
             self.logger.debug("    Creating SoftLink '%s/%s' to '%s'"
                               % (parent.name, name, link_obj.path))
         elif target_builder.source is not None:
             target_filename = os.path.abspath(target_builder.source)
-            parent_filename = os.path.abspath(parent.file.filename)
             relative_path = os.path.relpath(target_filename, os.path.dirname(parent_filename))
             if target_builder.location is not None:
                 path = target_builder.location + "/" + target_builder.name
             link_obj = ExternalLink(relative_path, path)
             self.logger.debug("    Creating ExternalLink '%s/%s' to '%s://%s'"
                               % (parent.name, name, link_obj.filename, link_obj.path))
         else:
```

### Comparing `hdmf-3.5.4/src/hdmf/backends/io.py` & `hdmf-3.5.5/src/hdmf/backends/io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABCMeta, abstractmethod
+import os
 from pathlib import Path
 
 from ..build import BuildManager, GroupBuilder
 from ..container import Container
 from .errors import UnsupportedOperation
 from ..utils import docval, getargs, popargs
 
@@ -11,15 +12,17 @@
     @docval({'name': 'manager', 'type': BuildManager,
              'doc': 'the BuildManager to use for I/O', 'default': None},
             {"name": "source", "type": (str, Path),
              "doc": "the source of container being built i.e. file path", 'default': None})
     def __init__(self, **kwargs):
         manager, source = getargs('manager', 'source', kwargs)
         if isinstance(source, Path):
-            source = str(source)
+            source = source.resolve()
+        elif isinstance(source, str):
+            source = os.path.abspath(source)
 
         self.__manager = manager
         self.__built = dict()
         self.__source = source
         self.open()
 
     @property
@@ -52,15 +55,17 @@
 
     @docval({'name': 'src_io', 'type': 'HDMFIO', 'doc': 'the HDMFIO object for reading the data to export'},
             {'name': 'container', 'type': Container,
              'doc': ('the Container object to export. If None, then the entire contents of the HDMFIO object will be '
                      'exported'),
              'default': None},
             {'name': 'write_args', 'type': dict, 'doc': 'arguments to pass to :py:meth:`write_builder`',
-             'default': dict()})
+             'default': dict()},
+            {'name': 'clear_cache', 'type': bool, 'doc': 'whether to clear the build manager cache',
+             'default': False})
     def export(self, **kwargs):
         """Export from one backend to the backend represented by this class.
 
         If `container` is provided, then the build manager of `src_io` is used to build the container, and the resulting
         builder will be exported to the new backend. So if `container` is provided, `src_io` must have a non-None
         manager property. If `container` is None, then the contents of `src_io` will be read and exported to the new
         backend.
@@ -80,29 +85,39 @@
                 new_io.export(old_io)
 
         NOTE: When implementing export support on custom backends. Export does not update the Builder.source
               on the Builders. As such, when writing LinkBuilders we need to determine if LinkBuilder.source
               and LinkBuilder.builder.source are the same, and if so the link should be internal to the
               current file (even if the Builder.source points to a different location).
         """
-        src_io, container, write_args = getargs('src_io', 'container', 'write_args', kwargs)
+        src_io, container, write_args, clear_cache = getargs('src_io', 'container', 'write_args', 'clear_cache', kwargs)
+        if container is None and clear_cache:
+            # clear all containers and builders from cache so that they can all get rebuilt with export=True.
+            # constructing the container is not efficient but there is no elegant way to trigger a
+            # rebuild of src_io with new source.
+            container = src_io.read()
         if container is not None:
             # check that manager exists, container was built from manager, and container is root of hierarchy
             if src_io.manager is None:
                 raise ValueError('When a container is provided, src_io must have a non-None manager (BuildManager) '
                                  'property.')
             old_bldr = src_io.manager.get_builder(container)
             if old_bldr is None:
                 raise ValueError('The provided container must have been read by the provided src_io.')
             if old_bldr.parent is not None:
                 raise ValueError('The provided container must be the root of the hierarchy of the '
                                  'source used to read the container.')
 
-            # build any modified containers
-            src_io.manager.purge_outdated()
+            # NOTE in HDF5IO, clear_cache is set to True when link_data is False
+            if clear_cache:
+                # clear all containers and builders from cache so that they can all get rebuilt with export=True
+                src_io.manager.clear_cache()
+            else:
+                # clear only cached containers and builders where the container was modified
+                src_io.manager.purge_outdated()
             bldr = src_io.manager.build(container, source=self.__source, root=True, export=True)
         else:
             bldr = src_io.read_builder()
         self.write_builder(builder=bldr, **write_args)
 
     @abstractmethod
     @docval(returns='a GroupBuilder representing the read data', rtype='GroupBuilder')
```

### Comparing `hdmf-3.5.4/src/hdmf/backends/utils.py` & `hdmf-3.5.5/src/hdmf/backends/utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/build/__init__.py` & `hdmf-3.5.5/src/hdmf/build/__init__.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/build/builders.py` & `hdmf-3.5.5/src/hdmf/build/builders.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/build/classgenerator.py` & `hdmf-3.5.5/src/hdmf/build/classgenerator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/build/errors.py` & `hdmf-3.5.5/src/hdmf/build/errors.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/build/manager.py` & `hdmf-3.5.5/src/hdmf/build/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,18 @@
                 builder_id = self.__bldrhash__(builder)
                 self.logger.debug("Purging %s '%s' for %s '%s' from prebuilt cache"
                                   % (builder.__class__.__name__, builder.name,
                                      container.__class__.__name__, container.name))
                 self.__builders.pop(container_id)
                 self.__containers.pop(builder_id)
 
+    def clear_cache(self):
+        self.__builders.clear()
+        self.__containers.clear()
+
     @docval({"name": "container", "type": AbstractContainer, "doc": "the container to get the builder for"})
     def get_builder(self, **kwargs):
         """Return the prebuilt builder for the given container or None if it does not exist."""
         container = getargs('container', kwargs)
         container_id = self.__conthash__(container)
         result = self.__builders.get(container_id)
         return result
```

### Comparing `hdmf-3.5.4/src/hdmf/build/objectmapper.py` & `hdmf-3.5.5/src/hdmf/build/objectmapper.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/build/warnings.py` & `hdmf-3.5.5/src/hdmf/build/warnings.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/__init__.py` & `hdmf-3.5.5/src/hdmf/common/__init__.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/alignedtable.py` & `hdmf-3.5.5/src/hdmf/common/alignedtable.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/base.yaml` & `hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/base.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/namespace.yaml` & `hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/namespace.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/resources.yaml` & `hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/resources.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/sparse.yaml` & `hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/sparse.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/hdmf-common-schema/common/table.yaml` & `hdmf-3.5.5/src/hdmf/common/hdmf-common-schema/common/table.yaml`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/hierarchicaltable.py` & `hdmf-3.5.5/src/hdmf/common/hierarchicaltable.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/io/alignedtable.py` & `hdmf-3.5.5/src/hdmf/common/io/alignedtable.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/io/multi.py` & `hdmf-3.5.5/src/hdmf/common/io/multi.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/io/resources.py` & `hdmf-3.5.5/src/hdmf/common/io/resources.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/io/table.py` & `hdmf-3.5.5/src/hdmf/common/io/table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/multi.py` & `hdmf-3.5.5/src/hdmf/common/multi.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/resources.py` & `hdmf-3.5.5/src/hdmf/common/resources.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/sparse.py` & `hdmf-3.5.5/src/hdmf/common/sparse.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/common/table.py` & `hdmf-3.5.5/src/hdmf/common/table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/container.py` & `hdmf-3.5.5/src/hdmf/container.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/data_utils.py` & `hdmf-3.5.5/src/hdmf/data_utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/monitor.py` & `hdmf-3.5.5/src/hdmf/monitor.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/query.py` & `hdmf-3.5.5/src/hdmf/query.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/region.py` & `hdmf-3.5.5/src/hdmf/region.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/spec/catalog.py` & `hdmf-3.5.5/src/hdmf/spec/catalog.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/spec/namespace.py` & `hdmf-3.5.5/src/hdmf/spec/namespace.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/spec/spec.py` & `hdmf-3.5.5/src/hdmf/spec/spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/spec/write.py` & `hdmf-3.5.5/src/hdmf/spec/write.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/testing/testcase.py` & `hdmf-3.5.5/src/hdmf/testing/testcase.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/testing/validate_spec.py` & `hdmf-3.5.5/src/hdmf/testing/validate_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/utils.py` & `hdmf-3.5.5/src/hdmf/utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/validate/errors.py` & `hdmf-3.5.5/src/hdmf/validate/errors.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf/validate/validator.py` & `hdmf-3.5.5/src/hdmf/validate/validator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/src/hdmf.egg-info/PKG-INFO` & `hdmf-3.5.5/src/hdmf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdmf
-Version: 3.5.4
+Version: 3.5.5
 Summary: A package for standardizing hierarchical object data
 Home-page: https://github.com/hdmf-dev/hdmf
 Author: Andrew Tritt
 Author-email: ajtritt@lbl.gov
 License: BSD
 Keywords: python HDF HDF5 cross-platform open-data data-format open-source open-science reproducible-research
 Classifier: Programming Language :: Python
```

### Comparing `hdmf-3.5.4/src/hdmf.egg-info/SOURCES.txt` & `hdmf-3.5.5/src/hdmf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/test.py` & `hdmf-3.5.5/test.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/back_compat_tests/1.0.5.h5` & `hdmf-3.5.5/tests/unit/back_compat_tests/1.0.5.h5`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/back_compat_tests/test_1_1_0.py` & `hdmf-3.5.5/tests/unit/back_compat_tests/test_1_1_0.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/build_tests/mapper_tests/test_build.py` & `hdmf-3.5.5/tests/unit/build_tests/mapper_tests/test_build.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/build_tests/mapper_tests/test_build_quantity.py` & `hdmf-3.5.5/tests/unit/build_tests/mapper_tests/test_build_quantity.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/build_tests/test_builder.py` & `hdmf-3.5.5/tests/unit/build_tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/build_tests/test_classgenerator.py` & `hdmf-3.5.5/tests/unit/build_tests/test_classgenerator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/build_tests/test_convert_dtype.py` & `hdmf-3.5.5/tests/unit/build_tests/test_convert_dtype.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/build_tests/test_io_manager.py` & `hdmf-3.5.5/tests/unit/build_tests/test_io_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,14 +113,33 @@
                 attributes={'attr2': 10})},
             attributes={'attr1': 'value1', 'namespace': CORE_NAMESPACE, 'data_type': 'Foo',
                         'object_id': -1})
         container1 = self.manager.construct(builder)
         container2 = self.manager.construct(builder)
         self.assertIs(container1, container2)
 
+    def test_clear_cache(self):
+        container_inst = Foo('my_foo', list(range(10)), 'value1', 10)
+        builder1 = self.manager.build(container_inst)
+        self.manager.clear_cache()
+        builder2 = self.manager.build(container_inst)
+        self.assertIsNot(builder1, builder2)
+
+        builder = GroupBuilder(
+            'my_foo', datasets={'my_data': DatasetBuilder(
+                'my_data',
+                list(range(10)),
+                attributes={'attr2': 10})},
+            attributes={'attr1': 'value1', 'namespace': CORE_NAMESPACE, 'data_type': 'Foo',
+                        'object_id': -1})
+        container1 = self.manager.construct(builder)
+        self.manager.clear_cache()
+        container2 = self.manager.construct(builder)
+        self.assertIsNot(container1, container2)
+
 
 class NestedBaseMixin(metaclass=ABCMeta):
 
     def setUp(self):
         super().setUp()
         self.foo_bucket = FooBucket('test_foo_bucket', [
                             Foo('my_foo1', list(range(10)), 'value1', 10),
```

### Comparing `hdmf-3.5.4/tests/unit/build_tests/test_io_map.py` & `hdmf-3.5.5/tests/unit/build_tests/test_io_map.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/build_tests/test_io_map_data.py` & `hdmf-3.5.5/tests/unit/build_tests/test_io_map_data.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/common/test_alignedtable.py` & `hdmf-3.5.5/tests/unit/common/test_alignedtable.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/common/test_common_io.py` & `hdmf-3.5.5/tests/unit/common/test_common_io.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/common/test_generate_table.py` & `hdmf-3.5.5/tests/unit/common/test_generate_table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/common/test_linkedtables.py` & `hdmf-3.5.5/tests/unit/common/test_linkedtables.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/common/test_multi.py` & `hdmf-3.5.5/tests/unit/common/test_multi.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/common/test_resources.py` & `hdmf-3.5.5/tests/unit/common/test_resources.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/common/test_sparse.py` & `hdmf-3.5.5/tests/unit/common/test_sparse.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/common/test_table.py` & `hdmf-3.5.5/tests/unit/common/test_table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_attribute_spec.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_attribute_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_dataset_spec.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_dataset_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_dtype_spec.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_dtype_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_group_spec.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_group_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_link_spec.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_link_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_load_namespace.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_load_namespace.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_ref_spec.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_ref_spec.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_spec_catalog.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_spec_catalog.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/spec_tests/test_spec_write.py` & `hdmf-3.5.5/tests/unit/spec_tests/test_spec_write.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/test_container.py` & `hdmf-3.5.5/tests/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/test_io_hdf5.py` & `hdmf-3.5.5/tests/unit/test_io_hdf5.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/test_io_hdf5_h5tools.py` & `hdmf-3.5.5/tests/unit/test_io_hdf5_h5tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -2413,14 +2413,73 @@
         with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='r') as read_io:
             self.ios.append(read_io)  # track IO objects for tearDown
             read_foofile2 = read_io.read()
 
             # make sure the linked dataset is within the same file
             self.assertEqual(read_foofile2.foofile_data.file.filename, self.paths[1])
 
+    def test_soft_link_group_modified(self):
+        """Test that exporting a written file with soft linked groups keeps links within the file."""
+        foo1 = Foo('foo1', [1, 2, 3, 4, 5], "I am foo1", 17, 3.14)
+        foobucket = FooBucket('bucket1', [foo1])
+        foofile = FooFile(buckets=[foobucket], foo_link=foo1)
+
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='w') as write_io:
+            write_io.write(foofile)
+
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io:
+            read_foofile2 = read_io.read()
+            read_foofile2.foo_link.set_modified()  # trigger a rebuild of foo_link and its parents
+
+            with HDF5IO(self.paths[1], mode='w') as export_io:
+                export_io.export(src_io=read_io, container=read_foofile2)
+
+        with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='r') as read_io:
+            self.ios.append(read_io)  # track IO objects for tearDown
+            read_foofile2 = read_io.read()
+
+            # make sure the linked group is within the same file
+            self.assertEqual(read_foofile2.foo_link.container_source, self.paths[1])
+
+        # make sure the linked group is a soft link
+        with File(self.paths[1], 'r') as f:
+            self.assertEqual(f['links/foo_link'].file.filename, self.paths[1])
+            self.assertIsInstance(f.get('links/foo_link', getlink=True), h5py.SoftLink)
+
+    def test_soft_link_group_modified_rel_path(self):
+        """Test that exporting a written file with soft linked groups keeps links within the file."""
+        foo1 = Foo('foo1', [1, 2, 3, 4, 5], "I am foo1", 17, 3.14)
+        foobucket = FooBucket('bucket1', [foo1])
+        foofile = FooFile(buckets=[foobucket], foo_link=foo1)
+        # make temp files in relative path location
+        self.paths[0] = os.path.basename(self.paths[0])
+        self.paths[1] = os.path.basename(self.paths[1])
+
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='w') as write_io:
+            write_io.write(foofile)
+
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io:
+            read_foofile2 = read_io.read()
+            read_foofile2.foo_link.set_modified()  # trigger a rebuild of foo_link and its parents
+
+            with HDF5IO(self.paths[1], mode='w') as export_io:
+                export_io.export(src_io=read_io, container=read_foofile2)
+
+        with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='r') as read_io:
+            self.ios.append(read_io)  # track IO objects for tearDown
+            read_foofile2 = read_io.read()
+
+            # make sure the linked group is within the same file
+            self.assertEqual(read_foofile2.foo_link.container_source, os.path.abspath(self.paths[1]))
+
+        # make sure the linked group is a soft link
+        with File(self.paths[1], 'r') as f:
+            self.assertEqual(f['links/foo_link'].file.filename, self.paths[1])
+            self.assertIsInstance(f.get('links/foo_link', getlink=True), h5py.SoftLink)
+
     def test_external_link_group(self):
         """Test that exporting a written file with external linked groups maintains the links."""
         foo1 = Foo('foo1', [1, 2, 3, 4, 5], "I am foo1", 17, 3.14)
         foobucket = FooBucket('bucket1', [foo1])
         foofile = FooFile(buckets=[foobucket])
 
         with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='w') as read_io:
@@ -2433,26 +2492,60 @@
             foofile2 = FooFile(foo_link=read_foofile.buckets['bucket1'].foos['foo1'])
 
             with HDF5IO(self.paths[1], manager=manager, mode='w') as write_io:
                 write_io.write(foofile2)
 
         with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='r') as read_io:
             self.ios.append(read_io)  # track IO objects for tearDown
-            read_foofile2 = read_io.read()
 
             with HDF5IO(self.paths[2], mode='w') as export_io:
                 export_io.export(src_io=read_io)
 
         with HDF5IO(self.paths[2], manager=get_foo_buildmanager(), mode='r') as read_io:
             self.ios.append(read_io)  # track IO objects for tearDown
             read_foofile2 = read_io.read()
 
             # make sure the linked group is read from the first file
             self.assertEqual(read_foofile2.foo_link.container_source, self.paths[0])
 
+    def test_external_link_group_rel_path(self):
+        """Test that exporting a written file from a relative filepath works."""
+        foo1 = Foo('foo1', [1, 2, 3, 4, 5], "I am foo1", 17, 3.14)
+        foobucket = FooBucket('bucket1', [foo1])
+        foofile = FooFile(buckets=[foobucket])
+        # make temp files in relative path location
+        self.paths[0] = os.path.basename(self.paths[0])
+        self.paths[1] = os.path.basename(self.paths[1])
+        self.paths[2] = os.path.basename(self.paths[2])
+
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='w') as read_io:
+            read_io.write(foofile)
+
+        manager = get_foo_buildmanager()
+        with HDF5IO(self.paths[0], manager=manager, mode='r') as read_io:
+            read_foofile = read_io.read()
+            # make external link to existing group
+            foofile2 = FooFile(foo_link=read_foofile.buckets['bucket1'].foos['foo1'])
+
+            with HDF5IO(self.paths[1], manager=manager, mode='w') as write_io:
+                write_io.write(foofile2)
+
+        with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='r') as read_io:
+            self.ios.append(read_io)  # track IO objects for tearDown
+
+            with HDF5IO(self.paths[2], mode='w') as export_io:
+                export_io.export(src_io=read_io)
+
+        with HDF5IO(self.paths[2], manager=get_foo_buildmanager(), mode='r') as read_io:
+            self.ios.append(read_io)  # track IO objects for tearDown
+            read_foofile2 = read_io.read()
+
+            # make sure the linked group is read from the first file
+            self.assertEqual(read_foofile2.foo_link.container_source, os.path.abspath(self.paths[0]))
+
     def test_external_link_dataset(self):
         """Test that exporting a written file with external linked datasets maintains the links."""
         foo1 = Foo('foo1', [1, 2, 3, 4, 5], "I am foo1", 17, 3.14)
         foobucket = FooBucket('bucket1', [foo1])
         foofile = FooFile(buckets=[foobucket], foofile_data=[1, 2, 3])
 
         with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='w') as write_io:
@@ -2756,14 +2849,157 @@
         with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io1:
             self.ios.append(read_io1)  # track IO objects for tearDown
             read_foofile3 = read_io1.read()
 
             with HDF5IO(self.paths[2], manager=get_foo_buildmanager(), mode='r') as read_io2:
                 self.ios.append(read_io2)  # track IO objects for tearDown
                 read_foofile4 = read_io2.read()
+
+                # check that file can be read
+                self.assertNotEqual(read_foofile4.buckets['bucket2'].foos['foo2'].my_data,
+                                    read_foofile3.buckets['bucket1'].foos['foo1'].my_data)
+                self.assertNotEqual(read_foofile4.foofile_data, read_foofile3.buckets['bucket1'].foos['foo1'].my_data)
+                self.assertNotEqual(read_foofile4.foofile_data, read_foofile4.buckets['bucket2'].foos['foo2'].my_data)
+
+        with File(self.paths[2], 'r') as f:
+            self.assertEqual(f['buckets/bucket2/foo_holder/foo2/my_data'].file.filename, self.paths[2])
+            self.assertEqual(f['foofile_data'].file.filename, self.paths[2])
+
+    def test_export_simple_link_data(self):
+        """Test simple exporting of data with a link with link_data=True links the data."""
+        foo1 = Foo('foo1', [1, 2, 3, 4, 5], "I am foo1", 17, 3.14)
+        foobucket = FooBucket('bucket1', [foo1])
+        foofile = FooFile([foobucket])
+
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='w') as write_io:
+            write_io.write(foofile)
+
+        # create new foofile with link from foo2.data to read foo1.data
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io:
+            read_foofile1 = read_io.read()
+            foo2 = Foo('foo2', read_foofile1.buckets['bucket1'].foos['foo1'].my_data, "I am foo2", 17, 3.14)
+            foobucket2 = FooBucket('bucket2', [foo2])
+            foofile2 = FooFile([foobucket2])
+
+            # also add link from foofile to new foo2.my_data dataset which is a link to foo1.my_data dataset
+            # this should make an external link within the exported file
+            foofile2.foofile_data = foo2.my_data
+
+            with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='w') as write_io:
+                write_io.write(foofile2)
+
+        # read the data with the linked dataset, do not modify it, and export it
+        with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='r') as read_io:
+            with HDF5IO(self.paths[2], mode='w') as export_io:
+                export_io.export(src_io=read_io)
+
+        # read the exported file and confirm that the dataset is linked to the correct foofile1
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io1:
+            self.ios.append(read_io1)  # track IO objects for tearDown
+            read_foofile3 = read_io1.read()
+
+            with HDF5IO(self.paths[2], manager=get_foo_buildmanager(), mode='r') as read_io2:
+                self.ios.append(read_io2)  # track IO objects for tearDown
+                read_foofile4 = read_io2.read()
+
+                self.assertEqual(read_foofile4.buckets['bucket2'].foos['foo2'].my_data,
+                                 read_foofile3.buckets['bucket1'].foos['foo1'].my_data)
+                self.assertEqual(read_foofile4.foofile_data, read_foofile3.buckets['bucket1'].foos['foo1'].my_data)
+
+        with File(self.paths[2], 'r') as f:
+            self.assertEqual(f['buckets/bucket2/foo_holder/foo2/my_data'].file.filename, self.paths[0])
+            self.assertEqual(f['foofile_data'].file.filename, self.paths[0])
+            self.assertIsInstance(f.get('buckets/bucket2/foo_holder/foo2/my_data', getlink=True),
+                                  h5py.ExternalLink)
+            self.assertIsInstance(f.get('foofile_data', getlink=True), h5py.ExternalLink)
+
+    def test_export_simple_link_data_false(self):
+        """Test simple exporting of data with a link with link_data=False copies the data."""
+        foo1 = Foo('foo1', [1, 2, 3, 4, 5], "I am foo1", 17, 3.14)
+        foobucket = FooBucket('bucket1', [foo1])
+        foofile = FooFile([foobucket])
+
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='w') as write_io:
+            write_io.write(foofile)
+
+        # create new foofile with link from foo2.data to read foo1.data
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io:
+            read_foofile1 = read_io.read()
+            foo2 = Foo('foo2', read_foofile1.buckets['bucket1'].foos['foo1'].my_data, "I am foo2", 17, 3.14)
+            foobucket2 = FooBucket('bucket2', [foo2])
+            foofile2 = FooFile([foobucket2])
+
+            # also add link from foofile to new foo2.my_data dataset which is a link to foo1.my_data dataset
+            # this should make an external link within the exported file
+            foofile2.foofile_data = foo2.my_data
+
+            with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='w') as write_io:
+                write_io.write(foofile2)
+
+        # read the data with the linked dataset, do not modify it, and export it
+        with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='r') as read_io:
+            with HDF5IO(self.paths[2], mode='w') as export_io:
+                export_io.export(src_io=read_io, write_args={'link_data': False})
+
+        # read the exported file and confirm that the dataset is copied
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io1:
+            self.ios.append(read_io1)  # track IO objects for tearDown
+            read_foofile3 = read_io1.read()
+
+            with HDF5IO(self.paths[2], manager=get_foo_buildmanager(), mode='r') as read_io2:
+                self.ios.append(read_io2)  # track IO objects for tearDown
+                read_foofile4 = read_io2.read()
+
+                # check that file can be read
+                self.assertNotEqual(read_foofile4.buckets['bucket2'].foos['foo2'].my_data,
+                                    read_foofile3.buckets['bucket1'].foos['foo1'].my_data)
+                self.assertNotEqual(read_foofile4.foofile_data, read_foofile3.buckets['bucket1'].foos['foo1'].my_data)
+                self.assertNotEqual(read_foofile4.foofile_data, read_foofile4.buckets['bucket2'].foos['foo2'].my_data)
+
+        with File(self.paths[2], 'r') as f:
+            self.assertEqual(f['buckets/bucket2/foo_holder/foo2/my_data'].file.filename, self.paths[2])
+            self.assertEqual(f['foofile_data'].file.filename, self.paths[2])
+
+    def test_export_simple_with_container_link_data_false(self):
+        """Test simple exporting of data with a link with link_data=False copies the data."""
+        foo1 = Foo('foo1', [1, 2, 3, 4, 5], "I am foo1", 17, 3.14)
+        foobucket = FooBucket('bucket1', [foo1])
+        foofile = FooFile([foobucket])
+
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='w') as write_io:
+            write_io.write(foofile)
+
+        # create new foofile with link from foo2.data to read foo1.data
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io:
+            read_foofile1 = read_io.read()
+            foo2 = Foo('foo2', read_foofile1.buckets['bucket1'].foos['foo1'].my_data, "I am foo2", 17, 3.14)
+            foobucket2 = FooBucket('bucket2', [foo2])
+            foofile2 = FooFile([foobucket2])
+
+            # also add link from foofile to new foo2.my_data dataset which is a link to foo1.my_data dataset
+            # this should make an external link within the exported file
+            foofile2.foofile_data = foo2.my_data
+
+            with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='w') as write_io:
+                write_io.write(foofile2)
+
+        # read the data with the linked dataset, do not modify it, and export it
+        with HDF5IO(self.paths[1], manager=get_foo_buildmanager(), mode='r') as read_io:
+            read_foofile2 = read_io.read()
+            with HDF5IO(self.paths[2], mode='w') as export_io:
+                export_io.export(src_io=read_io, container=read_foofile2, write_args={'link_data': False})
+
+        # read the exported file and confirm that the dataset is copied
+        with HDF5IO(self.paths[0], manager=get_foo_buildmanager(), mode='r') as read_io1:
+            self.ios.append(read_io1)  # track IO objects for tearDown
+            read_foofile3 = read_io1.read()
+
+            with HDF5IO(self.paths[2], manager=get_foo_buildmanager(), mode='r') as read_io2:
+                self.ios.append(read_io2)  # track IO objects for tearDown
+                read_foofile4 = read_io2.read()
 
                 # check that file can be read
                 self.assertNotEqual(read_foofile4.buckets['bucket2'].foos['foo2'].my_data,
                                     read_foofile3.buckets['bucket1'].foos['foo1'].my_data)
                 self.assertNotEqual(read_foofile4.foofile_data, read_foofile3.buckets['bucket1'].foos['foo1'].my_data)
                 self.assertNotEqual(read_foofile4.foofile_data, read_foofile4.buckets['bucket2'].foos['foo2'].my_data)
```

### Comparing `hdmf-3.5.4/tests/unit/test_multicontainerinterface.py` & `hdmf-3.5.5/tests/unit/test_multicontainerinterface.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/test_query.py` & `hdmf-3.5.5/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/test_table.py` & `hdmf-3.5.5/tests/unit/test_table.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils.py` & `hdmf-3.5.5/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils_test/test_core_DataChunk.py` & `hdmf-3.5.5/tests/unit/utils_test/test_core_DataChunk.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils_test/test_core_DataChunkIterator.py` & `hdmf-3.5.5/tests/unit/utils_test/test_core_DataChunkIterator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils_test/test_core_DataIO.py` & `hdmf-3.5.5/tests/unit/utils_test/test_core_DataIO.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils_test/test_core_GenericDataChunkIterator.py` & `hdmf-3.5.5/tests/unit/utils_test/test_core_GenericDataChunkIterator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils_test/test_core_ShapeValidator.py` & `hdmf-3.5.5/tests/unit/utils_test/test_core_ShapeValidator.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils_test/test_docval.py` & `hdmf-3.5.5/tests/unit/utils_test/test_docval.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils_test/test_labelleddict.py` & `hdmf-3.5.5/tests/unit/utils_test/test_labelleddict.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/utils_test/test_utils.py` & `hdmf-3.5.5/tests/unit/utils_test/test_utils.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/validator_tests/test_errors.py` & `hdmf-3.5.5/tests/unit/validator_tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tests/unit/validator_tests/test_validate.py` & `hdmf-3.5.5/tests/unit/validator_tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/tox.ini` & `hdmf-3.5.5/tox.ini`

 * *Files identical despite different names*

### Comparing `hdmf-3.5.4/versioneer.py` & `hdmf-3.5.5/versioneer.py`

 * *Files identical despite different names*

