# Comparing `tmp/linear_operator-0.3.0.tar.gz` & `tmp/linear_operator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear_operator-0.3.0.tar", last modified: Tue Nov 29 20:28:48 2022, max compression
+gzip compressed data, was "linear_operator-0.4.0.tar", last modified: Fri Apr 14 20:49:42 2023, max compression
```

## Comparing `linear_operator-0.3.0.tar` & `linear_operator-0.4.0.tar`

### file list

```diff
@@ -1,174 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.573931 linear_operator-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.561931 linear_operator-0.3.0/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.557931 linear_operator-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.561931 linear_operator-0.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      909 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.github/ISSUE_TEMPLATE/documentation_examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      915 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      494 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.github/ISSUE_TEMPLATE/refactor.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.561931 linear_operator-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.github/workflows/run_test_suite.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2022-11-29 20:28:39.000000 linear_operator-0.3.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2022-11-29 20:28:39.000000 linear_operator-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-11-29 20:28:39.000000 linear_operator-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2022-11-29 20:28:48.573931 linear_operator-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14634 2022-11-29 20:28:39.000000 linear_operator-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.561931 linear_operator-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      774 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.561931 linear_operator-0.3.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/composition_decoration_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/converting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/custom_linear_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/data_sparse_operators.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/linear_operator.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/namespace.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      304 2022-11-29 20:28:39.000000 linear_operator-0.3.0/docs/source/utils.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.561931 linear_operator-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2022-11-29 20:28:39.000000 linear_operator-0.3.0/examples/LinearOperator_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.561931 linear_operator-0.3.0/linear_operator/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.565931 linear_operator-0.3.0/linear_operator/functions/
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_dsmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_inv_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_inv_quad_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     6230 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_root_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4225 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/functions/_sqrt_inv_matmul.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.569931 linear_operator-0.3.0/linear_operator/operators/
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   121188 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14221 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/batch_repeat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/block_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/block_interleaved_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/block_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19513 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/cat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/chol_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/constant_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/dense_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/identity_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21161 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/interpolated_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/keops_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17843 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/kronecker_product_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/linear_operator_representation_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/low_rank_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/matmul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/permutation_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/psd_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/sum_batch_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/sum_kronecker_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/toeplitz_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/triangular_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/operators/zero_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18725 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.569931 linear_operator-0.3.0/linear_operator/test/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/test/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    55101 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/test/linear_operator_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.569931 linear_operator-0.3.0/linear_operator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/broadcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/contour_integral_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/lanczos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12328 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/minres.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/permutation.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/pinverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9828 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/stochastic_lq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/toeplitz.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2022-11-29 20:28:39.000000 linear_operator-0.3.0/linear_operator/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-11-29 20:28:48.000000 linear_operator-0.3.0/linear_operator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.565931 linear_operator-0.3.0/linear_operator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2022-11-29 20:28:48.000000 linear_operator-0.3.0/linear_operator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2022-11-29 20:28:48.000000 linear_operator-0.3.0/linear_operator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 20:28:48.000000 linear_operator-0.3.0/linear_operator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-11-29 20:28:48.000000 linear_operator-0.3.0/linear_operator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-11-29 20:28:48.000000 linear_operator-0.3.0/linear_operator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-11-29 20:28:39.000000 linear_operator-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2022-11-29 20:28:48.573931 linear_operator-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2022-11-29 20:28:39.000000 linear_operator-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.569931 linear_operator-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.569931 linear_operator-0.3.0/test/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/test_diagonalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/test_dsmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/test_inv_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/test_inv_quad_logdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/test_matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/test_root_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/functions/test_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.573931 linear_operator-0.3.0/test/operators/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_batch_repeat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_block_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_block_interleaved_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_cat_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_chol_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_constant_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_dense_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_identity_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_interpolated_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_kronecker_product_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_kronecker_product_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_low_rank_root_added_diag_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_low_rank_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_matmul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_mul_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_permutation_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_psd_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_root_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_sum_batch_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_sum_kronecker_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_sum_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_toeplitz_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_triangular_linear_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/operators/test_zero_linear_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 20:28:48.573931 linear_operator-0.3.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_lanczos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_minres.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_permutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2022-11-29 20:28:39.000000 linear_operator-0.3.0/test/utils/test_toeplitz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.232299 linear_operator-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.216298 linear_operator-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/documentation_examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/ISSUE_TEMPLATE/refactor.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.github/workflows/run_test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-14 20:49:29.000000 linear_operator-0.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-14 20:49:29.000000 linear_operator-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 20:49:29.000000 linear_operator-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-04-14 20:49:42.232299 linear_operator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14634 2023-04-14 20:49:29.000000 linear_operator-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/composition_decoration_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/converting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/custom_linear_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/data_sparse_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/linear_operator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/namespace.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-14 20:49:29.000000 linear_operator-0.4.0/docs/source/utils.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-04-14 20:49:29.000000 linear_operator-0.4.0/examples/LinearOperator_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.220299 linear_operator-0.4.0/linear_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.224299 linear_operator-0.4.0/linear_operator/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_dsmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_inv_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_inv_quad_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_root_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/functions/_sqrt_inv_matmul.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/linear_operator/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121537 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14269 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/batch_repeat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/block_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/block_interleaved_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/block_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19700 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/cat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/chol_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/constant_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/dense_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/identity_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/interpolated_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/keops_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17878 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/kronecker_product_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/linear_operator_representation_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/low_rank_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/matmul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/permutation_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/psd_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/sum_batch_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/sum_kronecker_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/toeplitz_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/triangular_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/operators/zero_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18403 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/linear_operator/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/test/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55783 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/test/linear_operator_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/linear_operator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/broadcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/contour_integral_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/minres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/pinverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/stochastic_lq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/toeplitz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-14 20:49:29.000000 linear_operator-0.4.0/linear_operator/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.224299 linear_operator-0.4.0/linear_operator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-14 20:49:42.000000 linear_operator-0.4.0/linear_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 20:49:41.000000 linear_operator-0.4.0/linear_operator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-14 20:49:29.000000 linear_operator-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 20:49:42.236299 linear_operator-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-14 20:49:29.000000 linear_operator-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.228299 linear_operator-0.4.0/test/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_diagonalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_dsmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_inv_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_inv_quad_logdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_root_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/functions/test_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.232299 linear_operator-0.4.0/test/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_batch_repeat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_block_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_block_interleaved_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_cat_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_chol_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_constant_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_dense_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_identity_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_interpolated_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_kronecker_product_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_kronecker_product_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_low_rank_root_added_diag_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_low_rank_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_matmul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_mul_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_permutation_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_psd_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_root_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_sum_batch_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_sum_kronecker_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_sum_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_toeplitz_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_triangular_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/operators/test_zero_linear_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:49:42.232299 linear_operator-0.4.0/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_minres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-14 20:49:29.000000 linear_operator-0.4.0/test/utils/test_toeplitz.py
```

### Comparing `linear_operator-0.3.0/.conda/meta.yaml` & `linear_operator-0.4.0/.conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `linear_operator-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/.github/ISSUE_TEMPLATE/documentation_examples.md` & `linear_operator-0.4.0/.github/ISSUE_TEMPLATE/documentation_examples.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `linear_operator-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/.github/workflows/deploy.yml` & `linear_operator-0.4.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/.github/workflows/run_test_suite.yml` & `linear_operator-0.4.0/.github/workflows/run_test_suite.yml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
         python-version: "3.8"
     - name: Install dependencies
       run: |
-        pip install flake8==4.0.1 flake8-print==4.0.0 pre-commit
+        pip install flake8==5.0.4 flake8-print==5.0.0 pre-commit
         pre-commit install
         pre-commit run seed-isort-config || true
     - name: Run linting
       run: |
         flake8
     - name: Run pre-commit checks
       # skipping flake8 here (run separatey above b/c pre-commit does not include flake8-print)
```

### Comparing `linear_operator-0.3.0/.gitignore` & `linear_operator-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/.readthedocs.yml` & `linear_operator-0.4.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/CONTRIBUTING.md` & `linear_operator-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/LICENSE` & `linear_operator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/PKG-INFO` & `linear_operator-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear_operator
-Version: 0.3.0
+Version: 0.4.0
 Summary: A linear operator implementation, primarily designed for finite-dimensional positive definite operators (i.e. kernel matrices).
 Home-page: UNKNOWN
 Author: Geoff Pleiss
 Author-email: gpleiss@gmail.com
 License: MIT
 Project-URL: Documentation, https://linear_operator.readthedocs.io
 Project-URL: Source, https://github.com/cornellius-gp/linear_operator/
```

### Comparing `linear_operator-0.3.0/README.md` & `linear_operator-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/docs/Makefile` & `linear_operator-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/docs/make.bat` & `linear_operator-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/docs/source/composition_decoration_operators.rst` & `linear_operator-0.4.0/docs/source/composition_decoration_operators.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/docs/source/conf.py` & `linear_operator-0.4.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 import os
 import sys
 import warnings
-import sphinx_rtd_theme  # noqa
 from typing import ForwardRef
 
+import sphinx_rtd_theme  # noqa
+
 
 sys.path.append(os.path.abspath(os.path.join(__file__, "..", "..", "..")))
 
 # -- Project information -----------------------------------------------------
 
 project = "linear_operator"
 copyright = "2022, Cornellius GP"
```

### Comparing `linear_operator-0.3.0/docs/source/custom_linear_operators.rst` & `linear_operator-0.4.0/docs/source/custom_linear_operators.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/docs/source/data_sparse_operators.rst` & `linear_operator-0.4.0/docs/source/data_sparse_operators.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/docs/source/index.rst` & `linear_operator-0.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/docs/source/namespace.rst` & `linear_operator-0.4.0/docs/source/namespace.rst`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/examples/LinearOperator_demo.ipynb` & `linear_operator-0.4.0/examples/LinearOperator_demo.ipynb`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/__init__.py` & `linear_operator-0.4.0/linear_operator/__init__.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/beta_features.py` & `linear_operator-0.4.0/linear_operator/beta_features.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/functions/__init__.py` & `linear_operator-0.4.0/linear_operator/functions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,18 @@
     """
     from ..operators import to_linear_operator
 
     return to_linear_operator(input).inv_quad(inv_quad_rhs, reduce_inv_quad=reduce_inv_quad)
 
 
 def inv_quad_logdet(
-    input: Anysor, inv_quad_rhs: Optional[torch.Tensor] = None, logdet: bool = False, reduce_inv_quad: bool = True
+    input: Anysor,
+    inv_quad_rhs: Optional[torch.Tensor] = None,
+    logdet: bool = False,
+    reduce_inv_quad: bool = True,
 ) -> Tuple[torch.Tensor, torch.Tensor]:
     r"""
     Calls both :func:`inv_quad_logdet` and :func:`logdet` on a positive definite matrix (or batch) :math:`\mathbf A`.
     However, calling this method is far more efficient and stable than calling each method independently.
 
     :param input: :math:`\mathbf A` - the positive definite matrix (... X N X N)
     :param inv_quad_rhs: :math:`\mathbf R` - the right hand sides of the inverse quadratic term (... x N x M)
@@ -124,15 +127,18 @@
     """
     from ..operators import to_linear_operator
 
     return to_linear_operator(input).inv_quad_logdet(inv_quad_rhs, logdet, reduce_inv_quad=reduce_inv_quad)
 
 
 def pivoted_cholesky(
-    input: Anysor, rank: int, error_tol: Optional[float] = None, return_pivots: bool = False
+    input: Anysor,
+    rank: int,
+    error_tol: Optional[float] = None,
+    return_pivots: bool = False,
 ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
     r"""
     Performs a partial pivoted Cholesky factorization of a positive definite matrix (or batch of matrices).
     :math:`\mathbf L \mathbf L^\top = \mathbf A`.
     The partial pivoted Cholesky factor :math:`\mathbf L \in \mathbb R^{N \times \text{rank}}`
     forms a low rank approximation to the LinearOperator.
```

### Comparing `linear_operator-0.3.0/linear_operator/functions/_diagonalization.py` & `linear_operator-0.4.0/linear_operator/functions/_diagonalization.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/functions/_inv_quad.py` & `linear_operator-0.4.0/linear_operator/functions/_inv_quad.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/functions/_inv_quad_logdet.py` & `linear_operator-0.4.0/linear_operator/functions/_inv_quad_logdet.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/functions/_matmul.py` & `linear_operator-0.4.0/linear_operator/functions/_matmul.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/functions/_pivoted_cholesky.py` & `linear_operator-0.4.0/linear_operator/functions/_pivoted_cholesky.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,21 @@
         #   the diagonal.
         matrix_diag = matrix_diag.clone()
 
         # Make sure max_iter isn't bigger than the matrix
         max_iter = min(max_iter, matrix_shape[-1])
 
         # What we're returning
-        L = torch.zeros(*batch_shape, max_iter, matrix_shape[-1], dtype=matrix.dtype, device=matrix.device)
+        L = torch.zeros(
+            *batch_shape,
+            max_iter,
+            matrix_shape[-1],
+            dtype=matrix.dtype,
+            device=matrix.device,
+        )
         orig_error = torch.max(matrix_diag, dim=-1)[0]
         errors = torch.norm(matrix_diag, 1, dim=-1) / orig_error
 
         # The permutation
         permutation = torch.arange(0, matrix_shape[-1], dtype=torch.long, device=matrix_diag.device)
         permutation = permutation.repeat(*batch_shape, 1)
 
@@ -72,15 +78,16 @@
                 row = apply_permutation(matrix, pi_m.unsqueeze(-1), right_permutation=None).squeeze(-2)
                 pi_i = permutation[..., m + 1 :].contiguous()
 
                 L_m_new = row.gather(-1, pi_i)
                 if m > 0:
                     L_prev = L[..., :m, :].gather(-1, pi_i.unsqueeze(-2).repeat(*(1 for _ in batch_shape), m, 1))
                     update = L[..., :m, :].gather(
-                        -1, pi_m.view(*pi_m.shape, 1, 1).repeat(*(1 for _ in batch_shape), m, 1)
+                        -1,
+                        pi_m.view(*pi_m.shape, 1, 1).repeat(*(1 for _ in batch_shape), m, 1),
                     )
                     L_m_new -= torch.sum(update * L_prev, dim=-2)
 
                 L_m_new /= L_m.gather(-1, pi_m.unsqueeze(-1))
                 L_m.scatter_(-1, pi_i, L_m_new)
 
                 matrix_diag_current = matrix_diag.gather(-1, pi_i)
@@ -116,17 +123,24 @@
             Krows = apply_permutation(matrix, full_permutation, short_permutation)
 
             # Get L - Cholesky factor of K[..., :m, :m]
             L = psd_safe_cholesky(Krows[..., :m, :])
 
             # Compute (Krows * L^{-T}) - the (pivoted) result of Pivoted Cholesky
             res_pivoted = torch.cat(
-                [L, torch.linalg.solve_triangular(L, Krows[..., m:, :].mT, upper=False).mT],
+                [
+                    L,
+                    torch.linalg.solve_triangular(L, Krows[..., m:, :].mT, upper=False).mT,
+                ],
                 dim=-2,
             )
-            res = apply_permutation(res_pivoted, left_permutation=_inverse_permutation, right_permutation=None)
+            res = apply_permutation(
+                res_pivoted,
+                left_permutation=_inverse_permutation,
+                right_permutation=None,
+            )
 
             # Now compute the backward pass of res
             res.backward(gradient=grad_output)
 
         # Define gradient placeholders
         return tuple([None, None, None] + [matrix_arg.grad for matrix_arg in matrix_args])
```

### Comparing `linear_operator-0.3.0/linear_operator/functions/_root_decomposition.py` & `linear_operator-0.4.0/linear_operator/functions/_root_decomposition.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/functions/_solve.py` & `linear_operator-0.4.0/linear_operator/functions/_solve.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,16 @@
                 left_solves = Solve.apply(ctx.representation_tree, False, grad_output, *matrix_args)
 
                 if any(ctx.needs_input_grad[3:]):
                     # We call _bilinear_derivative to compute dl/dK
                     # To ensure that this term is symmetric, we concatenate the left and right solves together,
                     # and divide the result by 1/2
                     arg_grads = linear_op._bilinear_derivative(
-                        torch.cat([left_solves, right_solves], -1), torch.cat([right_solves, left_solves], -1).mul(-0.5)
+                        torch.cat([left_solves, right_solves], -1),
+                        torch.cat([right_solves, left_solves], -1).mul(-0.5),
                     )
                 if ctx.needs_input_grad[2]:
                     right_grad = left_solves
                     if ctx.is_vector:
                         right_grad.squeeze_(-1)
 
                 return tuple([None, None] + [right_grad] + list(arg_grads))
@@ -114,15 +115,16 @@
                 left_solves = left_solves @ grad_output
 
                 if ctx.needs_input_grad[2]:
                     left_grad = grad_output @ right_solves.mT
                 if any(ctx.needs_input_grad[4:]):
                     # We do this concatenation to ensure that the gradient of linear_op is symmetric
                     arg_grads = linear_op._bilinear_derivative(
-                        torch.cat([left_solves, right_solves], -1), torch.cat([right_solves, left_solves], -1).mul(-0.5)
+                        torch.cat([left_solves, right_solves], -1),
+                        torch.cat([right_solves, left_solves], -1).mul(-0.5),
                     )
                 if ctx.needs_input_grad[3]:
                     right_grad = left_solves
                     if ctx.is_vector:
                         right_grad.squeeze_(-1)
 
                 return tuple([None, None] + [left_grad, right_grad] + list(arg_grads))
```

### Comparing `linear_operator-0.3.0/linear_operator/functions/_sqrt_inv_matmul.py` & `linear_operator-0.4.0/linear_operator/functions/_sqrt_inv_matmul.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,37 +18,52 @@
     def forward(ctx, representation_tree, rhs, lhs, *matrix_args):
         ctx.representation_tree = representation_tree
         ctx.linear_op = ctx.representation_tree(*matrix_args)
 
         if lhs is not None:
             terms = torch.cat([rhs, lhs.mT], dim=-1)
             solves, weights, no_shift_solves, shifts = utils.contour_integral_quad(
-                ctx.linear_op, terms, inverse=True, num_contour_quadrature=settings.num_contour_quadrature.value()
+                ctx.linear_op,
+                terms,
+                inverse=True,
+                num_contour_quadrature=settings.num_contour_quadrature.value(),
             )
             rhs_solves, lhs_solves = solves.split([rhs.size(-1), lhs.size(-2)], dim=-1)
             lhs_no_shift_solves = no_shift_solves[..., -lhs.size(-2) :]
             sqrt_inv_matmul_res = lhs @ (rhs_solves * weights).sum(0)
             inv_quad_res = (lhs_no_shift_solves.mT * lhs).sum(dim=-1).mul_(-1)
         else:
             rhs_solves, weights, _, shifts = utils.contour_integral_quad(
-                ctx.linear_op, rhs, inverse=True, num_contour_quadrature=settings.num_contour_quadrature.value()
+                ctx.linear_op,
+                rhs,
+                inverse=True,
+                num_contour_quadrature=settings.num_contour_quadrature.value(),
             )
             sqrt_inv_matmul_res = (rhs_solves * weights).sum(0)
             lhs_solves = None
             lhs_no_shift_solves = None
             inv_quad_res = torch.zeros(ctx.linear_op.batch_shape, dtype=rhs.dtype, device=rhs.device)
 
         # Save for backwards
         ctx.save_for_backward(rhs, lhs, rhs_solves, lhs_solves, weights, shifts, lhs_no_shift_solves, *matrix_args)
 
         return sqrt_inv_matmul_res, inv_quad_res
 
     @staticmethod
     def backward(ctx, sqrt_inv_matmul_grad, inv_quad_grad):
