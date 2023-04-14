# Comparing `tmp/devito-4.8.0.tar.gz` & `tmp/devito-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devito-4.8.0.tar", last modified: Tue Feb 14 12:43:06 2023, max compression
+gzip compressed data, was "devito-4.8.1.tar", last modified: Fri Apr 14 07:14:18 2023, max compression
```

## Comparing `devito-4.8.0.tar` & `devito-4.8.1.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-14 12:42:53.000000 devito-4.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-14 12:42:53.000000 devito-4.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-14 12:43:06.821235 devito-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-02-14 12:42:53.000000 devito-4.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.797235 devito-4.8.0/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 12:42:53.000000 devito-4.8.0/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.797235 devito-4.8.0/benchmarks/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 12:42:53.000000 devito-4.8.0/benchmarks/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.801235 devito-4.8.0/benchmarks/user/advisor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 12:42:53.000000 devito-4.8.0/benchmarks/user/advisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-14 12:42:53.000000 devito-4.8.0/benchmarks/user/advisor/advisor_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-02-14 12:42:53.000000 devito-4.8.0/benchmarks/user/advisor/roofline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-02-14 12:42:53.000000 devito-4.8.0/benchmarks/user/advisor/run_advisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-02-14 12:42:53.000000 devito-4.8.0/benchmarks/user/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-02-14 12:42:53.000000 devito-4.8.0/benchmarks/user/make-pbs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/devito/
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-02-14 12:42:53.000000 devito-4.8.0/devito/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-14 12:43:06.821235 devito-4.8.0/devito/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.801235 devito-4.8.0/devito/arch/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-14 12:42:53.000000 devito-4.8.0/devito/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-02-14 12:42:53.000000 devito-4.8.0/devito/arch/archinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    28521 2023-02-14 12:42:53.000000 devito-4.8.0/devito/arch/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.801235 devito-4.8.0/devito/builtins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-14 12:42:53.000000 devito-4.8.0/devito/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-02-14 12:42:53.000000 devito-4.8.0/devito/builtins/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-02-14 12:42:53.000000 devito-4.8.0/devito/builtins/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-02-14 12:42:53.000000 devito-4.8.0/devito/builtins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.801235 devito-4.8.0/devito/checkpointing/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-14 12:42:53.000000 devito-4.8.0/devito/checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-02-14 12:42:53.000000 devito-4.8.0/devito/checkpointing/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.801235 devito-4.8.0/devito/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-02-14 12:42:53.000000 devito-4.8.0/devito/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-14 12:42:53.000000 devito-4.8.0/devito/core/arm.py
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-02-14 12:42:53.000000 devito-4.8.0/devito/core/autotuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-02-14 12:42:53.000000 devito-4.8.0/devito/core/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-02-14 12:42:53.000000 devito-4.8.0/devito/core/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-14 12:42:53.000000 devito-4.8.0/devito/core/intel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-02-14 12:42:53.000000 devito-4.8.0/devito/core/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-14 12:42:53.000000 devito-4.8.0/devito/core/power.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.801235 devito-4.8.0/devito/data/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-14 12:42:53.000000 devito-4.8.0/devito/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-02-14 12:42:53.000000 devito-4.8.0/devito/data/allocators.py
--rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-02-14 12:42:53.000000 devito-4.8.0/devito/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    20653 2023-02-14 12:42:53.000000 devito-4.8.0/devito/data/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-14 12:42:53.000000 devito-4.8.0/devito/data/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-02-14 12:42:53.000000 devito-4.8.0/devito/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-14 12:42:53.000000 devito-4.8.0/devito/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/finite_differences/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-14 12:42:53.000000 devito-4.8.0/devito/finite_differences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-02-14 12:42:53.000000 devito-4.8.0/devito/finite_differences/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-02-14 12:42:53.000000 devito-4.8.0/devito/finite_differences/derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)    25775 2023-02-14 12:42:53.000000 devito-4.8.0/devito/finite_differences/differentiable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-02-14 12:42:53.000000 devito-4.8.0/devito/finite_differences/elementary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-02-14 12:42:53.000000 devito-4.8.0/devito/finite_differences/finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-14 12:42:53.000000 devito-4.8.0/devito/finite_differences/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-02-14 12:42:53.000000 devito-4.8.0/devito/finite_differences/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/ir/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/ir/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/clusters/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/clusters/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/clusters/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/clusters/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/ir/equations/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/equations/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/equations/equation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/ir/iet/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/iet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/iet/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/iet/efunc.py
--rw-r--r--   0 runner    (1001) docker     (123)    40349 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/iet/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/iet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40430 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/iet/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/ir/stree/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/stree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/stree/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/stree/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/ir/support/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36467 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    30255 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/symregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/syncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-02-14 12:42:53.000000 devito-4.8.0/devito/ir/support/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-02-14 12:42:53.000000 devito-4.8.0/devito/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-14 12:42:53.000000 devito-4.8.0/devito/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19562 2023-02-14 12:42:53.000000 devito-4.8.0/devito/mpi/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-02-14 12:42:53.000000 devito-4.8.0/devito/mpi/halo_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    40624 2023-02-14 12:42:53.000000 devito-4.8.0/devito/mpi/routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.805235 devito-4.8.0/devito/operations/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-14 12:42:53.000000 devito-4.8.0/devito/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-02-14 12:42:53.000000 devito-4.8.0/devito/operations/interpolators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-02-14 12:42:53.000000 devito-4.8.0/devito/operations/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.809235 devito-4.8.0/devito/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-14 12:42:53.000000 devito-4.8.0/devito/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43091 2023-02-14 12:42:53.000000 devito-4.8.0/devito/operator/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19606 2023-02-14 12:42:53.000000 devito-4.8.0/devito/operator/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-14 12:42:53.000000 devito-4.8.0/devito/operator/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-02-14 12:42:53.000000 devito-4.8.0/devito/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.809235 devito-4.8.0/devito/passes/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.809235 devito-4.8.0/devito/passes/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51341 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/asynchrony.py
--rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    27592 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/buffering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/cse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/factorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/implicit.py
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/clusters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.809235 devito-4.8.0/devito/passes/equations/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/equations/linearity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.813235 devito-4.8.0/devito/passes/iet/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/asynchrony.py
--rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/instrument.py
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/langbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.813235 devito-4.8.0/devito/passes/iet/languages/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/languages/C.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/languages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/languages/openacc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/languages/openmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/languages/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/languages/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/linearization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/orchestration.py
--rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-02-14 12:42:53.000000 devito-4.8.0/devito/passes/iet/parpragma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.813235 devito-4.8.0/devito/symbolics/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-14 12:42:53.000000 devito-4.8.0/devito/symbolics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17479 2023-02-14 12:42:53.000000 devito-4.8.0/devito/symbolics/extended_sympy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-02-14 12:42:53.000000 devito-4.8.0/devito/symbolics/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-02-14 12:42:53.000000 devito-4.8.0/devito/symbolics/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-02-14 12:42:53.000000 devito-4.8.0/devito/symbolics/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-02-14 12:42:53.000000 devito-4.8.0/devito/symbolics/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-02-14 12:42:53.000000 devito-4.8.0/devito/symbolics/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.817235 devito-4.8.0/devito/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/dtypes_lowering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/memoization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/os_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-02-14 12:42:53.000000 devito-4.8.0/devito/tools/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.817235 devito-4.8.0/devito/types/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/args.py
--rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    44040 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    63437 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    49816 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/equation.py
--rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/relational.py
--rw-r--r--   0 runner    (1001) docker     (123)    79984 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-14 12:42:53.000000 devito-4.8.0/devito/types/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.801235 devito-4.8.0/devito.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-14 12:43:06.000000 devito-4.8.0/devito.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-02-14 12:43:06.000000 devito-4.8.0/devito.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 12:43:06.000000 devito-4.8.0/devito.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-14 12:43:06.000000 devito-4.8.0/devito.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-14 12:43:06.000000 devito-4.8.0/devito.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.797235 devito-4.8.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.817235 devito-4.8.0/examples/cfd/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-14 12:42:53.000000 devito-4.8.0/examples/cfd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-02-14 12:42:53.000000 devito-4.8.0/examples/cfd/example_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-02-14 12:42:53.000000 devito-4.8.0/examples/cfd/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.817235 devito-4.8.0/examples/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 12:42:53.000000 devito-4.8.0/examples/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.817235 devito-4.8.0/examples/misc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 12:42:53.000000 devito-4.8.0/examples/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-02-14 12:42:53.000000 devito-4.8.0/examples/misc/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.817235 devito-4.8.0/examples/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 12:42:53.000000 devito-4.8.0/examples/mpi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.817235 devito-4.8.0/examples/performance/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-14 12:42:53.000000 devito-4.8.0/examples/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-14 12:42:53.000000 devito-4.8.0/examples/performance/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/examples/seismic/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/examples/seismic/acoustic/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/acoustic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/acoustic/acoustic_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/acoustic/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/acoustic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/examples/seismic/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/elastic/elastic_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/elastic/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/elastic/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/preset_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/examples/seismic/self_adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/self_adjoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/self_adjoint/example_iso.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/self_adjoint/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/self_adjoint/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/self_adjoint/test_wavesolver_iso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/self_adjoint/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/self_adjoint/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/test_seismic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/examples/seismic/tti/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/tti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25683 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/tti/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/tti/tti_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/tti/wavesolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/examples/seismic/viscoacoustic/
--rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/viscoacoustic/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22768 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/viscoacoustic/operators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3351 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/viscoacoustic/viscoacoustic_example.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17387 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/viscoacoustic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/examples/seismic/viscoelastic/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/viscoelastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/viscoelastic/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/viscoelastic/viscoelastic_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-02-14 12:42:53.000000 devito-4.8.0/examples/seismic/viscoelastic/wavesolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 12:43:06.821235 devito-4.8.0/examples/userapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 12:42:53.000000 devito-4.8.0/examples/userapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-14 12:42:53.000000 devito-4.8.0/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-14 12:42:53.000000 devito-4.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-02-14 12:43:06.821235 devito-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-02-14 12:42:53.000000 devito-4.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68629 2023-02-14 12:42:53.000000 devito-4.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.764798 devito-4.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-14 07:14:09.000000 devito-4.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 07:14:09.000000 devito-4.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-14 07:14:18.764798 devito-4.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-14 07:14:09.000000 devito-4.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.740798 devito-4.8.1/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:09.000000 devito-4.8.1/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.740798 devito-4.8.1/benchmarks/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:09.000000 devito-4.8.1/benchmarks/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.740798 devito-4.8.1/benchmarks/user/advisor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:09.000000 devito-4.8.1/benchmarks/user/advisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-14 07:14:09.000000 devito-4.8.1/benchmarks/user/advisor/advisor_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-14 07:14:09.000000 devito-4.8.1/benchmarks/user/advisor/roofline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-04-14 07:14:09.000000 devito-4.8.1/benchmarks/user/advisor/run_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-04-14 07:14:09.000000 devito-4.8.1/benchmarks/user/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-14 07:14:09.000000 devito-4.8.1/benchmarks/user/make-pbs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.764798 devito-4.8.1/devito/
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-14 07:14:09.000000 devito-4.8.1/devito/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 07:14:18.764798 devito-4.8.1/devito/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.740798 devito-4.8.1/devito/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-14 07:14:09.000000 devito-4.8.1/devito/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-04-14 07:14:09.000000 devito-4.8.1/devito/arch/archinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29000 2023-04-14 07:14:09.000000 devito-4.8.1/devito/arch/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.740798 devito-4.8.1/devito/builtins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-14 07:14:09.000000 devito-4.8.1/devito/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-04-14 07:14:09.000000 devito-4.8.1/devito/builtins/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-04-14 07:14:09.000000 devito-4.8.1/devito/builtins/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-14 07:14:09.000000 devito-4.8.1/devito/builtins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.740798 devito-4.8.1/devito/checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-14 07:14:09.000000 devito-4.8.1/devito/checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-14 07:14:09.000000 devito-4.8.1/devito/checkpointing/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.740798 devito-4.8.1/devito/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-14 07:14:09.000000 devito-4.8.1/devito/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-14 07:14:09.000000 devito-4.8.1/devito/core/arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-04-14 07:14:09.000000 devito-4.8.1/devito/core/autotuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-04-14 07:14:09.000000 devito-4.8.1/devito/core/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-04-14 07:14:09.000000 devito-4.8.1/devito/core/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-14 07:14:09.000000 devito-4.8.1/devito/core/intel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-04-14 07:14:09.000000 devito-4.8.1/devito/core/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 07:14:09.000000 devito-4.8.1/devito/core/power.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-14 07:14:09.000000 devito-4.8.1/devito/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-04-14 07:14:09.000000 devito-4.8.1/devito/data/allocators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26486 2023-04-14 07:14:09.000000 devito-4.8.1/devito/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20653 2023-04-14 07:14:09.000000 devito-4.8.1/devito/data/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-14 07:14:09.000000 devito-4.8.1/devito/data/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-04-14 07:14:09.000000 devito-4.8.1/devito/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-14 07:14:09.000000 devito-4.8.1/devito/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/finite_differences/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 07:14:09.000000 devito-4.8.1/devito/finite_differences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-04-14 07:14:09.000000 devito-4.8.1/devito/finite_differences/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-04-14 07:14:09.000000 devito-4.8.1/devito/finite_differences/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-04-14 07:14:09.000000 devito-4.8.1/devito/finite_differences/differentiable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-14 07:14:09.000000 devito-4.8.1/devito/finite_differences/elementary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-14 07:14:09.000000 devito-4.8.1/devito/finite_differences/finite_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-14 07:14:09.000000 devito-4.8.1/devito/finite_differences/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-04-14 07:14:09.000000 devito-4.8.1/devito/finite_differences/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/ir/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/clusters/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/clusters/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/clusters/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/clusters/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/ir/equations/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/equations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/equations/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/equations/equation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/ir/iet/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/iet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/iet/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/iet/efunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40529 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/iet/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/iet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42377 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/iet/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/ir/stree/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/stree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/stree/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/stree/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/ir/support/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36784 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/guards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30280 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/symregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/syncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-04-14 07:14:09.000000 devito-4.8.1/devito/ir/support/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-14 07:14:09.000000 devito-4.8.1/devito/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.744798 devito-4.8.1/devito/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-14 07:14:09.000000 devito-4.8.1/devito/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21800 2023-04-14 07:14:09.000000 devito-4.8.1/devito/mpi/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22747 2023-04-14 07:14:09.000000 devito-4.8.1/devito/mpi/halo_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41547 2023-04-14 07:14:09.000000 devito-4.8.1/devito/mpi/routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.748798 devito-4.8.1/devito/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-14 07:14:09.000000 devito-4.8.1/devito/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-04-14 07:14:09.000000 devito-4.8.1/devito/operations/interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-14 07:14:09.000000 devito-4.8.1/devito/operations/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.748798 devito-4.8.1/devito/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-14 07:14:09.000000 devito-4.8.1/devito/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43735 2023-04-14 07:14:09.000000 devito-4.8.1/devito/operator/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19837 2023-04-14 07:14:09.000000 devito-4.8.1/devito/operator/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-14 07:14:09.000000 devito-4.8.1/devito/operator/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-04-14 07:14:09.000000 devito-4.8.1/devito/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.748798 devito-4.8.1/devito/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.748798 devito-4.8.1/devito/passes/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51341 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/asynchrony.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27592 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/buffering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/cse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/factorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/implicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16647 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/clusters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.748798 devito-4.8.1/devito/passes/equations/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/equations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/equations/linearity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.748798 devito-4.8.1/devito/passes/iet/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/asynchrony.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19713 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/langbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.748798 devito-4.8.1/devito/passes/iet/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/languages/C.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/languages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/languages/openacc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/languages/openmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/languages/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/languages/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/linearization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22725 2023-04-14 07:14:09.000000 devito-4.8.1/devito/passes/iet/parpragma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.752798 devito-4.8.1/devito/symbolics/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 07:14:09.000000 devito-4.8.1/devito/symbolics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-04-14 07:14:09.000000 devito-4.8.1/devito/symbolics/extended_sympy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-14 07:14:09.000000 devito-4.8.1/devito/symbolics/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-04-14 07:14:09.000000 devito-4.8.1/devito/symbolics/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-14 07:14:09.000000 devito-4.8.1/devito/symbolics/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-14 07:14:09.000000 devito-4.8.1/devito/symbolics/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-14 07:14:09.000000 devito-4.8.1/devito/symbolics/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.752798 devito-4.8.1/devito/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/dtypes_lowering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/os_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-14 07:14:09.000000 devito-4.8.1/devito/tools/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.752798 devito-4.8.1/devito/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44335 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63437 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49815 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29045 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/relational.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79984 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13502 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 07:14:09.000000 devito-4.8.1/devito/types/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.740798 devito-4.8.1/devito.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-14 07:14:18.000000 devito-4.8.1/devito.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-14 07:14:18.000000 devito-4.8.1/devito.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:14:18.000000 devito-4.8.1/devito.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-14 07:14:18.000000 devito-4.8.1/devito.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 07:14:18.000000 devito-4.8.1/devito.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.736798 devito-4.8.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.752798 devito-4.8.1/examples/cfd/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 07:14:10.000000 devito-4.8.1/examples/cfd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-04-14 07:14:10.000000 devito-4.8.1/examples/cfd/example_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-14 07:14:10.000000 devito-4.8.1/examples/cfd/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.752798 devito-4.8.1/examples/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:10.000000 devito-4.8.1/examples/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.752798 devito-4.8.1/examples/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:10.000000 devito-4.8.1/examples/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-14 07:14:10.000000 devito-4.8.1/examples/misc/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.752798 devito-4.8.1/examples/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:10.000000 devito-4.8.1/examples/mpi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.756799 devito-4.8.1/examples/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 07:14:10.000000 devito-4.8.1/examples/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-14 07:14:10.000000 devito-4.8.1/examples/performance/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.756799 devito-4.8.1/examples/seismic/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.756799 devito-4.8.1/examples/seismic/acoustic/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/acoustic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/acoustic/acoustic_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/acoustic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/acoustic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.760799 devito-4.8.1/examples/seismic/elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/elastic/elastic_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/elastic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/elastic/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/preset_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.760799 devito-4.8.1/examples/seismic/self_adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/self_adjoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/self_adjoint/example_iso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/self_adjoint/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/self_adjoint/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/self_adjoint/test_wavesolver_iso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/self_adjoint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/self_adjoint/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/test_seismic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.764798 devito-4.8.1/examples/seismic/tti/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/tti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25683 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/tti/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/tti/tti_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15856 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/tti/wavesolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.764798 devito-4.8.1/examples/seismic/viscoacoustic/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      112 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/viscoacoustic/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22768 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/viscoacoustic/operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3351 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/viscoacoustic/viscoacoustic_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17387 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/viscoacoustic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.764798 devito-4.8.1/examples/seismic/viscoelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/viscoelastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/viscoelastic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/viscoelastic/viscoelastic_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-14 07:14:10.000000 devito-4.8.1/examples/seismic/viscoelastic/wavesolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:18.764798 devito-4.8.1/examples/userapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:14:10.000000 devito-4.8.1/examples/userapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 07:14:10.000000 devito-4.8.1/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-14 07:14:10.000000 devito-4.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 07:14:18.764798 devito-4.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-14 07:14:10.000000 devito-4.8.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68629 2023-04-14 07:14:10.000000 devito-4.8.1/versioneer.py
```

### Comparing `devito-4.8.0/LICENSE.md` & `devito-4.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/PKG-INFO` & `devito-4.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devito
-Version: 4.8.0
+Version: 4.8.1
 Summary: Finite Difference DSL for symbolic computation.
 Home-page: http://www.devitoproject.org
 Author: Imperial College London
 Author-email: g.gorman@imperial.ac.uk
 License: MIT
 Project-URL: Documentation, https://www.devitoproject.org/devito/index.html
 Project-URL: Source Code, https://github.com/devitocodes/devito
