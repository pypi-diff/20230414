# Comparing `tmp/osqp-0.6.2.post8.tar.gz` & `tmp/osqp-0.6.2.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osqp-0.6.2.post8.tar", last modified: Tue Nov 22 17:25:37 2022, max compression
+gzip compressed data, was "osqp-0.6.2.post9.tar", last modified: Fri Apr 14 21:06:18 2023, max compression
```

## Comparing `osqp-0.6.2.post8.tar` & `osqp-0.6.2.post9.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.979452 osqp-0.6.2.post8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.947452 osqp-0.6.2.post8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.955452 osqp-0.6.2.post8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1960 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1588 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/.github/workflows/build_aarch64.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      416 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2022-11-22 17:25:37.979452 osqp-0.6.2.post8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1047 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.955452 osqp-0.6.2.post8/osqp_sources/
--rw-r--r--   0 runner    (1001) docker     (122)    14003 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.955452 osqp-0.6.2.post8/osqp_sources/configure/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.955452 osqp-0.6.2.post8/osqp_sources/configure/cmake/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/configure/cmake/FindPythonModule.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      980 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/configure/cmake/FindR.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      168 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/configure/cmake/Utils.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     1002 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/configure/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      741 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/configure/osqp_configure.h.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.955452 osqp-0.6.2.post8/osqp_sources/include/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3901 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/auxil.h
--rw-r--r--   0 runner    (1001) docker     (122)     3729 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/constants.h
--rw-r--r--   0 runner    (1001) docker     (122)     4996 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/cs.h
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/ctrlc.h
--rw-r--r--   0 runner    (1001) docker     (122)      760 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/error.h
--rw-r--r--   0 runner    (1001) docker     (122)     4686 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/glob_opts.h
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/kkt.h
--rw-r--r--   0 runner    (1001) docker     (122)     5678 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/lin_alg.h
--rw-r--r--   0 runner    (1001) docker     (122)     1621 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/lin_sys.h
--rw-r--r--   0 runner    (1001) docker     (122)    11814 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/osqp.h
--rw-r--r--   0 runner    (1001) docker     (122)      434 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/polish.h
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/proj.h
--rw-r--r--   0 runner    (1001) docker     (122)      778 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/scaling.h
--rw-r--r--   0 runner    (1001) docker     (122)    10256 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/types.h
--rw-r--r--   0 runner    (1001) docker     (122)     4109 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/include/util.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.959452 osqp-0.6.2.post8/osqp_sources/lin_sys/
--rw-r--r--   0 runner    (1001) docker     (122)      773 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.959452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.959452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/
--rw-r--r--   0 runner    (1001) docker     (122)      338 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9844 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h
--rw-r--r--   0 runner    (1001) docker     (122)     3126 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.c
--rw-r--r--   0 runner    (1001) docker     (122)      645 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.959452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.959452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.959452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/include/
--rw-r--r--   0 runner    (1001) docker     (122)     8987 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/include/SuiteSparse_config.h
--rw-r--r--   0 runner    (1001) docker     (122)    17829 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/include/amd.h
--rw-r--r--   0 runner    (1001) docker     (122)     8239 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/include/amd_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.959452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/
--rw-r--r--   0 runner    (1001) docker     (122)    12237 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/SuiteSparse_config.c
--rw-r--r--   0 runner    (1001) docker     (122)     5712 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_1.c
--rw-r--r--   0 runner    (1001) docker     (122)    64841 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_2.c
--rw-r--r--   0 runner    (1001) docker     (122)     4854 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_aat.c
--rw-r--r--   0 runner    (1001) docker     (122)     1870 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_control.c
--rw-r--r--   0 runner    (1001) docker     (122)     1255 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_defaults.c
--rw-r--r--   0 runner    (1001) docker     (122)     4295 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_info.c
--rw-r--r--   0 runner    (1001) docker     (122)     6037 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_order.c
--rw-r--r--   0 runner    (1001) docker     (122)     3703 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_post_tree.c
--rw-r--r--   0 runner    (1001) docker     (122)     5509 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_postorder.c
--rw-r--r--   0 runner    (1001) docker     (122)     3808 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_preprocess.c
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_valid.c
--rw-r--r--   0 runner    (1001) docker     (122)    11867 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.c
--rw-r--r--   0 runner    (1001) docker     (122)     3729 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.963452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/
--rw-r--r--   0 runner    (1001) docker     (122)      164 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       92 2022-11-22 17:17:32.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.git
--rw-r--r--   0 runner    (1001) docker     (122)      502 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (122)      886 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     6222 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5727 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      996 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/appveyor.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.963452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.963452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/
--rw-r--r--   0 runner    (1001) docker     (122)     1003 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      571 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/qdldl_types.h.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.963452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     4513 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/example.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.963452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/
--rw-r--r--   0 runner    (1001) docker     (122)       14 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     6397 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/qdldl.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.963452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/
--rw-r--r--   0 runner    (1001) docker     (122)     7683 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/qdldl.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.963452 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      550 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      438 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/minunit.h
--rw-r--r--   0 runner    (1001) docker     (122)     4495 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/qdldl_tester.c
--rw-r--r--   0 runner    (1001) docker     (122)      871 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_basic.h
--rw-r--r--   0 runner    (1001) docker     (122)      511 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_identity.h
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_osqp_kkt.h
--rw-r--r--   0 runner    (1001) docker     (122)      401 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_rank_deficient.h
--rw-r--r--   0 runner    (1001) docker     (122)      470 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_singleton.h
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_sym_structure.h
--rw-r--r--   0 runner    (1001) docker     (122)      371 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_tril_structure.h
--rw-r--r--   0 runner    (1001) docker     (122)      491 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_two_by_two.h
--rw-r--r--   0 runner    (1001) docker     (122)      593 2022-11-22 17:17:33.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_zero_on_diag.h
--rw-r--r--   0 runner    (1001) docker     (122)     4190 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/lib_handler.c
--rw-r--r--   0 runner    (1001) docker     (122)      920 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/lin_sys/lib_handler.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.967452 osqp-0.6.2.post8/osqp_sources/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    31823 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/auxil.c
--rw-r--r--   0 runner    (1001) docker     (122)     8535 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/cs.c
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/ctrlc.c
--rw-r--r--   0 runner    (1001) docker     (122)      601 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/error.c
--rw-r--r--   0 runner    (1001) docker     (122)     6862 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/kkt.c
--rw-r--r--   0 runner    (1001) docker     (122)     8570 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/lin_alg.c
--rw-r--r--   0 runner    (1001) docker     (122)     2088 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/lin_sys.c
--rw-r--r--   0 runner    (1001) docker     (122)    47667 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/osqp.c
--rw-r--r--   0 runner    (1001) docker     (122)    10760 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/polish.c
--rw-r--r--   0 runner    (1001) docker     (122)      660 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/proj.c
--rw-r--r--   0 runner    (1001) docker     (122)     5469 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/scaling.c
--rw-r--r--   0 runner    (1001) docker     (122)    11623 2022-11-22 17:17:31.000000 osqp-0.6.2.post8/osqp_sources/src/util.c
--rw-r--r--   0 runner    (1001) docker     (122)      407 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       35 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-22 17:25:37.979452 osqp-0.6.2.post8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     9363 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.951452 osqp-0.6.2.post8/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.951452 osqp-0.6.2.post8/src/extension/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.967452 osqp-0.6.2.post8/src/extension/include/
--rw-r--r--   0 runner    (1001) docker     (122)     8222 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/extension/include/osqpinfopy.h
--rw-r--r--   0 runner    (1001) docker     (122)     2591 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/extension/include/osqpmodulemethods.h
--rw-r--r--   0 runner    (1001) docker     (122)    41043 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/extension/include/osqpobjectpy.h
--rw-r--r--   0 runner    (1001) docker     (122)     4345 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/extension/include/osqpresultspy.h
--rw-r--r--   0 runner    (1001) docker     (122)     5418 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/extension/include/osqputilspy.h
--rw-r--r--   0 runner    (1001) docker     (122)    13734 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/extension/include/osqpworkspacepy.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.967452 osqp-0.6.2.post8/src/extension/src/
--rw-r--r--   0 runner    (1001) docker     (122)       40 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/extension/src/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     2374 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/extension/src/osqpmodule.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.967452 osqp-0.6.2.post8/src/osqp/
--rw-r--r--   0 runner    (1001) docker     (122)      197 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.971452 osqp-0.6.2.post8/src/osqp/codegen/
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/codegen/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)       48 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6886 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/codegen/code_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.971452 osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/
--rw-r--r--   0 runner    (1001) docker     (122)     4187 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    18291 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/emosqpmodule.c
--rw-r--r--   0 runner    (1001) docker     (122)      573 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/example.c
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.951452 osqp-0.6.2.post8/src/osqp/codegen/sources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.971452 osqp-0.6.2.post8/src/osqp/codegen/sources/configure/
--rw-r--r--   0 runner    (1001) docker     (122)      741 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/configure/osqp_configure.h.in
--rw-r--r--   0 runner    (1001) docker     (122)      571 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/configure/qdldl_types.h.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.971452 osqp-0.6.2.post8/src/osqp/codegen/sources/include/
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3901 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/auxil.h
--rw-r--r--   0 runner    (1001) docker     (122)     3729 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/constants.h
--rw-r--r--   0 runner    (1001) docker     (122)      760 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/error.h
--rw-r--r--   0 runner    (1001) docker     (122)     4686 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/glob_opts.h
--rw-r--r--   0 runner    (1001) docker     (122)     3266 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/kkt.h
--rw-r--r--   0 runner    (1001) docker     (122)     5678 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/lin_alg.h
--rw-r--r--   0 runner    (1001) docker     (122)    11814 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/osqp.h
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/proj.h
--rw-r--r--   0 runner    (1001) docker     (122)     6397 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/qdldl.h
--rw-r--r--   0 runner    (1001) docker     (122)     3729 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/qdldl_interface.h
--rw-r--r--   0 runner    (1001) docker     (122)      778 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/scaling.h
--rw-r--r--   0 runner    (1001) docker     (122)    10256 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/types.h
--rw-r--r--   0 runner    (1001) docker     (122)     4109 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/include/util.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.975452 osqp-0.6.2.post8/src/osqp/codegen/sources/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1067 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    31823 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/auxil.c
--rw-r--r--   0 runner    (1001) docker     (122)      601 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/error.c
--rw-r--r--   0 runner    (1001) docker     (122)     6862 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/kkt.c
--rw-r--r--   0 runner    (1001) docker     (122)     8570 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/lin_alg.c
--rw-r--r--   0 runner    (1001) docker     (122)    47667 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/osqp.c
--rw-r--r--   0 runner    (1001) docker     (122)      660 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/proj.c
--rw-r--r--   0 runner    (1001) docker     (122)     7683 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/qdldl.c
--rw-r--r--   0 runner    (1001) docker     (122)    11867 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/qdldl_interface.c
--rw-r--r--   0 runner    (1001) docker     (122)     5469 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/scaling.c
--rw-r--r--   0 runner    (1001) docker     (122)    11623 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp/codegen/sources/src/util.c
--rw-r--r--   0 runner    (1001) docker     (122)    18466 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/codegen/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    14013 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.975452 osqp-0.6.2.post8/src/osqp/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     6227 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/basic_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7046 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/codegen_matrices_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3770 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/codegen_vectors_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6736 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/derivative_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/dual_infeasibility_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/feasibility_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      745 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/mkl_pardiso_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1714 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/multithread_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/non_convex_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3477 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/polishing_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/primal_infeasibility_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.979452 osqp-0.6.2.post8/src/osqp/tests/solutions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      808 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_basic_QP.npz
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_feasibility_problem.npz
--rw-r--r--   0 runner    (1001) docker     (122)     1392 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_polish_random.npz
--rw-r--r--   0 runner    (1001) docker     (122)      808 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_polish_simple.npz
--rw-r--r--   0 runner    (1001) docker     (122)      992 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_polish_unconstrained.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_solve.npz
--rw-r--r--   0 runner    (1001) docker     (122)      992 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_unconstrained_problem.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_A.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_A_allind.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_A_allind.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_A_indA.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_A_indP.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_A_indP_indA.npz
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_allind.npz
--rw-r--r--   0 runner    (1001) docker     (122)      808 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_bounds.npz
--rw-r--r--   0 runner    (1001) docker     (122)      808 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_l.npz
--rw-r--r--   0 runner    (1001) docker     (122)      808 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_q.npz
--rw-r--r--   0 runner    (1001) docker     (122)      808 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_u.npz
--rw-r--r--   0 runner    (1001) docker     (122)     1440 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/unconstrained_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     6299 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/update_matrices_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      292 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1724 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/tests/warm_start_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     5129 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.967452 osqp-0.6.2.post8/src/osqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8055 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       31 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-22 17:25:37.000000 osqp-0.6.2.post8/src/osqp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-22 17:25:37.979452 osqp-0.6.2.post8/src/osqppurepy/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqppurepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    63336 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqppurepy/_osqp.py
--rw-r--r--   0 runner    (1001) docker     (122)     9432 2022-11-22 17:17:28.000000 osqp-0.6.2.post8/src/osqppurepy/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.385226 osqp-0.6.2.post9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/.github/workflows/build_aarch64.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/osqp_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/osqp_sources/configure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/configure/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/cmake/FindPythonModule.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/cmake/FindR.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/cmake/Utils.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/configure/osqp_configure.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/auxil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/cs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/ctrlc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/glob_opts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/kkt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/lin_alg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/lin_sys.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/osqp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/polish.h
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/proj.h
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/include/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.c
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.393226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/SuiteSparse_config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/amd_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/SuiteSparse_config.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_1.c
+-rw-r--r--   0 runner    (1001) docker     (123)    64841 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_aat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_control.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_defaults.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_info.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6037 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_order.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_post_tree.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_postorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_preprocess.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_valid.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.git
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/appveyor.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/qdldl_types.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/example.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/qdldl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.397226 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/qdldl.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.401227 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/minunit.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/qdldl_tester.c
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_basic.h
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_identity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_osqp_kkt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_rank_deficient.h
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_singleton.h
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_sym_structure.h
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_tril_structure.h
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_two_by_two.h
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-14 20:59:05.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_zero_on_diag.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/lib_handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/lin_sys/lib_handler.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.401227 osqp-0.6.2.post9/osqp_sources/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31823 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/auxil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/cs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/ctrlc.c
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/error.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/kkt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/lin_alg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/lin_sys.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47667 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/osqp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/polish.c
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/proj.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/scaling.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-14 20:59:04.000000 osqp-0.6.2.post9/osqp_sources/src/util.c
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/src/extension/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.401227 osqp-0.6.2.post9/src/extension/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpinfopy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpmodulemethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41043 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpobjectpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpresultspy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqputilspy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/include/osqpworkspacepy.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/extension/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/src/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/extension/src/osqpmodule.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/code_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/emosqpmodule.c
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/example.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.389227 osqp-0.6.2.post9/src/osqp/codegen/sources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp/codegen/sources/configure/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/configure/osqp_configure.h.in
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/configure/qdldl_types.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.409227 osqp-0.6.2.post9/src/osqp/codegen/sources/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/auxil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/glob_opts.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/kkt.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/lin_alg.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/osqp.h
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/proj.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/qdldl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/qdldl_interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/include/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.409227 osqp-0.6.2.post9/src/osqp/codegen/sources/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31823 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/auxil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/error.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/kkt.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/lin_alg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47667 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/osqp.c
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/proj.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/qdldl.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/qdldl_interface.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/scaling.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp/codegen/sources/src/util.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/codegen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/src/osqp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/basic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/codegen_matrices_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/codegen_vectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/derivative_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/dual_infeasibility_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/feasibility_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/mkl_pardiso_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/multithread_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/non_convex_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/polishing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/primal_infeasibility_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/src/osqp/tests/solutions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_basic_QP.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_feasibility_problem.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_random.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_simple.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_unconstrained.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_solve.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_unconstrained_problem.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_A.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_A_allind.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_allind.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indA.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indP.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indP_indA.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_allind.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_bounds.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_l.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_q.npz
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_u.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/unconstrained_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/update_matrices_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/tests/warm_start_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.405227 osqp-0.6.2.post9/src/osqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 21:06:18.000000 osqp-0.6.2.post9/src/osqp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:06:18.413227 osqp-0.6.2.post9/src/osqppurepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqppurepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63336 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqppurepy/_osqp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-14 20:59:02.000000 osqp-0.6.2.post9/src/osqppurepy/interface.py
```

### Comparing `osqp-0.6.2.post8/.github/workflows/build.yml` & `osqp-0.6.2.post9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/.github/workflows/build_aarch64.yml` & `osqp-0.6.2.post9/.github/workflows/build_aarch64.yml`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/.gitignore` & `osqp-0.6.2.post9/.gitignore`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/LICENSE` & `osqp-0.6.2.post9/LICENSE`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/PKG-INFO` & `osqp-0.6.2.post9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osqp
-Version: 0.6.2.post8
+Version: 0.6.2.post9
 Summary: OSQP: The Operator Splitting QP Solver
 Home-page: https://osqp.org/
 Author: Bartolomeo Stellato, Goran Banjac
 Author-email: bartolomeo.stellato@gmail.com
 License: Apache 2.0
 License-File: LICENSE
 
@@ -29,14 +29,23 @@
 
 where ``x in R^n`` is the optimization variable. The objective function
 is defined by a positive semidefinite matrix ``P in S^n_+`` and vector
 ``q in R^n``. The linear constraints are defined by matrix
 ``A in R^{m x n}`` and vectors ``l in R^m U {-inf}^m``,
 ``u in R^m U {+inf}^m``.
 
+Installation
+------------
+
+To install ``osqp`` for python, make sure that you're using a recent version of ``pip`` (``pip install --upgrade pip``)
+and then use ``pip install osqp``.
+
+To install `osqp` from source, clone the repository (``git clone --recurse-submodules https://github.com/osqp/osqp-python``)
+and run ``pip install .`` from inside the cloned folder.
+
 Documentation
 -------------
 
 The interface is documented `here <https://osqp.org/>`__.
 
 
 Packaging