-        rhs, lhs, rhs_solves, lhs_solves, weights, shifts, lhs_no_shift_solves, *matrix_args = ctx.saved_tensors
+        (
+            rhs,
+            lhs,
+            rhs_solves,
+            lhs_solves,
+            weights,
+            shifts,
+            lhs_no_shift_solves,
+            *matrix_args,
+        ) = ctx.saved_tensors
         rhs_grad = None
         lhs_grad = None
         matrix_arg_grads = [None] * len(matrix_args)
 
         if lhs is not None:
             # Intermediate terms for sqrt_inv_matmul/quad
             weighted_rhs_solves_mul_grad = rhs_solves.mul(weights) @ sqrt_inv_matmul_grad.mT
@@ -63,17 +78,24 @@
 
             # Compute rhs grad
             if ctx.needs_input_grad[1]:
                 rhs_grad = (lhs_solves @ sqrt_inv_matmul_grad).mul(weights).sum(0)
 
             # Compute matrix grads
             terms1 = torch.cat([lhs_no_shift_solves.unsqueeze(0), lhs_solves], 0)
-            terms2 = torch.cat([neg_inv_quad_solves_mul_grad.unsqueeze(0), weighted_rhs_solves_mul_grad], 0)
+            terms2 = torch.cat(
+                [
+                    neg_inv_quad_solves_mul_grad.unsqueeze(0),
+                    weighted_rhs_solves_mul_grad,
+                ],
+                0,
+            )
             matrix_arg_grads = ctx.linear_op._bilinear_derivative(
-                torch.cat([terms1, terms2], -1), torch.cat([terms2, terms1], -1).mul_(0.5)
+                torch.cat([terms1, terms2], -1),
+                torch.cat([terms2, terms1], -1).mul_(0.5),
             )
 
         else:
             # Intermediate terms for sqrt_inv_matmul/quad
             grad_solves, _, _, _ = utils.contour_integral_quad(
                 ctx.linear_op,
                 sqrt_inv_matmul_grad,
@@ -91,12 +113,13 @@
             if ctx.needs_input_grad[1]:
                 rhs_grad = grad_solves_mul_weights.sum(0)
 
             # Compute matrix grads
             terms1 = grad_solves_mul_weights
             terms2 = rhs_solves
             matrix_arg_grads = ctx.linear_op._bilinear_derivative(
-                torch.cat([terms1, terms2], -1), torch.cat([terms2, terms1], -1).mul_(0.5)
+                torch.cat([terms1, terms2], -1),
+                torch.cat([terms2, terms1], -1).mul_(0.5),
             )
 
         res = (None, rhs_grad, lhs_grad, *matrix_arg_grads)
         return res
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/__init__.py` & `linear_operator-0.4.0/linear_operator/operators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from ._linear_operator import LinearOperator, to_dense
 from .added_diag_linear_operator import AddedDiagLinearOperator
 from .batch_repeat_linear_operator import BatchRepeatLinearOperator
 from .block_diag_linear_operator import BlockDiagLinearOperator
 from .block_interleaved_linear_operator import BlockInterleavedLinearOperator
 from .block_linear_operator import BlockLinearOperator
-from .cat_linear_operator import CatLinearOperator, cat
+from .cat_linear_operator import cat, CatLinearOperator
 from .chol_linear_operator import CholLinearOperator
 from .constant_mul_linear_operator import ConstantMulLinearOperator
 from .dense_linear_operator import DenseLinearOperator, to_linear_operator
 from .diag_linear_operator import ConstantDiagLinearOperator, DiagLinearOperator
 from .identity_linear_operator import IdentityLinearOperator
 from .interpolated_linear_operator import InterpolatedLinearOperator
 from .keops_linear_operator import KeOpsLinearOperator
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/_linear_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 from ..functions._inv_quad import InvQuad
 from ..functions._inv_quad_logdet import InvQuadLogdet
 from ..functions._matmul import Matmul
 from ..functions._pivoted_cholesky import PivotedCholesky
 from ..functions._root_decomposition import RootDecomposition
 from ..functions._solve import Solve
 from ..functions._sqrt_inv_matmul import SqrtInvMatmul
-from ..utils.broadcasting import _matmul_broadcast_shape, _to_helper
+from ..utils.broadcasting import _matmul_broadcast_shape
 from ..utils.cholesky import psd_safe_cholesky
 from ..utils.deprecation import _deprecate_renamed_methods
 from ..utils.errors import CachingError
+from ..utils.generic import _to_helper
 from ..utils.getitem import (
     _compute_getitem_size,
     _convert_indices_to_tensors,
     _is_noop_index,
     _is_tensor_index_moved_to_start,
     _noop_index,
 )
@@ -162,15 +163,15 @@
         :param rhs: the matrix :math:`\mathbf M` to multiply with (... x N x C).
         :return: :math:`\mathbf K \mathbf M` (... x M x C)
         """
         raise NotImplementedError("The class {} requires a _matmul function!".format(self.__class__.__name__))
 
     @abstractmethod
     def _size(self) -> torch.Size:
-        """
+        r"""
         Returns the size of the resulting Tensor that the linear operator represents.
 
         ..note::
             This method is used internally by the related function
             :func:`~linear_operator.LinearOperator.size`,
             which does some additional work. Calling this method directly is discouraged.
 
@@ -375,15 +376,18 @@
         current_shape = torch.Size([1 for _ in range(len(batch_shape) - self.dim() + 2)] + list(self.batch_shape))
         batch_repeat = torch.Size(
             [expand_size // current_size for expand_size, current_size in zip(batch_shape, current_shape)]
         )
         return self.repeat(*batch_repeat, 1, 1)
 
     def _get_indices(
-        self, row_index: torch.LongTensor, col_index: torch.LongTensor, *batch_indices: Tuple[torch.LongTensor, ...]
+        self,
+        row_index: torch.LongTensor,
+        col_index: torch.LongTensor,
+        *batch_indices: Tuple[torch.LongTensor, ...],
     ) -> torch.Tensor:
         """
         This method selects elements from the LinearOperator based on tensor indices for each dimension.
         All indices are tensor indices that are broadcastable.
         There will be exactly one index per dimension of the LinearOperator
 
         ..note::
@@ -564,15 +568,15 @@
         other = other.evaluate_kernel()
         if isinstance(self, DenseLinearOperator) or isinstance(other, DenseLinearOperator):
             return DenseLinearOperator(self.to_dense() * other.to_dense())
         else:
             return MulLinearOperator(self, other)
 
     def _preconditioner(self) -> Tuple[Callable, "LinearOperator", torch.Tensor]:
-        """
+        r"""
         (Optional) define a preconditioner (:math:`\mathbf P`) for linear conjugate gradients
 
         :return:
             - a function which performs :math:`\mathbf P^{-1}(\cdot)`,
             - a LinearOperator representation of :math:`\mathbf P`, and
             - a Tensor containing :math:`\log \Vert \mathbf P \Vert`.
         """
@@ -671,15 +675,15 @@
         return settings.max_root_decomposition_size.value()
 
     def _root_inv_decomposition(
         self,
         initial_vectors: Optional[torch.Tensor] = None,
         test_vectors: Optional[torch.Tensor] = None,
     ) -> LinearOperator:
-        """
+        r"""
         Returns the (usually low-rank) inverse root of a LinearOperator of a PSD matrix.
 
         ..note::
             This method is used internally by the related function
             :func:`~linear_operator.LinearOperator.root_inv_decomposition`, which does some additional work.
             Calling this method directly is discouraged.
 
@@ -753,15 +757,18 @@
 
         if base_precond is not None:
             return base_precond
         elif linear_operator.beta_features.default_preconditioner.on():
             if hasattr(self, "_default_preconditioner_cache"):
                 U, S, Vt = self._default_preconditioner_cache
             else:
-                precond_basis_size = min(linear_operator.settings.max_preconditioner_size.value(), self.size(-1))
+                precond_basis_size = min(
+                    linear_operator.settings.max_preconditioner_size.value(),
+                    self.size(-1),
+                )
                 random_basis = torch.randn(
                     self.batch_shape + torch.Size((self.size(-2), precond_basis_size)),
                     device=self.device,
                     dtype=self.dtype,
                 )
                 projected_mat = self._matmul(random_basis)
                 proj_q = torch.linalg.qr(projected_mat)
@@ -1053,15 +1060,19 @@
         updated_inv_root = current_inv_root.mT.matmul(inner_inv_root)
 
         if return_triangular:
             updated_root = TriangularLinearOperator(updated_root)
             updated_inv_root = TriangularLinearOperator(updated_inv_root)
 
         add_to_cache(new_linear_op, "root_decomposition", RootLinearOperator(updated_root))
-        add_to_cache(new_linear_op, "root_inv_decomposition", RootLinearOperator(updated_inv_root))
+        add_to_cache(
+            new_linear_op,
+            "root_inv_decomposition",
+            RootLinearOperator(updated_inv_root),
+        )
 
         return new_linear_op
 
     @property
     def batch_dim(self) -> int:
         return len(self.batch_shape)
 
@@ -1210,15 +1221,19 @@
                 new_inv_root = stable_pinverse(new_root).mT
             add_to_cache(
                 new_linear_op,
                 "root_inv_decomposition",
                 RootLinearOperator(to_linear_operator(new_inv_root)),
             )
 
-        add_to_cache(new_linear_op, "root_decomposition", RootLinearOperator(to_linear_operator(new_root)))
+        add_to_cache(
+            new_linear_op,
+            "root_decomposition",
+            RootLinearOperator(to_linear_operator(new_root)),
+        )
 
         return new_linear_op
 
     @_implements(torch.linalg.cholesky)
     def cholesky(self, upper: bool = False) -> "TriangularLinearOperator":  # noqa F811
         """
         Cholesky-factorizes the LinearOperator.
@@ -1480,15 +1495,18 @@
         allocating new memory.
 
         :param sizes: the desired expanded size
         :return: The expanded LinearOperator
         """
         if len(sizes) == 1 and hasattr(sizes, "__iter__"):
             sizes = sizes[0]
-        if len(sizes) < 2 or tuple(sizes[-2:]) not in {tuple(self.matrix_shape), (-1, -1)}:
+        if len(sizes) < 2 or tuple(sizes[-2:]) not in {
+            tuple(self.matrix_shape),
+            (-1, -1),
+        }:
             raise RuntimeError(
                 "Invalid expand arguments {}. Currently, repeat only works to create repeated "
                 "batches of a 2D LinearOperator.".format(tuple(sizes))
             )
         elif all(isinstance(size, int) for size in sizes):
             shape = torch.Size(sizes)
         else:
@@ -1556,15 +1574,18 @@
         inv_quad_term = func(self.representation_tree(), *args)
 
         if reduce_inv_quad:
             inv_quad_term = inv_quad_term.sum(-1)
         return inv_quad_term
 
     def inv_quad_logdet(
-        self, inv_quad_rhs: Optional[torch.Tensor] = None, logdet: bool = False, reduce_inv_quad: bool = True
+        self,
+        inv_quad_rhs: Optional[torch.Tensor] = None,
+        logdet: bool = False,
+        reduce_inv_quad: bool = True,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         r"""
         Calls both :func:`inv_quad_logdet` and :func:`logdet` on a positive
         definite matrix (or batch) :math:`\mathbf A`.  However, calling this
         method is far more efficient and stable than calling each method
         independently.
 
@@ -2210,15 +2231,19 @@
                 left_tensor,
                 right_tensor,
                 *self.representation(),
             )
 
     @_implements(torch.linalg.solve_triangular)
     def solve_triangular(
-        self, rhs: torch.Tensor, upper: bool, left: bool = True, unitriangular: bool = False
+        self,
+        rhs: torch.Tensor,
+        upper: bool,
+        left: bool = True,
+        unitriangular: bool = False,
     ) -> torch.Tensor:
         r"""
         Computes a triangular linear solve (w.r.t self = :math:`\mathbf A`) with right hand side :math:`\mathbf R`.
         If left=True, computes the soluton :math:`\mathbf X` to
 
         .. math::
            \begin{equation}
@@ -2387,15 +2412,17 @@
             - The left singular vectors :math:`\mathbf U` (... x M, M),
             - The singlar values :math:`\mathbf S` (... x min(M, N)),
             - The right singluar vectors :math:`\mathbf V` (... x N x N)),
         """
         return self._svd()
 
     @_implements(torch.linalg.svd)
-    def _torch_linalg_svd(self) -> Tuple["LinearOperator", torch.Tensor, "LinearOperator"]:
+    def _torch_linalg_svd(
+        self,
+    ) -> Tuple["LinearOperator", torch.Tensor, "LinearOperator"]:
         r"""
         A version of self.svd() that matches the torch.linalg.svd API.
 
         :returns:
             - The left singular vectors :math:`\mathbf U` (... x M, M),
             - The singlar values :math:`\mathbf S` (... x min(M, N)),
             - The right singluar vectors :math:`\mathbf V^\top` (... x N X N),
@@ -2756,15 +2783,19 @@
         return self.mul(-1) + other
 
     def __sub__(self, other: Union[torch.Tensor, LinearOperator, float]) -> LinearOperator:
         return self + other.mul(-1)
 
     @classmethod
     def __torch_function__(
-        cls, func: Callable, types: Tuple[type, ...], args: Tuple[Any, ...] = (), kwargs: Dict[str, Any] = None
+        cls,
+        func: Callable,
+        types: Tuple[type, ...],
+        args: Tuple[Any, ...] = (),
+        kwargs: Dict[str, Any] = None,
     ) -> Any:
         if kwargs is None:
             kwargs = {}
 
         if not isinstance(args[0], cls):
             if func not in _HANDLED_SECOND_ARG_FUNCTIONS or not all(
                 issubclass(t, (torch.Tensor, LinearOperator)) for t in types
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/added_diag_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/added_diag_linear_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 
     .. _Gardner et al., NeurIPS 2018:
         https://arxiv.org/abs/1809.11165
     """
 
     def __init__(
         self,
-        *linear_ops: Union[Tuple[LinearOperator, DiagLinearOperator], Tuple[DiagLinearOperator, LinearOperator]],
+        *linear_ops: Union[
+            Tuple[LinearOperator, DiagLinearOperator],
+            Tuple[DiagLinearOperator, LinearOperator],
+        ],
         preconditioner_override: Optional[Callable] = None,
     ):
         linear_ops = list(linear_ops)
         super(AddedDiagLinearOperator, self).__init__(*linear_ops, preconditioner_override=preconditioner_override)
         if len(linear_ops) > 2:
             raise RuntimeError("An AddedDiagLinearOperator can only have two components")
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/batch_repeat_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/batch_repeat_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,16 @@
         )
         return batch_repeat
 
     def _expand_batch(self, batch_shape):
         padding_dims = torch.Size(tuple(1 for _ in range(max(len(batch_shape) + 2 - self.base_linear_op.dim(), 0))))
         current_batch_shape = padding_dims + self.base_linear_op.batch_shape
         return self.__class__(
-            self.base_linear_op, batch_repeat=self._compute_batch_repeat_size(current_batch_shape, batch_shape)
+            self.base_linear_op,
+            batch_repeat=self._compute_batch_repeat_size(current_batch_shape, batch_shape),
         )
 
     def _get_indices(self, row_index, col_index, *batch_indices):
         # First remove any new batch indices that were added - they aren't necessary
         num_true_batch_indices = self.base_linear_op.dim() - 2
         batch_indices = batch_indices[len(batch_indices) - num_true_batch_indices :]
 
@@ -225,15 +226,18 @@
         # Otherwise we have to also unsqueeze the base_linear_op
         base_unsqueeze_dim = dim - (len(self.base_linear_op.batch_shape) - len(self.base_linear_op.batch_shape))
         if base_unsqueeze_dim > 0:
             base_linear_op = base_linear_op._unsqueeze_batch(base_unsqueeze_dim)
         return self.__class__(base_linear_op, batch_repeat=batch_repeat)
 
     def add_jitter(self, jitter_val=1e-3):
-        return self.__class__(self.base_linear_op.add_jitter(jitter_val=jitter_val), batch_repeat=self.batch_repeat)
+        return self.__class__(
+            self.base_linear_op.add_jitter(jitter_val=jitter_val),
+            batch_repeat=self.batch_repeat,
+        )
 
     def inv_quad_logdet(self, inv_quad_rhs=None, logdet=False, reduce_inv_quad=True):
         if not self.is_square:
             raise RuntimeError(
                 "inv_quad_logdet only operates on (batches of) square (positive semi-definite) LinearOperators. "
                 "Got a {} of size {}.".format(self.__class__.__name__, self.size())
             )
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/block_diag_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/block_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/block_interleaved_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/block_interleaved_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/block_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/block_linear_operator.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,16 +69,24 @@
         if not isinstance(row_index, slice) or not isinstance(col_index, slice):
             # It's too complicated to deal with tensor indices in this case - we'll use the super method
             return super()._getitem(row_index, col_index, *batch_indices)
 
         # Now we know that row_index and col_index
         num_blocks = self.num_blocks
         num_rows, num_cols = self.matrix_shape
-        row_start, row_end, row_step = row_index.start or 0, row_index.stop or num_rows, row_index.step
-        col_start, col_end, col_step = col_index.start or 0, col_index.stop or num_cols, col_index.step
+        row_start, row_end, row_step = (
+            row_index.start or 0,
+            row_index.stop or num_rows,
+            row_index.step,
+        )
+        col_start, col_end, col_step = (
+            col_index.start or 0,
+            col_index.stop or num_cols,
+            col_index.step,
+        )
 
         # If we have a step, it's too complicated - go with the base case
         if row_step is not None or col_step is not None:
             return super()._getitem(row_index, col_index, *batch_indices)
 
         # Let's make sure that the slice dimensions perfectly correspond with the number of
         # outputs per input that we have
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/cat_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/cat_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from __future__ import annotations
 
 from typing import Tuple, Union
 
 import torch
 
-from ..utils.broadcasting import _matmul_broadcast_shape, _to_helper
+from ..utils.broadcasting import _matmul_broadcast_shape
 from ..utils.deprecation import bool_compat
+from ..utils.generic import _to_helper
 from ..utils.getitem import _noop_index
 from ._linear_operator import LinearOperator, to_dense
 from .dense_linear_operator import DenseLinearOperator, to_linear_operator
 
 
 def cat(inputs, dim=0, output_device=None):
     if all(torch.is_tensor(i) for i in inputs):