```

### Comparing `devito-4.8.0/README.md` & `devito-4.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 generation and just-in-time compilation to execute optimized computational
 kernels on several computer platforms, including CPUs, GPUs, and clusters
 thereof.
 
 - [About Devito](#about-devito)
 - [Installation](#installation)
 - [Resources](#resources)
-- [FAQs](https://github.com/devitocodes/devito/FAQ.md)
+- [FAQs](https://github.com/devitocodes/devito/blob/master/FAQ.md)
 - [Performance](#performance)
 - [Get in touch](#get-in-touch)
 - [Interactive jupyter notebooks](#interactive-jupyter-notebooks)
 
 ## About Devito
 
 Devito provides a functional language to implement sophisticated operators that
```

### Comparing `devito-4.8.0/benchmarks/user/advisor/advisor_logging.py` & `devito-4.8.1/benchmarks/user/advisor/advisor_logging.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/benchmarks/user/advisor/roofline.py` & `devito-4.8.1/benchmarks/user/advisor/roofline.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/benchmarks/user/advisor/run_advisor.py` & `devito-4.8.1/benchmarks/user/advisor/run_advisor.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/benchmarks/user/benchmark.py` & `devito-4.8.1/benchmarks/user/benchmark.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/benchmarks/user/make-pbs.py` & `devito-4.8.1/benchmarks/user/make-pbs.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/__init__.py` & `devito-4.8.1/devito/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/arch/archinfo.py` & `devito-4.8.1/devito/arch/archinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from devito.tools import as_tuple, all_equal, memoized_func
 
 __all__ = ['platform_registry', 'get_cpu_info', 'get_gpu_info', 'get_nvidia_cc',
            'get_cuda_path', 'get_hip_path', 'check_cuda_runtime', 'get_m1_llvm_path',
            'Platform', 'Cpu64', 'Intel64', 'Amd', 'Arm', 'Power', 'Device',
            'NvidiaDevice', 'AmdDevice', 'IntelDevice',
            'INTEL64', 'SNB', 'IVB', 'HSW', 'BDW', 'SKX', 'KNL', 'KNL7210',  # Intel
-           'AMD', 'ARM', 'M1',  # ARM
+           'AMD', 'ARM', 'M1', 'GRAVITON',  # ARM
            'POWER8', 'POWER9',  # Other loosely supported CPU architectures
            'AMDGPUX', 'NVIDIAX', 'INTELGPUX']  # GPUs
 
 
 @memoized_func
 def get_cpu_info():
     """Attempt CPU info autodetection."""
@@ -724,14 +724,15 @@
 SKX = Intel64('skx')
 KLX = Intel64('klx')
 CLX = Intel64('clx')
 KNL = Intel64('knl')
 KNL7210 = Intel64('knl', cores_logical=256, cores_physical=64, isa='avx512')
 
 ARM = Arm('arm')
+GRAVITON = Arm('graviton')
 M1 = Arm('m1')
 
 AMD = Amd('amd')
 
 POWER8 = Power('power8')
 POWER9 = Power('power9')
 
@@ -750,14 +751,15 @@
     'bdw': BDW,  # Broadwell
     'skx': SKX,  # Skylake
     'klx': KLX,  # Kaby Lake
     'clx': CLX,  # Coffee Lake
     'knl': KNL,
     'knl7210': KNL7210,
     'arm': ARM,  # Generic ARM CPU
+    'graviton': GRAVITON,  # AMS arm
     'm1': M1,
     'amd': AMD,  # Generic AMD CPU
     'power8': POWER8,
     'power9': POWER9,
     'nvidiaX': NVIDIAX,  # Generic NVidia GPU
     'amdgpuX': AMDGPUX,   # Generic AMD GPU
     'intelgpuX': INTELGPUX   # Generic Intel GPU
```

### Comparing `devito-4.8.0/devito/arch/compiler.py` & `devito-4.8.1/devito/arch/compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import sys
 import time
 
 import numpy.ctypeslib as npct
 from codepy.jit import compile_from_string
 from codepy.toolchain import GCCToolchain
 
-from devito.arch import (AMDGPUX, Cpu64, M1, NVIDIAX, SKX, POWER8, POWER9,
+from devito.arch import (AMDGPUX, Cpu64, M1, NVIDIAX, SKX, POWER8, POWER9, GRAVITON,
                          get_nvidia_cc, check_cuda_runtime, get_m1_llvm_path)
 from devito.exceptions import CompilationError
 from devito.logger import debug, warning, error
 from devito.parameters import configuration
 from devito.tools import (as_list, change_directory, filter_ordered,
                           memoized_func, memoized_meth, make_tempdir)
 
@@ -101,15 +101,15 @@
             return 'IntelMPI'
     except (CalledProcessError, UnicodeDecodeError):
         pass
     return 'unknown'
 
 
 @memoized_func
-def sniff_mpi_flags():
+def sniff_mpi_flags(mpicc='mpicc'):
     mpi_distro = sniff_mpi_distro('mpiexec')
     if mpi_distro != 'OpenMPI':
         raise NotImplementedError("Unable to detect MPI compile and link flags")
 
     # OpenMPI's CC wrapper, namely mpicc, takes the --showme argument to find out
     # the flags used for compiling and linking
     compile_flags = check_output(['mpicc', "--showme:compile"]).decode("utf-8")
@@ -369,15 +369,15 @@
     def add_ldflags(self, flags):
         self.ldflags = filter_ordered(self.ldflags + as_list(flags))
 
 
 class GNUCompiler(Compiler):
 
     def __init__(self, *args, **kwargs):
-        super(GNUCompiler, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         self.cflags += ['-march=native', '-Wno-unused-result', '-Wno-unused-variable',
                         '-Wno-unused-but-set-variable']
         if configuration['safe-math']:
             self.cflags.append('-fno-unsafe-math-optimizations')
         else:
             self.cflags.append('-ffast-math')
@@ -396,14 +396,25 @@
     def __lookup_cmds__(self):
         self.CC = 'gcc'
         self.CXX = 'g++'
         self.MPICC = 'mpicc'
         self.MPICXX = 'mpicxx'
 
 
+class ArmCompiler(GNUCompiler):
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        platform = kwargs.pop('platform', configuration['platform'])
+        # Graviton flag
+        if platform is GRAVITON:
+            self.cflags += ['-mcpu=neoverse-n1']
+
+
 class ClangCompiler(Compiler):
 
     def __init__(self, *args, **kwargs):
         super(ClangCompiler, self).__init__(*args, **kwargs)
 
         self.cflags += ['-Wno-unused-result', '-Wno-unused-variable']
         if not configuration['safe-math']:
@@ -482,19 +493,21 @@
             self.cflags.remove('-std=c99')
         elif platform in [POWER8, POWER9]:
             # It doesn't make much sense to use AOMP on Power, but it should work
             self.cflags.append('-mcpu=native')
         else:
             self.cflags.append('-march=native')
 
-        # amdclang flags, used to be part of aompcc
-        self.ldflags.extend(['-target', 'x86_64-pc-linux-gnu'])
-        self.ldflags.extend(['-fopenmp', '-fopenmp-targets=amdgcn-amd-amdhsa',
-                             '-Xopenmp-target=amdgcn-amd-amdhsa'])
-        self.ldflags.append('-march=%s' % platform.march)
+        # Generic amd flags
+        self.ldflags.extend(['-fopenmp', '-target', 'x86_64-pc-linux-gnu'])
+        # amdclang gpu flags, used to be part of aompcc
+        if platform is AMDGPUX:
+            self.ldflags.extend(['-fopenmp-targets=amdgcn-amd-amdhsa',
+                                 '-Xopenmp-target=amdgcn-amd-amdhsa'])
+            self.ldflags.append('-march=%s' % platform.march)
 
     def __lookup_cmds__(self):
         self.CC = 'amdclang'
         self.CXX = 'amdclang++'
         self.MPICC = 'mpicc'
         self.MPICXX = 'mpicxx'
 
@@ -567,57 +580,67 @@
         super().__init__(*args, cpp=True, **kwargs)
 
         self.cflags.remove('-std=c99')
         self.cflags.remove('-Wall')
         self.cflags.remove('-fPIC')
         self.cflags.extend(['-std=c++14', '-Xcompiler', '-fPIC'])
 
+        if configuration['mpi']:
+            # We rather use `nvcc` to compile MPI, but for this we have to
+            # explicitly pass the flags that an `mpicc` would implicitly use
+            compile_flags, link_flags = sniff_mpi_flags('mpicxx')
+
+            try:
+                # No idea why `-pthread` would pop up among the `compile_flags`
+                compile_flags.remove('-pthread')
+            except ValueError:
+                # Just in case they fix it, we wrap it up within a try-except
+                pass
+            self.cflags.extend(compile_flags)
+
+            # Some arguments are for the host compiler
+            proc_link_flags = []
+            for i in link_flags:
+                if i == '-pthread':
+                    proc_link_flags.extend(['-Xcompiler', '-pthread'])
+                elif i.startswith('-Wl'):
+                    # E.g., `-Wl,-rpath` -> `-Xcompiler "-Wl\,-rpath"`
+                    proc_link_flags.extend([
+                        '-Xcompiler', '"%s"' % i.replace(',', r'\,')
+                    ])
+                else:
+                    proc_link_flags.append(i)
+            self.ldflags.extend(proc_link_flags)
+
+        self.cflags.append('-arch=native')
+
         # Disable `warning #1650-D: result of call is not used`
         # See `https://gist.github.com/gavinb/f2320f9eaa0e0a7efca6877a34047a9d` about
         # disabling specific warnings with nvcc
-        if configuration['mpi']:
-            # mpicc/mpicxx default to `nvc++ ...` (add `--showme` to print out the
-            # actual command line that results from expanding out the mpicc/mpicxx
-            # wrappers). However, mpicc/mpicxx also use the `'-Wl,-rpath'`
-            # GCC-specific options, which means we can't use `nvc++` as host
-            # compiler via `-ccbin=nvc++` either, as otherwise it will complain that
-            # `nvcc fatal   : Unknown option '-Wl,-rpath'`. So the simplest option
-            # for now is to avoid adding the flags below in the `else` branch as
-            # they are `nvcc` specific; `nvc++`, used by mpicc/mpicxx+, will use
-            # `nvcc` eventually (since it reads the file suffix .cu), but somehow
-            # it won't digest the options provided in this format...
-
-            # Also, no need to specify the compute capability via e.g. `-gpu=cc70`,
-            # as nvc++ will automatically compile for the GPU installed in this
-            # system by default
-
-            pass
-        else:
-            self.cflags.append('-arch=native')
-            self.cflags.extend(['-Xcudafe', '--display_error_number',
-                                '--diag-suppress', '1650'])
-            # Same as above but for the host compiler
-            self.cflags.extend(['-Xcompiler', '-Wno-unused-result'])
+        self.cflags.extend(['-Xcudafe', '--display_error_number',
+                            '--diag-suppress', '1650'])
+        # Same as above but for the host compiler
+        self.cflags.extend(['-Xcompiler', '-Wno-unused-result'])
 
-            if not configuration['safe-math']:
-                self.cflags.append('--use_fast_math')
+        if not configuration['safe-math']:
+            self.cflags.append('--use_fast_math')
 
         self.src_ext = 'cu'
 
         # NOTE: not sure where we should place this. It definitely needs
         # to be executed once to warn the user in case there's a CUDA/driver
         # mismatch that would cause the program to run, but likely producing
         # garbage, since the CUDA kernel behaviour would be undefined
         check_cuda_runtime()
 
     def __lookup_cmds__(self):
         self.CC = 'nvcc'
         self.CXX = 'nvcc'
-        self.MPICC = 'mpic++'
-        self.MPICXX = 'mpicxx'
+        self.MPICC = 'nvcc'
+        self.MPICXX = 'nvcc'
 
 
 class HipCompiler(Compiler):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, cpp=True, **kwargs)
 
@@ -760,14 +783,15 @@
         self.MPICXX = environ.get('MPICXX', 'mpicxx')
 
 
 compiler_registry = {
     'custom': CustomCompiler,
     'gnu': GNUCompiler,
     'gcc': GNUCompiler,
+    'arm': ArmCompiler,
     'clang': ClangCompiler,
     'cray': CrayCompiler,
     'aomp': AOMPCompiler,
     'amdclang': AOMPCompiler,
     'hip': HipCompiler,
     'pgcc': PGICompiler,
     'pgi': PGICompiler,
```

### Comparing `devito-4.8.0/devito/builtins/arithmetic.py` & `devito-4.8.1/devito/builtins/arithmetic.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/builtins/initializers.py` & `devito-4.8.1/devito/builtins/initializers.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/builtins/utils.py` & `devito-4.8.1/devito/builtins/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/checkpointing/checkpoint.py` & `devito-4.8.1/devito/checkpointing/checkpoint.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/core/__init__.py` & `devito-4.8.1/devito/core/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/core/autotuning.py` & `devito-4.8.1/devito/core/autotuning.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/core/cpu.py` & `devito-4.8.1/devito/core/cpu.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/core/gpu.py` & `devito-4.8.1/devito/core/gpu.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/core/operator.py` & `devito-4.8.1/devito/core/operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,25 +335,29 @@
     def __new__(cls, items, default=None):
         if not items:
             return None
         elif isinstance(items, bool):
             if not default:
                 raise ValueError("Expected `default` value, got None")
             items = (ParTileArg(as_tuple(default)),)
-        elif isinstance(items, tuple):
+        elif isinstance(items, (list, tuple)):
             if not items:
                 raise ValueError("Expected at least one value")
 
             # Normalize to tuple of ParTileArgs
 
             x = items[0]
             if is_integer(x):
                 # E.g., (32, 4, 8)
                 items = (ParTileArg(items),)
 
+            elif isinstance(x, ParTileArg):
+                # From a reconstruction
+                pass
+
             elif isinstance(x, Iterable):
                 if not x:
                     raise ValueError("Expected at least one value")
 
                 try:
                     y = items[1]
                     if is_integer(y):
@@ -370,10 +374,13 @@
                             items = tuple(ParTileArg(i) for i in items)
                 except IndexError:
                     # E.g., ((32, 4, 8),)
                     items = (ParTileArg(x),)
             else:
                 raise ValueError("Expected int or tuple, got %s instead" % type(x))
         else:
-            raise ValueError("Expected bool or tuple, got %s instead" % type(items))
+            raise ValueError("Expected bool or iterable, got %s instead" % type(items))
+
+        obj = super().__new__(cls, items)
+        obj.default = as_tuple(default)
 
-        return super().__new__(cls, items)
+        return obj
```

### Comparing `devito-4.8.0/devito/data/allocators.py` & `devito-4.8.1/devito/data/allocators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/data/data.py` & `devito-4.8.1/devito/data/data.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/data/decomposition.py` & `devito-4.8.1/devito/data/decomposition.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/data/meta.py` & `devito-4.8.1/devito/data/meta.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/data/utils.py` & `devito-4.8.1/devito/data/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/finite_differences/coefficients.py` & `devito-4.8.1/devito/finite_differences/coefficients.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/finite_differences/derivative.py` & `devito-4.8.1/devito/finite_differences/derivative.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/finite_differences/differentiable.py` & `devito-4.8.1/devito/finite_differences/differentiable.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,17 +224,20 @@
     def __rmod__(self, other):
         return Mod(other, self)
 
     def __neg__(self):
         return Mul(sympy.S.NegativeOne, self)
 
     def __eq__(self, other):
-        return super(Differentiable, self).__eq__(other) and\
-            all(getattr(self, i, None) == getattr(other, i, None)
-                for i in self.__rkwargs__)
+        ret = super(Differentiable, self).__eq__(other)
+        if ret is NotImplemented or not ret:
+            # Non comparable or not equal as sympy objects
+            return False
+        return all(getattr(self, i, None) == getattr(other, i, None)
+                   for i in self.__rkwargs__)
 
     @property
     def name(self):
         return "".join(f.name for f in self._functions)
 
     def shift(self, dim, shift):
         """
```

### Comparing `devito-4.8.0/devito/finite_differences/elementary.py` & `devito-4.8.1/devito/finite_differences/elementary.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,25 +89,21 @@
 def root(x):
     return diffify(sympy.root(x))
 
 
 class Min(sympy.Min, Evaluable):
 
     def _evaluate(self, **kwargs):
-        args = self._evaluate_args(**kwargs)
-        assert len(args) == 2
-        return self.func(args[0], args[1], evaluate=False)
+        return self.func(*self._evaluate_args(**kwargs), evaluate=False)
 
 
 class Max(sympy.Max, Evaluable):
 
     def _evaluate(self, **kwargs):
-        args = self._evaluate_args(**kwargs)
-        assert len(args) == 2
-        return self.func(args[0], args[1], evaluate=False)
+        return self.func(*self._evaluate_args(**kwargs), evaluate=False)
 
 
 def Id(x):
     return diffify(sympy.Id(x))
 
 
 def real_root(x):
```

### Comparing `devito-4.8.0/devito/finite_differences/finite_difference.py` & `devito-4.8.1/devito/finite_differences/finite_difference.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/finite_differences/operators.py` & `devito-4.8.1/devito/finite_differences/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/finite_differences/tools.py` & `devito-4.8.1/devito/finite_differences/tools.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/clusters/algorithms.py` & `devito-4.8.1/devito/ir/clusters/algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from devito.exceptions import InvalidOperator
 from devito.ir.support import (Any, Backward, Forward, IterationSpace,
                                PARALLEL_IF_ATOMIC, pull_dims)
 from devito.ir.clusters.analysis import analyze
 from devito.ir.clusters.cluster import Cluster, ClusterGroup
 from devito.ir.clusters.visitors import Queue, QueueStateful, cluster_pass
+from devito.mpi.halo_scheme import HaloScheme, HaloTouch
 from devito.symbolics import retrieve_indexed, uxreplace, xreplace_indices
 from devito.tools import (DefaultOrderedDict, Stamp, as_mapper, flatten,
                           is_integer, timed_pass)
 from devito.types import Array, Eq, Symbol
 from devito.types.dimension import BOTTOM, ModuloDimension
 
 __all__ = ['clusterize']
@@ -38,14 +39,17 @@
 
     # Determine relevant computational properties (e.g., parallelism)
     clusters = analyze(clusters)
 
     # Input normalization (e.g., SSA)
     clusters = normalize(clusters, **kwargs)
 
+    # Derive the necessary communications for distributed-memory parallelism
+    clusters = Communications().process(clusters)
+
     return ClusterGroup(clusters)
 
 
 class Schedule(QueueStateful):
 
     """
     This special Queue produces a new sequence of "scheduled" Clusters, which
@@ -235,17 +239,14 @@
 class Stepper(Queue):
 
     """
     Produce a new sequence of Clusters in which the IterationSpaces carry the
     sub-iterators induced by a SteppingDimension.
     """
 
-    def process(self, clusters):
-        return self._process_fdta(clusters, 1)
-
     def callback(self, clusters, prefix):
         if not prefix:
             return clusters
 
         d = prefix[-1].dim
 
         subiters = flatten([c.ispace.sub_iterators[d] for c in clusters])
@@ -334,14 +335,75 @@
                                     c.ispace.directions)
 
             processed.append(c.rebuild(exprs=exprs, ispace=ispace))
 
         return processed
 
 
+class Communications(Queue):
+
+    """
+    Enrich a sequence of Clusters by adding special Clusters representing data
+    communications, or "halo exchanges", for distributed parallelism.
+    """
+
+    _q_guards_in_key = True
+    _q_properties_in_key = True
+
+    B = Symbol(name='⊥')
+
+    @timed_pass(name='schedule')
+    def process(self, clusters):
+        return self._process_fatd(clusters, 1, seen=set())
+
+    def callback(self, clusters, prefix, seen=None):
+        if seen.issuperset(clusters):
+            return clusters
+
+        d = prefix[-1].dim
+
+        # Construct the mock exprs representing the halo accesses
+        exprs = []
+        for c in clusters:
+            if c.properties.is_sequential(d):
+                continue
+
+            halo_scheme = HaloScheme(c.exprs, c.ispace)
+
+            if not halo_scheme.is_void and \
+               c.properties.is_parallel_relaxed(d):
+                points = set()
+                for f in halo_scheme.fmapper:
+                    for a in c.scope.getreads(f):
+                        points.add(a.access)
+
+                # We also add all written symbols to ultimately create mock WARs
+                # with `c`, which will prevent the newly created HaloTouch to ever
+                # be rescheduled after `c` upon topological sorting
+                points.update(a.access for a in c.scope.accesses if a.is_write)
+
+                rhs = HaloTouch(*points, halo_scheme=halo_scheme)
+
+                # Insert only if not redundant, to avoid useless pollution
+                if not any(rhs == e.rhs for e in exprs):
+                    exprs.append(Eq(self.B, rhs))
+
+        processed = []
+        if exprs:
+            ispace = prefix[:prefix.index(d)]
+            properties = prefix.properties.drop(d)
+
+            processed.append(Cluster(exprs, ispace, c.guards, properties))
+            seen.update(clusters)
+
+        processed.extend(clusters)
+
+        return processed
+
+
 def normalize(clusters, **kwargs):
     options = kwargs['options']
     sregistry = kwargs['sregistry']
 
     clusters = normalize_nested_indexeds(clusters, sregistry)
     clusters = normalize_reductions(clusters, sregistry, options)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `devito-4.8.0/devito/ir/clusters/analysis.py` & `devito-4.8.1/devito/ir/clusters/analysis.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/clusters/cluster.py` & `devito-4.8.1/devito/ir/clusters/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from devito.ir.equations import ClusterizedEq
 from devito.ir.support import (PARALLEL, PARALLEL_IF_PVT, BaseGuardBoundNext,
                                Forward, Interval, IntervalGroup, IterationSpace,
                                DataSpace, Guards, Properties, Scope, detect_accesses,
                                detect_io, normalize_properties, normalize_syncs,
                                sdims_min, sdims_max)
+from devito.mpi.halo_scheme import HaloTouch
 from devito.symbolics import estimate_cost
 from devito.tools import as_tuple, flatten, frozendict, infer_dtype
 
 __all__ = ["Cluster", "ClusterGroup"]
 
 
 class Cluster(object):
@@ -101,19 +102,19 @@
         if args:
             if len(args) != 1:
                 raise ValueError("rebuild takes at most one positional argument (exprs)")
             if kwargs.get('exprs'):
                 raise ValueError("`exprs` provided both as arg and kwarg")
             kwargs['exprs'] = args[0]
 
-        return Cluster(exprs=kwargs.get('exprs', self.exprs),
-                       ispace=kwargs.get('ispace', self.ispace),
-                       guards=kwargs.get('guards', self.guards),
-                       properties=kwargs.get('properties', self.properties),
-                       syncs=kwargs.get('syncs', self.syncs))
+        return self.__class__(exprs=kwargs.get('exprs', self.exprs),
+                              ispace=kwargs.get('ispace', self.ispace),
+                              guards=kwargs.get('guards', self.guards),
+                              properties=kwargs.get('properties', self.properties),
+                              syncs=kwargs.get('syncs', self.syncs))
 
     @property
     def exprs(self):
         return self._exprs
 
     @property
     def ispace(self):
@@ -207,20 +208,26 @@
             return True
         except ValueError:
             pass
 
         # Fallback to legacy is_dense checks
         return (not any(e.conditionals for e in self.exprs) and
                 not any(f.is_SparseFunction for f in self.functions) and
+                not self.is_halo_touch and
                 all(a.is_regular for a in self.scope.accesses))
 
     @property
     def is_sparse(self):
         return not self.is_dense
 
+    @property
+    def is_halo_touch(self):
+        return (len(self.exprs) > 0 and
+                all(isinstance(e.rhs, HaloTouch) for e in self.exprs))
+
     @cached_property
     def dtype(self):
         """
         The arithmetic data type of the Cluster.
 
         If the Cluster performs floating point arithmetic, then the expressions
         performing integer arithmetic are ignored, assuming that they are only
@@ -409,14 +416,18 @@
         return tuple(i.syncs for i in self)
 
     @cached_property
     def dspace(self):
         """Return the DataSpace of this ClusterGroup."""
         return DataSpace.union(*[i.dspace.reset() for i in self])
 
+    @property
+    def is_halo_touch(self):
+        return all(i.is_halo_touch for i in self)
+
     @cached_property
     def dtype(self):
         """
         The arithmetic data type of this ClusterGroup.
 
         If at least one Cluster performs floating point arithmetic, then the
         Clusters performing integer arithmetic are ignored.
```

### Comparing `devito-4.8.0/devito/ir/clusters/visitors.py` & `devito-4.8.1/devito/ir/clusters/visitors.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     # Handlers for the construction of the key used in the visit
     # Some visitors may need a relaxed key to process together certain groups
     # of Clusters
     _q_ispace_in_key = True
     _q_guards_in_key = False
     _q_properties_in_key = False
+    _q_syncs_in_key = False
 
     def callback(self, *args):
         raise NotImplementedError
 
     def process(self, clusters):
         return self._process_fdta(clusters, 1)
 
@@ -49,15 +50,25 @@
             guards = None
 
         if self._q_properties_in_key:
             properties = cluster.properties.drop(cluster.ispace[level:].itdimensions)
         else:
             properties = None
 
-        prefix = Prefix(ispace, guards, properties)
+        if self._q_syncs_in_key:
+            try:
+                syncs = tuple(cluster.syncs.get(i.dim) for i in ispace)
+            except AttributeError:
+                # `cluster` is actually a ClusterGroup
+                assert len(cluster.syncs) == 1
+                syncs = tuple(cluster.syncs[0].get(i.dim) for i in ispace)
+        else:
+            syncs = None
+
+        prefix = Prefix(ispace, guards, properties, syncs)
 
         subkey = self._make_key_hook(cluster, level)
 
         return (prefix,) + subkey
 
     def _make_key_hook(self, cluster, level):
         return ()
@@ -144,29 +155,31 @@
             for i in prefix:
                 properties[i.dim].update(v.get(i.dim, set()))
         return properties
 
 
 class Prefix(IterationSpace):
 
-    def __init__(self, ispace, guards, properties):
+    def __init__(self, ispace, guards, properties, syncs):
         super().__init__(ispace.intervals, ispace.sub_iterators, ispace.directions)
 
         self.guards = guards
         self.properties = properties
+        self.syncs = syncs
 
     def __eq__(self, other):
         return (isinstance(other, Prefix) and
                 super().__eq__(other) and
                 self.guards == other.guards and
-                self.properties == other.properties)
+                self.properties == other.properties and
+                self.syncs == other.syncs)
 
     def __hash__(self):
         return hash((self.intervals, self.sub_iterators, self.directions,
-                     self.guards, self.properties))
+                     self.guards, self.properties, self.syncs))
 
 
 class cluster_pass(object):
 
     def __new__(cls, *args, mode='dense'):
         if args:
             if len(args) == 1:
```

### Comparing `devito-4.8.0/devito/ir/equations/algorithms.py` & `devito-4.8.1/devito/ir/equations/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/equations/equation.py` & `devito-4.8.1/devito/ir/equations/equation.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/iet/algorithms.py` & `devito-4.8.1/devito/ir/iet/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/iet/efunc.py` & `devito-4.8.1/devito/ir/iet/efunc.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,31 @@
     A Call to an ElementalFunction will "instantiate" such iteration space by
     supplying bounds and step increment for each Dimension listed in
     ``dynamic_parameters``.
     """
 
     is_ElementalFunction = True
 
-    def __init__(self, name, body, retval, parameters=None, prefix=('static', 'inline'),
+    def __init__(self, name, body, retval='void', parameters=None, prefix=('static',),
                  dynamic_parameters=None):
         super(ElementalFunction, self).__init__(name, body, retval, parameters, prefix)
 
         self._mapper = {}
         for i in as_tuple(dynamic_parameters):
             if i.is_Dimension:
                 self._mapper[i] = (parameters.index(i.symbolic_min),
                                    parameters.index(i.symbolic_max))
             else:
                 self._mapper[i] = (parameters.index(i),)
 
+    @classmethod
+    def make(cls, name, body):
+        parameters = derive_parameters(body)
+        return cls(name, body, parameters=parameters)
+
     @cached_property
     def dynamic_defaults(self):
         return {k: tuple(self.parameters[i] for i in v) for k, v in self._mapper.items()}
 
     def make_call(self, dynamic_args_mapper=None, incr=False, retobj=None,
                   is_indirect=False):
         return ElementalCall(self.name, list(self.parameters), dict(self._mapper),
@@ -82,16 +87,17 @@
         return {k: tuple(self.arguments[i] for i in v) for k, v in self._mapper.items()}
 
 
 def make_efunc(name, iet, dynamic_parameters=None, retval='void', prefix='static'):
     """
     Shortcut to create an ElementalFunction.
     """
-    return ElementalFunction(name, iet, retval, derive_parameters(iet), prefix,
-                             dynamic_parameters)
+    return ElementalFunction(name, iet, retval=retval,
+                             parameters=derive_parameters(iet), prefix=prefix,
+                             dynamic_parameters=dynamic_parameters)
 
 
 # Callable machinery
 
 
 def make_callable(name, iet, retval='void', prefix='static'):
     """
```

### Comparing `devito-4.8.0/devito/ir/iet/nodes.py` & `devito-4.8.1/devito/ir/iet/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -618,15 +618,39 @@
             + tuple(flatten(i.symbolic_incr.free_symbols for i in self.uindices))
 
     @property
     def defines(self):
         return self.dimensions
 
 
-class While(Node):
+class DoIf(Node):
+
+    """
+    An abstract Node to express computation subjected to a condition.
+    """
+
+    def __init__(self, condition):
+        self.condition = condition
+
+    @property
+    def functions(self):
+        ret = []
+        for i in self.condition.free_symbols:
+            try:
+                ret.append(i.function)
+            except AttributeError:
+                pass
+        return tuple(ret)
+
+    @property
+    def expr_symbols(self):
+        return tuple(self.condition.free_symbols)
+
+
+class While(DoIf):
 
     """
     Implement a while-loop.
 
     Parameters
     ----------
     condition : sympy.Function or sympy.Relation or bool
@@ -636,15 +660,15 @@
     """
 
     is_While = True
 
     _traversable = ['body']
 
     def __init__(self, condition, body=None):
-        self.condition = condition
+        super().__init__(condition)
         self.body = as_tuple(body)
 
     def __repr__(self):
         return "<While %s; %d>" % (self.condition, len(self.body))
 
 
 class Callable(Node):
@@ -755,15 +779,15 @@
         return ("<CallableBody <unpacks=%d, allocs=%d, casts=%d, maps=%d, "
                 "objs=%d> <unmaps=%d, frees=%d>>" %
                 (len(self.unpacks), len(self.allocs), len(self.casts),
                  len(self.maps), len(self.objs), len(self.unmaps),
                  len(self.frees)))
 
 
-class Conditional(Node):
+class Conditional(DoIf):
 
     """
     A node to express if-then-else blocks.
 
     Parameters
     ----------
     condition : expr-like
@@ -775,39 +799,25 @@
     """
 
     is_Conditional = True
 
     _traversable = ['then_body', 'else_body']
 
     def __init__(self, condition, then_body, else_body=None):
-        self.condition = condition
+        super().__init__(condition)
         self.then_body = as_tuple(then_body)
         self.else_body = as_tuple(else_body)
 
     def __repr__(self):
         if self.else_body:
             return "<[%s] ? [%s] : [%s]>" %\
                 (ccode(self.condition), repr(self.then_body), repr(self.else_body))
         else:
             return "<[%s] ? [%s]" % (ccode(self.condition), repr(self.then_body))
 
-    @property
-    def functions(self):
-        ret = []
-        for i in self.condition.free_symbols:
-            try:
-                ret.append(i.function)
-            except AttributeError:
-                pass
-        return tuple(ret)
-
-    @property
-    def expr_symbols(self):
-        return tuple(self.condition.free_symbols)
-
 
 # Second level IET nodes
 
 class TimedList(List):
 
     """
     Wrap a Node with C-level timers.
```

### Comparing `devito-4.8.0/devito/ir/iet/utils.py` & `devito-4.8.1/devito/ir/iet/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/iet/visitors.py` & `devito-4.8.1/devito/ir/iet/visitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,31 @@
 from collections import OrderedDict
 from collections.abc import Iterable
 from itertools import chain, groupby
 import ctypes
 
 import cgen as c
 from sympy import IndexedBase
+from sympy.core.function import Application
 
 from devito.exceptions import VisitorException
 from devito.ir.iet.nodes import (Node, Iteration, Expression, ExpressionBundle,
                                  Call, Lambda, BlankLine, Section)
 from devito.ir.support.space import Backward
 from devito.symbolics import ListInitializer, ccode, uxreplace
 from devito.tools import (GenericVisitor, as_tuple, ctypes_to_cstr, filter_ordered,
                           filter_sorted, flatten, is_external_ctype, c_restrict_void_p)
 from devito.types.basic import AbstractFunction, Basic
 from devito.types import (ArrayObject, CompositeObject, Dimension, Pointer,
                           IndexedData, DeviceMap)
 
 
-__all__ = ['FindNodes', 'FindSections', 'FindSymbols', 'MapExprStmts', 'MapNodes',
-           'IsPerfectIteration', 'printAST', 'CGen', 'CInterface', 'Transformer',
-           'Uxreplace']
+__all__ = ['FindApplications', 'FindNodes', 'FindSections', 'FindSymbols',
+           'MapExprStmts', 'MapNodes', 'IsPerfectIteration', 'printAST', 'CGen',
+           'CInterface', 'Transformer', 'Uxreplace']
 
 
 class Visitor(GenericVisitor):
 
     def visit_Node(self, o, **kwargs):
         return self._visit(o.children, **kwargs)
 
@@ -893,14 +894,20 @@
         return self.Retval(*[self._visit(i) for i in o])
 
     visit_list = visit_tuple
 
     def visit_Node(self, o):
         return self.Retval(self._visit(o.children), self.rule(o))
 
+    def visit_ThreadedProdder(self, o):
+        # TODO: this handle required because ThreadedProdder suffers from the
+        # long-standing issue affecting all Node subclasses which rely on
+        # multiple inheritance
+        return self.Retval(self._visit(o.then_body), self.rule(o))
+
     def visit_Operator(self, o):
         ret = self._visit(o.body)
         ret.extend(flatten(self._visit(v) for v in o._func_table.values()))
         return self.Retval(ret, self.rule(o))
 
 
 class FindNodes(Visitor):
@@ -949,14 +956,63 @@
         if self.rule(self.match, o):
             ret.append(o)
         for i in o.children:
             ret = self._visit(i, ret=ret)
         return ret
 
 
+class FindApplications(Visitor):
+
+    """
+    Find all SymPy applied functions (aka, `Application`s). The user may refine
+    the search by supplying a different target class.
+    """
+
+    def __init__(self, cls=Application):
+        super().__init__()
+        self.match = lambda i: isinstance(i, cls) and not isinstance(i, Basic)
+
+    @classmethod
+    def default_retval(cls):
+        return set()
+
+    def visit_object(self, o, **kwargs):
+        return self.default_retval()
+
+    def visit_tuple(self, o, ret=None):
+        ret = ret or self.default_retval()
+        for i in o:
+            ret.update(self._visit(i, ret=ret))
+        return ret
+
+    def visit_Node(self, o, ret=None):
+        ret = ret or self.default_retval()
+        for i in o.children:
+            ret.update(self._visit(i, ret=ret))
+        return ret
+
+    def visit_Expression(self, o, **kwargs):
+        return o.expr.find(self.match)
+
+    def visit_Iteration(self, o, **kwargs):
+        ret = self._visit(o.children) or self.default_retval()
+        ret.update(o.symbolic_min.find(self.match))
+        ret.update(o.symbolic_max.find(self.match))
+        return ret
+
+    def visit_Call(self, o, **kwargs):
+        ret = self.default_retval()
+        for i in o.arguments:
+            try:
+                ret.update(i.find(self.match))
+            except (AttributeError, TypeError):
+                continue
+        return ret
+
+
 class IsPerfectIteration(Visitor):
 
     """
     Return True if an Iteration defines a perfect loop nest, False otherwise.
     """
 
     def __init__(self, depth=None):
@@ -1069,16 +1125,19 @@
     """
 
     def visit_Expression(self, o):
         return o._rebuild(expr=uxreplace(o.expr, self.mapper))
 
     def visit_Iteration(self, o):
         nodes = self._visit(o.nodes)
+        dimension = uxreplace(o.dim, self.mapper)
         limits = [uxreplace(i, self.mapper) for i in o.limits]
-        return o._rebuild(nodes=nodes, limits=limits)
+        uindices = [uxreplace(i, self.mapper) for i in o.uindices]
+        return o._rebuild(nodes=nodes, dimension=dimension, limits=limits,
+                          uindices=uindices)
 
     def visit_Definition(self, o):
         try:
             return o._rebuild(function=self.mapper[o.function])
         except KeyError:
             return o
```

### Comparing `devito-4.8.0/devito/ir/stree/algorithms.py` & `devito-4.8.1/devito/ir/stree/algorithms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,220 +1,222 @@
+from collections import defaultdict
+from itertools import groupby
+
 from anytree import findall
 from sympy import And
 
-from itertools import groupby
-
 from devito.ir.clusters import Cluster
 from devito.ir.stree.tree import (ScheduleTree, NodeIteration, NodeConditional,
-                                  NodeSync, NodeExprs, NodeSection, NodeHalo, insert)
-from devito.ir.support import SEQUENTIAL, IterationSpace, normalize_properties
-from devito.mpi.halo_scheme import HaloScheme, HaloSchemeException
-from devito.parameters import configuration
-from devito.tools import Bunch, DefaultOrderedDict, flatten
+                                  NodeSync, NodeExprs, NodeSection, NodeHalo)
+from devito.ir.support import (SEQUENTIAL, Any, Interval, IterationInterval,
+                               IterationSpace, normalize_properties)
+from devito.mpi.halo_scheme import HaloScheme
+from devito.tools import Bunch, DefaultOrderedDict
+from devito.types.dimension import BOTTOM
 
 __all__ = ['stree_build']
 
 
-def stree_build(clusters, **kwargs):
+def stree_build(clusters, profiler=None, **kwargs):
     """
     Create a ScheduleTree from a ClusterGroup.
     """
-    # ClusterGroup -> ScheduleTree
-    stree = stree_schedule(clusters)
-
-    # Add in section nodes
-    stree = stree_section(stree, **kwargs)
-
-    # Add in halo update nodes
-    stree = stree_make_halo(stree)
-
-    return stree
-
+    clusters, hsmap = preprocess(clusters)
 
-def stree_schedule(clusters):
-    """
-    Arrange an iterable of Clusters into a ScheduleTree.
-    """
     stree = ScheduleTree()
+    section = None
 
+    base = IterationInterval(Interval(BOTTOM), [], Any)
     prev = Cluster(None)
-    mapper = DefaultOrderedDict(lambda: Bunch(top=None, bottom=None))
 
-    def reuse_metadata(c0, c1, d):
-        return (c0.guards.get(d) == c1.guards.get(d) and
-                c0.syncs.get(d) == c1.syncs.get(d))
-
-    def attach_metadata(cluster, d, tip):
-        if d in cluster.guards:
-            tip = NodeConditional(cluster.guards[d], tip)
-        if d in cluster.syncs:
-            tip = NodeSync(cluster.syncs[d], tip)
-        return tip
+    mapper = DefaultOrderedDict(lambda: Bunch(top=None, bottom=None))
+    mapper[base] = Bunch(top=stree, bottom=stree)
 
     for c in clusters:
-        index = 0
-
-        # Reuse or add in any Conditionals and Syncs outside of the outermost Iteration
-        if not reuse_metadata(c, prev, None):
-            tip = attach_metadata(c, None, stree)
-            maybe_reusable = []
-        else:
-            try:
-                tip = mapper[prev.itintervals[index]].top.parent
-            except IndexError:
-                tip = stree
+        if reuse_subtree(c, prev):
+            tip = mapper[base].bottom
             maybe_reusable = prev.itintervals
+        else:
+            # Add any guards/Syncs outside of the outermost Iteration
+            tip = augment_subtree(c, None, stree)
+            maybe_reusable = []
 
+        # Is there a HaloTouch to attach?
+        try:
+            hs = hsmap[c]
+        except KeyError:
+            hs = None
+
+        index = 0
         for it0, it1 in zip(c.itintervals, maybe_reusable):
             if it0 != it1:
                 break
-            index += 1
 
             d = it0.dim
+            if needs_nodehalo(d, hs):
+                break
+
+            index += 1
 
             # The reused sub-trees might acquire new sub-iterators as well as
             # new properties
             mapper[it0].top.ispace = IterationSpace.union(
                 mapper[it0].top.ispace, c.ispace.project([d])
             )
             mapper[it0].top.properties = normalize_properties(
                 mapper[it0].top.properties, c.properties[it0.dim]
             )
 
-            # Different guards or SyncOps cannot further be nested
-            if not reuse_metadata(c, prev, d):
+            if reuse_subtree(c, prev, d):
+                tip = mapper[it0].bottom
+            else:
                 tip = mapper[it0].top
-                tip = attach_metadata(c, d, tip)
+                tip = augment_subtree(c, d, tip)
                 mapper[it0].bottom = tip
                 break
-            else:
-                tip = mapper[it0].bottom
 
         # Nested sub-trees, instead, will not be used anymore
         for it in prev.itintervals[index:]:
             mapper.pop(it)
+        prev = c
 
-        # Add in Iterations, Conditionals, and Syncs
+        # Add in Node{Iteration,Conditional,Sync}
         for it in c.itintervals[index:]:
             d = it.dim
             tip = NodeIteration(c.ispace.project([d]), tip, c.properties.get(d, ()))
             mapper[it].top = tip
-            tip = attach_metadata(c, d, tip)
+            tip = augment_subtree(c, d, tip)
             mapper[it].bottom = tip
 
-        # Add in Expressions
+        # Attach NodeHalo if necessary
+        for it, v in mapper.items():
+            if needs_nodehalo(it.dim, hs):
+                v.bottom.parent = NodeHalo(hs, v.bottom.parent)
+                break
+
+        # Add in NodeExprs
         exprs = []
         for conditionals, g in groupby(c.exprs, key=lambda e: e.conditionals):
             exprs = list(g)
 
             # Indirect ConditionalDimensions induce expression-level guards
             if conditionals:
                 guard = And(*conditionals.values(), evaluate=False)
                 parent = NodeConditional(guard, tip)
             else:
                 parent = tip
 
             NodeExprs(exprs, c.ispace, c.dspace, c.ops, c.traffic, parent)
 
-        # Prepare for next iteration
-        prev = c
+        # Nest within a NodeSection if possible
+        if profiler is None or \
+           any(i.is_Section for i in reversed(tip.ancestors)):
+            continue
+
+        candidate = None
+        for i in reversed(tip.ancestors + (tip,)):
+            if i.is_Halo:
+                candidate = i
+            elif i.is_Sync:
+                attach_section(i)
+                section = None
+                break
+            elif i.is_Iteration:
+                if (i.dim.is_Time and SEQUENTIAL in i.properties):
+                    section = attach_section(candidate, section)
+                    break
+                else:
+                    candidate = i
+        else:
+            attach_section(candidate, section)
 
     return stree
 
 
-def stree_make_halo(stree):
+# *** Utility functions to construct the ScheduleTree
+
+
+def preprocess(clusters):
     """
-    Add NodeHalos to a ScheduleTree. A NodeHalo captures the halo exchanges
-    that should take place before executing the sub-tree; these are described
-    by means of a HaloScheme.
+    Remove the HaloTouches from `clusters` and create a mapping associating
+    each removed HaloTouch to the first Cluster necessitating it.
     """
-    # Build a HaloScheme for each expression bundle
-    halo_schemes = {}
-    for n in findall(stree, lambda i: i.is_Exprs):
-        try:
-            halo_schemes[n] = HaloScheme(n.exprs, n.ispace)
-        except HaloSchemeException as e:
-            if configuration['mpi']:
-                raise RuntimeError(str(e))
-
-    # Split a HaloScheme based on where it should be inserted
-    # For example, it's possible that, for a given HaloScheme, a Function's
-    # halo needs to be exchanged at a certain `stree` depth, while another
-    # Function's halo needs to be exchanged before some other nodes
-    mapper = {}
-    for k, hs in halo_schemes.items():
-        for f, v in hs.fmapper.items():
-            spot = k
-            ancestors = [n for n in k.ancestors if n.is_Iteration]
-            for n in ancestors:
-                # Place the halo exchange before the first distributed Dimension
-                if n.dim._defines.intersection(f._dist_dimensions):
-                    spot = n
-                    break
-            mapper.setdefault(spot, []).append(hs.project(f))
+    processed = []
+    hsmap = defaultdict(list)
 
-    # Now fuse the HaloSchemes at the same `stree` depth and perform the insertion
-    for spot, halo_schemes in mapper.items():
-        insert(NodeHalo(HaloScheme.union(halo_schemes)), spot.parent, [spot])
+    queue = []
 
-    return stree
+    for c in clusters:
+        if c.is_halo_touch:
+            queue.append(HaloScheme.union(e.rhs.halo_scheme for e in c.exprs))
+        else:
+            dims = set(c.ispace.promote(lambda d: d.is_Block).itdimensions)
 
+            for hs in list(queue):
+                if hs.distributed_aindices & dims:
+                    queue.remove(hs)
+                    hsmap[c].append(hs)
 
-def stree_section(stree, profiler=None, **kwargs):
-    """
-    Add NodeSections to a ScheduleTree. A NodeSection, or simply "section",
-    defines a sub-tree with the following properties:
+            processed.append(c)
 
-        * The root is a node of type NodeSection;
-        * The immediate children of the root are nodes of type NodeIteration;
-        * The Dimensions of the immediate children are either:
-            * identical, OR
-            * different, but all of type SubDimension;
-        * The Dimension of the immediate children cannot be a TimeDimension.
-    """
-    if profiler is None:
-        return stree
+    hsmap = {c: HaloScheme.union(hss) for c, hss in hsmap.items()}
 
-    class Section(object):
-        def __init__(self, node):
-            self.parent = node.parent
-            try:
-                self.dim = node.dim
-            except AttributeError:
-                self.dim = None
-            self.nodes = [node]
-
-        def is_compatible(self, node):
-            return self.parent == node.parent and self.dim.root == node.dim.root
-
-    # Search candidate sections
-    sections = []
-    for i in range(stree.height):
-        # Find all sections at depth `i`
-        section = None
-        for n in findall(stree, filter_=lambda n: n.depth == i):
-            if any(p in flatten(s.nodes for s in sections) for p in n.ancestors):
-                # Already within a section
-                continue
-            elif n.is_Sync:
-                # SyncNodes are self-contained
-                sections.append(Section(n))
-                section = None
-            elif n.is_Iteration:
-                if n.dim.is_Time and SEQUENTIAL in n.properties:
-                    # If n.dim.is_Time, we end up here in 99.9% of the cases.
-                    # Sometimes, however, time is a PARALLEL Dimension (e.g.,
-                    # think of `norm` Operators)
-                    section = None
-                elif section is None or not section.is_compatible(n):
-                    section = Section(n)
-                    sections.append(section)
-                else:
-                    section.nodes.append(n)
-            else:
-                section = None
+    return processed, hsmap
 
-    # Transform the schedule tree by adding in sections
-    for i in sections:
-        insert(NodeSection(), i.parent, i.nodes)
 
-    return stree
+def reuse_subtree(c0, c1, d=None):
+    return (c0.guards.get(d) == c1.guards.get(d) and
+            c0.syncs.get(d) == c1.syncs.get(d))
+
+
+def augment_subtree(cluster, d, tip):
+    if d in cluster.guards:
+        tip = NodeConditional(cluster.guards[d], tip)
+    if d in cluster.syncs:
+        tip = NodeSync(cluster.syncs[d], tip)
+    return tip
+
+
+def needs_nodehalo(d, hs):
+    return hs and d._defines.intersection(hs.distributed_aindices)
+
+
+def reuse_section(candidate, section):
+    try:
+        if not section or candidate.siblings[-1] is not section:
+            return False
+    except IndexError:
+        return False
+
+    key = lambda i: findall(i, lambda n: n.is_Iteration)
+    iters0 = key(section)
+    iters1 = key(candidate)
+
+    # Heuristics for NodeSection reuse:
+    # * Ignore some kinds of iteration Dimensions
+    key = lambda d: not (d.is_Custom or d.is_Stencil)
+    iters0 = [i for i in iters0 if key(i.dim)]
+    iters1 = [i for i in iters1 if key(i.dim)]
+
+    # * Same set of iteration Dimensions
+    key = lambda i: i.interval.promote(lambda d: d.is_Block).dim
+    test00 = len(iters0) == len(iters1)
+    test01 = all(key(i) is key(j) for i, j in zip(iters0, iters1))
+
+    # * All subtrees use at least one local SubDimension (i.e., BCs)
+    key = lambda iters: any(i.dim.is_Sub and i.dim.local for i in iters)
+    test1 = key(iters0) and key(iters1)
+
+    if (test00 and test01) or test1:
+        candidate.parent = section
+        return True
+    else:
+        return False
+
+
+def attach_section(candidate, section=None):
+    if candidate and not reuse_section(candidate, section):
+        section = NodeSection()
+        section.parent = candidate.parent
+        candidate.parent = section
+
+    return section
```

### Comparing `devito-4.8.0/devito/ir/stree/tree.py` & `devito-4.8.1/devito/ir/stree/tree.py`

 * *Files 26% similar despite different names*

```diff
@@ -120,33 +120,18 @@
         return "[%s]" % ret
 
 
 class NodeHalo(ScheduleTree):
 
     is_Halo = True
 
-    def __init__(self, halo_scheme):
+    def __init__(self, halo_scheme, parent=None):
+        super().__init__(parent)
         self.halo_scheme = halo_scheme
 
     @property
     def __repr_render__(self):
         return "<Halo>"
 
 
-def insert(node, parent, children):
-    """
-    Insert ``node`` between ``parent`` and ``children``, where ``children``
-    are a subset of nodes in ``parent.children``.
-    """
-    processed = []
-    for n in list(parent.children):
-        if n in children:
-            n.parent = node
-            if node not in processed:
-                processed.append(node)
-        else:
-            processed.append(n)
-    parent.children = processed
-
-
 def render(stree):
     return RenderTree(stree, style=ContStyle()).by_attr('__repr_render__')
```

### Comparing `devito-4.8.0/devito/ir/support/basic.py` & `devito-4.8.1/devito/ir/support/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from itertools import chain
 
 from cached_property import cached_property
 from sympy import S
-from sympy.tensor.indexed import IndexException
 
 from devito.ir.support.space import Backward, IterationSpace
 from devito.ir.support.utils import AccessMode
 from devito.ir.support.vector import LabeledVector, Vector
 from devito.symbolics import (retrieve_terminals, q_constant, q_affine, q_routine,
                               q_terminal)
 from devito.tools import (Tag, as_tuple, is_integer, filter_sorted, flatten,
                           memoized_meth, memoized_generator)
-from devito.types import Barrier, Dimension, DimensionTuple, Jump
+from devito.types import Barrier, Dimension, DimensionTuple, Jump, Symbol
 
 __all__ = ['IterationInstance', 'TimedAccess', 'Scope']
 
 
 class IndexMode(Tag):
     """Tag for access functions."""
     pass
 AFFINE = IndexMode('affine')  # noqa
 REGULAR = IndexMode('regular')
 IRREGULAR = IndexMode('irregular')
 
+mocksym = Symbol(name='⋈')
+"""
+A Symbol to create mock data depdendencies.
+"""
+
 
 class IterationInstance(LabeledVector):
 
     """
     A representation of the iteration and data points accessed by an
     Indexed object. Three different concepts are distinguished:
 
@@ -132,14 +136,18 @@
         return DimensionTuple(*retval, getters=self.findices)
 
     @property
     def findices(self):
         return self.labels
 
     @cached_property
+    def index_map(self):
+        return dict(zip(self.aindices, self.findices))
+
+    @cached_property
     def defined_findices_affine(self):
         ret = set()
         for fi, im in zip(self.findices, self.index_mode):
             if im is AFFINE:
                 ret.update(fi._defines)
         return ret
 
@@ -393,17 +401,25 @@
                 # E.g., `self=R<u,[t+1, ii_src_0+1, ii_src_1+2]>` and `fi=p_src` (`n=1`)
                 ret.append(S.Infinity)
                 break
 
         if S.Infinity in ret:
             return Vector(*ret)
 
+        n = len(ret)
+
+        # It might be `a[t, ⊥] -> a[t, x+1]`, that is the source is a special
+        # Indexed representing an arbitrary access along `x`, within the `t`
+        # IterationSpace, while the sink lives within the `tx` IterationSpace
+        if len(self.itintervals[n:]) != len(other.itintervals[n:]):
+            ret.append(S.Infinity)
+            return Vector(*ret)
+
         # It still could be an imaginary dependence, e.g. `a[3] -> a[4]` or, more
         # nasty, `a[i+1, 3] -> a[i, 4]`
-        n = len(ret)
         for i, j in zip(self[n:], other[n:]):
             if i == j:
                 ret.append(S.Zero)
             else:
                 v = i - j
                 if v.is_Number and v.is_finite:
                     return Vector(S.ImaginaryUnit)
@@ -815,25 +831,21 @@
                 v = self.reads.setdefault(i.function, [])
                 v.append(TimedAccess(i, 'R', -1))
 
         # Objects altering the control flow (e.g., synchronization barriers,
         # break statements, ...) are converted into mock dependences
         for i, e in enumerate(exprs):
             if e.find(Barrier) | e.find(Jump):
-                for a in self.accesses:
-                    f = a.function
-                    indices = [i if d in e.ispace else S.Infinity
-                               for i, d in zip(a, a.aindices)]
-                    try:
-                        mock = f.indexify(indices)
-                    except IndexException:
-                        continue
-                    v = self.writes.setdefault(f, [])
-                    v.extend([TimedAccess(mock, 'R', i, e.ispace),
-                              TimedAccess(mock, 'W', i, e.ispace)])
+                self.writes.setdefault(mocksym, []).append(
+                    TimedAccess(mocksym, 'W', i, e.ispace)
+                )
+                self.reads.setdefault(mocksym, []).extend([
+                    TimedAccess(mocksym, 'R', max(i, 0), e.ispace),
+                    TimedAccess(mocksym, 'R', i+1, e.ispace),
+                ])
 
         # A set of rules to drive the collection of dependencies
         self.rules = as_tuple(rules)
         assert all(callable(i) for i in self.rules)
 
     def getreads(self, function):
         return as_tuple(self.reads.get(function))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `devito-4.8.0/devito/ir/support/guards.py` & `devito-4.8.1/devito/ir/support/guards.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/support/properties.py` & `devito-4.8.1/devito/ir/support/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 
 VECTORIZED = Property('vector-dim')
 """A SIMD-vectorized Dimension."""
 
 TILABLE = Property('tilable')
 """A fully parallel Dimension that would benefit from tiling (or "blocking")."""
 
+TILABLE_SMALL = Property('tilable*')
+"""
+Like TILABLE, but it would benefit from relatively small block, since the
+iteration space is likely to be very small.
+"""
+
 SKEWABLE = Property('skewable')
 """A fully parallel Dimension that would benefit from wavefront/skewed tiling."""
 
 ROUNDABLE = Property('roundable')
 """
 A Dimension whose upper limit may be rounded up to a multiple of the SIMD
 vector length thanks to the presence of enough padding.
@@ -85,26 +91,31 @@
 """
 A Dimension defining an iteration space that is guaranteed to generate in-bounds
 array accesses, typically through the use of custom conditionals in the body. This
 is used for iteration spaces that are larger than the data space.
 """
 
 
+# Bundles
+PARALLELS = {PARALLEL, PARALLEL_INDEP, PARALLEL_IF_ATOMIC, PARALLEL_IF_PVT}
+TILABLES = {TILABLE, TILABLE_SMALL}
+
+
 def normalize_properties(*args):
     if not args:
         return
     elif len(args) == 1:
         return args[0]
 
     # Some properties are incompatible, such as SEQUENTIAL and PARALLEL where
     # SEQUENTIAL clearly takes precedence. The precedence chain, from the least
     # to the most restrictive property, is:
     # SEQUENTIAL > PARALLEL_IF_* > PARALLEL > PARALLEL_INDEP
     if any(SEQUENTIAL in p for p in args):
-        drop = {PARALLEL, PARALLEL_INDEP, PARALLEL_IF_ATOMIC, PARALLEL_IF_PVT}
+        drop = PARALLELS
     elif any(PARALLEL_IF_ATOMIC in p for p in args):
         drop = {PARALLEL, PARALLEL_INDEP}
     elif any(PARALLEL_IF_PVT in p for p in args):
         drop = {PARALLEL}
     elif any(PARALLEL_INDEP not in p for p in args):
         drop = {PARALLEL_INDEP}
     else:
@@ -133,15 +144,21 @@
 
     def add(self, dims, properties=None):
         m = dict(self)
         for d in as_tuple(dims):
             m[d] = set(self.get(d, [])) | set(as_tuple(properties))
         return Properties(m)
 
-    def drop(self, dims, properties=None):
+    def filter(self, key):
+        m = {d: v for d, v in self.items() if key(d)}
+        return Properties(m)
+
+    def drop(self, dims=None, properties=None):
+        if dims is None:
+            dims = list(self)
         m = dict(self)
         for d in as_tuple(dims):
             if properties is None:
                 m.pop(d, None)
             else:
                 m[d] = self[d] - set(as_tuple(properties))
         return Properties(m)
@@ -163,29 +180,50 @@
 
     def sequentialize(self, dims):
         m = dict(self)
         for d in as_tuple(dims):
             m[d] = normalize_properties(set(self.get(d, [])), {SEQUENTIAL})
         return Properties(m)
 
+    def block(self, dims, kind='default'):
+        if kind == 'default':
+            p = TILABLE
+        elif kind == 'small':
+            p = TILABLE_SMALL
+        else:
+            raise ValueError
+        m = dict(self)
+        for d in as_tuple(dims):
+            m[d] = set(self.get(d, [])) | {p}
+        return Properties(m)
+
     def inbound(self, dims):
         m = dict(self)
         for d in as_tuple(dims):
             m[d] = set(m.get(d, [])) | {INBOUND}
         return Properties(m)
 
     def is_parallel(self, dims):
         return any(len(self[d] & {PARALLEL, PARALLEL_INDEP}) > 0
                    for d in as_tuple(dims))
 
     def is_parallel_relaxed(self, dims):
-        items = {PARALLEL, PARALLEL_INDEP, PARALLEL_IF_ATOMIC, PARALLEL_IF_PVT}
-        return any(len(self[d] & items) > 0 for d in as_tuple(dims))
+        return any(len(self[d] & PARALLELS) > 0 for d in as_tuple(dims))
 
     def is_affine(self, dims):
         return any(AFFINE in self.get(d, ()) for d in as_tuple(dims))
 
     def is_inbound(self, dims):
         return any(INBOUND in self.get(d, ()) for d in as_tuple(dims))
 
     def is_sequential(self, dims):
         return any(SEQUENTIAL in self.get(d, ()) for d in as_tuple(dims))
+
+    def is_blockable(self, d):
+        return bool(self.get(d, set()) & {TILABLE, TILABLE_SMALL})
+
+    def is_blockable_small(self, d):
+        return TILABLE_SMALL in self.get(d, set())
+
+    @property
+    def nblockable(self):
+        return sum([self.is_blockable(d) for d in self])
```

### Comparing `devito-4.8.0/devito/ir/support/space.py` & `devito-4.8.1/devito/ir/support/space.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from devito.ir.support.utils import sdims_min, sdims_max
 from devito.ir.support.vector import Vector, vmin, vmax
 from devito.tools import (PartialOrderTuple, Stamp, as_list, as_tuple, filter_ordered,
                           flatten, frozendict, is_integer, toposort)
 from devito.types import Dimension, ModuloDimension
 
 __all__ = ['NullInterval', 'Interval', 'IntervalGroup', 'IterationSpace',
-           'DataSpace', 'Forward', 'Backward', 'Any']
+           'IterationInterval', 'DataSpace', 'Forward', 'Backward', 'Any']
 
 
 # The default Stamp, used by all new Intervals
 S0 = Stamp()
 
 
 class AbstractInterval(object):
@@ -118,15 +118,15 @@
     An Interval defines the compact region
 
         [dim.symbolic_min + lower, dim.symbolic_max + upper]
     """
 
     is_Defined = True
 
-    def __init__(self, dim, lower, upper, stamp=S0):
+    def __init__(self, dim, lower=0, upper=0, stamp=S0):
         super(Interval, self).__init__(dim, stamp)
 
         try:
             self.lower = int(lower)
         except TypeError:
             assert isinstance(lower, Expr)
             self.lower = lower
```

### Comparing `devito-4.8.0/devito/ir/support/symregistry.py` & `devito-4.8.1/devito/ir/support/symregistry.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/support/syncs.py` & `devito-4.8.1/devito/ir/support/syncs.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,16 @@
                 self.function is other.function and
                 self.findex == other.findex and
                 self.dim is other.dim and
                 self.size == other.size and
                 self.origin == other.origin)
 
     def __hash__(self):
-        return id(self)
+        return hash((self.__class__, self.handle, self.target, self.tindex,
+                     self.function, self.findex, self.dim, self.size, self.origin))
 
     def __repr__(self):
         return "%s<%s>" % (self.__class__.__name__, self.handle)
 
     __str__ = __repr__
 
     @property
```

### Comparing `devito-4.8.0/devito/ir/support/utils.py` & `devito-4.8.1/devito/ir/support/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/ir/support/vector.py` & `devito-4.8.1/devito/ir/support/vector.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/logger.py` & `devito-4.8.1/devito/logger.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/mpi/distributed.py` & `devito-4.8.1/devito/mpi/distributed.py`

 * *Files 11% similar despite different names*

```diff
@@ -200,14 +200,18 @@
                 # * topology[0] >= topology[1] >= topology[2]
                 # * topology[0] * topology[1] * topology[2] == self._input_comm.size
                 # However, `MPI.Compute_dims` is distro-dependent, so we have to enforce
                 # some properties through our own wrapper (e.g., OpenMPI v3 does not
                 # guarantee that 9 ranks are arranged into a 3x3 grid when shape=(9, 9))
                 self._topology = compute_dims(self._input_comm.size, len(shape))
             else:
+                # A custom topology may contain integers or the wildcard '*', which
+                # implies `nprocs // nstars`
+                topology = CustomTopology(topology, self._input_comm)
+
                 self._topology = topology
 
             if self._input_comm is not input_comm:
                 # By default, Devito arranges processes into a cartesian topology.
                 # MPI works with numbered dimensions and follows the C row-major
                 # numbering of the ranks, i.e. in a 2x3 Cartesian topology (0,0)
                 # maps to rank 0, (0,1) maps to rank 1, (0,2) maps to rank 2, (1,0)
@@ -249,17 +253,26 @@
         else:
             return 1
 
     @property
     def topology(self):
         return self._topology
 
+    @property
+    def topology_logical(self):
+        if isinstance(self.topology, CustomTopology):
+            return self.topology.logical
+        else:
+            return None
+
     @cached_property
     def is_boundary_rank(self):
-        """ MPI rank interfaces with the boundary of the domain. """
+        """
+        MPI rank interfaces with the boundary of the domain.
+        """
         return any([True if i == 0 or i == j-1 else False for i, j in
                    zip(self.mycoords, self.topology)])
 
     @cached_property
     def all_coords(self):
         """
         The coordinates of each MPI rank in the decomposed domain, ordered
@@ -546,14 +559,69 @@
         # Update `nb` based on object attached to `grid`
         if grid is not None:
             return grid.distributor._obj_neighborhood._arg_defaults()
         else:
             return self._arg_defaults()
 
 
+class CustomTopology(tuple):
+
+    """
+    A CustomTopology is a mechanism to describe parametric domain decompositions.
+
+    Examples
+    --------
+    Assuming a domain consisting of three distributed Dimensions x, y, and z, and
+    an MPI communicator comprising N processes, a CustomTopology might be:
+
+    With N known, say N=4:
+
+    * `(1, 1, 4)`: the z Dimension is decomposed into 4 chunks
+    * `(2, 1, 2)`: the x Dimension is decomposed into 2 chunks; the z Dimension
+                   is decomposed into 2 chunks
+
+    With N unknown:
+
+    * `(1, '*', 1)`: the wildcard `'*'` tells the runtime to decompose the y
+                     Dimension into N chunks
+    * `('*', '*', 1)`: the wildcard `'*'` tells the runtime to decompose both the
+                       x and y Dimensions into N / 2 chunks respectively.
+
+    Raises
+    ------
+    N must evenly divide the number of `'*'`, otherwise a ValueError exception
+    is raised.
+    If the wildcard `'*'` is used, then the CustomTopology can only contain either
+    `'*'` or 1's, otherwise a ValueError exception is raised.
+
+    Notes
+    -----
+    Users shouldn't use this class directly. It's up to the Devito runtime to
+    instantiate it based on the user input.
+    """
+
+    def __new__(cls, items, input_comm):
+        nstars = len([i for i in items if i == '*'])
+        if nstars > 0:
+            if input_comm.size % nstars != 0:
+                raise ValueError("Invalid `topology` for given nprocs")
+            if any(i not in ('*', 1) for i in items):
+                raise ValueError("Custom topology must be only 1 or *")
+
+            v = input_comm.size // nstars
+            processed = [i if i == 1 else v for i in items]
+        else:
+            processed = items
+
+        obj = super().__new__(cls, processed)
+        obj.logical = items
+
+        return obj
+
+
 def compute_dims(nprocs, ndim):
     # We don't do anything clever here. In fact, we do something very basic --
     # we just try to distribute `nprocs` evenly over the number of dimensions,
     # and if we can't we fallback to whatever MPI.Compute_dims gives...
     v = pow(nprocs, 1/ndim)
     if not v.is_integer():
         # Since pow(64, 1/3) == 3.999..4
```

### Comparing `devito-4.8.0/devito/mpi/halo_scheme.py` & `devito-4.8.1/devito/mpi/halo_scheme.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,76 @@
 from collections import OrderedDict, namedtuple, defaultdict
 from itertools import product
 from operator import attrgetter
 
 from cached_property import cached_property
 from sympy import Max, Min
+import sympy
 
+from devito import configuration
 from devito.data import CORE, OWNED, LEFT, CENTER, RIGHT
 from devito.ir.support import Forward, Scope
-from devito.tools import Tag, as_tuple, filter_ordered, flatten, frozendict, is_integer
+from devito.tools import (Reconstructable, Tag, as_tuple, filter_ordered, flatten,
+                          frozendict, is_integer)
 from devito.types import Grid
 
-__all__ = ['HaloScheme', 'HaloSchemeEntry', 'HaloSchemeException']
+__all__ = ['HaloScheme', 'HaloSchemeEntry', 'HaloSchemeException', 'HaloTouch']
 
 
 class HaloSchemeException(Exception):
     pass
 
 
 class HaloLabel(Tag):
     pass
 NONE = HaloLabel('none')  # noqa
 IDENTITY = HaloLabel('identity')
 STENCIL = HaloLabel('stencil')
 
 
-HaloSchemeEntry = namedtuple('HaloSchemeEntry', 'loc_indices loc_dirs halos')
+HaloSchemeEntry = namedtuple('HaloSchemeEntry', 'loc_indices loc_dirs halos dims')
 
 Halo = namedtuple('Halo', 'dim side')
 
 OMapper = namedtuple('OMapper', 'core owned')
 
 
 class HaloScheme(object):
 
     """
     A HaloScheme describes a set of halo exchanges through a mapper:
 
         `M : Function -> HaloSchemeEntry`
 
-    Where `HaloSchemeEntry` is a (named) 3-tuple:
+    Where `HaloSchemeEntry` is a (named) 4-tuple:
 
-        `(loc_indices={}, loc_dirs={}, halos=[(Dimension, DataSide), ...])`
+        `(loc_indices={}, loc_dirs={}, halos=set(), dims=set())`
 
     `loc_indices` is a dict telling how to access/insert the halo along non-halo
     indices. For example, consider the Function `u(t, x, y)`. Assume `x` and
     `y` require a halo exchange. The question is: once the halo exchange is
     performed, at what offset in `t` should it be placed? should it be at `u(0,
     ...)` or `u(1, ...)` or even `u(t-1, ...)`? `loc_indices` has as many
     entries as non-halo Dimensions, and each entry provides symbolic information
     about how to access the corresponding non-halo Dimension. For example, here
     `loc_indices` could be `{t: t-1}`.
 
     `loc_dirs` is a dict describing the iteration direction of each Dimension
     in `loc_indices`. This information is used to perform operations over a set
     of HaloSchemeEntries, such as computing their union.
 
-    `halos` is a list of 2-tuples `(Dimension, DataSide)`. This is metadata
+    `halos` is a set of 2-tuples `(Dimension, DataSide)`. This is metadata
     about the halo exchanges, such as the Dimensions along which a halo exchange
     is expected to be performed.
 
+    `dims` is the set of Dimensions with which the distributed Dimensions of the
+    HaloScheme are accessed. Most of the times `dims` will coincide with the set
+    of distributed Dimensions itself. However, we also support the case in which
+    arbitrary Dimensions are used in place of x/y/z, e.g. `u[t0, i]` for `u(t, x)`.
+
     Parameters
     ----------
     exprs : expr-like or list of expr-like
         The expressions for which the HaloScheme is derived.
     ispace : IterationSpace
         The iteration space of the expressions.
     """
@@ -86,15 +94,17 @@
         self._honored = frozendict(self._honored)
 
     def __repr__(self):
         fnames = ",".join(i.name for i in set(self._mapper))
         return "HaloScheme<%s>" % fnames
 
     def __eq__(self, other):
-        return isinstance(other, HaloScheme) and self.fmapper == other.fmapper
+        return (isinstance(other, HaloScheme) and
+                self._mapper == other._mapper and
+                self._honored == other._honored)
 
     def __len__(self):
         return len(self._mapper)
 
     def __hash__(self):
         return (self._mapper.__hash__(), self.honored.__hash__())
 
@@ -113,35 +123,37 @@
         fmapper = {}
         honored = {}
         for i in as_tuple(halo_schemes):
             # Compute the `fmapper `union`
             for k, v in i.fmapper.items():
                 hse = fmapper.setdefault(k, v)
 
-                if hse.loc_indices != v.loc_indices:
+                if not hse.loc_indices:
+                    loc_indices, loc_dirs = v.loc_indices, v.loc_dirs
+                elif not v.loc_indices or hse.loc_indices == v.loc_indices:
+                    loc_indices, loc_dirs = hse.loc_indices, hse.loc_dirs
+                else:
                     # The `loc_dirs` must match otherwise it'd be a symptom there's
                     # something horribly broken elsewhere!
                     assert hse.loc_dirs == v.loc_dirs
                     assert list(hse.loc_indices) == list(v.loc_indices)
 
                     # NOTE: we rarely end up here, but still, if we do, we need
                     # to compute the union of the loc_indices as well and then
                     # take the min/max along each direction, just like when we
                     # build an HaloScheme
                     raw_loc_indices = {d: (hse.loc_indices[d], v.loc_indices[d])
                                        for d in hse.loc_indices}
                     loc_indices, loc_dirs = process_loc_indices(raw_loc_indices,
                                                                 hse.loc_dirs)
-                else:
-                    loc_indices, loc_dirs = hse.loc_indices, hse.loc_dirs
 
-                # Potentially more halo exchanges required
                 halos = hse.halos | v.halos
+                dims = hse.dims | v.dims
 
-                fmapper[k] = HaloSchemeEntry(loc_indices, loc_dirs, halos)
+                fmapper[k] = HaloSchemeEntry(loc_indices, loc_dirs, halos, dims)
 
             # Compute the `honored` union
             for d, v in i.honored.items():
                 honored[d] = honored.get(d, frozenset()) | v
 
         return HaloScheme.build(fmapper, honored)
 
@@ -333,14 +345,22 @@
         for i in set().union(*self.halos.values()):
             if isinstance(i.dim, tuple) or i.side is CENTER:
                 continue
             retval.add(i.dim)
         return retval
 
     @cached_property
+    def distributed(self):
+        return set().union(*[f._dist_dimensions for f in self.fmapper])
+
+    @cached_property
+    def distributed_aindices(self):
+        return set().union(*[i.dims for i in self.fmapper.values()])
+
+    @cached_property
     def arguments(self):
         return self.dimensions | set(flatten(self.honored.values()))
 
     def project(self, functions):
         """
         Create a new HaloScheme which only retains the HaloSchemeEntries corresponding
         to the provided ``functions``.
@@ -355,44 +375,63 @@
         """
         fmapper = {f: v for f, v in self.fmapper.items() if f not in as_tuple(functions)}
         return HaloScheme.build(fmapper, self.honored)
 
 
 def classify(exprs, ispace):
     """
-    Produce the mapper ``Function -> HaloSchemeEntry``, which describes the
-    necessary halo exchanges in the given Scope.
+    Produce the mapper `Function -> HaloSchemeEntry`, which describes the necessary
+    halo exchanges in the given Scope.
     """
+
+    # Some MPI modes require pulling the `loc_indices` from the reads, others
+    # from the writes. It essentially depends on whether the halo exchange is
+    # performed before (reads) or after (writes) the OWNED region is computed
+    loc_indices_from_reads = configuration['mpi'] not in ('dual',)
+
     scope = Scope(exprs)
 
     mapper = {}
     for f, r in scope.reads.items():
         if not f.is_DiscreteFunction:
             continue
         elif not isinstance(f.grid, Grid):
             # TODO: improve me
             continue
 
+        # In the case of custom topologies, we ignore the Dimensions that aren't
+        # practically subjected to domain decomposition
+        dist = f.grid.distributor
+        try:
+            ignored = [d for i, d in zip(dist.topology_logical, dist.dimensions)
+                       if i == 1]
+        except TypeError:
+            ignored = []
+
         # For each data access, determine if (and what type of) a halo exchange
         # is required
+        dims = set()
         halo_labels = defaultdict(set)
         for i in r:
             v = {}
             for d in i.findices:
                 if f.grid.is_distributed(d):
-                    if i.affine(d):
+                    if d in ignored:
+                        v[(d, LEFT)] = IDENTITY
+                        v[(d, RIGHT)] = IDENTITY
+                    elif i.affine(d):
                         thl, thr = i.touched_halo(d)
                         # Note: if the left-HALO is touched (i.e., `thl = True`), then
                         # the *right-HALO* is to be sent over in a halo exchange
                         v[(d, LEFT)] = (thr and STENCIL) or IDENTITY
                         v[(d, RIGHT)] = (thl and STENCIL) or IDENTITY
                     else:
                         v[(d, LEFT)] = STENCIL
                         v[(d, RIGHT)] = STENCIL
-                else:
+                elif loc_indices_from_reads:
                     v[(d, i[d])] = NONE
 
             # Does `i` actually require a halo exchange?
             if not any(hl is STENCIL for hl in v.values()):
                 continue
 
             # Derive diagonal halo exchanges from the previous analysis
@@ -403,38 +442,56 @@
                 if all(v.get((d, s)) is STENCIL or s is CENTER for d, s in zip(*key)):
                     v[key] = STENCIL
 
             # Finally update the `halo_labels`
             for j, hl in v.items():
                 halo_labels[j].add(hl)
 
+            # Populate `dims`
+            for ai, d in i.index_map.items():
+                if ai is not None and f.grid.is_distributed(d):
+                    if ai.is_NonlinearDerived:
+                        dims.add(ai.parent)
+                    else:
+                        dims.add(ai)
+
         if not halo_labels:
             continue
 
-        # Distinguish between Dimensions requiring a halo exchange and those which don't
+        # Augment `halo_labels` with `loc_indices`-related information if necessary
+        if not loc_indices_from_reads:
+            for i in scope.writes.get(f, []):
+                for d in i.findices:
+                    if not f.grid.is_distributed(d):
+                        halo_labels[(d, i[d])].add(NONE)
+
+        # Separate halo-exchange Dimensions from `loc_indices`
         raw_loc_indices, halos = defaultdict(list), []
         for (d, s), hl in halo_labels.items():
             try:
                 hl.remove(IDENTITY)
             except KeyError:
                 pass
             if not hl:
                 continue
             elif len(hl) > 1:
                 raise HaloSchemeException("Inconsistency found while building a halo "
-                                          "scheme for `%s` along Dimension `%s`" % (f, d))
+                                          "scheme for `%s` along Dimension `%s`"
+                                          % (f, d))
             elif hl.pop() is STENCIL:
                 halos.append(Halo(d, s))
             else:
                 raw_loc_indices[d].append(s)
 
         loc_indices, loc_dirs = process_loc_indices(raw_loc_indices,
                                                     ispace.directions)
+        halos = frozenset(halos)
+        dims = frozenset(dims)
 
-        mapper[f] = HaloSchemeEntry(loc_indices, loc_dirs, frozenset(halos))
+        mapper[f] = HaloSchemeEntry(loc_indices, loc_dirs, halos, dims)
 
     return mapper
 
 
 def process_loc_indices(raw_loc_indices, directions):
     """
     Process the loc_indices given in raw form.
@@ -477,7 +534,38 @@
             loc_indices[d] = 0
 
     # Normalize directions
     known = set().union(*[i._defines for i in loc_indices])
     loc_dirs = {d: v for d, v in directions.items() if d in known}
 
     return frozendict(loc_indices), frozendict(loc_dirs)
+
+
+class HaloTouch(sympy.Function, Reconstructable):
+
+    """
+    A SymPy object representing halo accesses through a HaloScheme.
+    """
+
+    __rargs__ = ('args',)
+    __rkwargs__ = ('halo_scheme',)
+
+    def __new__(cls, *args, halo_scheme=None, **kwargs):
+        obj = super().__new__(cls, *args)
+        obj.halo_scheme = halo_scheme
+        return obj
+
+    def __repr__(self):
+        return "HaloTouch(%s)" % ",".join(f.name for f in self.halo_scheme.fmapper)
+
+    __str__ = __repr__
+
+    def _sympystr(self, printer):
+        return str(self)
+
+    def __hash__(self):
+        return id(self)
+
+    def __eq__(self, other):
+        return isinstance(other, HaloTouch) and self.halo_scheme == other.halo_scheme
+
+    func = Reconstructable._rebuild
```

### Comparing `devito-4.8.0/devito/mpi/routines.py` & `devito-4.8.1/devito/mpi/routines.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from itertools import product
 from operator import mul
 
 from sympy import Integer
 
 from devito.data import OWNED, HALO, NOPAD, LEFT, CENTER, RIGHT
 from devito.ir.equations import DummyEq
-from devito.ir.iet import (Call, Callable, Conditional, Expression, ExpressionBundle,
-                           AugmentedExpression, Iteration, List, Prodder, Return,
-                           make_efunc, FindNodes, Transformer)
+from devito.ir.iet import (Call, Callable, Conditional, ElementalFunction,
+                           Expression, ExpressionBundle, AugmentedExpression,
+                           Iteration, List, Prodder, Return, make_efunc, FindNodes,
+                           Transformer)
 from devito.mpi import MPI
 from devito.symbolics import (Byref, CondNe, FieldFromPointer, FieldFromComposite,
                               IndexedPointer, Macro, cast_mapper, subs_op_args)
 from devito.tools import (dtype_to_mpitype, dtype_len, dtype_to_ctype, flatten,
                           generator)
 from devito.types import Array, Dimension, Eq, Symbol, LocalObject, CompositeObject
 
@@ -54,21 +55,14 @@
     def msgs(self):
         return [i for i in self._msgs.values() if i is not None]
 
     @property
     def regions(self):
         return [i for i in self._regions.values() if i is not None]
 
-    @property
-    def headers(self):
-        """
-        No headers needed by default
-        """
-        return {}
-
     def make(self, hs):
         """
         Construct Callables and Calls implementing distributed-memory halo
         exchange for the HaloSpot ``hs``.
         """
         # Sanity check
         assert all(f.is_Function and f.grid is not None for f in hs.fmapper)
@@ -113,23 +107,18 @@
         halowaits = []
         for i, (f, hse) in enumerate(hs.fmapper.items()):
             msg = self._msgs[(f, hse)]
             haloupdate, halowait = mapper[(f, hse)]
             haloupdates.append(self._call_haloupdate(haloupdate.name, f, hse, msg))
             if halowait is not None:
                 halowaits.append(self._call_halowait(halowait.name, f, hse, msg))
-        body = []
-        body.append(HaloUpdateList(body=haloupdates))
-        if callcompute is not None:
-            body.append(callcompute)
-        body.append(HaloWaitList(body=halowaits))
-        if remainder is not None:
-            body.append(self._call_remainder(remainder))
 
-        return List(body=body)
+        body = self._make_body(callcompute, remainder, haloupdates, halowaits)
+
+        return body
 
     @abc.abstractmethod
     def _make_region(self, hs, key):
         """
         Construct an MPIRegion describing the HaloSpot's OWNED DataRegion.
         """
         return
@@ -258,14 +247,22 @@
     def _call_remainder(self, remainder):
         """
         Construct a Call to ``remainder``, the Callable produced by
         :meth:`_make_remainder`.
         """
         return
 
+    @abc.abstractmethod
+    def _make_body(self, callcompute, remainder, haloupdates, halowaits):
+        """
+        Chain together the `compute`, `remainder`, `haloupdate`, and `halowait`
+        Calls.
+        """
+        return
+
 
 class BasicHaloExchangeBuilder(HaloExchangeBuilder):
 
     """
     A HaloExchangeBuilder making use of synchronous MPI routines only.
 
     Generates:
@@ -340,16 +337,16 @@
 
         ofsg = [Symbol(name='og%s' % d.root) for d in f.dimensions]
         ofss = [Symbol(name='os%s' % d.root) for d in f.dimensions]
 
         fromrank = Symbol(name='fromrank')
         torank = Symbol(name='torank')
 
-        gather = Call('gather%s' % key, [bufg] + list(bufg.shape) + [f] + ofsg)
-        scatter = Call('scatter%s' % key, [bufs] + list(bufs.shape) + [f] + ofss)
+        gather = Gather('gather%s' % key, [bufg] + list(bufg.shape) + [f] + ofsg)
+        scatter = Scatter('scatter%s' % key, [bufs] + list(bufs.shape) + [f] + ofss)
 
         # The `gather` is unnecessary if sending to MPI.PROC_NULL
         gather = Conditional(CondNe(torank, Macro('MPI_PROC_NULL')), gather)
         # The `scatter` must be guarded as we must not alter the halo values along
         # the domain boundary, where the sender is actually MPI.PROC_NULL
         scatter = Conditional(CondNe(fromrank, Macro('MPI_PROC_NULL')), scatter)
 
@@ -450,14 +447,26 @@
 
     def _make_remainder(self, *args):
         return
 
     def _call_remainder(self, *args):
         return
 
+    def _make_body(self, callcompute, remainder, haloupdates, halowaits):
+        body = []
+
+        body.append(HaloUpdateList(body=haloupdates))
+        if callcompute is not None:
+            body.append(callcompute)
+        body.append(HaloWaitList(body=halowaits))
+        if remainder is not None:
+            body.append(self._call_remainder(remainder))
+
+        return List(body=body)
+
 
 class DiagHaloExchangeBuilder(BasicHaloExchangeBuilder):
 
     """
     Similar to a BasicHaloExchangeBuilder, but communications to diagonal
     neighbours are performed explicitly.
 
@@ -513,22 +522,14 @@
 
         haloupdate()
         compute_core()
         halowait()
         remainder()
     """
 
-    @property
-    def headers(self):
-        """
-        Overlap Mode uses MIN/MAX that need to be defined
-        """
-        return {'headers': [('MIN(a,b)', ('(((a) < (b)) ? (a) : (b))')),
-                            ('MAX(a,b)', ('(((a) > (b)) ? (a) : (b))'))]}
-
     def _make_msg(self, f, hse, key):
         # Only retain the halos required by the Diag scheme
         halos = sorted(i for i in hse.halos if isinstance(i.dim, tuple))
         return MPIMsg('msg%d' % key, f, halos)
 
     def _make_sendrecv(self, f, hse, key, msg=None):
         comm = f.grid.distributor._obj_comm
@@ -540,15 +541,15 @@
 
         fromrank = Symbol(name='fromrank')
         torank = Symbol(name='torank')
 
         sizes = [FieldFromPointer('%s[%d]' % (msg._C_field_sizes, i), msg)
                  for i in range(len(f._dist_dimensions))]
 
-        gather = Call('gather%s' % key, [bufg] + sizes + [f] + ofsg)
+        gather = Gather('gather%s' % key, [bufg] + sizes + [f] + ofsg)
         # The `gather` is unnecessary if sending to MPI.PROC_NULL
         gather = Conditional(CondNe(torank, Macro('MPI_PROC_NULL')), gather)
 
         count = reduce(mul, sizes, 1)*dtype_len(f.dtype)
         rrecv = Byref(FieldFromPointer(msg._C_field_rrecv, msg))
         rsend = Byref(FieldFromPointer(msg._C_field_rsend, msg))
         recv = IrecvCall([bufs, count, Macro(dtype_to_mpitype(f.dtype)),
@@ -596,15 +597,15 @@
 
         ofss = [Symbol(name='os%s' % d.root) for d in f.dimensions]
 
         fromrank = Symbol(name='fromrank')
 
         sizes = [FieldFromPointer('%s[%d]' % (msg._C_field_sizes, i), msg)
                  for i in range(len(f._dist_dimensions))]
-        scatter = Call('scatter%s' % key, [bufs] + sizes + [f] + ofss)
+        scatter = Scatter('scatter%s' % key, [bufs] + sizes + [f] + ofss)
 
         # The `scatter` must be guarded as we must not alter the halo values along
         # the domain boundary, where the sender is actually MPI.PROC_NULL
         scatter = Conditional(CondNe(fromrank, Macro('MPI_PROC_NULL')), scatter)
 
         rrecv = Byref(FieldFromPointer(msg._C_field_rrecv, msg))
         waitrecv = Call('MPI_Wait', [rrecv, Macro('MPI_STATUS_IGNORE')])
@@ -642,15 +643,15 @@
     def _call_halowait(self, name, f, hse, msg):
         nb = f.grid.distributor._obj_neighborhood
         return HaloWaitCall(name, [f] + list(hse.loc_indices.values()) + [nb, msg])
 
     def _make_remainder(self, hs, key, callcompute, *args):
         assert callcompute.is_Call
         body = [callcompute._rebuild(dynamic_args_mapper=i) for _, i in hs.omapper.owned]
-        return make_efunc('remainder%d' % key, body)
+        return Remainder.make('remainder%d' % key, body)
 
     def _call_remainder(self, remainder):
         efunc = remainder.make_call()
         call = RemainderCall(efunc.name, efunc.arguments)
         return call
 
 
@@ -703,15 +704,15 @@
                  for i in range(len(f._dist_dimensions))]
         ofsg = [FieldFromComposite('%s[%d]' % (msg._C_field_ofsg, i), msgi)
                 for i in range(len(f._dist_dimensions))]
         ofsg = [fixed.get(d) or ofsg.pop(0) for d in f.dimensions]
 
         # The `gather` is unnecessary if sending to MPI.PROC_NULL
 
-        gather = Call('gather%s' % key, [cast(bufg)] + sizes + [f] + ofsg)
+        gather = Gather('gather%s' % key, [cast(bufg)] + sizes + [f] + ofsg)
         gather = Conditional(CondNe(torank, Macro('MPI_PROC_NULL')), gather)
 
         # Make Irecv/Isend
         count = reduce(mul, sizes, 1)*dtype_len(f.dtype)
         rrecv = Byref(FieldFromComposite(msg._C_field_rrecv, msgi))
         rsend = Byref(FieldFromComposite(msg._C_field_rsend, msgi))
         recv = IrecvCall([bufs, count, Macro(dtype_to_mpitype(f.dtype)),
@@ -747,15 +748,15 @@
                  for i in range(len(f._dist_dimensions))]
         ofss = [FieldFromComposite('%s[%d]' % (msg._C_field_ofss, i), msgi)
                 for i in range(len(f._dist_dimensions))]
         ofss = [fixed.get(d) or ofss.pop(0) for d in f.dimensions]
 
         # The `scatter` must be guarded as we must not alter the halo values along
         # the domain boundary, where the sender is actually MPI.PROC_NULL
-        scatter = Call('scatter%s' % key, [cast(bufs)] + sizes + [f] + ofss)
+        scatter = Scatter('scatter%s' % key, [cast(bufs)] + sizes + [f] + ofss)
         scatter = Conditional(CondNe(fromrank, Macro('MPI_PROC_NULL')), scatter)
 
         rrecv = Byref(FieldFromComposite(msg._C_field_rrecv, msgi))
         waitrecv = Call('MPI_Wait', [rrecv, Macro('MPI_STATUS_IGNORE')])
         rsend = Byref(FieldFromComposite(msg._C_field_rsend, msgi))
         waitsend = Call('MPI_Wait', [rsend, Macro('MPI_STATUS_IGNORE')])
 
@@ -789,15 +790,15 @@
             else:
                 dynamic_args_mapper[i] = (FieldFromComposite(i.name, region_i),)
 
         iet = callcompute._rebuild(dynamic_args_mapper=dynamic_args_mapper)
         # The -1 below is because an Iteration, by default, generates <=
         iet = Iteration(iet, dim, region.nregions - 1)
 
-        return make_efunc('remainder%d' % key, iet)
+        return Remainder.make('remainder%d' % key, iet)
 
 
 class Diag2HaloExchangeBuilder(Overlap2HaloExchangeBuilder):
 
     """
     A DiagHaloExchangeBuilder which uses preallocated buffers for comms
     as in Overlap2HaloExchange builder.
@@ -822,14 +823,44 @@
         # Just a dummy value, other than a Callable, so that we enter `_call_remainder`
         return hs.body
 
     def _call_remainder(self, remainder):
         return remainder
 
 
+class DualHaloExchangeBuilder(Overlap2HaloExchangeBuilder):
+
+    """
+    "Dual" of Overlap2HaloExchangeBuilder, as the "remainder" is now the first
+    thing getting computed.
+
+    Generates:
+
+        remainder()
+        haloupdate()
+        compute_core()
+        halowait()
+    """
+
+    def _make_body(self, callcompute, remainder, haloupdates, halowaits):
+        body = []
+
+        assert remainder is not None
+        body.append(self._call_remainder(remainder))
+
+        body.append(HaloUpdateList(body=haloupdates))
+
+        assert callcompute is not None
+        body.append(callcompute)
+
+        body.append(HaloWaitList(body=halowaits))
+
+        return List(body=body)
+
+
 class FullHaloExchangeBuilder(Overlap2HaloExchangeBuilder):
 
     """
     An Overlap2HaloExchangeBuilder which generates explicit Calls to MPI_Test
     poking the MPI runtime to advance communication while computing.
 
     Generates:
@@ -884,15 +915,16 @@
 mpi_registry = {
     True: BasicHaloExchangeBuilder,
     'basic': BasicHaloExchangeBuilder,
     'diag': DiagHaloExchangeBuilder,
     'diag2': Diag2HaloExchangeBuilder,
     'overlap': OverlapHaloExchangeBuilder,
     'overlap2': Overlap2HaloExchangeBuilder,
-    'full': FullHaloExchangeBuilder
+    'full': FullHaloExchangeBuilder,
+    'dual': DualHaloExchangeBuilder
 }
 
 
 # Callable sub-hierarchy
 
 
 class MPICallable(Callable):
@@ -915,16 +947,28 @@
 
 class HaloUpdate(MPICallable):
 
     def __init__(self, name, body, parameters):
         super(HaloUpdate, self).__init__(name, body, parameters)
 
 
+class Remainder(ElementalFunction):
+    pass
+
+
 # Call sub-hierarchy
 
+class Gather(Call):
+    pass
+
+
+class Scatter(Call):
+    pass
+
+
 class IsendCall(Call):
 
     def __init__(self, arguments, **kwargs):
         super().__init__('MPI_Isend', arguments)
 
 
 class IrecvCall(Call):
```

### Comparing `devito-4.8.0/devito/operations/interpolators.py` & `devito-4.8.1/devito/operations/interpolators.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,15 @@
                 rd = DefaultDimension(name="r%s" % d.name, default_value=self.r)
                 dim_subs.append((d, INT(rd + self.obj.gridpoints[p, i])))
                 coeffs.append(self.obj.interpolation_coeffs[p, i, rd])
             # Apply optional time symbol substitutions to lhs of assignment
             lhs = self.obj.subs(self_subs)
             rhs = prod(coeffs) * _expr.subs(dim_subs)
 
-            return [Eq(lhs, lhs + rhs)]
+            return [Inc(lhs, rhs)]
 
         return Interpolation(expr, offset, increment, self_subs, self, callback)
 
     def inject(self, field, expr, offset=0):
         """
         Generate equations injecting an arbitrary expression into a field.
 
@@ -396,10 +396,10 @@
             coeffs = []
             for i, d in enumerate(self.obj.grid.dimensions):
                 rd = DefaultDimension(name="r%s" % d.name, default_value=self.r)
                 dim_subs.append((d, INT(rd + self.obj.gridpoints[p, i])))
                 coeffs.append(self.obj.interpolation_coeffs[p, i, rd])
             rhs = prod(coeffs) * _expr
             _field = _field.subs(dim_subs)
-            return [Eq(_field, _field + rhs.subs(dim_subs))]
+            return [Inc(_field, rhs.subs(dim_subs))]
 
         return Injection(field, expr, offset, self, callback)
```

### Comparing `devito-4.8.0/devito/operations/solve.py` & `devito-4.8.1/devito/operations/solve.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/operator/operator.py` & `devito-4.8.1/devito/operator/operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 from devito.logger import debug, info, perf, warning, is_log_enabled_for
 from devito.ir.equations import LoweredEq, lower_exprs
 from devito.ir.clusters import ClusterGroup, clusterize
 from devito.ir.iet import (Callable, CInterface, EntryFunction, FindSymbols, MetaCall,
                            derive_parameters, iet_build)
 from devito.ir.support import AccessMode, SymbolRegistry
 from devito.ir.stree import stree_build
-from devito.operator.profiling import create_profile
+from devito.operator.profiling import AdvancedProfilerVerbose, create_profile
 from devito.operator.registry import operator_selector
 from devito.mpi import MPI
 from devito.parameters import configuration
-from devito.passes import Graph, lower_index_derivatives, generate_implicit, instrument
+from devito.passes import (Graph, lower_index_derivatives, generate_implicit,
+                           generate_macros)
 from devito.symbolics import estimate_cost
 from devito.tools import (DAG, OrderedSet, Signer, ReducerMap, as_tuple, flatten,
                           filter_sorted, frozendict, is_integer, split, timed_pass,
                           timed_region)
 from devito.types import Grid, Evaluable
 
 __all__ = ['Operator']
@@ -438,21 +439,24 @@
 
         # Wrap the IET with an EntryFunction (a special Callable representing
         # the entry point of the generated library)
         parameters = derive_parameters(uiet, True)
         iet = EntryFunction(name, uiet, 'int', parameters, ())
 
         # Lower IET to a target-specific IET
-        graph = Graph(iet)
+        graph = Graph(iet, sregistry=sregistry)
         graph = cls._specialize_iet(graph, **kwargs)
 
         # Instrument the IET for C-level profiling
         # Note: this is postponed until after _specialize_iet because during
         # specialization further Sections may be introduced
-        instrument(graph, profiler=profiler, sregistry=sregistry)
+        cls._Target.instrument(graph, profiler=profiler, **kwargs)
+
+        # Extract the necessary macros from the symbolic objects
+        generate_macros(graph)
 
         return graph.root, graph
 
     # Read-only properties exposed to the outside world
 
     @cached_property
     def reads(self):
@@ -507,15 +511,16 @@
                 if k not in self._known_arguments:
                     raise ValueError("Unrecognized argument %s=%s" % (k, v))
 
         # Pre-process Dimension overrides. This may help ruling out ambiguities
         # when processing the `defaults` arguments. A topological sorting is used
         # as DerivedDimensions may depend on their parents
         nodes = self.dimensions
-        edges = [(i, i.parent) for i in self.dimensions if i.is_Derived]
+        edges = [(i, i.parent) for i in self.dimensions
+                 if i.is_Derived and i.parent in set(nodes)]
         toposort = DAG(nodes, edges).topological_sort()
         futures = {}
         for d in reversed(toposort):
             if set(d._arg_names).intersection(kwargs):
                 futures.update(d._arg_values(self._dspace[d], args={}, **kwargs))
 
         overrides, defaults = split(self.input, lambda p: p.name in kwargs)
@@ -886,32 +891,46 @@
                 perf("Global performance: [%s]" % ', '.join(metrics))
 
             perf("Local performance:")
             indent = " "*2
         else:
             indent = ""
 
+            if isinstance(self._profiler, AdvancedProfilerVerbose):
+                metrics = []
+
+                v = summary.globals.get('fdlike-nosetup')
+                if v is not None:
+                    metrics.append("%.2f GPts/s" % fround(v.gpointss))
+
+                if metrics:
+                    perf("Global performance <w/o setup>: [%s]" % ', '.join(metrics))
+
         # Emit local, i.e. "per-rank" performance. Without MPI, this is the only
         # thing that will be emitted
         for k, v in summary.items():
             rank = "[rank%d]" % k.rank if k.rank is not None else ""
-            oi = "OI=%.2f" % fround(v.oi)
-            gflopss = "%.2f GFlops/s" % fround(v.gflopss)
-            gpointss = "%.2f GPts/s" % fround(v.gpointss) if v.gpointss else None
-            metrics = ", ".join(i for i in [oi, gflopss, gpointss] if i is not None)
+            if v.gflopss:
+                oi = "OI=%.2f" % fround(v.oi)
+                gflopss = "%.2f GFlops/s" % fround(v.gflopss)
+                gpointss = "%.2f GPts/s" % fround(v.gpointss)
+                metrics = "[%s]" % ", ".join([oi, gflopss, gpointss])
+            else:
+                metrics = ""
+
             itershapes = [",".join(str(i) for i in its) for its in v.itershapes]
             if len(itershapes) > 1:
                 itershapes = ",".join("<%s>" % i for i in itershapes)
             elif len(itershapes) == 1:
                 itershapes = itershapes[0]
             else:
                 itershapes = ""
             name = "%s%s<%s>" % (k.name, rank, itershapes)
 
-            perf("%s* %s ran in %.2f s [%s]" % (indent, name, fround(v.time), metrics))
+            perf("%s* %s ran in %.2f s %s" % (indent, name, fround(v.time), metrics))
             for n, time in summary.subsections.get(k.name, {}).items():
                 perf("%s+ %s ran in %.2f s [%.2f%%]" %
                      (indent*2, n, time, fround(time/v.time*100)))
 
         # Emit performance mode and arguments
         perf_args = {}
         for i in self.input + self.dimensions:
```

### Comparing `devito-4.8.0/devito/operator/profiling.py` & `devito-4.8.1/devito/operator/profiling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections import OrderedDict, namedtuple
+from collections import OrderedDict, defaultdict, namedtuple
 from contextlib import contextmanager
 from functools import reduce
 from operator import mul
 from pathlib import Path
 from subprocess import DEVNULL, PIPE, run
 from time import time as seq_time
 import os
@@ -32,15 +32,15 @@
 
 class Profiler(object):
 
     _default_includes = []
     _default_libs = []
     _ext_calls = []
 
-    """Metadata for a profiled code section."""
+    _supports_async_sections = False
 
     def __init__(self, name):
         self.name = name
 
         # Operation reductions observed in sections
         self._ops = []
 
@@ -205,14 +205,16 @@
     @property
     def trackable_subsections(self):
         return (MPICall, BusyWait)
 
 
 class AdvancedProfiler(Profiler):
 
+    _supports_async_sections = True
+
     # Override basic summary so that arguments other than runtime are computed.
     def summary(self, args, dtype, reduce_over=None):
         grid = args.grid
         comm = args.comm
 
         # Produce sections summary
         summary = PerformanceSummary()
@@ -286,15 +288,18 @@
         # Add global performance data
         if reduce_over is not None:
             # Vanilla metrics
             summary.add_glb_vanilla('vanilla', reduce_over)
 
             # Same as above but without setup overheads (e.g., host-device
             # data transfers)
-            reduce_over_nosetup = sum(i.time for i in summary.values())
+            mapper = defaultdict(list)
+            for (name, rank), v in summary.items():
+                mapper[name].append(v.time)
+            reduce_over_nosetup = sum(max(i) for i in mapper.values())
             if reduce_over_nosetup == 0:
                 reduce_over_nosetup = reduce_over
             summary.add_glb_vanilla('vanilla-nosetup', reduce_over_nosetup)
 
             # Typical finite difference benchmark metrics
             if grid is not None:
                 dimensions = (grid.time_dim,) + grid.dimensions
@@ -308,22 +313,26 @@
                     # Same as above but without setup overheads (e.g., host-device
                     # data transfers)
                     summary.add_glb_fdlike('fdlike-nosetup', points, reduce_over_nosetup)
 
         return summary
 
 
-class AdvancedProfilerVerbose1(AdvancedProfiler):
+class AdvancedProfilerVerbose(AdvancedProfiler):
+    pass
+
+
+class AdvancedProfilerVerbose1(AdvancedProfilerVerbose):
 
     @property
     def trackable_subsections(self):
         return (MPIList, RemainderCall, BusyWait)
 
 
-class AdvancedProfilerVerbose2(AdvancedProfiler):
+class AdvancedProfilerVerbose2(AdvancedProfilerVerbose):
 
     @property
     def trackable_subsections(self):
         return (MPICall, BusyWait)
 
 
 class AdvisorProfiler(AdvancedProfiler):
@@ -387,24 +396,24 @@
     def add(self, name, rank, time,
             ops=None, points=None, traffic=None, sops=None, itershapes=None):
         """
         Add performance data for a given code section. With MPI enabled, the
         performance data is local, that is "per-rank".
         """
         # Do not show unexecuted Sections (i.e., loop trip count was 0)
-        if ops == 0 or traffic == 0:
+        if traffic == 0:
             return
         # Do not show dynamic Sections (i.e., loop trip counts varies dynamically)
         if traffic is not None and np.isnan(traffic):
             assert np.isnan(points)
             return
 
         k = PerfKey(name, rank)
 
-        if ops is None:
+        if not ops:
             self[k] = PerfEntry(time, 0.0, 0.0, 0.0, 0, [])
         else:
             gflops = float(ops)/10**9
             gpoints = float(points)/10**9
             gflopss = gflops/time
             gpointss = gpoints/time
             oi = float(ops/traffic)
```

### Comparing `devito-4.8.0/devito/operator/registry.py` & `devito-4.8.1/devito/operator/registry.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/parameters.py` & `devito-4.8.1/devito/parameters.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/__init__.py` & `devito-4.8.1/devito/passes/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,16 +19,22 @@
         `gpu-fit` and is propagated down here through the various stages of lowering.
     """
     try:
         functions = (obj.function,)
     except AttributeError:
         functions = as_tuple(obj)
 
-    fsave = [f for f in functions
-             if isinstance(f, TimeFunction) and is_integer(f.save)]
+    fsave = []
+    for i in functions:
+        try:
+            f = i.alias or i
+        except AttributeError:
+            f = i
+        if isinstance(f, TimeFunction) and is_integer(f.save):
+            fsave.append(f)
 
     if 'all-fallback' in gpu_fit and fsave:
         warning("TimeFunction %s assumed to fit the GPU memory" % fsave)
         return True
 
     return all(f in gpu_fit for f in fsave)
```

### Comparing `devito-4.8.0/devito/passes/clusters/aliases.py` & `devito-4.8.1/devito/passes/clusters/aliases.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/clusters/asynchrony.py` & `devito-4.8.1/devito/passes/clusters/asynchrony.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import OrderedDict, defaultdict
 
 from sympy import And
 
 from devito.ir import (Forward, GuardBoundNext, Queue, Vector, WaitLock, WithLock,
                        FetchUpdate, PrefetchUpdate, ReleaseLock, normalize_syncs)
 from devito.symbolics import uxreplace
-from devito.tools import is_integer, timed_pass
+from devito.tools import OrderedSet, is_integer, timed_pass
 from devito.types import CustomDimension, Lock
 
 __all__ = ['Tasker', 'Streaming']
 
 
 class Asynchronous(Queue):
 
@@ -44,15 +44,15 @@
     def callback(self, clusters, prefix):
         if not prefix:
             return clusters
 
         d = prefix[-1].dim
 
         locks = {}
-        waits = defaultdict(list)
+        waits = defaultdict(OrderedSet)
         tasks = defaultdict(list)
         for c0 in clusters:
             dims = self.key(c0)
             if d not in dims:
                 # Not a candidate asynchronous task
                 continue
 
@@ -107,15 +107,15 @@
                             assert ld.symbolic_size == 1
                             index = 0
                             logical_index = 0
 
                         if logical_index in protected[target]:
                             continue
 
-                        waits[c1].append(WaitLock(lock[index], target))
+                        waits[c1].add(WaitLock(lock[index], target))
                         protected[target].add(logical_index)
 
             # Taskify `c0`
             for target in protected:
                 lock = locks[target]
 
                 indices = sorted({r[d] for r in c0.scope.reads[target]})
@@ -137,15 +137,15 @@
                 for i in indices:
                     tasks[c0].append(ReleaseLock(lock[i], target))
                     tasks[c0].append(WithLock(lock[i], target, i, function, findex, d))
 
         processed = []
         for c in clusters:
             if waits[c] or tasks[c]:
-                processed.append(c.rebuild(syncs={d: waits[c] + tasks[c]}))
+                processed.append(c.rebuild(syncs={d: list(waits[c]) + tasks[c]}))
             else:
                 processed.append(c)
 
         return processed
 
 
 class Streaming(Asynchronous):
```

### Comparing `devito-4.8.0/devito/passes/clusters/blocking.py` & `devito-4.8.1/devito/passes/clusters/blocking.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from sympy import sympify
 
 from devito.ir.clusters import Queue
 from devito.ir.support import (AFFINE, PARALLEL, PARALLEL_IF_ATOMIC, PARALLEL_IF_PVT,
-                               SEQUENTIAL, SKEWABLE, TILABLE, Interval, IntervalGroup,
-                               IterationSpace, Scope)
+                               SEQUENTIAL, SKEWABLE, TILABLES, Interval,
+                               IntervalGroup, IterationSpace, Scope)
 from devito.passes import is_on_device
 from devito.symbolics import uxreplace, xreplace_indices
-from devito.tools import UnboundedMultiTuple, as_tuple, flatten, is_integer
+from devito.tools import UnboundedMultiTuple, as_tuple, flatten, is_integer, prod
 from devito.types import BlockDimension
 
 __all__ = ['blocking']
 
 
 def blocking(clusters, sregistry, options):
     """
@@ -84,15 +84,15 @@
 
     def _process_fatd(self, clusters, level, prefix=None):
         # Truncate recursion in case of TILABLE, non-perfect sub-nests, as
         # it's an unsupported case
         if prefix:
             d = prefix[-1].dim
 
-            if any(TILABLE in c.properties[d] for c in clusters) and \
+            if any(c.properties.is_blockable(d) for c in clusters) and \
                len({c.ispace[:level] for c in clusters}) > 1:
                 return clusters
 
         return super()._process_fatd(clusters, level, prefix)
 
     def _has_data_reuse(self, cluster):
         # A sufficient condition for the existance of data reuse in `cluster`
@@ -140,34 +140,55 @@
                 return clusters
 
             # Pointless if there's no data reuse
             if not self._has_data_reuse(c):
                 return clusters
 
             # All good so far, `d` is actually TILABLE
-            processed.append(c.rebuild(properties=c.properties.add(d, TILABLE)))
+            processed.append(c.rebuild(properties=c.properties.block(d)))
 
         return processed
 
 
 class AnalyzeDeviceAwareBlocking(AnalyzeBlocking):
 
     def __init__(self, options):
         super().__init__(options)
 
         self.gpu_fit = options.get('gpu-fit', ())
 
     def _make_key_hook(self, cluster, level):
         return (is_on_device(cluster.functions, self.gpu_fit),)
 
-    def _has_data_reuse(self, cluster):
-        if is_on_device(cluster.functions, self.gpu_fit):
-            return True
-        else:
-            return super()._has_data_reuse(cluster)
+    def callback(self, clusters, prefix):
+        if not prefix:
+            return clusters
+
+        d = prefix[-1].dim
+        if self._has_short_trip_count(d):
+            return clusters
+
+        processed = []
+        for c in clusters:
+            if not c.properties.is_parallel_relaxed(d):
+                return clusters
+
+            if is_on_device(c.functions, self.gpu_fit):
+                if self._has_data_reuse(c):
+                    properties = c.properties.block(d)
+                else:
+                    properties = c.properties.block(d, 'small')
+            elif self._has_data_reuse(c):
+                properties = c.properties.block(d)
+            else:
+                return clusters
+
+            processed.append(c.rebuild(properties=properties))
+
+        return processed
 
 
 class AnalyzeHeuristicBlocking(AnayzeBlockingBase):
 
     def __init__(self, options):
         super().__init__(options)
 
@@ -175,56 +196,56 @@
 
     def process(self, clusters):
         clusters = super().process(clusters)
 
         # Heuristic: if there aren't at least two TILABLE Dimensions, drop it
         processed = []
         for c in clusters:
-            ntilable = len([TILABLE for v in c.properties.values() if TILABLE in v])
-            if ntilable > 1:
+            if c.properties.nblockable > 1:
                 processed.append(c)
             else:
-                properties = {d: v - {TILABLE} for d, v in c.properties.items()}
+                properties = c.properties.drop(properties=TILABLES)
                 processed.append(c.rebuild(properties=properties))
 
         return processed
 
     def callback(self, clusters, prefix):
         if not prefix:
             return clusters
 
         d = prefix[-1].dim
         if self._has_short_trip_count(d):
             return clusters
 
+        # Pointless if there's no data reuse
+        if all(not self._has_data_reuse(c) for c in clusters):
+            return clusters
+
+        # Heuristic: if all Clusters operate on local SubDimensions, then it means
+        # that all IterationSpaces are tiny, hence we can skip
+        if all(any(i.dim.is_Sub and i.dim.local for i in c.ispace) for c in clusters):
+            return clusters
+
         processed = []
         for c in clusters:
             # PARALLEL* and AFFINE are necessary conditions
             if AFFINE not in c.properties[d] or \
                not ({PARALLEL, PARALLEL_IF_PVT} & c.properties[d]):
                 return clusters
 
-            # Pointless if there's no data reuse
-            if not self._has_data_reuse(c):
-                return clusters
-
             # Heuristic: innermost Dimensions may be ruled out a-priori
             is_inner = d is c.ispace[-1].dim
             if is_inner and not self.inner:
                 return clusters
 
             # Heuristic: TILABLE not worth it if not within a SEQUENTIAL Dimension
             if not any(SEQUENTIAL in c.properties[i.dim] for i in prefix[:-1]):
                 return clusters
 
-            # Heuristic: same as above if there's a local SubDimension
-            if any(i.dim.is_Sub and i.dim.local for i in c.ispace):
-                return clusters
-
-            processed.append(c.rebuild(properties=c.properties.add(d, TILABLE)))
+            processed.append(c.rebuild(properties=c.properties.block(d)))
 
         if len(clusters) > 1:
             # Heuristic: same as above if it induces dynamic bounds
             exprs = flatten(c.exprs for c in as_tuple(clusters))
             scope = Scope(exprs)
             if any(i.is_lex_non_stmt for i in scope.d_all_gen()):
                 return clusters
@@ -245,15 +266,15 @@
         if not prefix:
             return clusters
 
         d = prefix[-1].dim
 
         processed = []
         for c in clusters:
-            if TILABLE not in c.properties[d]:
+            if not c.properties.is_blockable(d):
                 return clusters
 
             processed.append(c.rebuild(properties=c.properties.add(d, SKEWABLE)))
 
         return processed
 
 
@@ -270,37 +291,37 @@
         self.par_tile = options['par-tile']
 
         super().__init__()
 
     def process(self, clusters):
         # A tool to unroll the explicit integer block shapes, should there be any
         if self.par_tile:
-            blk_size_gen = BlockSizeGenerator(*self.par_tile)
+            blk_size_gen = BlockSizeGenerator(self.par_tile)
         else:
             blk_size_gen = None
 
         return self._process_fdta(clusters, 1, blk_size_gen=blk_size_gen)
 
     def callback(self, clusters, prefix, blk_size_gen=None):
         if not prefix:
             return clusters
 
         d = prefix[-1].dim
 
-        if not any(TILABLE in c.properties[d] for c in clusters):
+        if not any(c.properties.is_blockable(d) for c in clusters):
             return clusters
 
         # Create the block Dimensions (in total `self.levels` Dimensions)
         base = self.sregistry.make_name(prefix=d.name)
 
         if blk_size_gen is not None:
             # By passing a suitable key to `next` we ensure that we pull the
             # next par-tile entry iff we're now blocking an unseen TILABLE nest
             try:
-                step = sympify(blk_size_gen.next(clusters))
+                step = sympify(blk_size_gen.next(clusters, d))
             except StopIteration:
                 return clusters
         else:
             # This will result in a parametric step, e.g. `x0_blk0_size`
             step = None
 
         name = self.sregistry.make_name(prefix="%s_blk" % base)
@@ -314,24 +335,23 @@
             block_dims.append(bd)
 
         bd = BlockDimension(d.name, bd, bd, bd + bd.step - 1, 1, size=step)
         block_dims.append(bd)
 
         processed = []
         for c in clusters:
-            if TILABLE in c.properties[d]:
+            if c.properties.is_blockable(d):
                 ispace = decompose(c.ispace, d, block_dims)
 
                 # Use the innermost BlockDimension in place of `d`
                 exprs = [uxreplace(e, {d: bd}) for e in c.exprs]
 
                 # The new Cluster properties -- TILABLE is dropped after blocking
-                properties = dict(c.properties)
-                properties.pop(d)
-                properties.update({bd: c.properties[d] - {TILABLE} for bd in block_dims})
+                properties = c.properties.drop(d)
+                properties = properties.add(block_dims, c.properties[d] - TILABLES)
 
                 processed.append(c.rebuild(exprs=exprs, ispace=ispace,
                                            properties=properties))
             else:
                 processed.append(c)
 
         return processed
@@ -389,20 +409,44 @@
     directions = dict(ispace.directions)
     directions.pop(d)
     directions.update({bd: ispace.directions[d] for bd in block_dims})
 
     return IterationSpace(intervals, sub_iterators, directions)
 
 
-class BlockSizeGenerator(UnboundedMultiTuple):
+class BlockSizeGenerator(object):
+
+    """
+    A wrapper for several UnboundedMultiTuples.
+    """
+
+    def __init__(self, par_tile):
+        self.umt = UnboundedMultiTuple(*par_tile)
+
+        # This is for Clusters that need a small par-tile to avoid under-utilizing
+        # computational resources (e.g., kernels running over iteration spaces that
+        # are relatively small for the underlying architecture)
+        if (len(par_tile) == 1 and
+            (len(par_tile[0]) < len(par_tile.default) or
+             prod(par_tile[0]) < prod(par_tile.default))):
+            # Ignore if, e.g., user supplies a lower dimensional block shape
+            self.umt_small = self.umt
+        else:
+            self.umt_small = UnboundedMultiTuple(par_tile.default)
+
+    def next(self, clusters, d):
+        # TODO: This is for now exceptionally rudimentary
+        if all(c.properties.is_blockable_small(d) for c in clusters):
+            umt = self.umt_small
+        else:
+            umt = self.umt
 
-    def next(self, clusters):
         if not any(i.dim.is_Block for i in flatten(c.ispace for c in clusters)):
-            self.iter()
-        return super().next()
+            umt.iter()
+        return umt.next()
 
 
 class SynthesizeSkewing(Queue):
 
     """
     Construct a new sequence of clusters with skewed expressions and iteration spaces.
```

### Comparing `devito-4.8.0/devito/passes/clusters/buffering.py` & `devito-4.8.1/devito/passes/clusters/buffering.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/clusters/cse.py` & `devito-4.8.1/devito/passes/clusters/cse.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/clusters/derivatives.py` & `devito-4.8.1/devito/passes/clusters/derivatives.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/clusters/factorization.py` & `devito-4.8.1/devito/passes/clusters/factorization.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/clusters/implicit.py` & `devito-4.8.1/devito/passes/clusters/implicit.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/clusters/misc.py` & `devito-4.8.1/devito/passes/clusters/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 class Fusion(Queue):
 
     """
     Fuse Clusters with compatible IterationSpace.
     """
 
     _q_guards_in_key = True
+    _q_syncs_in_key = True
 
     def __init__(self, toposort, options=None):
         options = options or {}
 
         self.toposort = toposort
         self.fusetasks = options.get('fuse-tasks', False)
 
@@ -180,14 +181,17 @@
                     else:
                         mapper[k].add(s)
                 mapper[k] = frozenset(mapper[k])
             if any(mapper.values()):
                 mapper = frozendict(mapper)
                 key += (mapper,)
 
+        # Clusters representing HaloTouches should get merged, if possible
+        key += (c.is_halo_touch,)
+
         return key
 
     def _apply_heuristics(self, clusters):
         # We know at this point that `clusters` are potentially fusible since
         # they have same `_key`, but should we actually fuse them? In most cases
         # yes, but there are exceptions...
 
@@ -213,14 +217,24 @@
                     dump()
                     flag = False
             else:
                 flag = True
             group.append(c)
         dump()
 
+        # 2) Don't group HaloTouch's
+
+        groups, processed = processed, []
+        for group in groups:
+            for flag, minigroup in groupby(group, key=lambda c: c.is_halo_touch):
+                if flag:
+                    processed.extend([(c,) for c in minigroup])
+                else:
+                    processed.append(tuple(minigroup))
+
         return processed
 
     def _toposort(self, cgroups, prefix):
         # Are there any ClusterGroups that could potentially be fused? If
         # not, do not waste time computing a new topological ordering
         counter = Counter(self._key(cg) for cg in cgroups)
         if not any(v > 1 for it, v in counter.most_common()):
@@ -285,27 +299,18 @@
                     for cg2 in cgroups[n:cgroups.index(cg1)]:
                         dag.add_edge(cg2, cg1)
                     for cg2 in cgroups[cgroups.index(cg1)+1:]:
                         dag.add_edge(cg1, cg2)
                     break
 
                 # Any anti- and iaw-dependences impose that `cg1` follows `cg0`
-                # while not being its immediate successor (unless it already is),
-                # to avoid they are fused together (thus breaking the dependence)
-                # TODO: the "not being its immediate successor" part *seems* to be
-                # a work around to the fact that any two Clusters characterized
-                # by anti-dependence should have been given a different stamp,
-                # and same for guarded Clusters, but that is not the case (yet)
+                # and forbid any sort of fusion
                 elif any(scope.d_anti_gen()) or\
                         any(i.is_iaw for i in scope.d_output_gen()):
                     dag.add_edge(cg0, cg1)
-                    index = cgroups.index(cg1) - 1
-                    if index > n and self._key(cg0) == self._key(cg1):
-                        dag.add_edge(cg0, cgroups[index])
-                        dag.add_edge(cgroups[index], cg1)
 
                 # Any flow-dependences along an inner Dimension (i.e., a Dimension
                 # that doesn't appear in `prefix`) impose that `cg1` follows `cg0`
                 elif any(not (i.cause and i.cause & prefix) for i in scope.d_flow_gen()):
                     dag.add_edge(cg0, cg1)
 
                 # Clearly, output dependences must be honored
```

### Comparing `devito-4.8.0/devito/passes/clusters/utils.py` & `devito-4.8.1/devito/passes/clusters/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/equations/linearity.py` & `devito-4.8.1/devito/passes/equations/linearity.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/asynchrony.py` & `devito-4.8.1/devito/passes/iet/asynchrony.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/definitions.py` & `devito-4.8.1/devito/passes/iet/definitions.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/engine.py` & `devito-4.8.1/devito/passes/iet/engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from collections import Counter, OrderedDict
+from collections import OrderedDict
 from functools import partial, singledispatch, wraps
 
 from devito.ir.iet import (Call, FindNodes, FindSymbols, MetaCall, Transformer,
                            EntryFunction, ThreadCallable, Uxreplace,
                            derive_parameters)
+from devito.ir.support import SymbolRegistry
 from devito.tools import DAG, as_tuple, filter_ordered, timed_pass
-from devito.types import Array, CompositeObject, Lock, Indirection, Temp
+from devito.types import (Array, CompositeObject, Lock, IncrDimension, Indirection,
+                          Temp)
 from devito.types.args import ArgProvider
 from devito.types.dense import DiscreteFunction
+from devito.types.dimension import AbstractIncrDimension, BlockDimension
 
 __all__ = ['Graph', 'iet_pass', 'iet_visit']
 
 
 class Graph(object):
 
     """
@@ -23,17 +26,19 @@
     The `apply` method may be used to visit the Graph and apply a transformer `T`
     to all nodes. This may change the state of the Graph: node `a` gets replaced
     by `a' = T(a)`; new nodes (Callables), and therefore new edges, may be added.
 
     The `visit` method collects info about the nodes in the Graph.
     """
 
-    def __init__(self, iet):
+    def __init__(self, iet, sregistry=None):
         self.efuncs = OrderedDict([(iet.name, iet)])
 
+        self.sregistry = sregistry
+
         self.includes = []
         self.headers = []
         self.globals = []
 
     @property
     def root(self):
         return self.efuncs[list(self.efuncs).pop(0)]
@@ -65,15 +70,16 @@
             except KeyError:
                 pass
 
             if efunc is self.efuncs[i]:
                 continue
 
             # Minimize code size by abstracting semantically identical efuncs
-            efunc, efuncs = reuse_efuncs(efunc, metadata.get('efuncs', []))
+            efunc, efuncs = reuse_efuncs(efunc, metadata.get('efuncs', []),
+                                         self.sregistry)
 
             self.efuncs[i] = efunc
             self.efuncs.update(OrderedDict([(i.name, i) for i in efuncs]))
 
             # Update the parameters / arguments lists since `func` may have
             # introduced or removed objects
             self.efuncs = update_args(efunc, self.efuncs, dag)
@@ -151,15 +157,15 @@
 
     # Sanity check
     assert dag.size == len(efuncs)
 
     return dag
 
 
-def reuse_efuncs(root, efuncs):
+def reuse_efuncs(root, efuncs, sregistry=None):
     """
     Generalise `efuncs` so that syntactically identical Callables may be dropped,
     thus maximizing code reuse.
 
     For example, given two Callables
 
         foo0(u(x)) : u(x)**2
@@ -219,121 +225,147 @@
 
         * The `efunc` names becomes "foo".
         * Symbolic objects get replaced with "more abstract" objects:
             - DiscreteFunctions are renamed as "f0", "f1", ...
             - Arrays are renamed as "a0", "a1", ...
             - Objects are renamed as "o0", "o1", ...
     """
-    functions = FindSymbols().visit(efunc)
+    functions = FindSymbols('symbolics|dimensions').visit(efunc)
 
     mapper = abstract_objects(functions)
 
     efunc = Uxreplace(mapper).visit(efunc)
     efunc = efunc._rebuild(name='foo')
 
     return efunc
 
 
-def abstract_objects(objects):
+def abstract_objects(objects, sregistry=None):
     """
     Proxy for `abstract_object`.
     """
     # Precedence rules make it possible to reconstruct objects that depend on
     # higher priority objects
     priority = {
         DiscreteFunction: 1,
+        AbstractIncrDimension: 2,
+        BlockDimension: 3,
     }
 
     def key(i):
-        try:
-            return priority[i]
-        except (KeyError, TypeError):
-            # TypeError is for unhashable objects
-            return 0
+        for cls in sorted(priority, key=priority.get, reverse=True):
+            if isinstance(i, cls):
+                return priority[cls]
+        return 0
 
     objects = sorted(objects, key=key, reverse=True)
 
     # Build abstraction mappings
     mapper = {}
-    counter = Counter()
+    sregistry = sregistry or SymbolRegistry()
     for i in objects:
-        abstract_object(i, mapper, counter)
+        abstract_object(i, mapper, sregistry)
 
     return mapper
 
 
 @singledispatch
-def abstract_object(i, mapper, counter):
+def abstract_object(i, mapper, sregistry):
     """
     Singledispatch-based implementation of object abstraction.
 
     Singledispatch allows foreign modules to specify their own rules for
     object abstraction.
     """
     return
 
 
 @abstract_object.register(DiscreteFunction)
-def _(i, mapper, counter):
-    base = 'f'
-    name = '%s%d' % (base, counter[base])
+def _(i, mapper, sregistry):
+    name = sregistry.make_name(prefix='f')
 
-    v = i._rebuild(name=name, initializer=None, alias=True)
+    v = i._rebuild(name=name, initializer=None, alias=i)
 
     mapper.update({
         i: v,
         i.indexed: v.indexed,
         i.dmap: v.dmap,
         i._C_symbol: v._C_symbol,
     })
-    counter[base] += 1
 
 
 @abstract_object.register(Array)
-def _(i, mapper, counter):
+def _(i, mapper, sregistry):
     if isinstance(i, Lock):
-        base = 'lock'
+        name = sregistry.make_name(prefix='lock')
     else:
-        base = 'a'
-    name = '%s%d' % (base, counter[base])
+        name = sregistry.make_name(prefix='a')
 
     v = i._rebuild(name=name)
 
     mapper.update({
         i: v,
         i.indexed: v.indexed,
         i._C_symbol: v._C_symbol,
     })
-    counter[base] += 1
 
 
 @abstract_object.register(CompositeObject)
-def _(i, mapper, counter):
-    base = 'o'
-    name = '%s%d' % (base, counter[base])
+def _(i, mapper, sregistry):
+    name = sregistry.make_name(prefix='o')
 
     v = i._rebuild(name)
 
     mapper[i] = v
-    counter[base] += 1
+
+
+@abstract_object.register(BlockDimension)
+def _(i, mapper, sregistry):
+    if i._depth != 2:
+        return
+
+    p = i.parent
+    pp = i.parent.parent
+
+    name0 = pp.name
+    base = sregistry.make_name(prefix=name0)
+    name1 = sregistry.make_name(prefix='%s_blk' % base)
+
+    bd = i.parent._rebuild(name1, pp)
+    d = i._rebuild(name0, bd, i._min.subs(p, bd), i._max.subs(p, bd))
+
+    mapper.update({
+        i: d,
+        i.parent: bd
+    })
+
+
+@abstract_object.register(IncrDimension)
+def _(i, mapper, sregistry):
+    try:
+        p = mapper[i.parent]
+    except KeyError:
+        return
+
+    v = i._rebuild(i.name, p)
+
+    mapper[i] = v
 
 
 @abstract_object.register(Indirection)
 @abstract_object.register(Temp)
-def _(i, mapper, counter):
+def _(i, mapper, sregistry):
     if isinstance(i, Indirection):
-        base = 'ind'
+        name = sregistry.make_name(prefix='ind')
     else:
-        base = 'r'
-    name = '%s%d' % (base, counter[base])
+        name = sregistry.make_name(prefix='r')
 
     v = i._rebuild(name=name)
 
     mapper[i] = v
-    counter[base] += 1
 
 
 def update_args(root, efuncs, dag):
     """
     Re-derive the parameters of `root` and apply the changes in cascade through
     the `efuncs`.
 
@@ -365,15 +397,14 @@
     """
     if isinstance(root, ThreadCallable):
         return efuncs
 
     # The parameters/arguments lists may have changed since a pass may have:
     # 1) introduced a new symbol
     new_args = derive_parameters(root)
-    new_args = [a for a in new_args if not a._mem_internal_eager]
 
     # 2) defined a symbol for which no definition was available yet (e.g.
     # via a malloc, or a Dereference)
     defines = FindSymbols('defines').visit(root.body)
     drop_args = [a for a in root.parameters if a in defines]
 
     if not (new_args or drop_args):
```

### Comparing `devito-4.8.0/devito/passes/iet/langbase.py` & `devito-4.8.1/devito/passes/iet/langbase.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/languages/C.py` & `devito-4.8.1/devito/passes/iet/languages/C.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/languages/openacc.py` & `devito-4.8.1/devito/passes/iet/languages/openacc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/languages/openmp.py` & `devito-4.8.1/devito/passes/iet/languages/openmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     def __init__(self, prodder, arguments=None):
         # Atomic-ize any single-thread Prodders in the parallel tree
         condition = CondEq(DefFunction(Ompizer.lang['thread-num']().name), 0)
 
         # Prod within a while loop until all communications have completed
         # In other words, the thread delegated to prodding is entrapped for as long
         # as it's required
-        prod_until = Not(DefFunction(prodder.name, [i.name for i in prodder.arguments]))
+        prod_until = Not(DefFunction(prodder.name, prodder.arguments))
         then_body = List(header=c.Comment('Entrap thread until comms have completed'),
                          body=While(prod_until))
         Conditional.__init__(self, condition, then_body)
 
         arguments = arguments or prodder.arguments
         Prodder.__init__(self, prodder.name, arguments, periodic=prodder.periodic)
```

### Comparing `devito-4.8.0/devito/passes/iet/languages/targets.py` & `devito-4.8.1/devito/passes/iet/languages/targets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from devito.passes.iet.languages.C import CDataManager, COrchestrator
 from devito.passes.iet.languages.openmp import (SimdOmpizer, Ompizer, DeviceOmpizer,
                                                 OmpDataManager, DeviceOmpDataManager,
                                                 OmpOrchestrator, DeviceOmpOrchestrator)
 from devito.passes.iet.languages.openacc import (DeviceAccizer, DeviceAccDataManager,
                                                  AccOrchestrator)
+from devito.passes.iet.instrument import instrument
 
 __all__ = ['CTarget', 'OmpTarget', 'DeviceOmpTarget', 'DeviceAccTarget']
 
 
 class Target(object):
     Parizer = None
     DataManager = None
     Orchestrator = None
 
+    @classmethod
+    def lang(cls):
+        return cls.Parizer.lang
+
+    @classmethod
+    def instrument(cls, *args, **kwargs):
+        instrument(*args, lang=cls.lang(), **kwargs)
+
 
 class CTarget(Target):
     Parizer = SimdOmpizer
     DataManager = CDataManager
     Orchestrator = COrchestrator
```

### Comparing `devito-4.8.0/devito/passes/iet/languages/utils.py` & `devito-4.8.1/devito/passes/iet/languages/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/linearization.py` & `devito-4.8.1/devito/passes/iet/linearization.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/misc.py` & `devito-4.8.1/devito/passes/iet/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from functools import singledispatch
+
 import cgen
+import sympy
 
-from devito.ir import (Any, Forward, List, Prodder, FindNodes, Transformer,
-                       filter_iterations, retrieve_iteration_tree)
+from devito.finite_differences import Max, Min
+from devito.ir import (Any, Forward, List, Prodder, FindApplications, FindNodes,
+                       Transformer, filter_iterations, retrieve_iteration_tree)
 from devito.passes.iet.engine import iet_pass
-from devito.symbolics import evalrel
+from devito.symbolics import evalrel, has_integer_args
 from devito.tools import split
 
-__all__ = ['avoid_denormals', 'hoist_prodders', 'relax_incr_dimensions']
+__all__ = ['avoid_denormals', 'hoist_prodders', 'relax_incr_dimensions',
+           'generate_macros']
 
 
 @iet_pass
 def avoid_denormals(iet, platform=None):
     """
     Introduce nodes in the Iteration/Expression tree that will expand to C
     macros telling the CPU to flush denormal numbers in hardware. Denormals
@@ -120,13 +125,39 @@
             root_max = roots_max[i.dim.root] + i.symbolic_max - i.dim.symbolic_max
             iter_max = evalrel(min, [i.symbolic_max, root_max])
             mapper[i] = i._rebuild(limits=(i.symbolic_min, iter_max, i.step))
 
     if mapper:
         iet = Transformer(mapper, nested=True).visit(iet)
 
-        headers = [('MIN(a,b)', ('(((a) < (b)) ? (a) : (b))')),
-                   ('MAX(a,b)', ('(((a) > (b)) ? (a) : (b))'))]
-    else:
-        headers = []
+    return iet, {}
+
+
+@iet_pass
+def generate_macros(iet):
+    applications = FindApplications().visit(iet)
+    headers = set().union(*[_generate_macros(i) for i in applications])
 
     return iet, {'headers': headers}
+
+
+@singledispatch
+def _generate_macros(expr):
+    return set()
+
+
+@_generate_macros.register(Min)
+@_generate_macros.register(sympy.Min)
+def _(expr):
+    if has_integer_args(*expr.args) and len(expr.args) == 2:
+        return {('MIN(a,b)', ('(((a) < (b)) ? (a) : (b))'))}
+    else:
+        return set()
+
+
+@_generate_macros.register(Max)
+@_generate_macros.register(sympy.Max)
+def _(expr):
+    if has_integer_args(*expr.args) and len(expr.args) == 2:
+        return {('MAX(a,b)', ('(((a) > (b)) ? (a) : (b))'))}
+    else:
+        return set()
```

### Comparing `devito-4.8.0/devito/passes/iet/mpi.py` & `devito-4.8.1/devito/passes/iet/mpi.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from devito.ir.iet import (Call, Expression, HaloSpot, Iteration, FindNodes,
                            MapNodes, Transformer, retrieve_iteration_tree)
 from devito.ir.support import PARALLEL, Scope
 from devito.mpi.halo_scheme import HaloScheme
 from devito.mpi.routines import HaloExchangeBuilder
 from devito.passes.iet.engine import iet_pass
-from devito.tools import as_mapper, generator
+from devito.tools import generator
 
 __all__ = ['mpiize']
 
 
 @iet_pass
 def optimize_halospots(iet):
     """
@@ -28,28 +28,19 @@
     return iet, {}
 
 
 def _drop_halospots(iet):
     """
     Remove HaloSpots that:
 
-        * Embed SEQUENTIAL Iterations
         * Would be used to compute Increments (in which case, a halo exchange
           is actually unnecessary)
     """
     mapper = defaultdict(set)
 
-    # If a HaloSpot Dimension turns out to be SEQUENTIAL, then the HaloSpot is useless
-    for hs, iterations in MapNodes(HaloSpot, Iteration).visit(iet).items():
-        dmapper = as_mapper(iterations, lambda i: i.dim.root)
-        for d, v in dmapper.items():
-            if d in hs.dimensions and all(i.is_Sequential for i in v):
-                mapper[hs].update(set(hs.functions))
-                break
-
     # If all HaloSpot reads pertain to reductions, then the HaloSpot is useless
     for hs, expressions in MapNodes(HaloSpot, Expression).visit(iet).items():
         for f in hs.fmapper:
             scope = Scope([i.expr for i in expressions])
             if all(i.is_reduction for i in scope.reads.get(f, [])):
                 mapper[hs].add(f)
 
@@ -246,33 +237,32 @@
         test = True
 
         # Comp/comm overlaps is legal only if the OWNED regions can grow
         # arbitrarly, which means all of the dependences must be carried
         # along a non-halo Dimension
         for dep in scope.d_all_gen():
             if dep.function in hs.functions:
-                if not dep.cause:
-                    # E.g. increments
-                    # for x
-                    #   for y
-                    #     f[x, y] = f[x, y] + 1
-                    test = False
-                    break
-                elif dep.cause & hs.dimensions:
-                    # E.g. dependences across PARALLEL iterations
+                cause = dep.cause & hs.dimensions
+                if any(dep.distance_mapper[d] is S.Infinity for d in cause):
+                    # E.g., dependences across PARALLEL iterations
                     # for x
                     #   for y
                     #     ... = ... f[x, y-1] ...
                     #   for y
                     #     f[x, y] = ...
                     test = False
                     break
 
         # Heuristic: avoid comp/comm overlap for sparse Iteration nests
-        test = test and all(i.is_Affine for i in FindNodes(Iteration).visit(hs))
+        if test:
+            for i in FindNodes(Iteration).visit(hs):
+                if i.dim._defines & set(hs.halo_scheme.distributed_aindices) and \
+                   not i.is_Affine:
+                    test = False
+                    break
 
         if test:
             found.append(hs)
 
     # Transform the IET replacing HaloSpots with OverlappableHaloSpots
     mapper = {hs: OverlappableHaloSpot(**hs.args) for hs in found}
     iet = Transformer(mapper, nested=True).visit(iet)
@@ -294,32 +284,30 @@
     mapper = {}
     for hs in FindNodes(HaloSpot).visit(iet):
         heb = user_heb if isinstance(hs, OverlappableHaloSpot) else sync_heb
         mapper[hs] = heb.make(hs)
 
     efuncs = sync_heb.efuncs + user_heb.efuncs
     iet = Transformer(mapper, nested=True).visit(iet)
-    headers = user_heb.headers
 
     # Must drop the PARALLEL tag from the Iterations within which halo
     # exchanges are performed
     mapper = {}
     for tree in retrieve_iteration_tree(iet):
         for i in reversed(tree):
             if i in mapper:
                 # Already seen this subtree, skip
                 break
             if FindNodes(Call).visit(i):
                 mapper.update({n: n._rebuild(properties=set(n.properties)-{PARALLEL})
                                for n in tree[:tree.index(i)+1]})
                 break
     iet = Transformer(mapper, nested=True).visit(iet)
-    headers.update({'includes': ['mpi.h'], 'efuncs': efuncs})
 
-    return iet, headers
+    return iet, {'includes': ['mpi.h'], 'efuncs': efuncs}
 
 
 def mpiize(graph, **kwargs):
     """
     Perform two IET passes:
 
         * Optimization of communications
```

### Comparing `devito-4.8.0/devito/passes/iet/orchestration.py` & `devito-4.8.1/devito/passes/iet/orchestration.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/passes/iet/parpragma.py` & `devito-4.8.1/devito/passes/iet/parpragma.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/symbolics/extended_sympy.py` & `devito-4.8.1/devito/symbolics/extended_sympy.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,19 +538,14 @@
     def name(self):
         return self._name
 
     @property
     def arguments(self):
         return self._arguments
 
-    @property
-    def free_symbols(self):
-        return set().union(*[i.free_symbols for i in self.arguments
-                             if isinstance(i, Expr)])
-
     def __str__(self):
         return "%s(%s)" % (self.name, ', '.join(str(i) for i in self.arguments))
 
     __repr__ = __str__
 
     def _sympystr(self, printer):
         return str(self)
```

### Comparing `devito-4.8.0/devito/symbolics/inspection.py` & `devito-4.8.1/devito/symbolics/inspection.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from devito.finite_differences.differentiable import IndexDerivative
 from devito.logger import warning
 from devito.symbolics.extended_sympy import (INT, CallFromPointer, Cast,
                                              DefFunction, ReservedWord)
 from devito.symbolics.queries import q_routine
 from devito.tools import as_tuple, prod
 
-__all__ = ['compare_ops', 'estimate_cost']
+__all__ = ['compare_ops', 'estimate_cost', 'has_integer_args']
 
 
 def compare_ops(e1, e2):
     """
     True if the two input expressions perform the same arithmetic operations
     over the same input "operands", False otherwise.
 
@@ -231,7 +231,32 @@
     flops += 1
 
     # To be multiplied by the number of points this index sum implicitly
     # iterates over
     flops *= prod(i._size for i in expr.dimensions)
 
     return flops, False
+
+
+def has_integer_args(*args):
+    """
+    True if all `args` are of integer type, False otherwise.
+    """
+    if len(args) == 0:
+        return False
+
+    if len(args) == 1:
+        try:
+            return np.issubdtype(args[0].dtype, np.integer)
+        except AttributeError:
+            return args[0].is_integer
+
+    res = True
+    for a in args:
+        try:
+            if len(a.args) > 0:
+                res = res and has_integer_args(*a.args)
+            else:
+                res = res and has_integer_args(a)
+        except AttributeError:
+            res = res and has_integer_args(a)
+    return res
```

### Comparing `devito-4.8.0/devito/symbolics/manipulation.py` & `devito-4.8.1/devito/symbolics/manipulation.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/symbolics/printer.py` & `devito-4.8.1/devito/symbolics/printer.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from mpmath.libmp import prec_to_dps, to_str
 from packaging.version import Version
 from sympy.logic.boolalg import BooleanFunction
 from sympy.printing.precedence import PRECEDENCE_VALUES, precedence
 from sympy.printing.c import C99CodePrinter
 
 from devito.arch.compiler import AOMPCompiler
+from devito.symbolics.inspection import has_integer_args
 
 __all__ = ['ccode']
 
 
 class CodePrinter(C99CodePrinter):
 
     """
@@ -98,22 +99,24 @@
 
     def _print_Mod(self, expr):
         """Print a Mod as a C-like %-based operation."""
         args = ['(%s)' % self._print(a) for a in expr.args]
         return '%'.join(args)
 
     def _print_Min(self, expr):
-        """Print Min using devito defined header Min"""
-        func = 'MIN' if has_integer_args(*expr.args) else 'fmin'
-        return "%s(%s)" % (func, self._print(expr.args)[1:-1])
+        if has_integer_args(*expr.args) and len(expr.args) == 2:
+            return "MIN(%s)" % self._print(expr.args)[1:-1]
+        else:
+            return super()._print_Min(expr)
 
     def _print_Max(self, expr):
-        """Print Max using devito defined header Max"""
-        func = 'MAX' if has_integer_args(*expr.args) else 'fmax'
-        return "%s(%s)" % (func, self._print(expr.args)[1:-1])
+        if has_integer_args(*expr.args) and len(expr.args) == 2:
+            return "MAX(%s)" % self._print(expr.args)[1:-1]
+        else:
+            return super()._print_Max(expr)
 
     def _print_Abs(self, expr):
         """Print an absolute value. Use `abs` if can infer it is an Integer"""
         # AOMPCC errors with abs, always use fabs
         if isinstance(self.compiler, AOMPCompiler):
             return "fabs(%s)" % self._print(expr.args[0])
         # Check if argument is an integer
@@ -254,34 +257,7 @@
     return CodePrinter(settings=settings).doprint(expr, None)
 
 
 # Sympy 1.11 has introduced a bug in `_print_Add`, so we enforce here
 # to always use the correct one from our printer
 if Version(sympy.__version__) >= Version("1.11"):
     setattr(sympy.printing.str.StrPrinter, '_print_Add', CodePrinter._print_Add)
-
-
-# Check arguements type
-def has_integer_args(*args):
-    """
-    Check if expression is Integer.
-    Used to choose the function printed in the c-code
-    """
-    if len(args) == 0:
-        return False
-
-    if len(args) == 1:
-        try:
-            return np.issubdtype(args[0].dtype, np.integer)
-        except AttributeError:
-            return args[0].is_integer
-
-    res = True
-    for a in args:
-        try:
-            if len(a.args) > 0:
-                res = res and has_integer_args(*a.args)
-            else:
-                res = res and has_integer_args(a)
-        except AttributeError:
-            res = res and has_integer_args(a)
-    return res
```

### Comparing `devito-4.8.0/devito/symbolics/queries.py` & `devito-4.8.1/devito/symbolics/queries.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/symbolics/search.py` & `devito-4.8.1/devito/symbolics/search.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/abc.py` & `devito-4.8.1/devito/tools/abc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/algorithms.py` & `devito-4.8.1/devito/tools/algorithms.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/data_structures.py` & `devito-4.8.1/devito/tools/data_structures.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/dtypes_lowering.py` & `devito-4.8.1/devito/tools/dtypes_lowering.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/memoization.py` & `devito-4.8.1/devito/tools/memoization.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/os_helper.py` & `devito-4.8.1/devito/tools/os_helper.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/threading.py` & `devito-4.8.1/devito/tools/threading.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/timing.py` & `devito-4.8.1/devito/tools/timing.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/utils.py` & `devito-4.8.1/devito/tools/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/tools/visitors.py` & `devito-4.8.1/devito/tools/visitors.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/__init__.py` & `devito-4.8.1/devito/types/__init__.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/args.py` & `devito-4.8.1/devito/types/args.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/array.py` & `devito-4.8.1/devito/types/array.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/basic.py` & `devito-4.8.1/devito/types/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -572,16 +572,16 @@
                          AbstractTensor
                                 |
                           TensorFunction
                                 |
                  ---------------------------------
                  |                               |
           VectorFunction                 TensorTimeFunction
-                        \-------\                |
-                                 \------- VectorTimeFunction
+                        \\-------\\              |
+                                 \\------- VectorTimeFunction
 
     There are four relevant AbstractTensor sub-types: ::
 
         * TensorFunction: A space-varying tensor valued function.
         * VectorFunction: A space-varying vector valued function.
         * TensorTimeFunction: A time-space-varying tensor valued function.
         * VectorTimeFunction: A time-space-varying vector valued function.
@@ -673,14 +673,24 @@
         pass
 
     __hash__ = sympy.ImmutableDenseMatrix.__hash__
 
     def doit(self, **hint):
         return self
 
+    def transpose(self, inner=True):
+        new = super().transpose()
+        if inner:
+            return new.applyfunc(lambda x: getattr(x, 'T', x))
+        return new
+
+    def adjoint(self, inner=True):
+        # Real valued adjoint is transpose
+        return self.transpose(inner=inner)
+
     def _eval_matrix_mul(self, other):
         """
         Copy paste from sympy to avoid explicit call to sympy.Add
         TODO: fix inside sympy
         """
         other_len = other.rows*other.cols
         new_len = self.rows*other.cols
```

### Comparing `devito-4.8.0/devito/types/caching.py` & `devito-4.8.1/devito/types/caching.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/constant.py` & `devito-4.8.1/devito/types/constant.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/dense.py` & `devito-4.8.1/devito/types/dense.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/dimension.py` & `devito-4.8.1/devito/types/dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1509,15 +1509,15 @@
 
         * the "main" Dimension (in practice a SpaceDimension or a TimeDimension);
         * an offset (number or symbolic expression, of dtype integer).
         * a StencilDimension;
 
     Examples
     --------
-    The AffineIndexAccessFunction `x + sd + 3`, with `sd \in [-2, 2]`, represents
+    The AffineIndexAccessFunction `x + sd + 3`, with `sd in [-2, 2]`, represents
     the index access functions `[x + 1, x + 2, x + 3, x + 4, x + 5]`
     """
 
     def __new__(cls, *args, **kwargs):
         d = 0
         sd = 0
         ofs_items = []
```

### Comparing `devito-4.8.0/devito/types/equation.py` & `devito-4.8.1/devito/types/equation.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/grid.py` & `devito-4.8.1/devito/types/grid.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/lazy.py` & `devito-4.8.1/devito/types/lazy.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/misc.py` & `devito-4.8.1/devito/types/misc.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/object.py` & `devito-4.8.1/devito/types/object.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/parallel.py` & `devito-4.8.1/devito/types/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,11 +278,11 @@
         kwargs.setdefault('is_const', True)
         return super().__new__(cls, *args, **kwargs)
 
 
 class Barrier(object):
 
     """
-    Mixin class for symbolic objects representing thread barriers.
+    Mixin class for symbolic objects representing synchronization barriers.
     """
 
     pass
```

### Comparing `devito-4.8.0/devito/types/relational.py` & `devito-4.8.1/devito/types/relational.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/sparse.py` & `devito-4.8.1/devito/types/sparse.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/tensor.py` & `devito-4.8.1/devito/types/tensor.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito/types/utils.py` & `devito-4.8.1/devito/types/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/devito.egg-info/PKG-INFO` & `devito-4.8.1/devito.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devito
-Version: 4.8.0
+Version: 4.8.1
 Summary: Finite Difference DSL for symbolic computation.
 Home-page: http://www.devitoproject.org
 Author: Imperial College London
 Author-email: g.gorman@imperial.ac.uk
 License: MIT
 Project-URL: Documentation, https://www.devitoproject.org/devito/index.html
 Project-URL: Source Code, https://github.com/devitocodes/devito
```

### Comparing `devito-4.8.0/devito.egg-info/SOURCES.txt` & `devito-4.8.1/devito.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/cfd/example_diffusion.py` & `devito-4.8.1/examples/cfd/example_diffusion.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/cfd/tools.py` & `devito-4.8.1/examples/cfd/tools.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/misc/linalg.py` & `devito-4.8.1/examples/misc/linalg.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/performance/utils.py` & `devito-4.8.1/examples/performance/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/acoustic/acoustic_example.py` & `devito-4.8.1/examples/seismic/acoustic/acoustic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/acoustic/operators.py` & `devito-4.8.1/examples/seismic/acoustic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/acoustic/wavesolver.py` & `devito-4.8.1/examples/seismic/acoustic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/elastic/elastic_example.py` & `devito-4.8.1/examples/seismic/elastic/elastic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/elastic/operators.py` & `devito-4.8.1/examples/seismic/elastic/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                              space_order=space_order, time_order=1)
 
     lam, mu, b = model.lam, model.mu, model.b
 
     # Particle velocity
     eq_v = v.dt - b * div(tau)
     # Stress
-    e = (grad(v.forward) + grad(v.forward).T)
+    e = (grad(v.forward) + grad(v.forward).transpose(inner=False))
     eq_tau = tau.dt - lam * diag(div(v.forward)) - mu * e
 
     u_v = Eq(v.forward, model.damp * solve(eq_v, v.forward))
     u_t = Eq(tau.forward, model.damp * solve(eq_tau, tau.forward))
 
     srcrec = src_rec(v, tau, model, geometry)
     op = Operator([u_v] + [u_t] + srcrec, subs=model.spacing_map, name="ForwardElastic",
```

### Comparing `devito-4.8.0/examples/seismic/elastic/wavesolver.py` & `devito-4.8.1/examples/seismic/elastic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/model.py` & `devito-4.8.1/examples/seismic/model.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/plotting.py` & `devito-4.8.1/examples/seismic/plotting.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/preset_models.py` & `devito-4.8.1/examples/seismic/preset_models.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/self_adjoint/example_iso.py` & `devito-4.8.1/examples/seismic/self_adjoint/example_iso.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/self_adjoint/operators.py` & `devito-4.8.1/examples/seismic/self_adjoint/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/self_adjoint/test_utils.py` & `devito-4.8.1/examples/seismic/self_adjoint/test_utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/self_adjoint/test_wavesolver_iso.py` & `devito-4.8.1/examples/seismic/self_adjoint/test_wavesolver_iso.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/self_adjoint/utils.py` & `devito-4.8.1/examples/seismic/self_adjoint/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/self_adjoint/wavesolver.py` & `devito-4.8.1/examples/seismic/self_adjoint/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/source.py` & `devito-4.8.1/examples/seismic/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         Discretized values of time in ms.
     a : float, optional
         Amplitude of the wavelet (defaults to 1).
     t0 : float, optional
         Firing time (defaults to 1 / f0)
     """
 
-    __rkwargs__ = PointSource.__rkwargs__ + ['f0', 'a', 'f0']
+    __rkwargs__ = PointSource.__rkwargs__ + ['f0', 'a', 't0']
 
     @classmethod
     def __args_setup__(cls, *args, **kwargs):
         kwargs.setdefault('npoint', 1)
 
         return super(WaveletSource, cls).__args_setup__(*args, **kwargs)
```

### Comparing `devito-4.8.0/examples/seismic/test_seismic_utils.py` & `devito-4.8.1/examples/seismic/test_seismic_utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/tti/operators.py` & `devito-4.8.1/examples/seismic/tti/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/tti/tti_example.py` & `devito-4.8.1/examples/seismic/tti/tti_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/tti/wavesolver.py` & `devito-4.8.1/examples/seismic/tti/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/utils.py` & `devito-4.8.1/examples/seismic/utils.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/viscoacoustic/operators.py` & `devito-4.8.1/examples/seismic/viscoacoustic/operators.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/viscoacoustic/viscoacoustic_example.py` & `devito-4.8.1/examples/seismic/viscoacoustic/viscoacoustic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/viscoacoustic/wavesolver.py` & `devito-4.8.1/examples/seismic/viscoacoustic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/viscoelastic/operators.py` & `devito-4.8.1/examples/seismic/viscoelastic/operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                            save=geometry.nt if save else None,
                            space_order=space_order, time_order=1)
 
     # Particle velocity
     pde_v = v.dt - b * div(tau)
     u_v = Eq(v.forward, model.damp * solve(pde_v, v.forward))
     # Strain
-    e = grad(v.forward) + grad(v.forward).T
+    e = grad(v.forward) + grad(v.forward).transpose(inner=False)
 
     # Stress equations
     pde_tau = tau.dt - r.forward - l * t_ep / t_s * diag(div(v.forward)) - \
         mu * t_es / t_s * e
     u_t = Eq(tau.forward, model.damp * solve(pde_tau, tau.forward))
 
     # Memory variable equations:
```

### Comparing `devito-4.8.0/examples/seismic/viscoelastic/viscoelastic_example.py` & `devito-4.8.1/examples/seismic/viscoelastic/viscoelastic_example.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/examples/seismic/viscoelastic/wavesolver.py` & `devito-4.8.1/examples/seismic/viscoelastic/wavesolver.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/setup.cfg` & `devito-4.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/setup.py` & `devito-4.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `devito-4.8.0/versioneer.py` & `devito-4.8.1/versioneer.py`

 * *Files identical despite different names*