```

### Comparing `osqp-0.6.2.post8/README.rst` & `osqp-0.6.2.post9/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,23 @@
 
 where ``x in R^n`` is the optimization variable. The objective function
 is defined by a positive semidefinite matrix ``P in S^n_+`` and vector
 ``q in R^n``. The linear constraints are defined by matrix
 ``A in R^{m x n}`` and vectors ``l in R^m U {-inf}^m``,
 ``u in R^m U {+inf}^m``.
 
+Installation
+------------
+
+To install ``osqp`` for python, make sure that you're using a recent version of ``pip`` (``pip install --upgrade pip``)
+and then use ``pip install osqp``.
+
+To install `osqp` from source, clone the repository (``git clone --recurse-submodules https://github.com/osqp/osqp-python``)
+and run ``pip install .`` from inside the cloned folder.
+
 Documentation
 -------------
 
 The interface is documented `here <https://osqp.org/>`__.
 
 
 Packaging
```

### Comparing `osqp-0.6.2.post8/osqp_sources/CMakeLists.txt` & `osqp-0.6.2.post9/osqp_sources/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/configure/cmake/FindPythonModule.cmake` & `osqp-0.6.2.post9/osqp_sources/configure/cmake/FindPythonModule.cmake`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/configure/cmake/FindR.cmake` & `osqp-0.6.2.post9/osqp_sources/configure/cmake/FindR.cmake`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/configure/cmake/cmake_uninstall.cmake.in` & `osqp-0.6.2.post9/osqp_sources/configure/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/configure/osqp_configure.h.in` & `osqp-0.6.2.post9/osqp_sources/configure/osqp_configure.h.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/CMakeLists.txt` & `osqp-0.6.2.post9/osqp_sources/include/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/auxil.h` & `osqp-0.6.2.post9/osqp_sources/include/auxil.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/constants.h` & `osqp-0.6.2.post9/osqp_sources/include/constants.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/cs.h` & `osqp-0.6.2.post9/osqp_sources/include/cs.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/ctrlc.h` & `osqp-0.6.2.post9/osqp_sources/include/ctrlc.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/error.h` & `osqp-0.6.2.post9/osqp_sources/include/error.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/glob_opts.h` & `osqp-0.6.2.post9/osqp_sources/include/glob_opts.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/kkt.h` & `osqp-0.6.2.post9/osqp_sources/include/kkt.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/lin_alg.h` & `osqp-0.6.2.post9/osqp_sources/include/lin_alg.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/lin_sys.h` & `osqp-0.6.2.post9/osqp_sources/include/lin_sys.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/osqp.h` & `osqp-0.6.2.post9/osqp_sources/include/osqp.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/proj.h` & `osqp-0.6.2.post9/osqp_sources/include/proj.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/scaling.h` & `osqp-0.6.2.post9/osqp_sources/include/scaling.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/types.h` & `osqp-0.6.2.post9/osqp_sources/include/types.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/include/util.h` & `osqp-0.6.2.post9/osqp_sources/include/util.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/CMakeLists.txt` & `osqp-0.6.2.post9/osqp_sources/lin_sys/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/CMakeLists.txt` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_interface.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/pardiso/pardiso_loader.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/CMakeLists.txt` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/LICENSE` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/LICENSE`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/include/SuiteSparse_config.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/include/amd.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/amd.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/include/amd_internal.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/include/amd_internal.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/SuiteSparse_config.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_1.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_1.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_2.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_2.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_aat.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_aat.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_control.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_control.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_defaults.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_info.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_info.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_order.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_order.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_post_tree.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_postorder.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_preprocess.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_valid.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/amd/src/amd_valid.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_interface.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.travis.yml` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/.travis.yml`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CHANGELOG.md` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CMakeLists.txt` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/LICENSE` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/LICENSE`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/README.md` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/README.md`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/appveyor.yml` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/appveyor.yml`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/cmake_uninstall.cmake.in` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/qdldl_types.h.in` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/configure/qdldl_types.h.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/example.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/examples/example.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/qdldl.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/include/qdldl.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/qdldl.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/src/qdldl.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/CMakeLists.txt` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/qdldl_tester.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/qdldl_tester.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_basic.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_basic.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_osqp_kkt.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_osqp_kkt.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_zero_on_diag.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/direct/qdldl/qdldl_sources/tests/test_zero_on_diag.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/lib_handler.c` & `osqp-0.6.2.post9/osqp_sources/lin_sys/lib_handler.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/lin_sys/lib_handler.h` & `osqp-0.6.2.post9/osqp_sources/lin_sys/lib_handler.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/CMakeLists.txt` & `osqp-0.6.2.post9/osqp_sources/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/auxil.c` & `osqp-0.6.2.post9/osqp_sources/src/auxil.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/cs.c` & `osqp-0.6.2.post9/osqp_sources/src/cs.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/ctrlc.c` & `osqp-0.6.2.post9/osqp_sources/src/ctrlc.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/error.c` & `osqp-0.6.2.post9/osqp_sources/src/error.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/kkt.c` & `osqp-0.6.2.post9/osqp_sources/src/kkt.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/lin_alg.c` & `osqp-0.6.2.post9/osqp_sources/src/lin_alg.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/lin_sys.c` & `osqp-0.6.2.post9/osqp_sources/src/lin_sys.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/osqp.c` & `osqp-0.6.2.post9/osqp_sources/src/osqp.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/polish.c` & `osqp-0.6.2.post9/osqp_sources/src/polish.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/proj.c` & `osqp-0.6.2.post9/osqp_sources/src/proj.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/scaling.c` & `osqp-0.6.2.post9/osqp_sources/src/scaling.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/osqp_sources/src/util.c` & `osqp-0.6.2.post9/osqp_sources/src/util.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/setup.py` & `osqp-0.6.2.post9/setup.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/extension/include/osqpinfopy.h` & `osqp-0.6.2.post9/src/extension/include/osqpinfopy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/extension/include/osqpmodulemethods.h` & `osqp-0.6.2.post9/src/extension/include/osqpmodulemethods.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/extension/include/osqpobjectpy.h` & `osqp-0.6.2.post9/src/extension/include/osqpobjectpy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/extension/include/osqpresultspy.h` & `osqp-0.6.2.post9/src/extension/include/osqpresultspy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/extension/include/osqputilspy.h` & `osqp-0.6.2.post9/src/extension/include/osqputilspy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/extension/include/osqpworkspacepy.h` & `osqp-0.6.2.post9/src/extension/include/osqpworkspacepy.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/extension/src/osqpmodule.c` & `osqp-0.6.2.post9/src/extension/src/osqpmodule.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/code_generator.py` & `osqp-0.6.2.post9/src/osqp/codegen/code_generator.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/CMakeLists.txt` & `osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/emosqpmodule.c` & `osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/emosqpmodule.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/example.c` & `osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/example.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/files_to_generate/setup.py` & `osqp-0.6.2.post9/src/osqp/codegen/files_to_generate/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                             libraries=libraries,
                             include_dirs=include_dirs,
                             sources=sources_files,
                             extra_compile_args=compile_args)
 
 
 setup(name='PYTHON_EXT_NAME',
-      version='0.6.2.post8',
+      version='0.6.2.post9',
       author='Bartolomeo Stellato, Goran Banjac',
       author_email='bartolomeo.stellato@gmail.com',
       description='This is the Python module for embedded OSQP: ' +
                   'Operator Splitting solver for Quadratic Programs.',
       setup_requires=["numpy >= 1.7"],
       install_requires=["numpy >= 1.7", "future"],
       license='Apache 2.0',
```

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/configure/osqp_configure.h.in` & `osqp-0.6.2.post9/src/osqp/codegen/sources/configure/osqp_configure.h.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/configure/qdldl_types.h.in` & `osqp-0.6.2.post9/src/osqp/codegen/sources/configure/qdldl_types.h.in`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/CMakeLists.txt` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/auxil.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/auxil.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/constants.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/constants.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/error.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/error.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/glob_opts.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/glob_opts.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/kkt.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/kkt.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/lin_alg.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/lin_alg.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/osqp.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/osqp.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/proj.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/proj.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/qdldl.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/qdldl.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/qdldl_interface.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/qdldl_interface.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/scaling.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/scaling.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/types.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/types.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/include/util.h` & `osqp-0.6.2.post9/src/osqp/codegen/sources/include/util.h`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/CMakeLists.txt` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/auxil.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/auxil.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/error.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/error.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/kkt.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/kkt.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/lin_alg.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/lin_alg.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/osqp.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/osqp.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/proj.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/proj.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/qdldl.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/qdldl.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/qdldl_interface.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/qdldl_interface.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/scaling.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/scaling.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/sources/src/util.c` & `osqp-0.6.2.post9/src/osqp/codegen/sources/src/util.c`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/codegen/utils.py` & `osqp-0.6.2.post9/src/osqp/codegen/utils.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/interface.py` & `osqp-0.6.2.post9/src/osqp/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Python interface module for OSQP solver v0.6.2.post8
+Python interface module for OSQP solver v0.6.2.post9
 """
 from __future__ import print_function
 from builtins import object
 import osqp._osqp as _osqp  # Internal low level module
 import numpy as np
 import scipy.sparse as spa
 from warnings import warn
```

### Comparing `osqp-0.6.2.post8/src/osqp/tests/basic_test.py` & `osqp-0.6.2.post9/src/osqp/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/codegen_matrices_test.py` & `osqp-0.6.2.post9/src/osqp/tests/codegen_matrices_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/codegen_vectors_test.py` & `osqp-0.6.2.post9/src/osqp/tests/codegen_vectors_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/derivative_test.py` & `osqp-0.6.2.post9/src/osqp/tests/derivative_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/dual_infeasibility_test.py` & `osqp-0.6.2.post9/src/osqp/tests/dual_infeasibility_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/feasibility_test.py` & `osqp-0.6.2.post9/src/osqp/tests/feasibility_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/mkl_pardiso_test.py` & `osqp-0.6.2.post9/src/osqp/tests/mkl_pardiso_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/multithread_test.py` & `osqp-0.6.2.post9/src/osqp/tests/multithread_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/non_convex_test.py` & `osqp-0.6.2.post9/src/osqp/tests/non_convex_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/polishing_test.py` & `osqp-0.6.2.post9/src/osqp/tests/polishing_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/primal_infeasibility_test.py` & `osqp-0.6.2.post9/src/osqp/tests/primal_infeasibility_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_basic_QP.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_basic_QP.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_feasibility_problem.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_feasibility_problem.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_polish_random.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_random.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_polish_simple.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_simple.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_polish_unconstrained.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_polish_unconstrained.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_solve.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_solve.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_unconstrained_problem.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_unconstrained_problem.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_A.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_A.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_A_allind.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_A_allind.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_A_allind.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_allind.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_A_indA.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indA.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_A_indP.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indP.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_A_indP_indA.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_A_indP_indA.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_P_allind.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_P_allind.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_bounds.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_bounds.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_l.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_l.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_q.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_q.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/solutions/test_update_u.npz` & `osqp-0.6.2.post9/src/osqp/tests/solutions/test_update_u.npz`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/unconstrained_test.py` & `osqp-0.6.2.post9/src/osqp/tests/unconstrained_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/update_matrices_test.py` & `osqp-0.6.2.post9/src/osqp/tests/update_matrices_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/tests/warm_start_test.py` & `osqp-0.6.2.post9/src/osqp/tests/warm_start_test.py`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqp/utils.py` & `osqp-0.6.2.post9/src/osqp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,24 +67,24 @@
             l = -np.inf * np.ones(A.shape[0])
         if A is not None and u is None:
             u = np.inf * np.ones(A.shape[0])
 
         # Create elements if they are not specified
         if P is None:
             P = sparse.csc_matrix((np.zeros((0,), dtype=np.double),
-                                   np.zeros((0,), dtype=np.int),
-                                   np.zeros((n+1,), dtype=np.int)),
+                                   np.zeros((0,), dtype=int),
+                                   np.zeros((n+1,), dtype=int)),
                                   shape=(n, n))
         if q is None:
             q = np.zeros(n)
 
         if A is None:
             A = sparse.csc_matrix((np.zeros((0,), dtype=np.double),
-                                   np.zeros((0,), dtype=np.int),
-                                   np.zeros((n+1,), dtype=np.int)),
+                                   np.zeros((0,), dtype=int),
+                                   np.zeros((n+1,), dtype=int)),
                                   shape=(m, n))
             l = np.zeros(A.shape[0])
             u = np.zeros(A.shape[0])
 
         #
         # Check vector dimensions (not checked from C solver)
         #