@@ -93,15 +94,19 @@
         for tsr_idx, (start_idx, end_idx) in enumerate(zip(cat_dim_cum_sizes[:-1], cat_dim_cum_sizes[1:])):
             idx_to_tensor_idx[start_idx.item() : end_idx.item()].fill_(tsr_idx)
 
         self.cat_dim_sizes = cat_dim_sizes
         self.cat_dim_cum_sizes = cat_dim_cum_sizes
         self.idx_to_tensor_idx = idx_to_tensor_idx
         self._shape = torch.Size(
-            (*rep_tensor.shape[:positive_dim], cat_dim_cum_sizes[-1].item(), *rep_tensor.shape[positive_dim + 1 :])
+            (
+                *rep_tensor.shape[:positive_dim],
+                cat_dim_cum_sizes[-1].item(),
+                *rep_tensor.shape[positive_dim + 1 :],
+            )
         )
 
     def _split_slice(self, slice_idx):
         """
         Splits a slice(a, b, None) in to a list of slices [slice(a1, b1, None), slice(a2, b2, None), ...]
         so that each slice in the list slices in to a single tensor that we have concatenated with this LinearOperator.
         """
@@ -146,15 +151,18 @@
                 n_rows, n_cols = t.shape[-2:]
                 rows = torch.arange(curr_row, curr_row + n_cols, dtype=torch.long, device=t.device)
                 cols = torch.arange(0, n_cols, dtype=torch.long, device=t.device)
                 curr_row += n_cols
                 res.append(t[..., rows, cols].to(self.device))
             res = torch.cat(res, dim=-1)
         else:
-            res = torch.cat([t._diagonal().to(self.device) for t in self.linear_ops], dim=self.cat_dim + 1)
+            res = torch.cat(
+                [t._diagonal().to(self.device) for t in self.linear_ops],
+                dim=self.cat_dim + 1,
+            )
         return res
 
     def _expand_batch(self, batch_shape):
         batch_dim = self.cat_dim + 2
         if batch_dim < 0:
             if batch_shape[batch_dim] != self.batch_shape[batch_dim]:
                 raise RuntimeError(
@@ -359,22 +367,26 @@
         if self.cat_dim == -2:
             new_dim = -1
         elif self.cat_dim == -1:
             new_dim = -2
         else:
             new_dim = self.cat_dim
         return self.__class__(
-            *[t._transpose_nonbatch() for t in self.linear_ops], dim=new_dim, output_device=self.output_device
+            *[t._transpose_nonbatch() for t in self.linear_ops],
+            dim=new_dim,
+            output_device=self.output_device,
         )
 
     def _unsqueeze_batch(self, dim):
         cat_dim = self.dim() + self.cat_dim
         linear_ops = [linear_op._unsqueeze_batch(dim) for linear_op in self.linear_ops]
         res = self.__class__(
-            *linear_ops, dim=(cat_dim + 1 if dim <= cat_dim else cat_dim), output_device=self.output_device
+            *linear_ops,
+            dim=(cat_dim + 1 if dim <= cat_dim else cat_dim),
+            output_device=self.output_device,
         )
         return res
 
     def to_dense(self):
         return torch.cat([to_dense(L) for L in self.linear_ops], dim=self.cat_dim)
 
     def inv_quad_logdet(self, inv_quad_rhs=None, logdet=False, reduce_inv_quad=True):
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/chol_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/chol_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Callable, Optional, Tuple
 
 import torch
 
 from ..utils.memoize import cached
 from ._linear_operator import LinearOperator
 from .root_linear_operator import RootLinearOperator
-from .triangular_linear_operator import TriangularLinearOperator, _TriangularLinearOperatorBase
+from .triangular_linear_operator import _TriangularLinearOperatorBase, TriangularLinearOperator
 
 
 class CholLinearOperator(RootLinearOperator):
     r"""
     A LinearOperator that represents a positive definite matrix given
     a lower trinagular Cholesky factor :math:`\mathbf L`
     (or upper triangular Cholesky factor :math:`\mathbf R`).
@@ -88,15 +88,18 @@
             R = self.root.solve(tensor)
         inv_quad_term = (R**2).sum(dim=-2)
         if inv_quad_term.numel() and reduce_inv_quad:
             inv_quad_term = inv_quad_term.sum(-1)
         return inv_quad_term
 
     def inv_quad_logdet(
-        self, inv_quad_rhs: Optional[torch.Tensor] = None, logdet: bool = False, reduce_inv_quad: bool = True
+        self,
+        inv_quad_rhs: Optional[torch.Tensor] = None,
+        logdet: bool = False,
+        reduce_inv_quad: bool = True,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         if not self.is_square:
             raise RuntimeError(
                 "inv_quad_logdet only operates on (batches of) square (positive semi-definite) LinearOperators. "
                 "Got a {} of size {}.".format(self.__class__.__name__, self.size())
             )
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/constant_mul_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/constant_mul_linear_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,16 @@
     def _matmul(self, rhs):
         res = self.base_linear_op._matmul(rhs)
         res = res * self.expanded_constant
         return res
 
     def _permute_batch(self, *dims):
         return self.__class__(
-            self.base_linear_op._permute_batch(*dims), self._constant.expand(self.batch_shape).permute(*dims)
+            self.base_linear_op._permute_batch(*dims),
+            self._constant.expand(self.batch_shape).permute(*dims),
         )
 
     def _bilinear_derivative(self, left_vecs, right_vecs):
         # Gradient with respect to the constant
         constant_deriv = left_vecs * self.base_linear_op._matmul(right_vecs)
         constant_deriv = constant_deriv.sum(-2).sum(-1)
         while constant_deriv.dim() > self._constant.dim():
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/dense_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/dense_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/diag_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/diag_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,18 @@
     def _expand_batch(self, batch_shape: torch.Size) -> "DiagLinearOperator":
         return self.__class__(self._diag.expand(*batch_shape, self._diag.size(-1)))
 
     def _diagonal(self) -> Tensor:
         return self._diag
 
     def _get_indices(
-        self, row_index: torch.LongTensor, col_index: torch.LongTensor, *batch_indices: Tuple[torch.LongTensor, ...]
+        self,
+        row_index: torch.LongTensor,
+        col_index: torch.LongTensor,
+        *batch_indices: Tuple[torch.LongTensor, ...],
     ) -> Tensor:
         res = self._diag[(*batch_indices, row_index)]
         # If row and col index don't agree, then we have off diagonal elements
         # Those should be zero'd out
         res = res * torch.eq(row_index, col_index).to(device=res.device, dtype=res.dtype)
         return res
 
@@ -118,15 +121,18 @@
     def inverse(self) -> "DiagLinearOperator":
         """
         Returns the inverse of the DiagLinearOperator.
         """
         return self.__class__(self._diag.reciprocal())
 
     def inv_quad_logdet(
-        self, inv_quad_rhs: Optional[Tensor] = None, logdet: bool = False, reduce_inv_quad: bool = True
+        self,
+        inv_quad_rhs: Optional[Tensor] = None,
+        logdet: bool = False,
+        reduce_inv_quad: bool = True,
     ) -> Tuple[Tensor, Tensor]:
         # TODO: Use proper batching for inv_quad_rhs (prepand to shape rathern than append)
         if inv_quad_rhs is None:
             rhs_batch_shape = torch.Size()
         else:
             rhs_batch_shape = inv_quad_rhs.shape[1 + self.batch_dim :]
 
@@ -184,15 +190,19 @@
     def solve(self, right_tensor: Tensor, left_tensor: Optional[Tensor] = None) -> Tensor:
         res = self.inverse()._matmul(right_tensor)
         if left_tensor is not None:
             res = left_tensor @ res
         return res
 
     def solve_triangular(
-        self, rhs: torch.Tensor, upper: bool, left: bool = True, unitriangular: bool = False
+        self,
+        rhs: torch.Tensor,
+        upper: bool,
+        left: bool = True,
+        unitriangular: bool = False,
     ) -> torch.Tensor:
         # upper or lower doesn't matter here, it's all the same
         if unitriangular:
             if not torch.all(self.diagonal() == 1):
                 raise RuntimeError("Received `unitriangular=True` but `LinearOperator` does not have a unit diagonal.")
             return rhs
         return self.solve(right_tensor=rhs)
@@ -328,15 +338,19 @@
 
     def matmul(self, other: Union[Tensor, LinearOperator]) -> Union[Tensor, LinearOperator]:
         if isinstance(other, ConstantDiagLinearOperator):
             return self._mul_matrix(other)
         return super().matmul(other)
 
     def solve_triangular(
-        self, rhs: torch.Tensor, upper: bool, left: bool = True, unitriangular: bool = False
+        self,
+        rhs: torch.Tensor,
+        upper: bool,
+        left: bool = True,
+        unitriangular: bool = False,
     ) -> torch.Tensor:
         return rhs / self.diag_values
 
     def sqrt(self) -> "ConstantDiagLinearOperator":
         """
         Returns a DiagLinearOperator with the square root of all diagonal entries.
         """
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/identity_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/identity_linear_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,21 @@
         self,
         diag_shape: int,
         batch_shape: Optional[torch.Size] = torch.Size([]),
         dtype: Optional[torch.dtype] = None,
         device: Optional[torch.device] = None,
     ):
         one = torch.tensor(1.0, dtype=dtype, device=device)
-        LinearOperator.__init__(self, diag_shape=diag_shape, batch_shape=batch_shape, dtype=dtype, device=device)
+        LinearOperator.__init__(
+            self,
+            diag_shape=diag_shape,
+            batch_shape=batch_shape,
+            dtype=dtype,
+            device=device,
+        )
         self.diag_values = one.expand(torch.Size([*batch_shape, 1]))
         self.diag_shape = diag_shape
         self._batch_shape = batch_shape
         self._dtype = dtype
         self._device = device
 
     @property
@@ -64,29 +70,35 @@
         return self
 
     def _cholesky_solve(self, rhs: torch.Tensor) -> torch.Tensor:
         return self._maybe_reshape_rhs(rhs)
 
     def _expand_batch(self, batch_shape: torch.Size) -> LinearOperator:
         return IdentityLinearOperator(
-            diag_shape=self.diag_shape, batch_shape=batch_shape, dtype=self.dtype, device=self.device
+            diag_shape=self.diag_shape,
+            batch_shape=batch_shape,
+            dtype=self.dtype,
+            device=self.device,
         )
 
     def _getitem(
         self,
         row_index: Union[slice, torch.LongTensor],
         col_index: Union[slice, torch.LongTensor],
         *batch_indices: Tuple[Union[int, slice, torch.LongTensor], ...],
     ) -> LinearOperator:
         # Special case: if both row and col are not indexed, then we are done
         if _is_noop_index(row_index) and _is_noop_index(col_index):
             if len(batch_indices):
                 new_batch_shape = _compute_getitem_size(self, (*batch_indices, row_index, col_index))[:-2]
                 res = IdentityLinearOperator(
-                    diag_shape=self.diag_shape, batch_shape=new_batch_shape, dtype=self._dtype, device=self._device
+                    diag_shape=self.diag_shape,
+                    batch_shape=new_batch_shape,
+                    dtype=self._dtype,
+                    device=self._device,
                 )
                 return res
             else:
                 return self
 
         return super()._getitem(row_index, col_index, *batch_indices)
 
@@ -98,22 +110,28 @@
 
     def _mul_matrix(self, other: Union[torch.Tensor, LinearOperator]) -> LinearOperator:
         return other
 
     def _permute_batch(self, *dims: Tuple[int, ...]) -> LinearOperator:
         batch_shape = self.diag_values.permute(*dims, -1).shape[:-1]
         return IdentityLinearOperator(
-            diag_shape=self.diag_shape, batch_shape=batch_shape, dtype=self._dtype, device=self._device
+            diag_shape=self.diag_shape,
+            batch_shape=batch_shape,
+            dtype=self._dtype,
+            device=self._device,
         )
 
     def _prod_batch(self, dim: int) -> LinearOperator:
         batch_shape = list(self.batch_shape)
         del batch_shape[dim]
         return IdentityLinearOperator(
-            diag_shape=self.diag_shape, batch_shape=torch.Size(batch_shape), dtype=self.dtype, device=self.device
+            diag_shape=self.diag_shape,
+            batch_shape=torch.Size(batch_shape),
+            dtype=self.dtype,
+            device=self.device,
         )
 
     def _root_decomposition(self) -> LinearOperator:
         return self.sqrt()
 
     def _root_inv_decomposition(
         self,
@@ -139,28 +157,34 @@
         return self
 
     def _unsqueeze_batch(self, dim: int) -> IdentityLinearOperator:
         batch_shape = list(self._batch_shape)
         batch_shape.insert(dim, 1)
         batch_shape = torch.Size(batch_shape)
         return IdentityLinearOperator(
-            diag_shape=self.diag_shape, batch_shape=batch_shape, dtype=self.dtype, device=self.device
+            diag_shape=self.diag_shape,
+            batch_shape=batch_shape,
+            dtype=self.dtype,
+            device=self.device,
         )
 
     def abs(self) -> LinearOperator:
         return self
 
     def exp(self) -> LinearOperator:
         return self
 
     def inverse(self) -> LinearOperator:
         return self
 
     def inv_quad_logdet(
-        self, inv_quad_rhs: Optional[torch.Tensor] = None, logdet: bool = False, reduce_inv_quad: bool = True
+        self,
+        inv_quad_rhs: Optional[torch.Tensor] = None,
+        logdet: bool = False,
+        reduce_inv_quad: bool = True,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         # TODO: Use proper batching for inv_quad_rhs (prepand to shape rathern than append)
         if inv_quad_rhs is None:
             inv_quad_term = torch.empty(0, dtype=self.dtype, device=self.device)
         else:
             rhs_batch_shape = inv_quad_rhs.shape[1 + self.batch_dim :]
             inv_quad_term = inv_quad_rhs.mul(inv_quad_rhs).sum(-(1 + len(rhs_batch_shape)))
@@ -172,15 +196,19 @@
         else:
             logdet_term = torch.empty(0, dtype=self.dtype, device=self.device)
 
         return inv_quad_term, logdet_term
 
     def log(self) -> LinearOperator:
         return ZeroLinearOperator(
-            *self._batch_shape, self.diag_shape, self.diag_shape, dtype=self._dtype, device=self._device
+            *self._batch_shape,
+            self.diag_shape,
+            self.diag_shape,
+            dtype=self._dtype,
+            device=self._device,
         )
 
     def matmul(self, other: Union[torch.Tensor, LinearOperator]) -> Union[torch.Tensor, LinearOperator]:
         is_vec = False
         if other.dim() == 1:
             is_vec = True
             other = other.unsqueeze(-1)
@@ -204,13 +232,16 @@
         else:
             sqrt_inv_matmul = lhs @ rhs
             inv_quad = lhs.pow(2).sum(dim=-1)
             return sqrt_inv_matmul, inv_quad
 
     def type(self, dtype: torch.dtype) -> LinearOperator:
         return IdentityLinearOperator(
-            diag_shape=self.diag_shape, batch_shape=self.batch_shape, dtype=dtype, device=self.device
+            diag_shape=self.diag_shape,
+            batch_shape=self.batch_shape,
+            dtype=dtype,
+            device=self.device,
         )
 
     def zero_mean_mvn_samples(self, num_samples: int) -> torch.Tensor:
         base_samples = torch.randn(num_samples, *self.shape[:-1], dtype=self.dtype, device=self.device)
         return base_samples
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/interpolated_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/interpolated_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 from .dense_linear_operator import DenseLinearOperator, to_linear_operator
 from .diag_linear_operator import DiagLinearOperator
 from .root_linear_operator import RootLinearOperator
 
 
 class InterpolatedLinearOperator(LinearOperator):
     def _check_args(
-        self, base_linear_op, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
+        self,
+        base_linear_op,
+        left_interp_indices,
+        left_interp_values,
+        right_interp_indices,
+        right_interp_values,
     ):
         if left_interp_indices.size() != left_interp_values.size():
             return "Expected left_interp_indices ({}) to have the same size as left_interp_values ({})".format(
                 left_interp_indices.size(), left_interp_values.size()
             )
         if right_interp_indices.size() != right_interp_values.size():
             return "Expected right_interp_indices ({}) to have the same size as right_interp_values ({})".format(
@@ -53,63 +58,83 @@
             num_rows = base_linear_op.size(-2)
             left_interp_indices = torch.arange(0, num_rows, dtype=torch.long, device=base_linear_op.device)
             left_interp_indices.unsqueeze_(-1)
             left_interp_indices = left_interp_indices.expand(*base_linear_op.batch_shape, num_rows, 1)
 
         if left_interp_values is None:
             left_interp_values = torch.ones(
-                left_interp_indices.size(), dtype=base_linear_op.dtype, device=base_linear_op.device
+                left_interp_indices.size(),
+                dtype=base_linear_op.dtype,
+                device=base_linear_op.device,
             )
 
         if right_interp_indices is None:
             num_cols = base_linear_op.size(-1)
             right_interp_indices = torch.arange(0, num_cols, dtype=torch.long, device=base_linear_op.device)
             right_interp_indices.unsqueeze_(-1)
             right_interp_indices = right_interp_indices.expand(*base_linear_op.batch_shape, num_cols, 1)
 
         if right_interp_values is None:
             right_interp_values = torch.ones(
-                right_interp_indices.size(), dtype=base_linear_op.dtype, device=base_linear_op.device
+                right_interp_indices.size(),
+                dtype=base_linear_op.dtype,
+                device=base_linear_op.device,
             )
 
         if left_interp_indices.shape[:-2] != base_linear_op.batch_shape:
             try:
                 base_linear_op = base_linear_op._expand_batch(left_interp_indices.shape[:-2])
             except RuntimeError:
                 raise RuntimeError(
                     "interp size ({}) is incompatible with base_linear_op size ({}). ".format(
                         right_interp_indices.size(), base_linear_op.size()
                     )
                 )
 
         super(InterpolatedLinearOperator, self).__init__(
-            base_linear_op, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
+            base_linear_op,
+            left_interp_indices,
+            left_interp_values,
+            right_interp_indices,
+            right_interp_values,
         )
         self.base_linear_op = base_linear_op
         self.left_interp_indices = left_interp_indices
         self.left_interp_values = left_interp_values
         self.right_interp_indices = right_interp_indices
         self.right_interp_values = right_interp_values
 
     def _approx_diagonal(self):
         base_diag_root = self.base_linear_op._diagonal().sqrt()
-        left_res = left_interp(self.left_interp_indices, self.left_interp_values, base_diag_root.unsqueeze(-1))
-        right_res = left_interp(self.right_interp_indices, self.right_interp_values, base_diag_root.unsqueeze(-1))
+        left_res = left_interp(
+            self.left_interp_indices,
+            self.left_interp_values,
+            base_diag_root.unsqueeze(-1),
+        )
+        right_res = left_interp(
+            self.right_interp_indices,
+            self.right_interp_values,
+            base_diag_root.unsqueeze(-1),
+        )
         res = left_res * right_res
         return res.squeeze(-1)
 
     def _diagonal(self):
         if isinstance(self.base_linear_op, RootLinearOperator) and isinstance(
             self.base_linear_op.root, DenseLinearOperator
         ):
             left_interp_vals = left_interp(
-                self.left_interp_indices, self.left_interp_values, self.base_linear_op.root.to_dense()
+                self.left_interp_indices,
+                self.left_interp_values,
+                self.base_linear_op.root.to_dense(),
             )
             right_interp_vals = left_interp(
-                self.right_interp_indices, self.right_interp_values, self.base_linear_op.root.to_dense()
+                self.right_interp_indices,
+                self.right_interp_values,
+                self.base_linear_op.root.to_dense(),
             )
             return (left_interp_vals * right_interp_vals).sum(-1)
         else:
             return super(InterpolatedLinearOperator, self)._diagonal()
 
     def _expand_batch(self, batch_shape):
         return self.__class__(
@@ -337,30 +362,34 @@
         if hasattr(self, "_sparse_left_interp_t_memo"):
             if torch.equal(self._left_interp_indices_memo, left_interp_indices_tensor) and torch.equal(
                 self._left_interp_values_memo, left_interp_values_tensor
             ):
                 return self._sparse_left_interp_t_memo
 
         left_interp_t = sparse.make_sparse_from_indices_and_values(
-            left_interp_indices_tensor, left_interp_values_tensor, self.base_linear_op.size()[-2]
+            left_interp_indices_tensor,
+            left_interp_values_tensor,
+            self.base_linear_op.size()[-2],
         )
         self._left_interp_indices_memo = left_interp_indices_tensor
         self._left_interp_values_memo = left_interp_values_tensor
         self._sparse_left_interp_t_memo = left_interp_t
         return self._sparse_left_interp_t_memo
 
     def _sparse_right_interp_t(self, right_interp_indices_tensor, right_interp_values_tensor):
         if hasattr(self, "_sparse_right_interp_t_memo"):
             if torch.equal(self._right_interp_indices_memo, right_interp_indices_tensor) and torch.equal(
                 self._right_interp_values_memo, right_interp_values_tensor
             ):
                 return self._sparse_right_interp_t_memo
 
         right_interp_t = sparse.make_sparse_from_indices_and_values(
-            right_interp_indices_tensor, right_interp_values_tensor, self.base_linear_op.size()[-1]
+            right_interp_indices_tensor,
+            right_interp_values_tensor,
+            self.base_linear_op.size()[-1],
         )
         self._right_interp_indices_memo = right_interp_indices_tensor
         self._right_interp_values_memo = right_interp_values_tensor
         self._sparse_right_interp_t_memo = right_interp_t
         return self._sparse_right_interp_t_memo
 
     def _sum_batch(self, dim):
@@ -377,29 +406,41 @@
         right_factor = torch.arange(0, right_interp_indices.size(dim), dtype=torch.long, device=self.device)
         right_factor = _pad_with_singletons(right_factor, 0, self.dim() - dim - 1)
         right_factor = right_factor * self.base_linear_op.size(-1)
         right_interp_indices = right_interp_indices.add(right_factor)
 
         # Rearrange the indices and values
         permute_order = (*range(0, dim), *range(dim + 1, self.dim()), dim)
-        left_shape = (*left_interp_indices.shape[:dim], *left_interp_indices.shape[dim + 1 : -1], -1)
-        right_shape = (*right_interp_indices.shape[:dim], *right_interp_indices.shape[dim + 1 : -1], -1)
+        left_shape = (
+            *left_interp_indices.shape[:dim],
+            *left_interp_indices.shape[dim + 1 : -1],
+            -1,
+        )
+        right_shape = (
+            *right_interp_indices.shape[:dim],
+            *right_interp_indices.shape[dim + 1 : -1],
+            -1,
+        )
         left_interp_indices = left_interp_indices.permute(permute_order).reshape(left_shape)
         left_interp_values = left_interp_values.permute(permute_order).reshape(left_shape)
         right_interp_indices = right_interp_indices.permute(permute_order).reshape(right_shape)
         right_interp_values = right_interp_values.permute(permute_order).reshape(right_shape)
 
         # Make the base_lazy tensor block diagonal
         from .block_diag_linear_operator import BlockDiagLinearOperator
 
         block_diag = BlockDiagLinearOperator(self.base_linear_op, block_dim=dim)
 
         # Finally! We have an interpolated lazy tensor again
         return InterpolatedLinearOperator(
-            block_diag, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
+            block_diag,
+            left_interp_indices,
+            left_interp_values,
+            right_interp_indices,
+            right_interp_values,
         )
 
     def double(self, device_id=None):
         # We need to ensure that the indices remain integers.
         new_lt = super().double(device_id=device_id)
         new_lt.left_interp_indices = new_lt.left_interp_indices.type(torch.int64)
         new_lt.right_interp_indices = new_lt.right_interp_indices.type(torch.int64)
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/keops_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/keops_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/kronecker_product_added_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/kronecker_product_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/kronecker_product_linear_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .. import settings
 from ..utils.broadcasting import _matmul_broadcast_shape
 from ..utils.memoize import cached
 from ._linear_operator import LinearOperator
 from .dense_linear_operator import to_linear_operator
 from .diag_linear_operator import ConstantDiagLinearOperator, DiagLinearOperator
-from .triangular_linear_operator import TriangularLinearOperator, _TriangularLinearOperatorBase
+from .triangular_linear_operator import _TriangularLinearOperatorBase, TriangularLinearOperator
 
 
 def _kron_diag(*lts) -> Tensor:
     """Compute diagonal of a KroneckerProductLinearOperator from the diagonals of the constituiting tensors"""
     lead_diag = lts[0]._diagonal()
     if len(lts) == 1:  # base case:
         return lead_diag
@@ -302,15 +302,18 @@
         res = _t_matmul(self.linear_ops, self.shape, rhs.contiguous())
 
         if is_vec:
             res = res.squeeze(-1)
         return res
 
     def _transpose_nonbatch(self):
-        return self.__class__(*(linear_op._transpose_nonbatch() for linear_op in self.linear_ops), **self._kwargs)
+        return self.__class__(
+            *(linear_op._transpose_nonbatch() for linear_op in self.linear_ops),
+            **self._kwargs,
+        )
 
 
 class KroneckerProductTriangularLinearOperator(KroneckerProductLinearOperator, _TriangularLinearOperatorBase):
     def __init__(self, *linear_ops, upper=False):
         if not all(isinstance(lt, TriangularLinearOperator) for lt in linear_ops):
             raise RuntimeError(
                 "Components of KroneckerProductTriangularLinearOperator must be TriangularLinearOperator."
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/linear_operator_representation_tree.py` & `linear_operator-0.4.0/linear_operator/operators/linear_operator_representation_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,20 @@
         self._kwargs = linear_op._kwargs
 
         counter = 0
         self.children = []
         for arg in linear_op._args:
             if hasattr(arg, "representation") and callable(arg.representation):  # Is it a lazy tensor?
                 representation_size = len(arg.representation())
-                self.children.append((slice(counter, counter + representation_size, None), arg.representation_tree()))
+                self.children.append(
+                    (
+                        slice(counter, counter + representation_size, None),
+                        arg.representation_tree(),
+                    )
+                )
                 counter += representation_size
             else:
                 self.children.append((counter, None))
                 counter += 1
 
     def __call__(self, *flattened_representation):
         unflattened_representation = []
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/low_rank_root_added_diag_linear_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
     def _mul_constant(self, constant):
         # We have to over-ride this here for the case where the constant is negative
         if constant > 0:
             res = super()._mul_constant(constant)
         else:
             res = AddedDiagLinearOperator(
-                self._linear_op._mul_constant(constant), self._diag_tensor._mul_constant(constant)
+                self._linear_op._mul_constant(constant),
+                self._diag_tensor._mul_constant(constant),
             )
         return res
 
     def _preconditioner(self):
         return None, None, None
 
     def _solve(self, rhs, preconditioner=None, num_tridiag=0):
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/low_rank_root_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/low_rank_root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/matmul_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/matmul_linear_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         if right_linear_op.batch_shape != batch_shape:
             self.right_linear_op = right_linear_op._expand_batch(batch_shape)
         else:
             self.right_linear_op = right_linear_op
 
     def _expand_batch(self, batch_shape):
         return self.__class__(
-            self.left_linear_op._expand_batch(batch_shape), self.right_linear_op._expand_batch(batch_shape)
+            self.left_linear_op._expand_batch(batch_shape),
+            self.right_linear_op._expand_batch(batch_shape),
         )
 
     def _get_indices(self, row_index, col_index, *batch_indices):
         row_index = row_index.unsqueeze(-1)
         col_index = col_index.unsqueeze(-1)
         batch_indices = tuple(batch_index.unsqueeze(-1) for batch_index in batch_indices)
         inner_index = torch.arange(0, self.left_linear_op.size(-1), device=self.device)
@@ -103,18 +104,24 @@
         right_grad = self.right_linear_op._bilinear_derivative(left_vecs_times_left_linear_op_t, right_vecs)
 
         left_grad = (left_grad,) if not isinstance(left_grad, tuple) else left_grad
         right_grad = (right_grad,) if not isinstance(right_grad, tuple) else right_grad
         return left_grad + right_grad
 
     def _permute_batch(self, *dims):
-        return self.__class__(self.left_linear_op._permute_batch(*dims), self.right_linear_op._permute_batch(*dims))
+        return self.__class__(
+            self.left_linear_op._permute_batch(*dims),
+            self.right_linear_op._permute_batch(*dims),
+        )
 
     def _size(self):
         return _matmul_broadcast_shape(self.left_linear_op.shape, self.right_linear_op.shape)
 
     def _transpose_nonbatch(self, *args):
-        return self.__class__(self.right_linear_op._transpose_nonbatch(), self.left_linear_op._transpose_nonbatch())
+        return self.__class__(
+            self.right_linear_op._transpose_nonbatch(),
+            self.left_linear_op._transpose_nonbatch(),
+        )
 
     @cached
     def to_dense(self):
         return torch.matmul(self.left_linear_op.to_dense(), self.right_linear_op.to_dense())
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/mul_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/mul_linear_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,16 @@
         right_factor = right_factor.view(*batch_shape, n, num_vecs * left_rank)
         right_deriv_args = self.right_linear_op._bilinear_derivative(left_factor, right_factor)
 
         return tuple(list(left_deriv_args) + list(right_deriv_args))
 
     def _expand_batch(self, batch_shape):
         return self.__class__(
-            self.left_linear_op._expand_batch(batch_shape), self.right_linear_op._expand_batch(batch_shape)
+            self.left_linear_op._expand_batch(batch_shape),
+            self.right_linear_op._expand_batch(batch_shape),
         )
 
     @cached
     def to_dense(self):
         return self.left_linear_op.to_dense() * self.right_linear_op.to_dense()
 
     def _size(self):
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/permutation_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/permutation_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/root_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/sum_batch_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/sum_batch_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/sum_kronecker_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/sum_kronecker_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/sum_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/sum_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/toeplitz_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/toeplitz_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/operators/triangular_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/triangular_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,18 @@
 
     def _expand_batch(self, batch_shape: torch.Size) -> "TriangularLinearOperator":
         if len(batch_shape) == 0:
             return self
         return self.__class__(tensor=self._tensor._expand_batch(batch_shape), upper=self.upper)
 
     def _get_indices(
-        self, row_index: torch.LongTensor, col_index: torch.LongTensor, *batch_indices: Tuple[torch.LongTensor, ...]
+        self,
+        row_index: torch.LongTensor,
+        col_index: torch.LongTensor,
+        *batch_indices: Tuple[torch.LongTensor, ...],
     ) -> Tensor:
         return self._tensor._get_indices(row_index, col_index, *batch_indices)
 
     def _matmul(self, rhs: Tensor) -> Tensor:
         return self._tensor.matmul(rhs)
 
     def _mul_constant(self, constant: Tensor) -> "TriangularLinearOperator":
@@ -126,15 +129,14 @@
         """
         return self.__class__(self._tensor.abs(), upper=self.upper)
 
     def add_diagonal(self, added_diag: Tensor) -> "TriangularLinearOperator":
         added_diag_lt = self._tensor.add_diagonal(added_diag)
         return self.__class__(added_diag_lt, upper=self.upper)
 
-    @cached
     def to_dense(self) -> Tensor:
         return self._tensor.to_dense()
 
     def exp(self) -> "TriangularLinearOperator":
         """
         Returns a TriangleLinearOperator with all diagonal entries exponentiated.
         """
@@ -191,15 +193,19 @@
             res = res.squeeze(-1)
 
         if left_tensor is not None:
             res = left_tensor @ res
         return res
 
     def solve_triangular(
-        self, rhs: torch.Tensor, upper: bool, left: bool = True, unitriangular: bool = False
+        self,
+        rhs: torch.Tensor,
+        upper: bool,
+        left: bool = True,
+        unitriangular: bool = False,
     ) -> torch.Tensor:
         if upper != self.upper:
             raise RuntimeError(
                 f"Incompatible argument: {self.__class__.__name__}.solve_triangular called with `upper={upper}`, "
                 f"but `LinearOperator` has `upper={self.upper}`."
             )
         if not left:
```

### Comparing `linear_operator-0.3.0/linear_operator/operators/zero_linear_operator.py` & `linear_operator-0.4.0/linear_operator/operators/zero_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
     :param sizes: The size of each dimension (including batch dimensions).
     :param dtype: Dtype that the LinearOperator will be operating on. (Default: :meth:`torch.get_default_dtype()`).
     :param device: Device that the LinearOperator will be operating on. (Default: CPU).
     """
 
     def __init__(
-        self, *sizes: Tuple[int, ...], dtype: Optional[torch.dtype] = None, device: Optional[torch.device] = None
+        self,
+        *sizes: Tuple[int, ...],
+        dtype: Optional[torch.dtype] = None,
+        device: Optional[torch.device] = None,
     ):
         super(ZeroLinearOperator, self).__init__(*sizes)
         self.sizes = list(sizes)
 
         self._dtype = dtype or torch.get_default_dtype()
         self._device = device or torch.device("cpu")
 
@@ -44,15 +47,18 @@
         shape = self.shape
         return torch.zeros(shape[:-1], dtype=self.dtype, device=self.device)
 
     def _expand_batch(self, batch_shape: torch.Size) -> LinearOperator:
         return self.__class__(*batch_shape, *self.sizes[-2:], dtype=self._dtype, device=self._device)
 
     def _get_indices(
-        self, row_index: torch.LongTensor, col_index: torch.LongTensor, *batch_indices: Tuple[torch.LongTensor, ...]
+        self,
+        row_index: torch.LongTensor,
+        col_index: torch.LongTensor,
+        *batch_indices: Tuple[torch.LongTensor, ...],
     ) -> torch.Tensor:
         new_size = _compute_getitem_size(self, batch_indices + (row_index, col_index))
         return ZeroLinearOperator(*new_size)
 
     def _getitem(
         self,
         row_index: Union[slice, torch.LongTensor],
@@ -162,15 +168,18 @@
     def div(self, other: Union[float, torch.Tensor]) -> LinearOperator:
         return self
 
     def inv_quad(self, inv_quad_rhs: torch.Tensor, reduce_inv_quad: bool = True) -> torch.Tensor:
         raise RuntimeError("ZeroLinearOperators are not invertible!")
 
     def inv_quad_logdet(
-        self, inv_quad_rhs: Optional[torch.Tensor] = None, logdet: bool = False, reduce_inv_quad: bool = True
+        self,
+        inv_quad_rhs: Optional[torch.Tensor] = None,
+        logdet: bool = False,
+        reduce_inv_quad: bool = True,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         raise RuntimeError("ZeroLinearOperators are not invertible!")
 
     def logdet(self) -> torch.Tensor:
         return torch.log(torch.tensor(0.0))
 
     def matmul(self, other: Union[torch.Tensor, LinearOperator]) -> Union[torch.Tensor, LinearOperator]:
```

### Comparing `linear_operator-0.3.0/linear_operator/settings.py` & `linear_operator-0.4.0/linear_operator/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 
 import logging
-import warnings
 
 import torch
 
 
 class _dtype_value_context:
     _global_float_value = None
     _global_double_value = None
@@ -29,21 +28,21 @@
         if float_value is not None:
             cls._global_float_value = float_value
         if double_value is not None:
             cls._global_double_value = double_value
         if half_value is not None:
             cls._global_half_value = half_value
 
-    def __init__(self, float=None, double=None, half=None):
-        self._orig_float_value = self.__class__.value()
-        self._instance_float_value = float
-        self._orig_double_value = self.__class__.value()
-        self._instance_double_value = double
-        self._orig_half_value = self.__class__.value()
-        self._instance_half_value = half
+    def __init__(self, float_value=None, double_value=None, half_value=None):
+        self._orig_float_value = self.__class__.value(dtype=torch.float)
+        self._instance_float_value = float_value
+        self._orig_double_value = self.__class__.value(dtype=torch.double)
+        self._instance_double_value = double_value
+        self._orig_half_value = self.__class__.value(dtype=torch.half)
+        self._instance_half_value = half_value
 
     def __enter__(
         self,
     ):
         self.__class__._set_value(
             self._instance_float_value,
             self._instance_double_value,
@@ -198,25 +197,14 @@
     - Default for `float`: 1e-6
     - Default for `double`: 1e-8
     """
 
     _global_float_value = 1e-6
     _global_double_value = 1e-8
 
-    @classmethod
-    def value(cls, dtype=None):
-        if dtype is None:
-            # Deprecated in 1.4: remove in 1.5
-            warnings.warn(
-                "cholesky_jitter is now a _dtype_value_context and should be called with a dtype argument",
-                DeprecationWarning,
-            )
-            return cls._global_float_value
-        return super().value(dtype=dtype)
-
 
 class cholesky_max_tries(_value_context):
     """
     The max_tries value used by `psd_safe_cholesky` when using cholesky solves.
 
     (Default: 3)
     """
```

### Comparing `linear_operator-0.3.0/linear_operator/test/base_test_case.py` & `linear_operator-0.4.0/linear_operator/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/test/linear_operator_test_case.py` & `linear_operator-0.4.0/linear_operator/test/linear_operator_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,22 +245,28 @@
                 res, actual = linear_op[index], evaluated[index]
                 self.assertAllClose(res, actual)
                 index = (
                     *batch_index,
                     torch.tensor([0, 1, 0, 2]),
                     slice(None, None, None),
                 )
-                res, actual = linear_operator.to_dense(linear_op[index]), evaluated[index]
+                res, actual = (
+                    linear_operator.to_dense(linear_op[index]),
+                    evaluated[index],
+                )
                 self.assertAllClose(res, actual)
                 index = (
                     *batch_index,
                     slice(None, None, None),
                     torch.tensor([0, 1, 2, 1]),
                 )
-                res, actual = linear_operator.to_dense(linear_op[index]), evaluated[index]
+                res, actual = (
+                    linear_operator.to_dense(linear_op[index]),
+                    evaluated[index],
+                )
                 self.assertAllClose(res, actual)
                 index = (*batch_index, slice(None, None, None), slice(None, None, None))
                 res, actual = linear_op[index].to_dense(), evaluated[index]
                 self.assertAllClose(res, actual)
 
             # Ellipsis
             res = linear_op.__getitem__((Ellipsis, torch.tensor([0, 1, 0, 2]), torch.tensor([1, 2, 0, 1])))
@@ -274,18 +280,25 @@
 
     def test_getitem_broadcasted_tensor_index(self):
         linear_op = self.create_linear_op()
         evaluated = self.evaluate_linear_op(linear_op)
 
         # Non-batch case
         if linear_op.ndimension() == 2:
-            index = (torch.tensor([0, 0, 1, 2]).unsqueeze(-1), torch.tensor([0, 1, 0, 2]).unsqueeze(-2))
+            index = (
+                torch.tensor([0, 0, 1, 2]).unsqueeze(-1),
+                torch.tensor([0, 1, 0, 2]).unsqueeze(-2),
+            )
             res, actual = linear_op[index], evaluated[index]
             self.assertAllClose(res, actual)
-            index = (Ellipsis, torch.tensor([0, 0, 1, 2]).unsqueeze(-2), torch.tensor([0, 1, 0, 2]).unsqueeze(-1))
+            index = (
+                Ellipsis,
+                torch.tensor([0, 0, 1, 2]).unsqueeze(-2),
+                torch.tensor([0, 1, 0, 2]).unsqueeze(-1),
+            )
             res, actual = linear_op[index], evaluated[index]
             self.assertAllClose(res, actual)
 
         # Batch case
         else:
             for batch_index in product(
                 [torch.tensor([0, 1, 1]).view(-1, 1, 1), slice(None, None, None)],
@@ -294,35 +307,54 @@
                 index = (
                     *batch_index,
                     torch.tensor([0, 1]).view(-1, 1),
                     torch.tensor([1, 2, 0, 1]).view(1, -1),
                 )
                 res, actual = linear_op[index], evaluated[index]
                 self.assertAllClose(res, actual)
-                res, actual = linear_operator.to_dense(linear_op[index]), evaluated[index]
+                res, actual = (
+                    linear_operator.to_dense(linear_op[index]),
+                    evaluated[index],
+                )
                 self.assertAllClose(res, actual)
                 index = (*batch_index, slice(None, None, None), slice(None, None, None))
                 res, actual = linear_op[index].to_dense(), evaluated[index]
                 self.assertAllClose(res, actual)
 
             # Ellipsis
             res = linear_op.__getitem__(
-                (Ellipsis, torch.tensor([0, 1, 0]).view(-1, 1, 1), torch.tensor([1, 2, 0, 1]).view(1, 1, -1))
+                (
+                    Ellipsis,
+                    torch.tensor([0, 1, 0]).view(-1, 1, 1),
+                    torch.tensor([1, 2, 0, 1]).view(1, 1, -1),
+                )
             )
             actual = evaluated.__getitem__(
-                (Ellipsis, torch.tensor([0, 1, 0]).view(-1, 1, 1), torch.tensor([1, 2, 0, 1]).view(1, 1, -1))
+                (
+                    Ellipsis,
+                    torch.tensor([0, 1, 0]).view(-1, 1, 1),
+                    torch.tensor([1, 2, 0, 1]).view(1, 1, -1),
+                )
             )
             self.assertAllClose(res, actual)
             res = linear_operator.to_dense(
                 linear_op.__getitem__(
-                    (torch.tensor([0, 1, 0]).view(1, -1), Ellipsis, torch.tensor([1, 2, 0, 1]).view(-1, 1))
+                    (
+                        torch.tensor([0, 1, 0]).view(1, -1),
+                        Ellipsis,
+                        torch.tensor([1, 2, 0, 1]).view(-1, 1),
+                    )
                 )
             )
             actual = evaluated.__getitem__(
-                (torch.tensor([0, 1, 0]).view(1, -1), Ellipsis, torch.tensor([1, 2, 0, 1]).view(-1, 1))
+                (
+                    torch.tensor([0, 1, 0]).view(1, -1),
+                    Ellipsis,
+                    torch.tensor([1, 2, 0, 1]).view(-1, 1),
+                )
             )
             self.assertAllClose(res, actual)
 
     def test_permute(self):
         linear_op = self.create_linear_op()
         if linear_op.dim() >= 4:
             evaluated = self.evaluate_linear_op(linear_op)
@@ -504,15 +536,17 @@
                 with linear_operator.settings.num_trace_samples(256), linear_operator.settings.max_cholesky_size(
                     math.inf if cholesky else 0
                 ), linear_operator.settings.cg_tolerance(1e-5):
                     with linear_operator.settings.min_preconditioning_size(
                         4
                     ), linear_operator.settings.max_preconditioner_size(2):
                         res_inv_quad, res_logdet = linear_op.inv_quad_logdet(
-                            inv_quad_rhs=vecs, logdet=True, reduce_inv_quad=reduce_inv_quad
+                            inv_quad_rhs=vecs,
+                            logdet=True,
+                            reduce_inv_quad=reduce_inv_quad,
                         )
 
             actual_inv_quad = evaluated.inverse().matmul(vecs_copy).mul(vecs_copy).sum(-2)
             if reduce_inv_quad:
                 actual_inv_quad = actual_inv_quad.sum(-1)
             actual_logdet = torch.cat(
                 [torch.logdet(flattened_evaluated[i]).unsqueeze(0) for i in range(linear_op.batch_shape.numel())]
```

### Comparing `linear_operator-0.3.0/linear_operator/test/utils.py` & `linear_operator-0.4.0/linear_operator/test/utils.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/utils/__init__.py` & `linear_operator-0.4.0/linear_operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/utils/broadcasting.py` & `linear_operator-0.4.0/linear_operator/utils/broadcasting.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,31 +35,7 @@
     Example:
         >>> x = torch.randn(10, 5)
         >>> _pad_width_singletons(x, 2, 3).shape
         >>> # [1, 1, 10, 5, 1, 1, 1]
     """
     new_shape = [1] * num_singletons_before + list(obj.shape) + [1] * num_singletons_after
     return obj.view(*new_shape)
-
-
-def _to_helper(*args, **kwargs):
-    """
-    Silently plucks out dtype and devices from a list.
-
-    Example:
-        >>> dtype, device = _to_helper(dtype=torch.float, device=torch.device("cpu"))
-        >>> dtype, device = _to_helper(torch.float, torch.device("cpu"))
-    """
-    dtype = kwargs.pop("dtype", None)
-    device = kwargs.pop("device", None)
-
-    if dtype is None:
-        dtype_list = [x for x in args if type(x) is torch.dtype]
-        if len(dtype_list) > 0:
-            dtype = dtype_list[0]
-
-    if device is None:
-        device_list = [x for x in args if type(x) is torch.device]
-        if len(device_list) > 0:
-            device = device_list[0]
-
-    return device, dtype
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/cholesky.py` & `linear_operator-0.4.0/linear_operator/utils/cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/utils/contour_integral_quad.py` & `linear_operator-0.4.0/linear_operator/utils/contour_integral_quad.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,20 @@
     # if not inverse:
     rhs = sqrt_precond_matmul(rhs)
 
     if shifts is None:
         # Determine if init_vecs has extra_dimensions
         num_extra_dims = max(0, rhs.dim() - linear_op.dim())
         lanczos_init = rhs.__getitem__(
-            (*([0] * num_extra_dims), Ellipsis, slice(None, None, None), slice(None, 1, None))
+            (
+                *([0] * num_extra_dims),
+                Ellipsis,
+                slice(None, None, None),
+                slice(None, 1, None),
+            )
         ).expand(*linear_op.shape[:-1], 1)
         with warnings.catch_warnings(), torch.no_grad():
             warnings.simplefilter("ignore", NumericalWarning)  # Supress CG stopping warning
             _, lanczos_mat = linear_cg(
                 lambda v: linear_op._matmul(v),
                 rhs=lanczos_init,
                 n_tridiag=1,
@@ -130,14 +135,20 @@
         if k2.shape != output_batch_shape:
             weights = torch.stack([w.expand(*output_batch_shape, 1, 1) for w in weights], 0)
             shifts = torch.stack([s.expand(output_batch_shape) for s in shifts], 0)
 
     # Compute the solves at the given shifts
     # Do one more matmul if we don't want to include the inverse
     with torch.no_grad():
-        solves = minres(lambda v: linear_op._matmul(v), rhs, value=-1, shifts=shifts, preconditioner=preconditioner)
+        solves = minres(
+            lambda v: linear_op._matmul(v),
+            rhs,
+            value=-1,
+            shifts=shifts,
+            preconditioner=preconditioner,
+        )
     no_shift_solves = solves[0]
     solves = solves[1:]
     if not inverse:
         solves = linear_op._matmul(solves)
 
     return solves, weights, no_shift_solves, shifts
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/deprecation.py` & `linear_operator-0.4.0/linear_operator/utils/deprecation.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,31 @@
 
     return _deprecated_function
 
 
 def _deprecate_kwarg(kwargs, old_kw, new_kw, new_kw_value):
     old_kwarg = kwargs.get(old_kw)
     if old_kwarg is not None:
-        warnings.warn("The `{}` argument is deprecated. Use `{}` instead.".format(old_kw, new_kw), DeprecationWarning)
+        warnings.warn(
+            "The `{}` argument is deprecated. Use `{}` instead.".format(old_kw, new_kw),
+            DeprecationWarning,
+        )
         if new_kw_value is not None:
             raise ValueError("Cannot set both `{}` and `{}`".format(old_kw, new_kw))
         return old_kwarg
     return new_kw_value
 
 
 def _deprecate_kwarg_with_transform(kwargs, old_kw, new_kw, new_kw_value, transform):
     old_kwarg = kwargs.get(old_kw)
     if old_kwarg is not None:
-        warnings.warn("The `{}` argument is deprecated. Use `{}` instead.".format(old_kw, new_kw), DeprecationWarning)
+        warnings.warn(
+            "The `{}` argument is deprecated. Use `{}` instead.".format(old_kw, new_kw),
+            DeprecationWarning,
+        )
         return transform(old_kwarg)
     return new_kw_value
 
 
 def _deprecated_renamed_method(cls, old_method_name, new_method_name):
     def _deprecated_method(self, *args, **kwargs):
         warnings.warn(
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/getitem.py` & `linear_operator-0.4.0/linear_operator/utils/getitem.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from .broadcasting import _pad_with_singletons
 
 # A slice that does nothing to a dimension
 _noop_index = slice(None, None, None)
 
 
 def _compute_getitem_size(
-    obj: Union[torch.Tensor, "LinearOperator"], indices: Tuple[Union[slice, torch.LongTensor, int], ...]  # noqa F811
+    obj: Union[torch.Tensor, "LinearOperator"],  # noqa F821
+    indices: Tuple[Union[slice, torch.LongTensor, int], ...],  # noqa F811
 ) -> torch.Size:
     """
     Given an object and a tuple of indices, computes the final size of the
     Indices is a tuple containing ints, slices, and tensors
 
     .. note::
         The length of indices must match the dimensionality of obj
@@ -88,15 +89,16 @@
     if tensor_idx is not None:
         final_shape = final_shape[:tensor_idx] + list(tensor_idx_shape) + final_shape[tensor_idx:]
 
     return torch.Size(final_shape)
 
 
 def _convert_indices_to_tensors(
-    obj: Union[torch.Tensor, "LinearOperator"], indices: Tuple[Union[slice, torch.LongTensor, int], ...]  # noqa F811
+    obj: Union[torch.Tensor, "LinearOperator"],  # noqa F821
+    indices: Tuple[Union[slice, torch.LongTensor, int], ...],  # noqa F811
 ) -> Tuple[torch.LongTensor, ...]:
     """
     Given an index made up of tensors/slices/ints, returns a tensor-only index that has the
     same outcome as the original index (when applied to the obj)
 
     .. note::
         The length of indices must match the dimensionality of obj
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/interpolation.py` & `linear_operator-0.4.0/linear_operator/utils/interpolation.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,17 @@
     interp_indices = interp_indices.expand(*batch_shape, *interp_indices.shape[-2:]).contiguous()
     batch_indices = torch.arange(0, batch_size, dtype=torch.long, device=values.device).unsqueeze_(1)
     batch_indices = batch_indices.repeat(1, num_data * num_interp)
     column_indices = torch.arange(0, num_data * num_interp, dtype=torch.long, device=values.device).unsqueeze_(1)
     column_indices = column_indices.repeat(batch_size, 1)
     summing_matrix_indices = torch.stack([batch_indices.view(-1), interp_indices.view(-1), column_indices.view(-1)], 0)
     summing_matrix_values = torch.ones(
-        batch_size * num_data * num_interp, dtype=interp_values.dtype, device=interp_values.device
+        batch_size * num_data * num_interp,
+        dtype=interp_values.dtype,
+        device=interp_values.device,
     )
     size = torch.Size((batch_size, output_dim, num_data * num_interp))
     type_name = summing_matrix_values.type().split(".")[-1]  # e.g. FloatTensor
     if interp_values.is_cuda:
         cls = getattr(torch.cuda.sparse, type_name)
     else:
         cls = getattr(torch.sparse, type_name)
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/lanczos.py` & `linear_operator-0.4.0/linear_operator/utils/lanczos.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,22 @@
             f"Running Lanczos on a {matrix_shape} matrix with a {init_vecs.shape} RHS for {num_iter} iterations."
         )
 
     # Create storage for q_mat, alpha,and beta
     # q_mat - batch version of Q - orthogonal matrix of decomp
     # alpha - batch version main diagonal of T
     # beta - batch version of off diagonal of T
-    q_mat = torch.zeros(num_iter, *batch_shape, matrix_shape[-1], num_init_vecs, dtype=dtype, device=device)
+    q_mat = torch.zeros(
+        num_iter,
+        *batch_shape,
+        matrix_shape[-1],
+        num_init_vecs,
+        dtype=dtype,
+        device=device,
+    )
     t_mat = torch.zeros(num_iter, num_iter, *batch_shape, num_init_vecs, dtype=dtype, device=device)
 
     # Begin algorithm
     # Initial Q vector: q_0_vec
     q_0_vec = init_vecs / torch.norm(init_vecs, 2, dim=dim_dimension).unsqueeze(dim_dimension)
     q_mat[0].copy_(q_0_vec)
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/linear_cg.py` & `linear_operator-0.4.0/linear_operator/utils/linear_cg.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,24 @@
 
 def _default_preconditioner(x):
     return x.clone()
 
 
 @torch.jit.script
 def _jit_linear_cg_updates(
-    result, alpha, residual_inner_prod, eps, beta, residual, precond_residual, mul_storage, is_zero, curr_conjugate_vec
+    result,
+    alpha,
+    residual_inner_prod,
+    eps,
+    beta,
+    residual,
+    precond_residual,
+    mul_storage,
+    is_zero,
+    curr_conjugate_vec,
 ):
     # # Update result
     # # result_{k} = result_{k-1} + alpha_{k} p_vec_{k-1}
     result = torch.addcmul(result, alpha, curr_conjugate_vec, out=result)
 
     # beta_{k} = (precon_residual{k}^T r_vec_{k}) / (precon_residual{k-1}^T r_vec_{k-1})
     beta.resize_as_(residual_inner_prod).copy_(residual_inner_prod)
@@ -209,15 +218,20 @@
         alpha = torch.empty(*batch_shape, 1, rhs.size(-1), dtype=residual.dtype, device=residual.device)
         beta = torch.empty_like(alpha)
         is_zero = torch.empty(*batch_shape, 1, rhs.size(-1), dtype=bool_compat, device=residual.device)
 
     # Define tridiagonal matrices, if applicable
     if n_tridiag:
         t_mat = torch.zeros(
-            n_tridiag_iter, n_tridiag_iter, *batch_shape, n_tridiag, dtype=alpha.dtype, device=alpha.device
+            n_tridiag_iter,
+            n_tridiag_iter,
+            *batch_shape,
+            n_tridiag,
+            dtype=alpha.dtype,
+            device=alpha.device,
         )
         alpha_tridiag_is_zero = torch.empty(*batch_shape, n_tridiag, dtype=bool_compat, device=t_mat.device)
         alpha_reciprocal = torch.empty(*batch_shape, n_tridiag, dtype=t_mat.dtype, device=t_mat.device)
         prev_alpha_reciprocal = torch.empty_like(alpha_reciprocal)
         prev_beta = torch.empty_like(alpha_reciprocal)
 
     update_tridiag = True
@@ -332,10 +346,13 @@
         )
 
     if is_vector:
         result = result.squeeze(-1)
 
     if n_tridiag:
         t_mat = t_mat[: last_tridiag_iter + 1, : last_tridiag_iter + 1]
-        return result, t_mat.permute(-1, *range(2, 2 + len(batch_shape)), 0, 1).contiguous()
+        return (
+            result,
+            t_mat.permute(-1, *range(2, 2 + len(batch_shape)), 0, 1).contiguous(),
+        )
     else:
         return result
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/memoize.py` & `linear_operator-0.4.0/linear_operator/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/utils/minres.py` & `linear_operator-0.4.0/linear_operator/utils/minres.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 
 import torch
 
 from .. import settings
 from .broadcasting import _pad_with_singletons
 
 
-def minres(matmul_closure, rhs, eps=1e-25, shifts=None, value=None, max_iter=None, preconditioner=None):
+def minres(
+    matmul_closure,
+    rhs,
+    eps=1e-25,
+    shifts=None,
+    value=None,
+    max_iter=None,
+    preconditioner=None,
+):
     r"""
     Perform MINRES to find solutions to :math:`(\mathbf K + \alpha \sigma \mathbf I) \mathbf x = \mathbf b`.
     Will find solutions for multiple shifts :math:`\sigma` at the same time.
 
     :param callable matmul_closure: Function to perform matmul with.
     :param torch.Tensor rhs: The vector :math:`\mathbf b` to solve against.
     :param torch.Tensor shifts: (default None) The shift :math:`\sigma` values. If set to None,
@@ -99,15 +107,20 @@
     # 2) The "scaling" terms of the search vectors
     # Equivalent to the terms of V^T Q^T rhs, where Q is the matrix of Lanczos vectors and
     # V is the QR orthonormal of the tridiagonal Lanczos matrix.
     scale_prev = beta_prev.repeat(shifts.size(0), *([1] * beta_prev.dim()))
     scale_curr = torch.empty_like(scale_prev)
 
     # Terms for checking for convergence
-    solution_norm = torch.zeros(*solution.shape[:-2], solution.size(-1), dtype=solution.dtype, device=solution.device)
+    solution_norm = torch.zeros(
+        *solution.shape[:-2],
+        solution.size(-1),
+        dtype=solution.dtype,
+        device=solution.device,
+    )
     search_update_norm = torch.zeros_like(solution_norm)
 
     # Maybe log
     if settings.verbose_linalg.on():
         settings.verbose_linalg.logger.debug(
             f"Running MINRES on a {rhs.shape} RHS for {max_iter} iterations (tol={settings.minres_tolerance.value()}). "
             f"Output: {solution.shape}."
@@ -179,15 +192,19 @@
         zvec_prev2, zvec_prev1 = zvec_prev1, prod
         qvec_prev1 = qvec_curr
         beta_prev, beta_curr = beta_curr, beta_prev
         # Givens rotations terms
         cos_prev2, cos_prev1, cos_curr = cos_prev1, cos_curr, cos_prev2
         sin_prev2, sin_prev1, sin_curr = sin_prev1, sin_curr, sin_prev2
         # Search vector terms)
-        search_prev2, search_prev1, search_curr = search_prev1, search_curr, search_prev2
+        search_prev2, search_prev1, search_curr = (
+            search_prev1,
+            search_curr,
+            search_prev2,
+        )
         scale_prev, scale_curr = scale_curr, scale_prev
 
     # For rhs-s that are close to zero, set them to zero
     solution.masked_fill_(rhs_is_zero, 0)
 
     if squeeze:
         solution = solution.squeeze(-1)
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/permutation.py` & `linear_operator-0.4.0/linear_operator/utils/permutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,23 @@
     # If we don't have a left_permutation vector, we'll just use a slice
     if left_permutation is None:
         left_permutation = torch.arange(matrix.size(-2), device=matrix.device)
     if right_permutation is None:
         right_permutation = torch.arange(matrix.size(-1), device=matrix.device)
 
     # Apply permutations
-    return to_dense(matrix.__getitem__((*batch_idx, left_permutation.unsqueeze(-1), right_permutation.unsqueeze(-2))))
+    return to_dense(
+        matrix.__getitem__(
+            (
+                *batch_idx,
+                left_permutation.unsqueeze(-1),
+                right_permutation.unsqueeze(-2),
+            )
+        )
+    )
 
 
 def inverse_permutation(permutation):
     r"""
     Given a (batch of) permutation vector(s),
     return a permutation vector that inverts the original permutation.
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/pinverse.py` & `linear_operator-0.4.0/linear_operator/utils/pinverse.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/utils/qr.py` & `linear_operator-0.4.0/linear_operator/utils/qr.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/utils/sparse.py` & `linear_operator-0.4.0/linear_operator/utils/sparse.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,18 @@
 
     # Index tensor
     batch_tensors = []
     for i, batch_size in enumerate(batch_shape):
         batch_tensor = torch.arange(0, batch_size, dtype=torch.long, device=interp_values.device)
         batch_tensor = (
             batch_tensor.unsqueeze_(1)
-            .repeat(batch_shape[:i].numel(), batch_shape[i + 1 :].numel() * n_target_points * n_coefficients)
+            .repeat(
+                batch_shape[:i].numel(),
+                batch_shape[i + 1 :].numel() * n_target_points * n_coefficients,
+            )
             .view(-1)
         )
         batch_tensors.append(batch_tensor)
 
     row_tensor = torch.arange(0, n_target_points, dtype=torch.long, device=interp_values.device)
     row_tensor = row_tensor.unsqueeze_(1).repeat(batch_shape.numel(), n_coefficients).view(-1)
     index_tensor = torch.stack([*batch_tensors, interp_indices.reshape(-1), row_tensor], 0)
@@ -154,15 +157,18 @@
 
     for i, idx in list(enumerate(idxs))[::-1]:
         if isinstance(idx, int):
             del size[i]
             mask = indices[i].eq(idx)
             if torch.any(mask):
                 new_indices = torch.zeros(
-                    indices.size(0) - 1, torch.sum(mask), dtype=indices.dtype, device=indices.device
+                    indices.size(0) - 1,
+                    torch.sum(mask),
+                    dtype=indices.dtype,
+                    device=indices.device,
                 )
                 for j in range(indices.size(0)):
                     if i > j:
                         new_indices[j].copy_(indices[j][mask])
                     elif i < j:
                         new_indices[j - 1].copy_(indices[j][mask])
                 indices = new_indices
@@ -177,15 +183,20 @@
         elif isinstance(idx, slice):
             start, stop, step = idx.indices(size[i])
             size = list(size[:i]) + [stop - start] + list(size[i + 1 :])
             if step != 1:
                 raise RuntimeError("Slicing with step is not supported")
             mask = indices[i].lt(stop) & indices[i].ge(start)
             if torch.any(mask):
-                new_indices = torch.zeros(indices.size(0), torch.sum(mask), dtype=indices.dtype, device=indices.device)
+                new_indices = torch.zeros(
+                    indices.size(0),
+                    torch.sum(mask),
+                    dtype=indices.dtype,
+                    device=indices.device,
+                )
                 for j in range(indices.size(0)):
                     new_indices[j].copy_(indices[j][mask])
                 new_indices[i].sub_(start)
                 indices = new_indices
                 values = values[mask]
             else:
                 indices.resize_(indices.size(0), 1).zero_()
@@ -203,15 +214,20 @@
         repeat_sizes = repeat_sizes[0]
 
     if len(repeat_sizes) > len(sparse.shape):
         num_new_dims = len(repeat_sizes) - len(sparse.shape)
         new_indices = sparse._indices()
         new_indices = torch.cat(
             [
-                torch.zeros(num_new_dims, new_indices.size(1), dtype=new_indices.dtype, device=new_indices.device),
+                torch.zeros(
+                    num_new_dims,
+                    new_indices.size(1),
+                    dtype=new_indices.dtype,
+                    device=new_indices.device,
+                ),
                 new_indices,
             ],
             0,
         )
         sparse = torch.sparse_coo_tensor(
             new_indices,
             sparse._values(),
@@ -226,15 +242,21 @@
             adding_factor = torch.arange(0, repeat_size, dtype=new_indices.dtype, device=new_indices.device).unsqueeze_(
                 1
             )
             new_indices[i].view(repeat_size, -1).add_(adding_factor)
             sparse = torch.sparse_coo_tensor(
                 new_indices,
                 sparse._values().repeat(repeat_size),
-                torch.Size((*sparse.shape[:i], repeat_size * sparse.size(i), *sparse.shape[i + 1 :])),
+                torch.Size(
+                    (
+                        *sparse.shape[:i],
+                        repeat_size * sparse.size(i),
+                        *sparse.shape[i + 1 :],
+                    )
+                ),
                 dtype=sparse.dtype,
                 device=sparse.device,
             )
 
     return sparse
```

### Comparing `linear_operator-0.3.0/linear_operator/utils/stochastic_lq.py` & `linear_operator-0.4.0/linear_operator/utils/stochastic_lq.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/linear_operator/utils/toeplitz.py` & `linear_operator-0.4.0/linear_operator/utils/toeplitz.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,18 @@
     if type(toeplitz_column) != type(toeplitz_row):
         raise RuntimeError("toeplitz_column and toeplitz_row should be the same type.")
 
     if len(toeplitz_column) == 1:
         return toeplitz_column.view(1, 1)
 
     res = torch.empty(
-        len(toeplitz_column), len(toeplitz_column), dtype=toeplitz_column.dtype, device=toeplitz_column.device
+        len(toeplitz_column),
+        len(toeplitz_column),
+        dtype=toeplitz_column.dtype,
+        device=toeplitz_column.device,
     )
     for i, val in enumerate(toeplitz_column):
         for j in range(len(toeplitz_column) - i):
             res[j + i, j] = val
     for i, val in list(enumerate(toeplitz_row))[1:]:
         for j in range(len(toeplitz_row) - i):
             res[j, j + i] = val
```

### Comparing `linear_operator-0.3.0/linear_operator.egg-info/PKG-INFO` & `linear_operator-0.4.0/linear_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-operator
-Version: 0.3.0
+Version: 0.4.0
 Summary: A linear operator implementation, primarily designed for finite-dimensional positive definite operators (i.e. kernel matrices).
 Home-page: UNKNOWN
 Author: Geoff Pleiss
 Author-email: gpleiss@gmail.com
 License: MIT
 Project-URL: Documentation, https://linear_operator.readthedocs.io
 Project-URL: Source, https://github.com/cornellius-gp/linear_operator/
```

### Comparing `linear_operator-0.3.0/linear_operator.egg-info/SOURCES.txt` & `linear_operator-0.4.0/linear_operator.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -89,28 +89,30 @@
 linear_operator/test/utils.py
 linear_operator/utils/__init__.py
 linear_operator/utils/broadcasting.py
 linear_operator/utils/cholesky.py
 linear_operator/utils/contour_integral_quad.py
 linear_operator/utils/deprecation.py
 linear_operator/utils/errors.py
+linear_operator/utils/generic.py
 linear_operator/utils/getitem.py
 linear_operator/utils/interpolation.py
 linear_operator/utils/lanczos.py
 linear_operator/utils/linear_cg.py
 linear_operator/utils/memoize.py
 linear_operator/utils/minres.py
 linear_operator/utils/permutation.py
 linear_operator/utils/pinverse.py
 linear_operator/utils/qr.py
 linear_operator/utils/sparse.py
 linear_operator/utils/stochastic_lq.py
 linear_operator/utils/toeplitz.py
 linear_operator/utils/warnings.py
 test/__init__.py
+test/test_settings.py
 test/functions/__init__.py
 test/functions/test_diagonalization.py
 test/functions/test_dsmm.py
 test/functions/test_inv_quad.py
 test/functions/test_inv_quad_logdet.py
 test/functions/test_matmul.py
 test/functions/test_pivoted_cholesky.py
@@ -141,14 +143,15 @@
 test/operators/test_sum_kronecker_linear_operator.py
 test/operators/test_sum_linear_operator.py
 test/operators/test_toeplitz_linear_operator.py
 test/operators/test_triangular_linear_operator.py
 test/operators/test_zero_linear_operator.py
 test/utils/__init__.py
 test/utils/test_cholesky.py
+test/utils/test_generic.py
 test/utils/test_getitem.py
 test/utils/test_interpolation.py
 test/utils/test_lanczos.py
 test/utils/test_linear_cg.py
 test/utils/test_minres.py
 test/utils/test_permutation.py
 test/utils/test_sparse.py
```

### Comparing `linear_operator-0.3.0/setup.py` & `linear_operator-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,17 +64,20 @@
     author="Geoff Pleiss",
     author_email="gpleiss@gmail.com",
     project_urls={
         "Documentation": "https://linear_operator.readthedocs.io",
         "Source": "https://github.com/cornellius-gp/linear_operator/",
     },
     license="MIT",
-    classifiers=["Development Status :: 2 - Pre-Alpha", "Programming Language :: Python :: 3"],
+    classifiers=[
+        "Development Status :: 2 - Pre-Alpha",
+        "Programming Language :: Python :: 3",
+    ],
     packages=find_packages(exclude=["test", "test.*"]),
     python_requires=">=3.8",
     install_requires=install_requires,
     extras_require={
-        "dev": ["black", "twine", "pre-commit"],
-        "test": ["flake8==4.0.1", "flake8-print==4.0.0"],
+        "dev": ["ufmt", "twine", "pre-commit"],
+        "test": ["flake8==5.0.4", "flake8-print==5.0.0"],
     },
     test_suite="test",
 )
```

### Comparing `linear_operator-0.3.0/test/functions/test_diagonalization.py` & `linear_operator-0.4.0/test/functions/test_diagonalization.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/functions/test_dsmm.py` & `linear_operator-0.4.0/test/functions/test_dsmm.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,26 +15,35 @@
         dense = torch.randn(3, 3)
 
         res = linear_operator.dsmm(sparse, dense)
         actual = torch.mm(sparse.to_dense(), dense)
         self.assertLess(torch.norm(res - actual), 1e-5)
 
     def test_forward_batch(self):
-        i = torch.tensor([[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]], dtype=torch.long)
+        i = torch.tensor(
+            [[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]],
+            dtype=torch.long,
+        )
         v = torch.tensor([3, 4, 5, 6, 7, 8], dtype=torch.float)
         sparse = torch.sparse.FloatTensor(i, v, torch.Size([2, 2, 3]))
         dense = torch.randn(2, 3, 3)
 
         res = linear_operator.dsmm(sparse, dense)
         actual = torch.matmul(sparse.to_dense(), dense)
         self.assertLess(torch.norm(res - actual), 1e-5)
 
     def test_forward_multi_batch(self):
         i = torch.tensor(
-            [[0, 1, 1, 0, 0, 1], [0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]], dtype=torch.long
+            [
+                [0, 1, 1, 0, 0, 1],
+                [0, 0, 0, 1, 1, 1],
+                [0, 1, 1, 0, 1, 1],
+                [2, 0, 2, 2, 0, 2],
+            ],
+            dtype=torch.long,
         )
         v = torch.tensor([3, 4, 5, 6, 7, 8], dtype=torch.float)
         sparse = torch.sparse.FloatTensor(i, v, torch.Size([2, 2, 2, 3]))
         dense = torch.randn(2, 2, 3, 3)
 
         res = linear_operator.dsmm(sparse, dense)
         actual = torch.matmul(sparse.to_dense(), dense)
@@ -51,30 +60,39 @@
         res = linear_operator.dsmm(sparse, dense)
         res.backward(grad_output)
         actual = torch.mm(sparse.to_dense(), dense_copy)
         actual.backward(grad_output)
         self.assertLess(torch.norm(dense.grad - dense_copy.grad).item(), 1e-5)
 
     def test_backward_batch(self):
-        i = torch.tensor([[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]], dtype=torch.long)
+        i = torch.tensor(
+            [[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]],
+            dtype=torch.long,
+        )
         v = torch.tensor([3, 4, 5, 6, 7, 8], dtype=torch.float)
         sparse = torch.sparse.FloatTensor(i, v, torch.Size([2, 2, 3]))
         dense = torch.randn(2, 3, 4, requires_grad=True)
         dense_copy = dense.clone().detach().requires_grad_(True)
         grad_output = torch.randn(2, 2, 4)
 
         res = linear_operator.dsmm(sparse, dense)
         res.backward(grad_output)
         actual = torch.matmul(sparse.to_dense(), dense_copy)
         actual.backward(grad_output)
         self.assertLess(torch.norm(dense.grad - dense_copy.grad).item(), 1e-5)
 
     def test_backward_multi_batch(self):
         i = torch.tensor(
-            [[0, 1, 1, 0, 0, 1], [0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]], dtype=torch.long
+            [
+                [0, 1, 1, 0, 0, 1],
+                [0, 0, 0, 1, 1, 1],
+                [0, 1, 1, 0, 1, 1],
+                [2, 0, 2, 2, 0, 2],
+            ],
+            dtype=torch.long,
         )
         v = torch.tensor([3, 4, 5, 6, 7, 8], dtype=torch.float)
         sparse = torch.sparse.FloatTensor(i, v, torch.Size([2, 2, 2, 3]))
         dense = torch.randn(2, 2, 3, 4, requires_grad=True)
         dense_copy = dense.clone().detach().requires_grad_(True)
         grad_output = torch.randn(2, 2, 2, 4)
 
@@ -96,15 +114,18 @@
         self.assertLess(torch.norm(res - actual), 1e-5)
 
         grad_output = torch.randn(4, 2, 2, 4)
         res.backward(grad_output)
         actual.backward(grad_output)
         self.assertLess(torch.norm(dense.grad - dense_copy.grad).item(), 1e-5)
 
-        i = torch.tensor([[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]], dtype=torch.long)
+        i = torch.tensor(
+            [[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]],
+            dtype=torch.long,
+        )
         v = torch.tensor([3, 4, 5, 6, 7, 8], dtype=torch.float)
         sparse = torch.sparse.FloatTensor(i, v, torch.Size([2, 2, 3]))
         dense = torch.randn(4, 2, 3, 4, requires_grad=True)
         dense_copy = dense.clone().detach().requires_grad_(True)
 
         res = linear_operator.dsmm(sparse, dense)
         actual = torch.matmul(sparse.to_dense(), dense_copy)
@@ -112,15 +133,18 @@
 
         grad_output = torch.randn(4, 2, 2, 4)
         res.backward(grad_output)
         actual.backward(grad_output)
         self.assertLess(torch.norm(dense.grad - dense_copy.grad).item(), 1e-5)
 
     def test_broadcast_sparse(self):
-        i = torch.tensor([[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]], dtype=torch.long)
+        i = torch.tensor(
+            [[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]],
+            dtype=torch.long,
+        )
         v = torch.tensor([3, 4, 5, 6, 7, 8], dtype=torch.float)
         sparse = torch.sparse.FloatTensor(i, v, torch.Size([2, 2, 3]))
         dense = torch.randn(3, 4, requires_grad=True)
         dense_copy = dense.clone().detach().requires_grad_(True)
 
         res = linear_operator.dsmm(sparse, dense)
         actual = torch.matmul(sparse.to_dense(), dense_copy)
@@ -128,15 +152,18 @@
 
         grad_output = torch.randn(2, 2, 4)
         res.backward(grad_output)
         actual.backward(grad_output)
         self.assertLess(torch.norm(dense.grad - dense_copy.grad).item(), 1e-5)
 
     def test_broadcast_singleton(self):
-        i = torch.tensor([[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]], dtype=torch.long)
+        i = torch.tensor(
+            [[0, 0, 0, 1, 1, 1], [0, 1, 1, 0, 1, 1], [2, 0, 2, 2, 0, 2]],
+            dtype=torch.long,
+        )
         v = torch.tensor([3, 4, 5, 6, 7, 8], dtype=torch.float)
         sparse = torch.sparse.FloatTensor(i, v, torch.Size([2, 2, 3]))
         dense = torch.randn(1, 3, 4, requires_grad=True)
         dense_copy = dense.clone().detach().requires_grad_(True)
 
         res = linear_operator.dsmm(sparse, dense)
         actual = torch.matmul(sparse.to_dense(), dense_copy)
```

### Comparing `linear_operator-0.3.0/test/functions/test_inv_quad.py` & `linear_operator-0.4.0/test/functions/test_inv_quad.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/functions/test_inv_quad_logdet.py` & `linear_operator-0.4.0/test/functions/test_inv_quad_logdet.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/functions/test_matmul.py` & `linear_operator-0.4.0/test/functions/test_matmul.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/functions/test_pivoted_cholesky.py` & `linear_operator-0.4.0/test/functions/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/functions/test_root_decomposition.py` & `linear_operator-0.4.0/test/functions/test_root_decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,18 @@
         mat = self._create_mat().detach().requires_grad_(True)
         mat_clone = mat.detach().clone().requires_grad_(True)
 
         # Forward
         probe_vectors = torch.randn(*mat.shape[:-2], 4, 5)
         test_vectors = torch.randn(*mat.shape[:-2], 4, 5)
         root = linear_operator.root_inv_decomposition(
-            mat, method="lanczos", initial_vectors=probe_vectors, test_vectors=test_vectors
+            mat,
+            method="lanczos",
+            initial_vectors=probe_vectors,
+            test_vectors=test_vectors,
         ).root.to_dense()
         res = root.matmul(root.mT)
         actual = mat_clone.inverse()
         self.assertAllClose(res, actual)
 
         # Backward
         sum([mat.trace() for mat in res.view(-1, mat.size(-2), mat.size(-1))]).backward()
```

### Comparing `linear_operator-0.3.0/test/functions/test_solve.py` & `linear_operator-0.4.0/test/functions/test_solve.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_added_diag_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_added_diag_linear_operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,20 @@
     seed = 4
     should_test_sample = True
 
     def create_linear_op(self):
         tensor = torch.randn(3, 5, 5)
         tensor = tensor.mT.matmul(tensor).detach()
         diag = torch.tensor(
-            [[1.0, 2.0, 4.0, 2.0, 3.0], [2.0, 1.0, 2.0, 1.0, 4.0], [1.0, 2.0, 2.0, 3.0, 4.0]], requires_grad=True
+            [
+                [1.0, 2.0, 4.0, 2.0, 3.0],
+                [2.0, 1.0, 2.0, 1.0, 4.0],
+                [1.0, 2.0, 2.0, 3.0, 4.0],
+            ],
+            requires_grad=True,
         )
         return AddedDiagLinearOperator(DenseLinearOperator(tensor), DiagLinearOperator(diag))
 
     def evaluate_linear_op(self, linear_op):
         diag = linear_op._diag_tensor._diag
         tensor = linear_op._linear_op.tensor
         return tensor + torch.diag_embed(diag, dim1=-2, dim2=-1)
@@ -54,15 +59,20 @@
     skip_slq_tests = True
 
     def create_linear_op(self):
         tensor = torch.randn(4, 3, 5, 5)
         tensor = tensor.mT.matmul(tensor).detach()
         diag = (
             torch.tensor(
-                [[1.0, 2.0, 4.0, 2.0, 3.0], [2.0, 1.0, 2.0, 1.0, 4.0], [1.0, 2.0, 2.0, 3.0, 4.0]], requires_grad=True
+                [
+                    [1.0, 2.0, 4.0, 2.0, 3.0],
+                    [2.0, 1.0, 2.0, 1.0, 4.0],
+                    [1.0, 2.0, 2.0, 3.0, 4.0],
+                ],
+                requires_grad=True,
             )
             .repeat(4, 1, 1)
             .detach()
         )
         return AddedDiagLinearOperator(DenseLinearOperator(tensor), DiagLinearOperator(diag))
 
     def evaluate_linear_op(self, linear_op):
@@ -93,15 +103,17 @@
             def precond_closure(rhs):
                 rhs2 = top_100_evecs.t() @ rhs
                 return top_100_evecs @ torch.diag_embed(1.0 / top_100_evals) @ rhs2
 
             return precond_closure, precond_lt, logdet
 
         overrode_lt = AddedDiagLinearOperator(
-            RootLinearOperator(tensor), DiagLinearOperator(diag), preconditioner_override=nonstandard_preconditioner
+            RootLinearOperator(tensor),
+            DiagLinearOperator(diag),
+            preconditioner_override=nonstandard_preconditioner,
         )
 
         # compute a solve - mostly to make sure that we can actually perform the solve
         rhs = torch.randn(1000, 1)
         standard_solve = standard_lt.solve(rhs)
         overrode_solve = overrode_lt.solve(rhs)
```

### Comparing `linear_operator-0.3.0/test/operators/test_batch_repeat_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_batch_repeat_linear_operator.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 class TestBatchRepeatLinearOperatorMultiBatch(LinearOperatorTestCase, unittest.TestCase):
     seed = 0
     # Because these LTs are large, we'll skil the big tests
     skip_slq_tests = True
 
     def create_linear_op(self):
         toeplitz_column = torch.tensor(
-            [[[4, 0, 0, 1], [3, 0, -0.5, -1]], [[2, 0.1, 0.01, 0.0], [3, 0, -0.1, -2]]], dtype=torch.float
+            [[[4, 0, 0, 1], [3, 0, -0.5, -1]], [[2, 0.1, 0.01, 0.0], [3, 0, -0.1, -2]]],
+            dtype=torch.float,
         )
         toeplitz_column.detach_()
         return BatchRepeatLinearOperator(ToeplitzLinearOperator(toeplitz_column), torch.Size((2, 3, 1, 4)))
 
     def evaluate_linear_op(self, linear_op):
         evaluated = linear_op.base_linear_op.to_dense()
         return evaluated.repeat(*linear_op.batch_repeat, 1, 1)
```

### Comparing `linear_operator-0.3.0/test/operators/test_block_diag_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_block_diag_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_block_interleaved_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_block_interleaved_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_cat_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_cat_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_chol_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_chol_linear_operator.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,21 @@
     should_test_sample = True
     should_call_cg = False
     should_call_lanczos = False
     should_call_lanczos_diagonalization = True
 
     def create_linear_op(self):
         chol = torch.tensor(
-            [[3, 0, 0, 0, 0], [-1, 2, 0, 0, 0], [1, 4, 1, 0, 0], [0, 2, 3, 2, 0], [-4, -2, 1, 3, 4]],
+            [
+                [3, 0, 0, 0, 0],
+                [-1, 2, 0, 0, 0],
+                [1, 4, 1, 0, 0],
+                [0, 2, 3, 2, 0],
+                [-4, -2, 1, 3, 4],
+            ],
             dtype=torch.float,
             requires_grad=True,
         )
         return CholLinearOperator(TriangularLinearOperator(chol))
 
     def evaluate_linear_op(self, linear_op):
         chol = linear_op.root.to_dense()
@@ -50,16 +56,28 @@
 
 class TestCholLinearOperatorBatch(TestCholLinearOperator):
     seed = 0
 
     def create_linear_op(self):
         chol = torch.tensor(
             [
-                [[3, 0, 0, 0, 0], [-1, 2, 0, 0, 0], [1, 4, 1, 0, 0], [0, 2, 3, 2, 0], [-4, -2, 1, 3, 4]],
-                [[2, 0, 0, 0, 0], [3, 1, 0, 0, 0], [-2, 3, 2, 0, 0], [-2, 1, -1, 3, 0], [-4, -4, 5, 2, 3]],
+                [
+                    [3, 0, 0, 0, 0],
+                    [-1, 2, 0, 0, 0],
+                    [1, 4, 1, 0, 0],
+                    [0, 2, 3, 2, 0],
+                    [-4, -2, 1, 3, 4],
+                ],
+                [
+                    [2, 0, 0, 0, 0],
+                    [3, 1, 0, 0, 0],
+                    [-2, 3, 2, 0, 0],
+                    [-2, 1, -1, 3, 0],
+                    [-4, -4, 5, 2, 3],
+                ],
             ],
             dtype=torch.float,
         )
         chol.add_(torch.eye(5).unsqueeze(0))
         chol.requires_grad_(True)
         return CholLinearOperator(TriangularLinearOperator(chol))
 
@@ -69,16 +87,28 @@
     # Because these LTs are large, we'll skil the big tests
     should_test_sample = False
     skip_slq_tests = True
 
     def create_linear_op(self):
         chol = torch.tensor(
             [
-                [[3, 0, 0, 0, 0], [-1, 2, 0, 0, 0], [1, 4, 1, 0, 0], [0, 2, 3, 2, 0], [-4, -2, 1, 3, 4]],
-                [[2, 0, 0, 0, 0], [3, 1, 0, 0, 0], [-2, 3, 2, 0, 0], [-2, 1, -1, 3, 0], [-4, -4, 5, 2, 3]],
+                [
+                    [3, 0, 0, 0, 0],
+                    [-1, 2, 0, 0, 0],
+                    [1, 4, 1, 0, 0],
+                    [0, 2, 3, 2, 0],
+                    [-4, -2, 1, 3, 4],
+                ],
+                [
+                    [2, 0, 0, 0, 0],
+                    [3, 1, 0, 0, 0],
+                    [-2, 3, 2, 0, 0],
+                    [-2, 1, -1, 3, 0],
+                    [-4, -4, 5, 2, 3],
+                ],
             ],
             dtype=torch.float,
         )
         chol = chol.repeat(3, 1, 1, 1)
         chol[1].mul_(2)
         chol[2].mul_(0.5)
         chol.add_(torch.eye(5).unsqueeze_(0).unsqueeze_(0))
```

### Comparing `linear_operator-0.3.0/test/operators/test_constant_mul_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_constant_mul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_dense_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_dense_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_diag_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_diag_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         self.assertAllClose(torch.abs(linear_op).to_dense(), torch.abs(evaluated))
 
     def test_exp(self):
         linear_op = self.create_linear_op()
         linear_op_copy = linear_op.detach().clone()
         evaluated = self.evaluate_linear_op(linear_op_copy)
         self.assertAllClose(
-            torch.exp(linear_op).diagonal(dim1=-1, dim2=-2), torch.exp(evaluated.diagonal(dim1=-1, dim2=-2))
+            torch.exp(linear_op).diagonal(dim1=-1, dim2=-2),
+            torch.exp(evaluated.diagonal(dim1=-1, dim2=-2)),
         )
 
     def test_inverse(self):
         linear_op = self.create_linear_op()
         linear_op_copy = linear_op.detach().clone()
         linear_op.requires_grad_(True)
         linear_op_copy.requires_grad_(True)
@@ -57,15 +58,16 @@
                 self.assertAllClose(arg.grad, arg_copy.grad)
 
     def test_log(self):
         linear_op = self.create_linear_op()
         linear_op_copy = linear_op.detach().clone()
         evaluated = self.evaluate_linear_op(linear_op_copy)
         self.assertAllClose(
-            torch.log(linear_op).diagonal(dim1=-1, dim2=-2), torch.log(evaluated.diagonal(dim1=-1, dim2=-2))
+            torch.log(linear_op).diagonal(dim1=-1, dim2=-2),
+            torch.log(evaluated.diagonal(dim1=-1, dim2=-2)),
         )
 
     def test_solve_triangular(self):
         linear_op = self.create_linear_op()
         rhs = torch.randn(linear_op.size(-1))
         res = torch.linalg.solve_triangular(linear_op, rhs, upper=False)
         res_actual = rhs / linear_op.diagonal()
@@ -88,15 +90,20 @@
 
 
 class TestDiagLinearOperatorBatch(TestDiagLinearOperator):
     seed = 0
 
     def create_linear_op(self):
         diag = torch.tensor(
-            [[1.0, 2.0, 4.0, 2.0, 3.0], [2.0, 1.0, 2.0, 1.0, 4.0], [1.0, 2.0, 2.0, 3.0, 4.0]], requires_grad=True
+            [
+                [1.0, 2.0, 4.0, 2.0, 3.0],
+                [2.0, 1.0, 2.0, 1.0, 4.0],
+                [1.0, 2.0, 2.0, 3.0, 4.0],
+            ],
+            requires_grad=True,
         )
         return DiagLinearOperator(diag)
 
     def evaluate_linear_op(self, linear_op):
         diag = linear_op._diag
         return torch.diag_embed(diag)
```

### Comparing `linear_operator-0.3.0/test/operators/test_identity_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_identity_linear_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,18 @@
 
         # Check forward pass
         self.assertAllClose(sqrt_inv_matmul_res, sqrt_inv_matmul_actual, **self.tolerances["sqrt_inv_matmul"])
 
     def test_root_decomposition(self, cholesky=False):
         linear_op = self.create_linear_op()
         root_decomp = linear_op.root_decomposition().root
-        self.assertAllClose(root_decomp.to_dense(), torch.eye(linear_op.size(-1)).expand(linear_op.shape))
+        self.assertAllClose(
+            root_decomp.to_dense(),
+            torch.eye(linear_op.size(-1)).expand(linear_op.shape),
+        )
 
     def test_svd(self):
         linear_op = self.create_linear_op()
         U, S, Vt = linear_op.svd()
         self.assertAllClose(S, torch.ones(linear_op.shape[:-1]))
         self.assertAllClose(U.to_dense(), torch.eye(linear_op.size(-1)).expand(linear_op.shape))
         self.assertAllClose(Vt.to_dense(), torch.eye(linear_op.size(-1)).expand(linear_op.shape))
```

### Comparing `linear_operator-0.3.0/test/operators/test_interpolated_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_interpolated_linear_operator.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 
         base_tensor = torch.randn(6, 6)
         base_tensor = base_tensor.t().matmul(base_tensor)
         base_tensor.requires_grad = True
         base_linear_op = DenseLinearOperator(base_tensor)
 
         return InterpolatedLinearOperator(
-            base_linear_op, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
+            base_linear_op,
+            left_interp_indices,
+            left_interp_values,
+            right_interp_indices,
+            right_interp_values,
         )
 
     def evaluate_linear_op(self, linear_op):
         left_matrix = torch.zeros(4, 6, dtype=linear_op.dtype)
         right_matrix = torch.zeros(4, 6, dtype=linear_op.dtype)
         left_matrix.scatter_(1, linear_op.left_interp_indices, linear_op.left_interp_values)
         right_matrix.scatter_(1, linear_op.right_interp_indices, linear_op.right_interp_values)
@@ -64,15 +68,19 @@
 
         base_tensor = torch.randn(5, 6, 6)
         base_tensor = base_tensor.mT.matmul(base_tensor)
         base_tensor.requires_grad = True
         base_linear_op = DenseLinearOperator(base_tensor)
 
         return InterpolatedLinearOperator(
-            base_linear_op, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
+            base_linear_op,
+            left_interp_indices,
+            left_interp_values,
+            right_interp_indices,
+            right_interp_values,
         )
 
     def evaluate_linear_op(self, linear_op):
         left_matrix_comps = []
         right_matrix_comps = []
         for i in range(5):
             left_matrix_comp = torch.zeros(4, 6, dtype=linear_op.dtype)
@@ -109,26 +117,38 @@
         right_interp_values.requires_grad = True
 
         base_tensor = torch.randn(5, 6, 6)
         base_tensor = base_tensor.mT.matmul(base_tensor)
         base_linear_op = DenseLinearOperator(base_tensor)
 
         return InterpolatedLinearOperator(
-            base_linear_op, left_interp_indices, left_interp_values, right_interp_indices, right_interp_values
+            base_linear_op,
+            left_interp_indices,
+            left_interp_values,
+            right_interp_indices,
+            right_interp_values,
         )
 
     def evaluate_linear_op(self, linear_op):
         left_matrix_comps = []
         right_matrix_comps = []
         for i in range(2):
             for j in range(5):
                 left_matrix_comp = torch.zeros(4, 6, dtype=linear_op.dtype)
                 right_matrix_comp = torch.zeros(4, 6, dtype=linear_op.dtype)
-                left_matrix_comp.scatter_(1, linear_op.left_interp_indices[i, j], linear_op.left_interp_values[i, j])
-                right_matrix_comp.scatter_(1, linear_op.right_interp_indices[i, j], linear_op.right_interp_values[i, j])
+                left_matrix_comp.scatter_(
+                    1,
+                    linear_op.left_interp_indices[i, j],
+                    linear_op.left_interp_values[i, j],
+                )
+                right_matrix_comp.scatter_(
+                    1,
+                    linear_op.right_interp_indices[i, j],
+                    linear_op.right_interp_values[i, j],
+                )
                 left_matrix_comps.append(left_matrix_comp.unsqueeze(0))
                 right_matrix_comps.append(right_matrix_comp.unsqueeze(0))
         left_matrix = torch.cat(left_matrix_comps)
         right_matrix = torch.cat(right_matrix_comps)
         left_matrix = left_matrix.view(2, 5, 4, 6)
         right_matrix = right_matrix.view(2, 5, 4, 6)
```

### Comparing `linear_operator-0.3.0/test/operators/test_kronecker_product_added_diag_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_kronecker_product_added_diag_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,18 @@
         "grad": {"rtol": 0.03, "atol": 1e-4},
         "solve": {"rtol": 0.02, "atol": 1e-4},
     }
 
     def create_linear_op(self):
         a = torch.tensor([[4, 0, 2], [0, 3, -1], [2, -1, 3]], dtype=torch.float)
         b = torch.tensor([[2, 1], [1, 2]], dtype=torch.float)
-        c = torch.tensor([[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]], dtype=torch.float)
+        c = torch.tensor(
+            [[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]],
+            dtype=torch.float,
+        )
         d = 0.5 * torch.rand(24, dtype=torch.float)
         a.requires_grad_(True)
         b.requires_grad_(True)
         c.requires_grad_(True)
         d.requires_grad_(True)
         kp_linear_op = KroneckerProductLinearOperator(
             DenseLinearOperator(a), DenseLinearOperator(b), DenseLinearOperator(c)
@@ -53,15 +56,18 @@
     skip_slq_tests = True
     should_call_cg = False
     should_call_lanczos = False
 
     def create_linear_op(self):
         a = torch.tensor([[4, 0, 2], [0, 3, -1], [2, -1, 3]], dtype=torch.float)
         b = torch.tensor([[2, 1], [1, 2]], dtype=torch.float)
-        c = torch.tensor([[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]], dtype=torch.float)
+        c = torch.tensor(
+            [[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]],
+            dtype=torch.float,
+        )
         d = torch.tensor([2, 1, 3], dtype=torch.float)
         e = torch.tensor([5], dtype=torch.float)
         f = torch.tensor([2.5], dtype=torch.float)
         a.requires_grad_(True)
         b.requires_grad_(True)
         c.requires_grad_(True)
         d.requires_grad_(True)
@@ -80,15 +86,18 @@
 
 class TestKroneckerProductAddedKroneckerConstDiagLinearOperator(TestKroneckerProductAddedKroneckerDiagLinearOperator):
     should_call_lanczos = True
 
     def create_linear_op(self):
         a = torch.tensor([[4, 0, 2], [0, 3, -1], [2, -1, 3]], dtype=torch.float)
         b = torch.tensor([[2, 1], [1, 2]], dtype=torch.float)
-        c = torch.tensor([[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]], dtype=torch.float)
+        c = torch.tensor(
+            [[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]],
+            dtype=torch.float,
+        )
         d = torch.tensor([2], dtype=torch.float)
         e = torch.tensor([5], dtype=torch.float)
         f = torch.tensor([2.5], dtype=torch.float)
         a.requires_grad_(True)
         b.requires_grad_(True)
         c.requires_grad_(True)
         d.requires_grad_(True)
@@ -108,15 +117,18 @@
 class TestKroneckerProductAddedConstDiagLinearOperator(TestKroneckerProductAddedDiagLinearOperator):
     should_call_cg = False
     should_call_lanczos = False
 
     def create_linear_op(self):
         a = torch.tensor([[4, 0, 2], [0, 3, -1], [2, -1, 3]], dtype=torch.float)
         b = torch.tensor([[2, 1], [1, 2]], dtype=torch.float)
-        c = torch.tensor([[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]], dtype=torch.float)
+        c = torch.tensor(
+            [[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]],
+            dtype=torch.float,
+        )
         a.requires_grad_(True)
         b.requires_grad_(True)
         c.requires_grad_(True)
         kp_linear_op = KroneckerProductLinearOperator(
             DenseLinearOperator(a), DenseLinearOperator(b), DenseLinearOperator(c)
         )
         diag_linear_op = ConstantDiagLinearOperator(
```

### Comparing `linear_operator-0.3.0/test/operators/test_kronecker_product_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_kronecker_product_linear_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,18 @@
     seed = 0
     should_call_lanczos = True
     should_call_lanczos_diagonalization = False
 
     def create_linear_op(self):
         a = torch.tensor([[4, 0, 2], [0, 3, -1], [2, -1, 3]], dtype=torch.float)
         b = torch.tensor([[2, 1], [1, 2]], dtype=torch.float)
-        c = torch.tensor([[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]], dtype=torch.float)
+        c = torch.tensor(
+            [[4, 0.5, 1, 0], [0.5, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]],
+            dtype=torch.float,
+        )
         a.requires_grad_(True)
         b.requires_grad_(True)
         c.requires_grad_(True)
         kp_linear_op = KroneckerProductLinearOperator(
             DenseLinearOperator(a), DenseLinearOperator(b), DenseLinearOperator(c)
         )
         return kp_linear_op
@@ -88,17 +91,18 @@
     seed = 0
     should_call_lanczos = True
     should_call_lanczos_diagonalization = False
 
     def create_linear_op(self):
         a = torch.tensor([[4, 0, 2], [0, 3, -1], [2, -1, 3]], dtype=torch.float).repeat(3, 1, 1)
         b = torch.tensor([[2, 1], [1, 2]], dtype=torch.float).repeat(3, 1, 1)
-        c = torch.tensor([[4, 0.1, 1, 0], [0.1, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]], dtype=torch.float).repeat(
-            3, 1, 1
-        )
+        c = torch.tensor(
+            [[4, 0.1, 1, 0], [0.1, 4, -1, 0], [1, -1, 3, 0], [0, 0, 0, 4]],
+            dtype=torch.float,
+        ).repeat(3, 1, 1)
         a.requires_grad_(True)
         b.requires_grad_(True)
         c.requires_grad_(True)
         kp_linear_op = KroneckerProductLinearOperator(
             DenseLinearOperator(a), DenseLinearOperator(b), DenseLinearOperator(c)
         )
         return kp_linear_op
```

### Comparing `linear_operator-0.3.0/test/operators/test_low_rank_root_added_diag_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_low_rank_root_added_diag_linear_operator.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,15 +107,21 @@
 
 class TestLowRankRootAddedDiagLinearOperatorBatch(TestLowRankRootAddedDiagLinearOperator):
     seed = 4
     should_test_sample = True
 
     def create_linear_op(self):
         tensor = torch.randn(3, 5, 2)
-        diag = torch.tensor([[1.0, 2.0, 4.0, 2.0, 3.0], [2.0, 1.0, 2.0, 1.0, 4.0], [1.0, 2.0, 2.0, 3.0, 4.0]])
+        diag = torch.tensor(
+            [
+                [1.0, 2.0, 4.0, 2.0, 3.0],
+                [2.0, 1.0, 2.0, 1.0, 4.0],
+                [1.0, 2.0, 2.0, 3.0, 4.0],
+            ]
+        )
         lt = LowRankRootLinearOperator(tensor).add_diagonal(diag)
         assert isinstance(lt, LowRankRootAddedDiagLinearOperator)
         return lt
 
     def evaluate_linear_op(self, linear_op):
         diag = linear_op._diag_tensor._diag
         root = linear_op._linear_op.root.tensor
@@ -126,17 +132,21 @@
     seed = 4
     # Because these LTs are large, we'll skil the big tests
     should_test_sample = False
     skip_slq_tests = True
 
     def create_linear_op(self):
         tensor = torch.randn(4, 3, 5, 2)
-        diag = torch.tensor([[1.0, 2.0, 4.0, 2.0, 3.0], [2.0, 1.0, 2.0, 1.0, 4.0], [1.0, 2.0, 2.0, 3.0, 4.0]]).repeat(
-            4, 1, 1
-        )
+        diag = torch.tensor(
+            [
+                [1.0, 2.0, 4.0, 2.0, 3.0],
+                [2.0, 1.0, 2.0, 1.0, 4.0],
+                [1.0, 2.0, 2.0, 3.0, 4.0],
+            ]
+        ).repeat(4, 1, 1)
         lt = LowRankRootLinearOperator(tensor).add_diagonal(diag)
         assert isinstance(lt, LowRankRootAddedDiagLinearOperator)
         return lt
 
     def evaluate_linear_op(self, linear_op):
         diag = linear_op._diag_tensor._diag
         root = linear_op._linear_op.root.tensor
```

### Comparing `linear_operator-0.3.0/test/operators/test_low_rank_root_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_low_rank_root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_matmul_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_matmul_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_mul_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_mul_linear_operator.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,18 @@
         mat1 = make_random_mat(6, 6)
         mat2 = make_random_mat(6, 6)
         res = torch.mul(RootLinearOperator(mat1), RootLinearOperator(mat2))
         return res.add_diagonal(torch.tensor(2.0))
 
     def evaluate_linear_op(self, linear_op):
         diag_tensor = linear_op._diag_tensor.to_dense()
-        res = torch.mul(linear_op._linear_op.left_linear_op.to_dense(), linear_op._linear_op.right_linear_op.to_dense())
+        res = torch.mul(
+            linear_op._linear_op.left_linear_op.to_dense(),
+            linear_op._linear_op.right_linear_op.to_dense(),
+        )
         res = res + diag_tensor
         return res
 
 
 class TestMulLinearOperatorBatch(LinearOperatorTestCase, unittest.TestCase):
     seed = 2
 
@@ -36,15 +39,18 @@
         mat1 = make_random_mat(6, rank=6, batch_shape=torch.Size((2,)))
         mat2 = make_random_mat(6, rank=6, batch_shape=torch.Size((2,)))
         res = RootLinearOperator(mat1) * RootLinearOperator(mat2)
         return res.add_diagonal(torch.tensor(2.0))
 
     def evaluate_linear_op(self, linear_op):
         diag_tensor = linear_op._diag_tensor.to_dense()
-        res = torch.mul(linear_op._linear_op.left_linear_op.to_dense(), linear_op._linear_op.right_linear_op.to_dense())
+        res = torch.mul(
+            linear_op._linear_op.left_linear_op.to_dense(),
+            linear_op._linear_op.right_linear_op.to_dense(),
+        )
         res = res + diag_tensor
         return res
 
 
 class TestMulLinearOperatorMultiBatch(LinearOperatorTestCase, unittest.TestCase):
     seed = 1
     skip_slq_tests = True
@@ -53,15 +59,18 @@
         mat1 = make_random_mat(6, rank=6, batch_shape=torch.Size((2, 3)))
         mat2 = make_random_mat(6, rank=6, batch_shape=torch.Size((2, 3)))
         res = RootLinearOperator(mat1) * RootLinearOperator(mat2)
         return res.add_diagonal(torch.tensor(0.5))
 
     def evaluate_linear_op(self, linear_op):
         diag_tensor = linear_op._diag_tensor.to_dense()
-        res = torch.mul(linear_op._linear_op.left_linear_op.to_dense(), linear_op._linear_op.right_linear_op.to_dense())
+        res = torch.mul(
+            linear_op._linear_op.left_linear_op.to_dense(),
+            linear_op._linear_op.right_linear_op.to_dense(),
+        )
         res = res + diag_tensor
         return res
 
     def test_inv_quad_logdet(self):
         pass
```

### Comparing `linear_operator-0.3.0/test/operators/test_permutation_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_permutation_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_psd_sum_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_psd_sum_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_root_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_root_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_sum_batch_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_sum_batch_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_sum_kronecker_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_sum_kronecker_linear_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,10 +36,16 @@
         d.requires_grad_(True)
         kp_lt_1 = KroneckerProductLinearOperator(DenseLinearOperator(a), DenseLinearOperator(b))
         kp_lt_2 = KroneckerProductLinearOperator(DenseLinearOperator(c), DenseLinearOperator(d))
 
         return SumKroneckerLinearOperator(kp_lt_1, kp_lt_2)
 
     def evaluate_linear_op(self, linear_op):
-        res1 = kron(linear_op.linear_ops[0].linear_ops[0].tensor, linear_op.linear_ops[0].linear_ops[1].tensor)
-        res2 = kron(linear_op.linear_ops[1].linear_ops[0].tensor, linear_op.linear_ops[1].linear_ops[1].tensor)
+        res1 = kron(
+            linear_op.linear_ops[0].linear_ops[0].tensor,
+            linear_op.linear_ops[0].linear_ops[1].tensor,
+        )
+        res2 = kron(
+            linear_op.linear_ops[1].linear_ops[0].tensor,
+            linear_op.linear_ops[1].linear_ops[1].tensor,
+        )
         return res1 + res2
```

### Comparing `linear_operator-0.3.0/test/operators/test_sum_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_sum_linear_operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 import unittest
 
 import torch
 
-from linear_operator.operators import ToeplitzLinearOperator, to_linear_operator
+from linear_operator.operators import to_linear_operator, ToeplitzLinearOperator
 from linear_operator.test.linear_operator_test_case import LinearOperatorTestCase
 
 
 class TestSumLinearOperator(LinearOperatorTestCase, unittest.TestCase):
     seed = 0
 
     def create_linear_op(self):
```

### Comparing `linear_operator-0.3.0/test/operators/test_toeplitz_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_toeplitz_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_triangular_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_triangular_linear_operator.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/operators/test_zero_linear_operator.py` & `linear_operator-0.4.0/test/operators/test_zero_linear_operator.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,29 +62,61 @@
         self.assertTrue(approx_equal(linear_op[index].to_dense(), evaluated[index]))
 
     def test_get_item_tensor_index_on_batch(self):
         # Tests the default LV.__getitem__ behavior
         linear_op = ZeroLinearOperator(3, 5, 5)
         evaluated = linear_op.to_dense()
 
-        index = (torch.tensor([0, 1, 1, 0]), torch.tensor([0, 1, 0, 2]), torch.tensor([1, 2, 0, 1]))
-        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
-        index = (torch.tensor([0, 1, 1, 0]), torch.tensor([0, 1, 0, 2]), slice(None, None, None))
-        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
-        index = (torch.tensor([0, 1, 1]), slice(None, None, None), torch.tensor([0, 1, 2]))
-        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
-        index = (slice(None, None, None), torch.tensor([0, 1, 1, 0]), torch.tensor([0, 1, 0, 2]))
-        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
-        index = (torch.tensor([0, 0, 1, 1]), slice(None, None, None), slice(None, None, None))
+        index = (
+            torch.tensor([0, 1, 1, 0]),
+            torch.tensor([0, 1, 0, 2]),
+            torch.tensor([1, 2, 0, 1]),
+        )
+        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
+        index = (
+            torch.tensor([0, 1, 1, 0]),
+            torch.tensor([0, 1, 0, 2]),
+            slice(None, None, None),
+        )
+        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
+        index = (
+            torch.tensor([0, 1, 1]),
+            slice(None, None, None),
+            torch.tensor([0, 1, 2]),
+        )
+        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
+        index = (
+            slice(None, None, None),
+            torch.tensor([0, 1, 1, 0]),
+            torch.tensor([0, 1, 0, 2]),
+        )
+        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
+        index = (
+            torch.tensor([0, 0, 1, 1]),
+            slice(None, None, None),
+            slice(None, None, None),
+        )
         self.assertTrue(approx_equal(linear_op[index].to_dense(), evaluated[index]))
-        index = (slice(None, None, None), torch.tensor([0, 0, 1, 2]), torch.tensor([0, 0, 1, 1]))
-        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
-        index = (torch.tensor([0, 1, 1, 0]), torch.tensor([0, 1, 0, 2]), slice(None, None, None))
-        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
-        index = (torch.tensor([0, 0, 1, 0]), slice(None, None, None), torch.tensor([0, 0, 1, 1]))
+        index = (
+            slice(None, None, None),
+            torch.tensor([0, 0, 1, 2]),
+            torch.tensor([0, 0, 1, 1]),
+        )
+        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
+        index = (
+            torch.tensor([0, 1, 1, 0]),
+            torch.tensor([0, 1, 0, 2]),
+            slice(None, None, None),
+        )
+        self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
+        index = (
+            torch.tensor([0, 0, 1, 0]),
+            slice(None, None, None),
+            torch.tensor([0, 0, 1, 1]),
+        )
         self.assertTrue(approx_equal(linear_op[index], evaluated[index]))
         index = (Ellipsis, torch.tensor([0, 1, 1, 0]))
         self.assertTrue(approx_equal(linear_op[index].to_dense(), evaluated[index]))
 
     def test_add_diagonal(self):
         diag = torch.tensor(1.5)
         res = ZeroLinearOperator(5, 5).add_diagonal(diag).to_dense()
```

### Comparing `linear_operator-0.3.0/test/utils/test_cholesky.py` & `linear_operator-0.4.0/test/utils/test_cholesky.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/utils/test_getitem.py` & `linear_operator-0.4.0/test/utils/test_getitem.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,21 +8,27 @@
 from linear_operator.utils.getitem import _compute_getitem_size, _convert_indices_to_tensors
 
 
 class TestGetitem(unittest.TestCase):
     def test_compute_getitem_size(self):
         a = torch.tensor(0.0).expand(5, 5, 5, 5, 5)
 
-        for indices in product([torch.tensor([0, 1, 1, 0]), slice(None, None, None), 1, slice(0, 2, None)], repeat=5):
+        for indices in product(
+            [torch.tensor([0, 1, 1, 0]), slice(None, None, None), 1, slice(0, 2, None)],
+            repeat=5,
+        ):
             res = _compute_getitem_size(a, indices)
             actual = a[indices].shape
             self.assertEqual(res, actual)
 
     def test_convert_indices_to_tensors(self):
         a = torch.randn(5, 5, 5, 5, 5)
 
-        for indices in product([torch.tensor([0, 1, 1, 0]), slice(None, None, None), 1, slice(0, 2, None)], repeat=5):
+        for indices in product(
+            [torch.tensor([0, 1, 1, 0]), slice(None, None, None), 1, slice(0, 2, None)],
+            repeat=5,
+        ):
             if not any(torch.is_tensor(index) for index in indices):
                 continue
             new_indices = _convert_indices_to_tensors(a, indices)
             self.assertTrue(all(torch.is_tensor(index) for index in new_indices))
             self.assertTrue(torch.equal(a[indices], a[new_indices]))
```

### Comparing `linear_operator-0.3.0/test/utils/test_interpolation.py` & `linear_operator-0.4.0/test/utils/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/utils/test_lanczos.py` & `linear_operator-0.4.0/test/utils/test_lanczos.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/utils/test_linear_cg.py` & `linear_operator-0.4.0/test/utils/test_linear_cg.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,21 @@
         matrix = torch.randn(size, size, dtype=torch.float64)
         matrix = matrix.matmul(matrix.mT)
         matrix.div_(matrix.norm())
         matrix.add_(torch.eye(matrix.size(-1), dtype=torch.float64).mul_(1e-1))
 
         rhs = torch.randn(size, 50, dtype=torch.float64)
         solves, t_mats = linear_cg(
-            matrix.matmul, rhs=rhs, n_tridiag=5, max_tridiag_iter=10, max_iter=size, tolerance=0, eps=1e-15
+            matrix.matmul,
+            rhs=rhs,
+            n_tridiag=5,
+            max_tridiag_iter=10,
+            max_iter=size,
+            tolerance=0,
+            eps=1e-15,
         )
 
         # Check cg
         matrix_chol = torch.linalg.cholesky(matrix)
         actual = torch.cholesky_solve(rhs, matrix_chol)
         self.assertTrue(torch.allclose(solves, actual, atol=1e-3, rtol=1e-4))
 
@@ -106,15 +112,21 @@
         matrix = torch.randn(batch, size, size, dtype=torch.float64)
         matrix = matrix.matmul(matrix.mT)
         matrix.div_(matrix.norm())
         matrix.add_(torch.eye(matrix.size(-1), dtype=torch.float64).mul_(1e-1))
 
         rhs = torch.randn(batch, size, 10, dtype=torch.float64)
         solves, t_mats = linear_cg(
-            matrix.matmul, rhs=rhs, n_tridiag=8, max_iter=size, max_tridiag_iter=10, tolerance=0, eps=1e-30
+            matrix.matmul,
+            rhs=rhs,
+            n_tridiag=8,
+            max_iter=size,
+            max_tridiag_iter=10,
+            tolerance=0,
+            eps=1e-30,
         )
 
         # Check cg
         matrix_chol = torch.linalg.cholesky(matrix)
         actual = torch.cholesky_solve(rhs, matrix_chol)
         self.assertTrue(torch.allclose(solves, actual, atol=1e-3, rtol=1e-4))
```

### Comparing `linear_operator-0.3.0/test/utils/test_minres.py` & `linear_operator-0.4.0/test/utils/test_minres.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         # Make sure that we're not getting weird batch dim effects
         while matrix.dim() < len(rhs_shape):
             matrix = matrix.unsqueeze(0)
 
         # Maybe add shifts
         if shifts is not None:
             matrix = matrix - torch.mul(
-                torch.eye(size, dtype=torch.float64), shifts.view(*shifts.shape, *[1 for _ in matrix.shape])
+                torch.eye(size, dtype=torch.float64),
+                shifts.view(*shifts.shape, *[1 for _ in matrix.shape]),
             )
 
         # Compute solves exactly
         actual = torch.linalg.solve(-matrix, rhs.unsqueeze(-1) if rhs.dim() == 1 else rhs)
         if rhs.dim() == 1:
             actual = actual.squeeze(-1)
```

### Comparing `linear_operator-0.3.0/test/utils/test_permutation.py` & `linear_operator-0.4.0/test/utils/test_permutation.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,34 +15,43 @@
         return torch.tensor([[[0.25, -0.75], [-0.75, 2.25]], [[1.0, 1.2], [1.2, 0.5]]])
 
     def test_apply_permutation_left_and_right(self):
         A = self._gen_test_psd()
         left_permutation = torch.tensor([[0, 1], [1, 0]])
         right_permutation = torch.tensor([1, 0])
         res = apply_permutation(A, left_permutation, right_permutation)
-        self.assertAllClose(res, torch.tensor([[[-0.75, 0.25], [2.25, -0.75]], [[0.5, 1.2], [1.2, 1.0]]]))
+        self.assertAllClose(
+            res,
+            torch.tensor([[[-0.75, 0.25], [2.25, -0.75]], [[0.5, 1.2], [1.2, 1.0]]]),
+        )
 
     def test_apply_permutation_left_partial_and_right(self):
         A = self._gen_test_psd()
         left_permutation = torch.tensor([[0], [1]])
         right_permutation = torch.tensor([1, 0])
         res = apply_permutation(A, left_permutation, right_permutation)
         self.assertAllClose(res, torch.tensor([[[-0.75, 0.25]], [[0.5, 1.2]]]))
 
     def test_apply_permutation_left_only(self):
         A = self._gen_test_psd()
         left_permutation = torch.tensor([[0, 1], [1, 0]])
         res = apply_permutation(A, left_permutation=left_permutation)
-        self.assertAllClose(res, torch.tensor([[[0.25, -0.75], [-0.75, 2.25]], [[1.2, 0.5], [1.0, 1.2]]]))
+        self.assertAllClose(
+            res,
+            torch.tensor([[[0.25, -0.75], [-0.75, 2.25]], [[1.2, 0.5], [1.0, 1.2]]]),
+        )
 
     def test_apply_permutation_right_only(self):
         A = self._gen_test_psd()
         right_permutation = torch.tensor([1, 0])
         res = apply_permutation(A, right_permutation=right_permutation)
-        self.assertAllClose(res, torch.tensor([[[-0.75, 0.25], [2.25, -0.75]], [[1.2, 1.0], [0.5, 1.2]]]))
+        self.assertAllClose(
+            res,
+            torch.tensor([[[-0.75, 0.25], [2.25, -0.75]], [[1.2, 1.0], [0.5, 1.2]]]),
+        )
 
     def test_inverse_permutation(self):
         permutation = torch.tensor([[2, 3, 4, 0, 1], [4, 3, 0, 2, 1]])
         res = inverse_permutation(permutation)
         self.assertAllClose(res, torch.tensor([[3, 4, 0, 1, 2], [2, 4, 3, 1, 0]]))
```

### Comparing `linear_operator-0.3.0/test/utils/test_sparse.py` & `linear_operator-0.4.0/test/utils/test_sparse.py`

 * *Files identical despite different names*

### Comparing `linear_operator-0.3.0/test/utils/test_toeplitz.py` & `linear_operator-0.4.0/test/utils/test_toeplitz.py`

 * *Files identical despite different names*