```

### Comparing `osqp-0.6.2.post8/src/osqp.egg-info/PKG-INFO` & `osqp-0.6.2.post9/src/osqp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osqp
-Version: 0.6.2.post8
+Version: 0.6.2.post9
 Summary: OSQP: The Operator Splitting QP Solver
 Home-page: https://osqp.org/
 Author: Bartolomeo Stellato, Goran Banjac
 Author-email: bartolomeo.stellato@gmail.com
 License: Apache 2.0
 License-File: LICENSE
 
@@ -29,14 +29,23 @@
 
 where ``x in R^n`` is the optimization variable. The objective function
 is defined by a positive semidefinite matrix ``P in S^n_+`` and vector
 ``q in R^n``. The linear constraints are defined by matrix
 ``A in R^{m x n}`` and vectors ``l in R^m U {-inf}^m``,
 ``u in R^m U {+inf}^m``.
 
+Installation
+------------
+
+To install ``osqp`` for python, make sure that you're using a recent version of ``pip`` (``pip install --upgrade pip``)
+and then use ``pip install osqp``.
+
+To install `osqp` from source, clone the repository (``git clone --recurse-submodules https://github.com/osqp/osqp-python``)
+and run ``pip install .`` from inside the cloned folder.
+
 Documentation
 -------------
 
 The interface is documented `here <https://osqp.org/>`__.
 
 
 Packaging
```

### Comparing `osqp-0.6.2.post8/src/osqp.egg-info/SOURCES.txt` & `osqp-0.6.2.post9/src/osqp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osqp-0.6.2.post8/src/osqppurepy/_osqp.py` & `osqp-0.6.2.post9/src/osqppurepy/_osqp.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 class OSQP(object):
     """OSQP solver lower level interface
     Attributes
     ----------
     work    - workspace
     """
     def __init__(self):
-        self._version = "0.6.2.post8"
+        self._version = "0.6.2.post9"
 
     @property
     def version(self):
         """Return solver version
         """
         return self._version
```

### Comparing `osqp-0.6.2.post8/src/osqppurepy/interface.py` & `osqp-0.6.2.post9/src/osqppurepy/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,24 +57,24 @@
             l = -np.inf * np.ones(A.shape[0])
         if A is not None and u is None:
             u = np.inf * np.ones(A.shape[0])
 
         # Create elements if they are not specified
         if P is None:
             P = sparse.csc_matrix((np.zeros((0,), dtype=np.double),
-                                  np.zeros((0,), dtype=np.int),
-                                  np.zeros((n+1,), dtype=np.int)),
+                                  np.zeros((0,), dtype=int),
+                                  np.zeros((n+1,), dtype=int)),
                                   shape=(n, n))
         if q is None:
             q = np.zeros(n)
 
         if A is None:
             A = sparse.csc_matrix((np.zeros((0,), dtype=np.double),
-                                  np.zeros((0,), dtype=np.int),
-                                  np.zeros((n+1,), dtype=np.int)),
+                                  np.zeros((0,), dtype=int),
+                                  np.zeros((n+1,), dtype=int)),
                                   shape=(m, n))
             l = np.zeros(A.shape[0])
             u = np.zeros(A.shape[0])
 
         #
         # Check vector dimensions (not checked from C solver)
         #
```

