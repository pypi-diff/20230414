# Comparing `tmp/pymc-5.2.0.tar.gz` & `tmp/pymc-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.2.0.tar", last modified: Thu Mar 30 10:39:24 2023, max compression
+gzip compressed data, was "dist/pymc-5.3.0.tar", last modified: Fri Apr 14 03:09:00 2023, max compression
```

## Comparing `pymc-5.2.0.tar` & `pymc-5.3.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-03-30 10:39:14.000000 pymc-5.2.0/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-30 10:39:14.000000 pymc-5.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-30 10:39:14.000000 pymc-5.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-03-30 10:39:14.000000 pymc-5.2.0/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-03-30 10:39:14.000000 pymc-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-30 10:39:14.000000 pymc-5.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-03-30 10:39:24.000000 pymc-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-03-30 10:39:14.000000 pymc-5.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-03-30 10:39:14.000000 pymc-5.2.0/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   114525 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    51737 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    89390 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39771 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32077 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    47914 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    34734 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    83735 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    48752 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    35693 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-30 10:39:14.000000 pymc-5.2.0/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 10:39:24.000000 pymc-5.2.0/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-30 10:39:14.000000 pymc-5.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-30 10:39:14.000000 pymc-5.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 10:39:24.000000 pymc-5.2.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-03-30 10:39:14.000000 pymc-5.2.0/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-03-30 10:39:14.000000 pymc-5.2.0/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-30 10:39:24.000000 pymc-5.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-03-30 10:39:14.000000 pymc-5.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-03-30 10:39:14.000000 pymc-5.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-14 03:08:48.000000 pymc-5.3.0/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-14 03:08:48.000000 pymc-5.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-14 03:08:48.000000 pymc-5.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-04-14 03:08:48.000000 pymc-5.3.0/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-14 03:08:48.000000 pymc-5.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 03:08:48.000000 pymc-5.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-14 03:09:00.000000 pymc-5.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-14 03:08:48.000000 pymc-5.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-14 03:08:48.000000 pymc-5.3.0/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21384 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115522 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51737 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20940 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89379 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32077 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49754 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14276 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34745 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90137 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37227 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48752 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15009 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14866 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35693 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-14 03:08:48.000000 pymc-5.3.0/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-14 03:08:59.000000 pymc-5.3.0/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-14 03:08:48.000000 pymc-5.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 03:08:48.000000 pymc-5.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:09:00.000000 pymc-5.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-04-14 03:08:48.000000 pymc-5.3.0/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-04-14 03:08:48.000000 pymc-5.3.0/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-14 03:09:00.000000 pymc-5.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-04-14 03:08:48.000000 pymc-5.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-04-14 03:08:48.000000 pymc-5.3.0/versioneer.py
```

### Comparing `pymc-5.2.0/ARCHITECTURE.md` & `pymc-5.3.0/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/CODE_OF_CONDUCT.md` & `pymc-5.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/CONTRIBUTING.md` & `pymc-5.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/GOVERNANCE.md` & `pymc-5.3.0/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/LICENSE` & `pymc-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/PKG-INFO` & `pymc-5.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.2.0
+Version: 5.3.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
@@ -165,21 +165,21 @@
            :target: https://mybinder.org/v2/gh/pymc-devs/pymc/main?filepath=%2Fdocs%2Fsource%2Fnotebooks
         .. |Build Status| image:: https://github.com/pymc-devs/pymc/workflows/pytest/badge.svg
            :target: https://github.com/pymc-devs/pymc/actions
         .. |Coverage| image:: https://codecov.io/gh/pymc-devs/pymc/branch/main/graph/badge.svg
            :target: https://codecov.io/gh/pymc-devs/pymc
         .. |Dockerhub| image:: https://img.shields.io/docker/automated/pymc/pymc.svg
            :target: https://hub.docker.com/r/pymc/pymc
-        .. |NumFOCUS| image:: https://www.numfocus.org/wp-content/uploads/2017/03/1457562110.png
-           :target: http://www.numfocus.org/
         .. |NumFOCUS_badge| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
            :target: http://www.numfocus.org/
-        .. |PyMCLabs| image:: https://raw.githubusercontent.com/pymc-devs/pymc/main/docs/logos/sponsors/pymc-labs.png
+        .. |NumFOCUS| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_numfocus.png?raw=true
+           :target: http://www.numfocus.org/
+        .. |PyMCLabs| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_pymc_labs.png?raw=true
            :target: https://pymc-labs.io
-        .. |Mistplay| image:: https://github.com/pymc-devs/pymcon_web_series_website/blob/main/static/images/sponsors_logos/mistplay_label_dark.png?raw=true
+        .. |Mistplay| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_mistplay.png?raw=true
            :target: https://www.mistplay.com/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pymc-5.2.0/README.rst` & `pymc-5.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -157,15 +157,15 @@
    :target: https://mybinder.org/v2/gh/pymc-devs/pymc/main?filepath=%2Fdocs%2Fsource%2Fnotebooks
 .. |Build Status| image:: https://github.com/pymc-devs/pymc/workflows/pytest/badge.svg
    :target: https://github.com/pymc-devs/pymc/actions
 .. |Coverage| image:: https://codecov.io/gh/pymc-devs/pymc/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/pymc-devs/pymc
 .. |Dockerhub| image:: https://img.shields.io/docker/automated/pymc/pymc.svg
    :target: https://hub.docker.com/r/pymc/pymc
-.. |NumFOCUS| image:: https://www.numfocus.org/wp-content/uploads/2017/03/1457562110.png
-   :target: http://www.numfocus.org/
 .. |NumFOCUS_badge| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
    :target: http://www.numfocus.org/
-.. |PyMCLabs| image:: https://raw.githubusercontent.com/pymc-devs/pymc/main/docs/logos/sponsors/pymc-labs.png
+.. |NumFOCUS| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_numfocus.png?raw=true
+   :target: http://www.numfocus.org/
+.. |PyMCLabs| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_pymc_labs.png?raw=true
    :target: https://pymc-labs.io
-.. |Mistplay| image:: https://github.com/pymc-devs/pymcon_web_series_website/blob/main/static/images/sponsors_logos/mistplay_label_dark.png?raw=true
+.. |Mistplay| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_mistplay.png?raw=true
    :target: https://www.mistplay.com/
```

### Comparing `pymc-5.2.0/RELEASE-NOTES.md` & `pymc-5.3.0/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/__init__.py` & `pymc-5.3.0/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/backends/__init__.py` & `pymc-5.3.0/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/backends/arviz.py` & `pymc-5.3.0/pymc/backends/arviz.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/backends/base.py` & `pymc-5.3.0/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/backends/mcbackend.py` & `pymc-5.3.0/pymc/backends/mcbackend.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/backends/ndarray.py` & `pymc-5.3.0/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/backends/report.py` & `pymc-5.3.0/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/blocking.py` & `pymc-5.3.0/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/data.py` & `pymc-5.3.0/pymc/data.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/__init__.py` & `pymc-5.3.0/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/bound.py` & `pymc-5.3.0/pymc/distributions/bound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/censored.py` & `pymc-5.3.0/pymc/distributions/censored.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,23 @@
             1-\text{CDF}(upper, dist) & \text {for} x = upper, \\
             0 & \text{for } x > upper,
         \end{cases}
 
 
     Parameters
     ----------
-    dist: unnamed distribution
-        Univariate distribution created via the `.dist()` API, which will be censored.
+    dist : unnamed_distribution
+        Univariate distribution which will be censored.
         This distribution must have a logcdf method implemented for sampling.
 
         .. warning:: dist will be cloned, rendering it independent of the one passed as input.
 
-    lower: float or None
+    lower : float or None
         Lower (left) censoring point. If `None` the distribution will not be left censored
-    upper: float or None
+    upper : float or None
         Upper (right) censoring point. If `None`, the distribution will not be right censored.
 
     Warnings
     --------
     Continuous censored distributions should only be used as likelihoods.
     Continuous censored distributions are a form of discrete-continuous mixture
     and as such cannot be sampled properly without a custom step sampler.
```

### Comparing `pymc-5.2.0/pymc/distributions/continuous.py` & `pymc-5.3.0/pymc/distributions/continuous.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,32 +230,34 @@
     """
     if tau is None:
         if sigma is None:
             sigma = 1.0
             tau = 1.0
         else:
             if isinstance(sigma, Variable):
-                sigma_ = check_parameters(sigma, sigma > 0, msg="sigma > 0")
+                # Keep tau negative, if sigma was negative, so that it will fail when used
+                tau = (sigma**-2.0) * pt.sign(sigma)
             else:
                 sigma_ = np.asarray(sigma)
                 if np.any(sigma_ <= 0):
                     raise ValueError("sigma must be positive")
-            tau = sigma_**-2.0
+                tau = sigma_**-2.0
 
     else:
         if sigma is not None:
             raise ValueError("Can't pass both tau and sigma")
         else:
             if isinstance(tau, Variable):
-                tau_ = check_parameters(tau, tau > 0, msg="tau > 0")
+                # Keep sigma negative, if tau was negative, so that it will fail when used
+                sigma = pt.abs(tau) ** (-0.5) * pt.sign(tau)
             else:
                 tau_ = np.asarray(tau)
                 if np.any(tau_ <= 0):
                     raise ValueError("tau must be positive")
-            sigma = tau_**-0.5
+                sigma = tau_**-0.5
 
     return floatX(tau), floatX(sigma)
 
 
 class Uniform(BoundedContinuous):
     r"""
     Continuous uniform log-likelihood.
@@ -810,15 +812,21 @@
 
         with pm.Model():
             x = pm.HalfNormal('x', tau=1/15)
     """
     rv_op = halfnormal
 
     @classmethod
-    def dist(cls, sigma=None, tau=None, *args, **kwargs):
+    def dist(
+        cls,
+        sigma: Optional[DIST_PARAMETER_TYPES] = None,
+        tau: Optional[DIST_PARAMETER_TYPES] = None,
+        *args,
+        **kwargs,
+    ):
         tau, sigma = get_tau_sigma(tau=tau, sigma=sigma)
 
         return super().dist([0.0, sigma], **kwargs)
 
     def moment(rv, size, loc, sigma):
         moment = loc + sigma
         if not rv_size_is_none(size):
@@ -942,15 +950,22 @@
 
     .. [Giner2016] Göknur Giner, Gordon K. Smyth (2016)
        statmod: Probability Calculations for the Inverse Gaussian Distribution
     """
     rv_op = wald
 
     @classmethod
-    def dist(cls, mu=None, lam=None, phi=None, alpha=0.0, **kwargs):
+    def dist(
+        cls,
+        mu: Optional[DIST_PARAMETER_TYPES] = None,
+        lam: Optional[DIST_PARAMETER_TYPES] = None,
+        phi: Optional[DIST_PARAMETER_TYPES] = None,
+        alpha: Optional[DIST_PARAMETER_TYPES] = 0.0,
+        **kwargs,
+    ):
         mu, lam, phi = cls.get_mu_lam_phi(mu, lam, phi)
         alpha = pt.as_tensor_variable(floatX(alpha))
         mu = pt.as_tensor_variable(floatX(mu))
         lam = pt.as_tensor_variable(floatX(lam))
         return super().dist([mu, lam, alpha], **kwargs)
 
     def moment(rv, size, mu, lam, alpha):
@@ -1109,15 +1124,24 @@
     Beta distribution is a conjugate prior for the parameter :math:`p` of
     the binomial distribution.
     """
 
     rv_op = pytensor.tensor.random.beta
 
     @classmethod
-    def dist(cls, alpha=None, beta=None, mu=None, sigma=None, nu=None, *args, **kwargs):
+    def dist(
+        cls,
+        alpha: Optional[DIST_PARAMETER_TYPES] = None,
+        beta: Optional[DIST_PARAMETER_TYPES] = None,
+        mu: Optional[DIST_PARAMETER_TYPES] = None,
+        sigma: Optional[DIST_PARAMETER_TYPES] = None,
+        nu: Optional[DIST_PARAMETER_TYPES] = None,
+        *args,
+        **kwargs,
+    ):
         alpha, beta = cls.get_alpha_beta(alpha, beta, mu, sigma, nu)
         alpha = pt.as_tensor_variable(floatX(alpha))
         beta = pt.as_tensor_variable(floatX(beta))
 
         return super().dist([alpha, beta], **kwargs)
 
     def moment(rv, size, alpha, beta):
@@ -1237,15 +1261,15 @@
         a > 0.
     b : tensor_like of float
         b > 0.
     """
     rv_op = kumaraswamy
 
     @classmethod
-    def dist(cls, a, b, *args, **kwargs):
+    def dist(cls, a: DIST_PARAMETER_TYPES, b: DIST_PARAMETER_TYPES, *args, **kwargs):
         a = pt.as_tensor_variable(floatX(a))
         b = pt.as_tensor_variable(floatX(b))
 
         return super().dist([a, b], *args, **kwargs)
 
     def moment(rv, size, a, b):
         mean = pt.exp(pt.log(b) + pt.gammaln(1 + 1 / a) + pt.gammaln(b) - pt.gammaln(1 + 1 / a + b))
@@ -1323,15 +1347,15 @@
     ----------
     lam : tensor_like of float
         Rate or inverse scale (``lam`` > 0).
     """
     rv_op = exponential
 
     @classmethod
-    def dist(cls, lam, *args, **kwargs):
+    def dist(cls, lam: DIST_PARAMETER_TYPES, *args, **kwargs):
         lam = pt.as_tensor_variable(floatX(lam))
 
         # PyTensor exponential op is parametrized in terms of mu (1/lam)
         return super().dist([pt.reciprocal(lam)], **kwargs)
 
     def moment(rv, size, mu):
         if not rv_size_is_none(size):
@@ -1357,14 +1381,23 @@
 
         return check_parameters(
             res,
             lam >= 0,
             msg="lam >= 0",
         )
 
+    def icdf(value, mu):
+        res = -mu * pt.log(1 - value)
+        res = check_icdf_value(res, value)
+        return check_icdf_parameters(
+            res,
+            mu >= 0,
+            msg="mu >= 0",
+        )
+
 
 class Laplace(Continuous):
     r"""
     Laplace log-likelihood.
 
     The pdf of this distribution is
 
@@ -2465,15 +2498,15 @@
     ndim_supp = 0
     ndims_params = [0, 0]
     dtype = "floatX"
     _print_name = ("HalfStudentT", "\\operatorname{HalfStudentT}")
 
     @classmethod
     def rng_fn(cls, rng, nu, sigma, size=None) -> np.ndarray:
-        return np.asarray(np.abs(stats.t.rvs(nu, sigma, size=size, random_state=rng)))
+        return np.asarray(np.abs(stats.t.rvs(nu, scale=sigma, size=size, random_state=rng)))
 
 
 halfstudentt = HalfStudentTRV()
 
 
 class HalfStudentT(PositiveContinuous):
     r"""
```

### Comparing `pymc-5.2.0/pymc/distributions/discrete.py` & `pymc-5.3.0/pymc/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/dist_math.py` & `pymc-5.3.0/pymc/distributions/dist_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
 
     def impl(self, x):
         return scipy.special.i0e(x)
 
     def grad(self, inp, grads):
         (x,) = inp
         (gz,) = grads
-        return (gz * (i1e_scalar(x) - pytensor.scalar.sgn(x) * i0e_scalar(x)),)
+        return (gz * (i1e_scalar(x) - pytensor.scalar.sign(x) * i0e_scalar(x)),)
 
 
 i0e_scalar = I0e(upgrade_to_float_no_complex, name="i0e")
 i0e = Elemwise(i0e_scalar, name="Elemwise{i0e,no_inplace}")
 
 
 def random_choice(p, size):
```

### Comparing `pymc-5.2.0/pymc/distributions/distribution.py` & `pymc-5.3.0/pymc/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/mixture.py` & `pymc-5.3.0/pymc/distributions/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/multivariate.py` & `pymc-5.3.0/pymc/distributions/multivariate.py`

 * *Files 0% similar despite different names*

```diff
@@ -4416,1172 +4416,1172 @@
 000113f0: 7379 6d6d 6574 7269 6320 6164 6a61 6365  symmetric adjace
 00011400: 6e63 7920 6d61 7472 6978 2e22 0a20 2020  ncy matrix.".   
 00011410: 2020 2020 2069 6620 7370 6172 7365 3a0a       if sparse:.
 00011420: 2020 2020 2020 2020 2020 2020 6162 735f              abs_
 00011430: 6469 6666 203d 2070 7974 656e 736f 722e  diff = pytensor.
 00011440: 7370 6172 7365 2e62 6173 6963 2e6d 756c  sparse.basic.mul
 00011450: 2870 7974 656e 736f 722e 7370 6172 7365  (pytensor.sparse
-00011460: 2e62 6173 6963 2e73 676e 2857 202d 2057  .basic.sgn(W - W
-00011470: 2e54 292c 2057 202d 2057 2e54 290a 2020  .T), W - W.T).  
-00011480: 2020 2020 2020 2020 2020 5720 3d20 4173            W = As
-00011490: 7365 7274 286d 7367 2928 572c 2070 742e  sert(msg)(W, pt.
-000114a0: 6973 636c 6f73 6528 7079 7465 6e73 6f72  isclose(pytensor
-000114b0: 2e73 7061 7273 652e 6261 7369 632e 7370  .sparse.basic.sp
-000114c0: 5f73 756d 2861 6273 5f64 6966 6629 2c20  _sum(abs_diff), 
-000114d0: 3029 290a 2020 2020 2020 2020 656c 7365  0)).        else
-000114e0: 3a0a 2020 2020 2020 2020 2020 2020 5720  :.            W 
-000114f0: 3d20 4173 7365 7274 286d 7367 2928 572c  = Assert(msg)(W,
-00011500: 2070 742e 616c 6c63 6c6f 7365 2857 2c20   pt.allclose(W, 
-00011510: 572e 5429 290a 0a20 2020 2020 2020 2074  W.T))..        t
-00011520: 6175 203d 2070 742e 6173 5f74 656e 736f  au = pt.as_tenso
-00011530: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
-00011540: 5828 7461 7529 290a 2020 2020 2020 2020  X(tau)).        
-00011550: 616c 7068 6120 3d20 7074 2e61 735f 7465  alpha = pt.as_te
-00011560: 6e73 6f72 5f76 6172 6961 626c 6528 666c  nsor_variable(fl
-00011570: 6f61 7458 2861 6c70 6861 2929 0a0a 2020  oatX(alpha))..  
-00011580: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-00011590: 6572 2829 2e6d 616b 655f 6e6f 6465 2872  er().make_node(r
-000115a0: 6e67 2c20 7369 7a65 2c20 6474 7970 652c  ng, size, dtype,
-000115b0: 206d 752c 2057 2c20 616c 7068 612c 2074   mu, W, alpha, t
-000115c0: 6175 290a 0a20 2020 2064 6566 205f 696e  au)..    def _in
-000115d0: 6665 725f 7368 6170 6528 7365 6c66 2c20  fer_shape(self, 
-000115e0: 7369 7a65 2c20 6469 7374 5f70 6172 616d  size, dist_param
-000115f0: 732c 2070 6172 616d 5f73 6861 7065 733d  s, param_shapes=
-00011600: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-00011610: 6861 7065 203d 2074 7570 6c65 2873 697a  hape = tuple(siz
-00011620: 6529 202b 2028 6469 7374 5f70 6172 616d  e) + (dist_param
-00011630: 735b 305d 2e73 6861 7065 5b2d 315d 2c29  s[0].shape[-1],)
-00011640: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011650: 7368 6170 650a 0a20 2020 2040 636c 6173  shape..    @clas
-00011660: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00011670: 726e 675f 666e 2863 6c73 2c20 726e 673a  rng_fn(cls, rng:
-00011680: 206e 702e 7261 6e64 6f6d 2e52 616e 646f   np.random.Rando
-00011690: 6d53 7461 7465 2c20 6d75 2c20 572c 2061  mState, mu, W, a
-000116a0: 6c70 6861 2c20 7461 752c 2073 697a 6529  lpha, tau, size)
-000116b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000116c0: 2020 2020 2020 496d 706c 656d 656e 7461        Implementa
-000116d0: 7469 6f6e 206f 6620 616c 676f 7269 7468  tion of algorith
-000116e0: 6d20 6672 6f6d 2070 6170 6572 0a20 2020  m from paper.   
-000116f0: 2020 2020 2048 6176 6172 6420 5275 652c       Havard Rue,
-00011700: 2032 3030 312e 2022 4661 7374 2073 616d   2001. "Fast sam
-00011710: 706c 696e 6720 6f66 2047 6175 7373 6961  pling of Gaussia
-00011720: 6e20 4d61 726b 6f76 2072 616e 646f 6d20  n Markov random 
-00011730: 6669 656c 6473 2c22 0a20 2020 2020 2020  fields,".       
-00011740: 204a 6f75 726e 616c 206f 6620 7468 6520   Journal of the 
-00011750: 526f 7961 6c20 5374 6174 6973 7469 6361  Royal Statistica
-00011760: 6c20 536f 6369 6574 7920 5365 7269 6573  l Society Series
-00011770: 2042 2c20 526f 7961 6c20 5374 6174 6973   B, Royal Statis
-00011780: 7469 6361 6c20 536f 6369 6574 792c 0a20  tical Society,. 
-00011790: 2020 2020 2020 2076 6f6c 2e20 3633 2832         vol. 63(2
-000117a0: 292c 2070 6167 6573 2033 3235 2d33 3338  ), pages 325-338
-000117b0: 2e20 444f 493a 2031 302e 3131 3131 2f31  . DOI: 10.1111/1
-000117c0: 3436 372d 3938 3638 2e30 3032 3838 0a20  467-9868.00288. 
-000117d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000117e0: 2020 2069 6620 6e6f 7420 7363 6970 792e     if not scipy.
-000117f0: 7370 6172 7365 2e69 7373 7061 7273 6528  sparse.issparse(
-00011800: 5729 3a0a 2020 2020 2020 2020 2020 2020  W):.            
-00011810: 5720 3d20 7363 6970 792e 7370 6172 7365  W = scipy.sparse
-00011820: 2e63 7372 5f6d 6174 7269 7828 5729 0a20  .csr_matrix(W). 
-00011830: 2020 2020 2020 2073 203d 206e 702e 6173         s = np.as
-00011840: 6172 7261 7928 572e 7375 6d28 6178 6973  array(W.sum(axis
-00011850: 3d30 2929 5b30 5d0a 2020 2020 2020 2020  =0))[0].        
-00011860: 4420 3d20 7363 6970 792e 7370 6172 7365  D = scipy.sparse
-00011870: 2e64 6961 6773 2873 290a 2020 2020 2020  .diags(s).      
-00011880: 2020 7461 7520 3d20 7363 6970 792e 7370    tau = scipy.sp
-00011890: 6172 7365 2e63 7372 5f6d 6174 7269 7828  arse.csr_matrix(
-000118a0: 7461 7529 0a20 2020 2020 2020 2061 6c70  tau).        alp
-000118b0: 6861 203d 2073 6369 7079 2e73 7061 7273  ha = scipy.spars
-000118c0: 652e 6373 725f 6d61 7472 6978 2861 6c70  e.csr_matrix(alp
-000118d0: 6861 290a 0a20 2020 2020 2020 2051 203d  ha)..        Q =
-000118e0: 2074 6175 2e6d 756c 7469 706c 7928 4420   tau.multiply(D 
-000118f0: 2d20 616c 7068 612e 6d75 6c74 6970 6c79  - alpha.multiply
-00011900: 2857 2929 0a0a 2020 2020 2020 2020 7065  (W))..        pe
-00011910: 726d 5f61 7272 6179 203d 2073 6369 7079  rm_array = scipy
-00011920: 2e73 7061 7273 652e 6373 6772 6170 682e  .sparse.csgraph.
-00011930: 7265 7665 7273 655f 6375 7468 696c 6c5f  reverse_cuthill_
-00011940: 6d63 6b65 6528 512c 2073 796d 6d65 7472  mckee(Q, symmetr
-00011950: 6963 5f6d 6f64 653d 5472 7565 290a 2020  ic_mode=True).  
-00011960: 2020 2020 2020 696e 765f 7065 726d 203d        inv_perm =
-00011970: 206e 702e 6172 6773 6f72 7428 7065 726d   np.argsort(perm
-00011980: 5f61 7272 6179 290a 0a20 2020 2020 2020  _array)..       
-00011990: 2051 203d 2051 5b70 6572 6d5f 6172 7261   Q = Q[perm_arra
-000119a0: 792c 203a 5d5b 3a2c 2070 6572 6d5f 6172  y, :][:, perm_ar
-000119b0: 7261 795d 0a0a 2020 2020 2020 2020 5162  ray]..        Qb
-000119c0: 203d 2051 2e64 6961 676f 6e61 6c28 290a   = Q.diagonal().
-000119d0: 2020 2020 2020 2020 7520 3d20 310a 2020          u = 1.  
-000119e0: 2020 2020 2020 7768 696c 6520 6e70 2e63        while np.c
-000119f0: 6f75 6e74 5f6e 6f6e 7a65 726f 2851 2e64  ount_nonzero(Q.d
-00011a00: 6961 676f 6e61 6c28 7529 2920 3e20 303a  iagonal(u)) > 0:
-00011a10: 0a20 2020 2020 2020 2020 2020 2051 6220  .            Qb 
-00011a20: 3d20 6e70 2e76 7374 6163 6b28 286e 702e  = np.vstack((np.
-00011a30: 7061 6428 512e 6469 6167 6f6e 616c 2875  pad(Q.diagonal(u
-00011a40: 292c 2028 752c 2030 292c 2063 6f6e 7374  ), (u, 0), const
-00011a50: 616e 745f 7661 6c75 6573 3d28 302c 2030  ant_values=(0, 0
-00011a60: 2929 2c20 5162 2929 0a20 2020 2020 2020  )), Qb)).       
-00011a70: 2020 2020 2075 202b 3d20 310a 0a20 2020       u += 1..   
-00011a80: 2020 2020 204c 203d 2073 6369 7079 2e6c       L = scipy.l
-00011a90: 696e 616c 672e 6368 6f6c 6573 6b79 5f62  inalg.cholesky_b
-00011aa0: 616e 6465 6428 5162 2c20 6c6f 7765 723d  anded(Qb, lower=
-00011ab0: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
-00011ac0: 7369 7a65 203d 2074 7570 6c65 2873 697a  size = tuple(siz
-00011ad0: 6520 6f72 2028 2929 0a20 2020 2020 2020  e or ()).       
-00011ae0: 2069 6620 7369 7a65 3a0a 2020 2020 2020   if size:.      
-00011af0: 2020 2020 2020 6d75 203d 206e 702e 6272        mu = np.br
-00011b00: 6f61 6463 6173 745f 746f 286d 752c 2073  oadcast_to(mu, s
-00011b10: 697a 6520 2b20 286d 752e 7368 6170 655b  ize + (mu.shape[
-00011b20: 2d31 5d2c 2929 0a20 2020 2020 2020 207a  -1],)).        z
-00011b30: 203d 2072 6e67 2e6e 6f72 6d61 6c28 7369   = rng.normal(si
-00011b40: 7a65 3d6d 752e 7368 6170 6529 0a20 2020  ze=mu.shape).   
-00011b50: 2020 2020 2073 616d 706c 6573 203d 206e       samples = n
-00011b60: 702e 656d 7074 7928 7a2e 7368 6170 6529  p.empty(z.shape)
-00011b70: 0a20 2020 2020 2020 2066 6f72 2069 6478  .        for idx
-00011b80: 2069 6e20 6e70 2e6e 6469 6e64 6578 286d   in np.ndindex(m
-00011b90: 752e 7368 6170 655b 3a2d 315d 293a 0a20  u.shape[:-1]):. 
-00011ba0: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
-00011bb0: 6573 5b69 6478 5d20 3d20 7363 6970 792e  es[idx] = scipy.
-00011bc0: 6c69 6e61 6c67 2e63 686f 5f73 6f6c 7665  linalg.cho_solve
-00011bd0: 5f62 616e 6465 6428 284c 2c20 4661 6c73  _banded((L, Fals
-00011be0: 6529 2c20 7a5b 6964 785d 2920 2b20 6d75  e), z[idx]) + mu
-00011bf0: 5b69 6478 5d5b 7065 726d 5f61 7272 6179  [idx][perm_array
-00011c00: 5d0a 2020 2020 2020 2020 7361 6d70 6c65  ].        sample
-00011c10: 7320 3d20 7361 6d70 6c65 735b 2e2e 2e2c  s = samples[...,
-00011c20: 2069 6e76 5f70 6572 6d5d 0a20 2020 2020   inv_perm].     
-00011c30: 2020 2072 6574 7572 6e20 7361 6d70 6c65     return sample
-00011c40: 730a 0a0a 6361 7220 3d20 4341 5252 5628  s...car = CARRV(
-00011c50: 290a 0a0a 636c 6173 7320 4341 5228 436f  )...class CAR(Co
-00011c60: 6e74 696e 756f 7573 293a 0a20 2020 2072  ntinuous):.    r
-00011c70: 2222 220a 2020 2020 4c69 6b65 6c69 686f  """.    Likeliho
-00011c80: 6f64 2066 6f72 2061 2063 6f6e 6469 7469  od for a conditi
-00011c90: 6f6e 616c 2061 7574 6f72 6567 7265 7373  onal autoregress
-00011ca0: 696f 6e2e 2054 6869 7320 6973 2061 2073  ion. This is a s
-00011cb0: 7065 6369 616c 2063 6173 6520 6f66 2074  pecial case of t
-00011cc0: 6865 0a20 2020 206d 756c 7469 7661 7269  he.    multivari
-00011cd0: 6174 6520 6e6f 726d 616c 2077 6974 6820  ate normal with 
-00011ce0: 616e 2061 646a 6163 656e 6379 2d73 7472  an adjacency-str
-00011cf0: 7563 7475 7265 6420 636f 7661 7269 616e  uctured covarian
-00011d00: 6365 206d 6174 7269 782e 0a0a 2020 2020  ce matrix...    
-00011d10: 2e2e 206d 6174 683a 3a0a 0a20 2020 2020  .. math::..     
-00011d20: 2020 6628 7820 5c6d 6964 2057 2c20 5c61    f(x \mid W, \a
-00011d30: 6c70 6861 2c20 5c74 6175 2920 3d0a 2020  lpha, \tau) =.  
-00011d40: 2020 2020 2020 2020 205c 6672 6163 7b7c           \frac{|
-00011d50: 547c 5e7b 312f 327d 7d7b 2832 5c70 6929  T|^{1/2}}{(2\pi)
-00011d60: 5e7b 6b2f 327d 7d0a 2020 2020 2020 2020  ^{k/2}}.        
-00011d70: 2020 205c 6578 705c 6c65 6674 5c7b 202d     \exp\left\{ -
-00011d80: 5c66 7261 637b 317d 7b32 7d20 2878 2d5c  \frac{1}{2} (x-\
-00011d90: 6d75 295e 7b5c 7072 696d 657d 2054 5e7b  mu)^{\prime} T^{
-00011da0: 2d31 7d20 2878 2d5c 6d75 2920 5c72 6967  -1} (x-\mu) \rig
-00011db0: 6874 5c7d 0a0a 2020 2020 7768 6572 6520  ht\}..    where 
-00011dc0: 3a6d 6174 683a 6054 203d 2028 5c74 6175  :math:`T = (\tau
-00011dd0: 2044 2849 2d5c 616c 7068 6120 5729 295e   D(I-\alpha W))^
-00011de0: 7b2d 317d 6020 616e 6420 3a6d 6174 683a  {-1}` and :math:
-00011df0: 6044 203d 2064 6961 6728 5c73 756d 5f69  `D = diag(\sum_i
-00011e00: 2057 5f7b 696a 7d29 602e 0a0a 2020 2020   W_{ij})`...    
-00011e10: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
-00011e20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011e30: 3d3d 3d3d 0a20 2020 2053 7570 706f 7274  ====.    Support
-00011e40: 2020 203a 6d61 7468 3a60 7820 5c69 6e20     :math:`x \in 
-00011e50: 5c6d 6174 6862 627b 527d 5e6b 600a 2020  \mathbb{R}^k`.  
-00011e60: 2020 4d65 616e 2020 2020 2020 3a6d 6174    Mean      :mat
-00011e70: 683a 605c 6d75 205c 696e 205c 6d61 7468  h:`\mu \in \math
-00011e80: 6262 7b52 7d5e 6b60 0a20 2020 2056 6172  bb{R}^k`.    Var
-00011e90: 6961 6e63 6520 203a 6d61 7468 3a60 285c  iance  :math:`(\
-00011ea0: 7461 7520 4428 492d 5c61 6c70 6861 2057  tau D(I-\alpha W
-00011eb0: 2929 5e7b 2d31 7d60 0a20 2020 203d 3d3d  ))^{-1}`.    ===
-00011ec0: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
-00011ed0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011ee0: 3d0a 0a20 2020 2050 6172 616d 6574 6572  =..    Parameter
-00011ef0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
-00011f00: 0a20 2020 206d 7520 3a20 7465 6e73 6f72  .    mu : tensor
-00011f10: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
-00011f20: 2020 2020 2020 2052 6561 6c2d 7661 6c75         Real-valu
-00011f30: 6564 206d 6561 6e20 7665 6374 6f72 0a20  ed mean vector. 
-00011f40: 2020 2057 203a 2028 4d2c 204d 2920 7465     W : (M, M) te
-00011f50: 6e73 6f72 5f6c 696b 6520 6f66 2069 6e74  nsor_like of int
-00011f60: 0a20 2020 2020 2020 2053 796d 6d65 7472  .        Symmetr
-00011f70: 6963 2061 646a 6163 656e 6379 206d 6174  ic adjacency mat
-00011f80: 7269 7820 6f66 2031 7320 616e 6420 3073  rix of 1s and 0s
-00011f90: 2069 6e64 6963 6174 696e 670a 2020 2020   indicating.    
-00011fa0: 2020 2020 6164 6a61 6365 6e63 7920 6265      adjacency be
-00011fb0: 7477 6565 6e20 656c 656d 656e 7473 2e20  tween elements. 
-00011fc0: 4966 2070 6f73 7369 626c 652c 202a 572a  If possible, *W*
-00011fd0: 2069 7320 636f 6e76 6572 7465 640a 2020   is converted.  
-00011fe0: 2020 2020 2020 746f 2061 2073 7061 7273        to a spars
-00011ff0: 6520 6d61 7472 6978 2c20 6661 6c6c 696e  e matrix, fallin
-00012000: 6720 6261 636b 2074 6f20 6120 6465 6e73  g back to a dens
-00012010: 6520 7661 7269 6162 6c65 2e0a 2020 2020  e variable..    
-00012020: 2020 2020 3a66 756e 633a 607e 7079 7465      :func:`~pyte
-00012030: 6e73 6f72 2e73 7061 7273 652e 6261 7369  nsor.sparse.basi
-00012040: 632e 6173 5f73 7061 7273 655f 6f72 5f74  c.as_sparse_or_t
-00012050: 656e 736f 725f 7661 7269 6162 6c65 6020  ensor_variable` 
-00012060: 6973 0a20 2020 2020 2020 2075 7365 6420  is.        used 
-00012070: 666f 7220 7468 6973 2073 7061 7273 6520  for this sparse 
-00012080: 6f72 2074 656e 736f 7276 6172 6961 626c  or tensorvariabl
-00012090: 6520 636f 6e76 6572 7369 6f6e 2e0a 2020  e conversion..  
-000120a0: 2020 616c 7068 6120 3a20 7465 6e73 6f72    alpha : tensor
-000120b0: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
-000120c0: 2020 2020 2020 2041 7574 6f72 6567 7265         Autoregre
-000120d0: 7373 696f 6e20 7061 7261 6d65 7465 7220  ssion parameter 
-000120e0: 7461 6b69 6e67 2076 616c 7565 7320 6265  taking values be
-000120f0: 7477 6565 6e20 2d31 2061 6e64 2031 2e20  tween -1 and 1. 
-00012100: 5661 6c75 6573 2063 6c6f 7365 7220 746f  Values closer to
-00012110: 2030 2069 6e64 6963 6174 6520 7765 616b   0 indicate weak
-00012120: 6572 0a20 2020 2020 2020 2063 6f72 7265  er.        corre
-00012130: 6c61 7469 6f6e 2061 6e64 2076 616c 7565  lation and value
-00012140: 7320 636c 6f73 6572 2074 6f20 3120 696e  s closer to 1 in
-00012150: 6469 6361 7465 2068 6967 6865 7220 6175  dicate higher au
-00012160: 746f 636f 7272 656c 6174 696f 6e2e 2046  tocorrelation. F
-00012170: 6f72 206d 6f73 7420 7573 6520 6361 7365  or most use case
-00012180: 732c 2074 6865 0a20 2020 2020 2020 2073  s, the.        s
-00012190: 7570 706f 7274 206f 6620 616c 7068 6120  upport of alpha 
-000121a0: 7368 6f75 6c64 2062 6520 7265 7374 7269  should be restri
-000121b0: 6374 6564 2074 6f20 2830 2c20 3129 2e0a  cted to (0, 1)..
-000121c0: 2020 2020 7461 7520 3a20 7465 6e73 6f72      tau : tensor
-000121d0: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
-000121e0: 2020 2020 2020 2050 6f73 6974 6976 6520         Positive 
-000121f0: 7072 6563 6973 696f 6e20 7661 7269 6162  precision variab
-00012200: 6c65 2063 6f6e 7472 6f6c 6c69 6e67 2074  le controlling t
-00012210: 6865 2073 6361 6c65 206f 6620 7468 6520  he scale of the 
-00012220: 756e 6465 726c 7969 6e67 206e 6f72 6d61  underlying norma
-00012230: 6c20 7661 7269 6174 6573 2e0a 0a20 2020  l variates...   
-00012240: 2052 6566 6572 656e 6365 730a 2020 2020   References.    
-00012250: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e  ----------.    .
-00012260: 2e20 204a 696e 2c20 582e 2c20 4361 726c  .  Jin, X., Carl
-00012270: 696e 2c20 422e 2c20 4261 6e65 726a 6565  in, B., Banerjee
-00012280: 2c20 532e 0a20 2020 2020 2020 2022 4765  , S..        "Ge
-00012290: 6e65 7261 6c69 7a65 6420 4869 6572 6172  neralized Hierar
-000122a0: 6368 6963 616c 204d 756c 7469 7661 7269  chical Multivari
-000122b0: 6174 6520 4341 5220 4d6f 6465 6c73 2066  ate CAR Models f
-000122c0: 6f72 2041 7265 616c 2044 6174 6122 0a20  or Areal Data". 
-000122d0: 2020 2020 2020 2042 696f 6d65 7472 6963         Biometric
-000122e0: 732c 2056 6f6c 2e20 3631 2c20 4e6f 2e20  s, Vol. 61, No. 
-000122f0: 3420 2844 6563 2e2c 2032 3030 3529 2c20  4 (Dec., 2005), 
-00012300: 7070 2e20 3935 302d 3936 310a 2020 2020  pp. 950-961.    
-00012310: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
-00012320: 6361 720a 0a20 2020 2040 636c 6173 736d  car..    @classm
-00012330: 6574 686f 640a 2020 2020 6465 6620 6469  ethod.    def di
-00012340: 7374 2863 6c73 2c20 6d75 2c20 572c 2061  st(cls, mu, W, a
-00012350: 6c70 6861 2c20 7461 752c 202a 6172 6773  lpha, tau, *args
-00012360: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00012370: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00012380: 7228 292e 6469 7374 285b 6d75 2c20 572c  r().dist([mu, W,
-00012390: 2061 6c70 6861 2c20 7461 755d 2c20 2a2a   alpha, tau], **
-000123a0: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
-000123b0: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
-000123c0: 2c20 6d75 2c20 572c 2061 6c70 6861 2c20  , mu, W, alpha, 
-000123d0: 7461 7529 3a0a 2020 2020 2020 2020 7265  tau):.        re
-000123e0: 7475 726e 2070 742e 6675 6c6c 5f6c 696b  turn pt.full_lik
-000123f0: 6528 7276 2c20 6d75 290a 0a20 2020 2064  e(rv, mu)..    d
-00012400: 6566 206c 6f67 7028 7661 6c75 652c 206d  ef logp(value, m
-00012410: 752c 2057 2c20 616c 7068 612c 2074 6175  u, W, alpha, tau
-00012420: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00012430: 2020 2020 2020 2043 616c 6375 6c61 7465         Calculate
-00012440: 206c 6f67 2d70 726f 6261 6269 6c69 7479   log-probability
-00012450: 206f 6620 6120 4341 522d 6469 7374 7269   of a CAR-distri
-00012460: 6275 7465 6420 7665 6374 6f72 0a20 2020  buted vector.   
-00012470: 2020 2020 2061 7420 7370 6563 6966 6965       at specifie
-00012480: 6420 7661 6c75 652e 2054 6869 7320 6c6f  d value. This lo
-00012490: 6720 7072 6f62 6162 696c 6974 7920 6675  g probability fu
-000124a0: 6e63 7469 6f6e 2064 6966 6665 7273 2066  nction differs f
-000124b0: 726f 6d0a 2020 2020 2020 2020 7468 6520  rom.        the 
-000124c0: 7472 7565 2043 4152 206c 6f67 2064 656e  true CAR log den
-000124d0: 7369 7479 2028 414b 4120 6120 6d75 6c74  sity (AKA a mult
-000124e0: 6976 6172 6961 7465 206e 6f72 6d61 6c20  ivariate normal 
-000124f0: 7769 7468 2043 4152 2d73 7472 7563 7475  with CAR-structu
-00012500: 7265 640a 2020 2020 2020 2020 636f 7661  red.        cova
-00012510: 7269 616e 6365 206d 6174 7269 7829 2062  riance matrix) b
-00012520: 7920 616e 2061 6464 6974 6976 6520 636f  y an additive co
-00012530: 6e73 7461 6e74 2e0a 0a20 2020 2020 2020  nstant...       
-00012540: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00012550: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00012560: 2020 2020 2020 2076 616c 7565 3a20 6172         value: ar
-00012570: 7261 790a 2020 2020 2020 2020 2020 2020  ray.            
-00012580: 5661 6c75 6520 666f 7220 7768 6963 6820  Value for which 
-00012590: 6c6f 672d 7072 6f62 6162 696c 6974 7920  log-probability 
-000125a0: 6973 2063 616c 6375 6c61 7465 642e 0a0a  is calculated...
-000125b0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-000125c0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-000125d0: 2020 2020 2020 2020 5465 6e73 6f72 5661          TensorVa
-000125e0: 7269 6162 6c65 0a20 2020 2020 2020 2022  riable.        "
-000125f0: 2222 0a0a 2020 2020 2020 2020 7370 6172  ""..        spar
-00012600: 7365 203d 2069 7369 6e73 7461 6e63 6528  se = isinstance(
-00012610: 572c 2028 7079 7465 6e73 6f72 2e73 7061  W, (pytensor.spa
-00012620: 7273 652e 5370 6172 7365 436f 6e73 7461  rse.SparseConsta
-00012630: 6e74 2c20 7079 7465 6e73 6f72 2e73 7061  nt, pytensor.spa
-00012640: 7273 652e 5370 6172 7365 5661 7269 6162  rse.SparseVariab
-00012650: 6c65 2929 0a0a 2020 2020 2020 2020 6966  le))..        if
-00012660: 2073 7061 7273 653a 0a20 2020 2020 2020   sparse:.       
-00012670: 2020 2020 2044 203d 2073 705f 7375 6d28       D = sp_sum(
-00012680: 572c 2061 7869 733d 3029 0a20 2020 2020  W, axis=0).     
-00012690: 2020 2020 2020 2044 696e 765f 7371 7274         Dinv_sqrt
-000126a0: 203d 2070 742e 6469 6167 2831 202f 2070   = pt.diag(1 / p
-000126b0: 742e 7371 7274 2844 2929 0a20 2020 2020  t.sqrt(D)).     
-000126c0: 2020 2020 2020 2044 5744 203d 2070 742e         DWD = pt.
-000126d0: 646f 7428 7079 7465 6e73 6f72 2e73 7061  dot(pytensor.spa
-000126e0: 7273 652e 646f 7428 4469 6e76 5f73 7172  rse.dot(Dinv_sqr
-000126f0: 742c 2057 292c 2044 696e 765f 7371 7274  t, W), Dinv_sqrt
-00012700: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00012710: 2020 2020 2020 2020 2020 2020 4420 3d20              D = 
-00012720: 572e 7375 6d28 6178 6973 3d30 290a 2020  W.sum(axis=0).  
-00012730: 2020 2020 2020 2020 2020 4469 6e76 5f73            Dinv_s
-00012740: 7172 7420 3d20 7074 2e64 6961 6728 3120  qrt = pt.diag(1 
-00012750: 2f20 7074 2e73 7172 7428 4429 290a 2020  / pt.sqrt(D)).  
-00012760: 2020 2020 2020 2020 2020 4457 4420 3d20            DWD = 
-00012770: 7074 2e64 6f74 2870 742e 646f 7428 4469  pt.dot(pt.dot(Di
-00012780: 6e76 5f73 7172 742c 2057 292c 2044 696e  nv_sqrt, W), Din
-00012790: 765f 7371 7274 290a 2020 2020 2020 2020  v_sqrt).        
-000127a0: 6c61 6d20 3d20 7074 2e73 6c69 6e61 6c67  lam = pt.slinalg
-000127b0: 2e65 6967 7661 6c73 6828 4457 442c 2070  .eigvalsh(DWD, p
-000127c0: 742e 6579 6528 4457 442e 7368 6170 655b  t.eye(DWD.shape[
-000127d0: 305d 2929 0a0a 2020 2020 2020 2020 642c  0]))..        d,
-000127e0: 205f 203d 2057 2e73 6861 7065 0a0a 2020   _ = W.shape..  
-000127f0: 2020 2020 2020 6966 2076 616c 7565 2e6e        if value.n
-00012800: 6469 6d20 3d3d 2031 3a0a 2020 2020 2020  dim == 1:.      
-00012810: 2020 2020 2020 7661 6c75 6520 3d20 7661        value = va
-00012820: 6c75 655b 4e6f 6e65 2c20 3a5d 0a0a 2020  lue[None, :]..  
-00012830: 2020 2020 2020 6c6f 6774 6175 203d 2064        logtau = d
-00012840: 202a 2070 742e 6c6f 6728 7461 7529 2e73   * pt.log(tau).s
-00012850: 756d 2829 0a20 2020 2020 2020 206c 6f67  um().        log
-00012860: 6465 7420 3d20 7074 2e6c 6f67 2831 202d  det = pt.log(1 -
-00012870: 2061 6c70 6861 2e54 202a 206c 616d 5b3a   alpha.T * lam[:
-00012880: 2c20 4e6f 6e65 5d29 2e73 756d 2829 0a20  , None]).sum(). 
-00012890: 2020 2020 2020 2064 656c 7461 203d 2076         delta = v
-000128a0: 616c 7565 202d 206d 750a 0a20 2020 2020  alue - mu..     
-000128b0: 2020 2069 6620 7370 6172 7365 3a0a 2020     if sparse:.  
-000128c0: 2020 2020 2020 2020 2020 5764 656c 7461            Wdelta
-000128d0: 203d 2070 7974 656e 736f 722e 7370 6172   = pytensor.spar
-000128e0: 7365 2e64 6f74 2864 656c 7461 2c20 5729  se.dot(delta, W)
-000128f0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00012900: 2020 2020 2020 2020 2020 2057 6465 6c74             Wdelt
-00012910: 6120 3d20 7074 2e64 6f74 2864 656c 7461  a = pt.dot(delta
-00012920: 2c20 5729 0a0a 2020 2020 2020 2020 7461  , W)..        ta
-00012930: 755f 646f 745f 6465 6c74 6120 3d20 445b  u_dot_delta = D[
-00012940: 4e6f 6e65 2c20 3a5d 202a 2064 656c 7461  None, :] * delta
-00012950: 202d 2061 6c70 6861 202a 2057 6465 6c74   - alpha * Wdelt
-00012960: 610a 2020 2020 2020 2020 6c6f 6771 7561  a.        logqua
-00012970: 6420 3d20 2874 6175 202a 2064 656c 7461  d = (tau * delta
-00012980: 202a 2074 6175 5f64 6f74 5f64 656c 7461   * tau_dot_delta
-00012990: 292e 7375 6d28 6178 6973 3d2d 3129 0a20  ).sum(axis=-1). 
-000129a0: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
-000129b0: 6563 6b5f 7061 7261 6d65 7465 7273 280a  eck_parameters(.
-000129c0: 2020 2020 2020 2020 2020 2020 302e 3520              0.5 
-000129d0: 2a20 286c 6f67 7461 7520 2b20 6c6f 6764  * (logtau + logd
-000129e0: 6574 202d 206c 6f67 7175 6164 292c 0a20  et - logquad),. 
-000129f0: 2020 2020 2020 2020 2020 202d 3120 3c3d             -1 <=
-00012a00: 2061 6c70 6861 2c0a 2020 2020 2020 2020   alpha,.        
-00012a10: 2020 2020 616c 7068 6120 3c3d 2031 2c0a      alpha <= 1,.
-00012a20: 2020 2020 2020 2020 2020 2020 7461 7520              tau 
-00012a30: 3e20 302c 0a20 2020 2020 2020 2020 2020  > 0,.           
-00012a40: 206d 7367 3d22 2d31 203c 3d20 616c 7068   msg="-1 <= alph
-00012a50: 6120 3c3d 2031 2c20 7461 7520 3e20 3022  a <= 1, tau > 0"
-00012a60: 2c0a 2020 2020 2020 2020 290a 0a0a 636c  ,.        )...cl
-00012a70: 6173 7320 5374 6963 6b42 7265 616b 696e  ass StickBreakin
-00012a80: 6757 6569 6768 7473 5256 2852 616e 646f  gWeightsRV(Rando
-00012a90: 6d56 6172 6961 626c 6529 3a0a 2020 2020  mVariable):.    
-00012aa0: 6e61 6d65 203d 2022 7374 6963 6b5f 6272  name = "stick_br
-00012ab0: 6561 6b69 6e67 5f77 6569 6768 7473 220a  eaking_weights".
-00012ac0: 2020 2020 6e64 696d 5f73 7570 7020 3d20      ndim_supp = 
-00012ad0: 310a 2020 2020 6e64 696d 735f 7061 7261  1.    ndims_para
-00012ae0: 6d73 203d 205b 302c 2030 5d0a 2020 2020  ms = [0, 0].    
-00012af0: 6474 7970 6520 3d20 2266 6c6f 6174 5822  dtype = "floatX"
-00012b00: 0a20 2020 205f 7072 696e 745f 6e61 6d65  .    _print_name
-00012b10: 203d 2028 2253 7469 636b 4272 6561 6b69   = ("StickBreaki
-00012b20: 6e67 5765 6967 6874 7322 2c20 225c 5c6f  ngWeights", "\\o
-00012b30: 7065 7261 746f 726e 616d 657b 5374 6963  peratorname{Stic
-00012b40: 6b42 7265 616b 696e 6757 6569 6768 7473  kBreakingWeights
-00012b50: 7d22 290a 0a20 2020 2064 6566 206d 616b  }")..    def mak
-00012b60: 655f 6e6f 6465 2873 656c 662c 2072 6e67  e_node(self, rng
-00012b70: 2c20 7369 7a65 2c20 6474 7970 652c 2061  , size, dtype, a
-00012b80: 6c70 6861 2c20 4b29 3a0a 2020 2020 2020  lpha, K):.      
-00012b90: 2020 616c 7068 6120 3d20 7074 2e61 735f    alpha = pt.as_
-00012ba0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
-00012bb0: 616c 7068 6129 0a20 2020 2020 2020 204b  alpha).        K
-00012bc0: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
-00012bd0: 7661 7269 6162 6c65 2869 6e74 5828 4b29  variable(intX(K)
-00012be0: 290a 0a20 2020 2020 2020 2069 6620 4b2e  )..        if K.
-00012bf0: 6e64 696d 203e 2030 3a0a 2020 2020 2020  ndim > 0:.      
-00012c00: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00012c10: 6545 7272 6f72 2822 4b20 6d75 7374 2062  eError("K must b
-00012c20: 6520 6120 7363 616c 6172 2e22 290a 0a20  e a scalar.").. 
-00012c30: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00012c40: 7065 7228 292e 6d61 6b65 5f6e 6f64 6528  per().make_node(
-00012c50: 726e 672c 2073 697a 652c 2064 7479 7065  rng, size, dtype
-00012c60: 2c20 616c 7068 612c 204b 290a 0a20 2020  , alpha, K)..   
-00012c70: 2064 6566 205f 7375 7070 5f73 6861 7065   def _supp_shape
-00012c80: 5f66 726f 6d5f 7061 7261 6d73 2873 656c  _from_params(sel
-00012c90: 662c 2064 6973 745f 7061 7261 6d73 2c20  f, dist_params, 
-00012ca0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-00012cb0: 2020 204b 203d 2064 6973 745f 7061 7261     K = dist_para
-00012cc0: 6d73 5b31 5d0a 2020 2020 2020 2020 7265  ms[1].        re
-00012cd0: 7475 726e 2028 4b20 2b20 312c 290a 0a20  turn (K + 1,).. 
-00012ce0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00012cf0: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
-00012d00: 6c73 2c20 726e 672c 2061 6c70 6861 2c20  ls, rng, alpha, 
-00012d10: 4b2c 2073 697a 6529 3a0a 2020 2020 2020  K, size):.      
-00012d20: 2020 6966 204b 203c 2030 3a0a 2020 2020    if K < 0:.    
-00012d30: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00012d40: 6c75 6545 7272 6f72 2822 4b20 6e65 6564  lueError("K need
-00012d50: 7320 746f 2062 6520 706f 7369 7469 7665  s to be positive
-00012d60: 2e22 290a 0a20 2020 2020 2020 2073 697a  .")..        siz
-00012d70: 6520 3d20 746f 5f74 7570 6c65 2873 697a  e = to_tuple(siz
-00012d80: 6529 2069 6620 7369 7a65 2069 7320 6e6f  e) if size is no
-00012d90: 7420 4e6f 6e65 2065 6c73 6520 616c 7068  t None else alph
-00012da0: 612e 7368 6170 650a 2020 2020 2020 2020  a.shape.        
-00012db0: 7369 7a65 203d 2073 697a 6520 2b20 284b  size = size + (K
-00012dc0: 2c29 0a20 2020 2020 2020 2061 6c70 6861  ,).        alpha
-00012dd0: 203d 2061 6c70 6861 5b2e 2e2e 2c20 6e70   = alpha[..., np
-00012de0: 2e6e 6577 6178 6973 5d0a 0a20 2020 2020  .newaxis]..     
-00012df0: 2020 2062 6574 6173 203d 2072 6e67 2e62     betas = rng.b
-00012e00: 6574 6128 312c 2061 6c70 6861 2c20 7369  eta(1, alpha, si
-00012e10: 7a65 3d73 697a 6529 0a0a 2020 2020 2020  ze=size)..      
-00012e20: 2020 7374 6963 6b73 203d 206e 702e 636f    sticks = np.co
-00012e30: 6e63 6174 656e 6174 6528 0a20 2020 2020  ncatenate(.     
-00012e40: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-00012e50: 2020 2020 2020 2020 206e 702e 6f6e 6573           np.ones
-00012e60: 2873 6861 7065 3d28 7369 7a65 5b3a 2d31  (shape=(size[:-1
-00012e70: 5d20 2b20 2831 2c29 2929 2c0a 2020 2020  ] + (1,))),.    
-00012e80: 2020 2020 2020 2020 2020 2020 6e70 2e63              np.c
-00012e90: 756d 7072 6f64 2831 202d 2062 6574 6173  umprod(1 - betas
-00012ea0: 5b2e 2e2e 2c20 3a2d 315d 2c20 6178 6973  [..., :-1], axis
-00012eb0: 3d2d 3129 2c0a 2020 2020 2020 2020 2020  =-1),.          
-00012ec0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00012ed0: 2061 7869 733d 2d31 2c0a 2020 2020 2020   axis=-1,.      
-00012ee0: 2020 290a 0a20 2020 2020 2020 2077 6569    )..        wei
-00012ef0: 6768 7473 203d 2073 7469 636b 7320 2a20  ghts = sticks * 
-00012f00: 6265 7461 730a 2020 2020 2020 2020 7765  betas.        we
-00012f10: 6967 6874 7320 3d20 6e70 2e63 6f6e 6361  ights = np.conca
-00012f20: 7465 6e61 7465 280a 2020 2020 2020 2020  tenate(.        
-00012f30: 2020 2020 2877 6569 6768 7473 2c20 3120      (weights, 1 
-00012f40: 2d20 7765 6967 6874 732e 7375 6d28 6178  - weights.sum(ax
-00012f50: 6973 3d2d 3129 5b2e 2e2e 2c20 6e70 2e6e  is=-1)[..., np.n
-00012f60: 6577 6178 6973 5d29 2c0a 2020 2020 2020  ewaxis]),.      
-00012f70: 2020 2020 2020 6178 6973 3d2d 312c 0a20        axis=-1,. 
-00012f80: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00012f90: 2020 7265 7475 726e 2077 6569 6768 7473    return weights
-00012fa0: 0a0a 0a73 7469 636b 6272 6561 6b69 6e67  ...stickbreaking
-00012fb0: 7765 6967 6874 7320 3d20 5374 6963 6b42  weights = StickB
-00012fc0: 7265 616b 696e 6757 6569 6768 7473 5256  reakingWeightsRV
-00012fd0: 2829 0a0a 0a63 6c61 7373 2053 7469 636b  ()...class Stick
-00012fe0: 4272 6561 6b69 6e67 5765 6967 6874 7328  BreakingWeights(
-00012ff0: 5369 6d70 6c65 7843 6f6e 7469 6e75 6f75  SimplexContinuou
-00013000: 7329 3a0a 2020 2020 7222 2222 0a20 2020  s):.    r""".   
-00013010: 204c 696b 656c 6968 6f6f 6420 6f66 2074   Likelihood of t
-00013020: 7275 6e63 6174 6564 2073 7469 636b 2d62  runcated stick-b
-00013030: 7265 616b 696e 6720 7765 6967 6874 732e  reaking weights.
-00013040: 2054 6865 2077 6569 6768 7473 2061 7265   The weights are
-00013050: 2067 656e 6572 6174 6564 2066 726f 6d20   generated from 
-00013060: 610a 2020 2020 7374 6963 6b2d 6272 6561  a.    stick-brea
-00013070: 6b69 6e67 2070 726f 6365 6475 6365 2077  king proceduce w
-00013080: 6865 7265 203a 6d61 7468 3a60 785f 6b20  here :math:`x_k 
-00013090: 3d20 765f 6b20 5c70 726f 645f 7b5c 656c  = v_k \prod_{\el
-000130a0: 6c20 3c20 6b7d 2028 3120 2d20 765f 5c65  l < k} (1 - v_\e
-000130b0: 6c6c 2960 2066 6f72 0a20 2020 203a 6d61  ll)` for.    :ma
-000130c0: 7468 3a60 6b20 5c69 6e20 5c7b 312c 205c  th:`k \in \{1, \
-000130d0: 6c64 6f74 732c 204b 5c7d 6020 616e 6420  ldots, K\}` and 
-000130e0: 3a6d 6174 683a 6078 5f4b 203d 205c 7072  :math:`x_K = \pr
-000130f0: 6f64 5f7b 5c65 6c6c 203d 2031 7d5e 7b4b  od_{\ell = 1}^{K
-00013100: 7d20 2831 202d 2076 5f5c 656c 6c29 203d  } (1 - v_\ell) =
-00013110: 2031 202d 205c 7375 6d5f 7b5c 656c 6c3d   1 - \sum_{\ell=
-00013120: 317d 5e4b 2078 5f5c 656c 6c60 0a20 2020  1}^K x_\ell`.   
-00013130: 2077 6974 6820 3a6d 6174 683a 6076 5f6b   with :math:`v_k
-00013140: 205c 7374 6163 6b72 656c 7b5c 7465 7874   \stackrel{\text
-00013150: 7b69 2e69 2e64 2e7d 7d7b 5c73 696d 7d20  {i.i.d.}}{\sim} 
-00013160: 5c74 6578 747b 4265 7461 7d28 312c 205c  \text{Beta}(1, \
-00013170: 616c 7068 6129 602e 0a0a 2020 2020 2e2e  alpha)`...    ..
-00013180: 206d 6174 683a 0a0a 2020 2020 2020 2020   math:..        
-00013190: 6628 5c6d 6174 6862 667b 787d 7c5c 616c  f(\mathbf{x}|\al
-000131a0: 7068 612c 204b 2920 3d0a 2020 2020 2020  pha, K) =.      
-000131b0: 2020 2020 2020 4228 312c 205c 616c 7068        B(1, \alph
-000131c0: 6129 5e7b 2d4b 7d78 5f7b 4b2b 317d 5e5c  a)^{-K}x_{K+1}^\
-000131d0: 616c 7068 6120 5c70 726f 645f 7b6b 3d31  alpha \prod_{k=1
-000131e0: 7d5e 7b4b 2b31 7d5c 6c65 6674 5c7b 5c73  }^{K+1}\left\{\s
-000131f0: 756d 5f7b 6a3d 6b7d 5e7b 4b2b 317d 2078  um_{j=k}^{K+1} x
-00013200: 5f6a 5c72 6967 6874 5c7d 5e7b 2d31 7d0a  _j\right\}^{-1}.
-00013210: 0a20 2020 203d 3d3d 3d3d 3d3d 3d20 203d  .    ========  =
+00011460: 2e73 6967 6e28 5720 2d20 572e 5429 2c20  .sign(W - W.T), 
+00011470: 5720 2d20 572e 5429 0a20 2020 2020 2020  W - W.T).       
+00011480: 2020 2020 2057 203d 2041 7373 6572 7428       W = Assert(
+00011490: 6d73 6729 2857 2c20 7074 2e69 7363 6c6f  msg)(W, pt.isclo
+000114a0: 7365 2870 7974 656e 736f 722e 7370 6172  se(pytensor.spar
+000114b0: 7365 2e73 705f 7375 6d28 6162 735f 6469  se.sp_sum(abs_di
+000114c0: 6666 292c 2030 2929 0a20 2020 2020 2020  ff), 0)).       
+000114d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000114e0: 2020 2057 203d 2041 7373 6572 7428 6d73     W = Assert(ms
+000114f0: 6729 2857 2c20 7074 2e61 6c6c 636c 6f73  g)(W, pt.allclos
+00011500: 6528 572c 2057 2e54 2929 0a0a 2020 2020  e(W, W.T))..    
+00011510: 2020 2020 7461 7520 3d20 7074 2e61 735f      tau = pt.as_
+00011520: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
+00011530: 666c 6f61 7458 2874 6175 2929 0a20 2020  floatX(tau)).   
+00011540: 2020 2020 2061 6c70 6861 203d 2070 742e       alpha = pt.
+00011550: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+00011560: 6c65 2866 6c6f 6174 5828 616c 7068 6129  le(floatX(alpha)
+00011570: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00011580: 6e20 7375 7065 7228 292e 6d61 6b65 5f6e  n super().make_n
+00011590: 6f64 6528 726e 672c 2073 697a 652c 2064  ode(rng, size, d
+000115a0: 7479 7065 2c20 6d75 2c20 572c 2061 6c70  type, mu, W, alp
+000115b0: 6861 2c20 7461 7529 0a0a 2020 2020 6465  ha, tau)..    de
+000115c0: 6620 5f69 6e66 6572 5f73 6861 7065 2873  f _infer_shape(s
+000115d0: 656c 662c 2073 697a 652c 2064 6973 745f  elf, size, dist_
+000115e0: 7061 7261 6d73 2c20 7061 7261 6d5f 7368  params, param_sh
+000115f0: 6170 6573 3d4e 6f6e 6529 3a0a 2020 2020  apes=None):.    
+00011600: 2020 2020 7368 6170 6520 3d20 7475 706c      shape = tupl
+00011610: 6528 7369 7a65 2920 2b20 2864 6973 745f  e(size) + (dist_
+00011620: 7061 7261 6d73 5b30 5d2e 7368 6170 655b  params[0].shape[
+00011630: 2d31 5d2c 290a 2020 2020 2020 2020 7265  -1],).        re
+00011640: 7475 726e 2073 6861 7065 0a0a 2020 2020  turn shape..    
+00011650: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00011660: 2064 6566 2072 6e67 5f66 6e28 636c 732c   def rng_fn(cls,
+00011670: 2072 6e67 3a20 6e70 2e72 616e 646f 6d2e   rng: np.random.
+00011680: 5261 6e64 6f6d 5374 6174 652c 206d 752c  RandomState, mu,
+00011690: 2057 2c20 616c 7068 612c 2074 6175 2c20   W, alpha, tau, 
+000116a0: 7369 7a65 293a 0a20 2020 2020 2020 2022  size):.        "
+000116b0: 2222 0a20 2020 2020 2020 2049 6d70 6c65  "".        Imple
+000116c0: 6d65 6e74 6174 696f 6e20 6f66 2061 6c67  mentation of alg
+000116d0: 6f72 6974 686d 2066 726f 6d20 7061 7065  orithm from pape
+000116e0: 720a 2020 2020 2020 2020 4861 7661 7264  r.        Havard
+000116f0: 2052 7565 2c20 3230 3031 2e20 2246 6173   Rue, 2001. "Fas
+00011700: 7420 7361 6d70 6c69 6e67 206f 6620 4761  t sampling of Ga
+00011710: 7573 7369 616e 204d 6172 6b6f 7620 7261  ussian Markov ra
+00011720: 6e64 6f6d 2066 6965 6c64 732c 220a 2020  ndom fields,".  
+00011730: 2020 2020 2020 4a6f 7572 6e61 6c20 6f66        Journal of
+00011740: 2074 6865 2052 6f79 616c 2053 7461 7469   the Royal Stati
+00011750: 7374 6963 616c 2053 6f63 6965 7479 2053  stical Society S
+00011760: 6572 6965 7320 422c 2052 6f79 616c 2053  eries B, Royal S
+00011770: 7461 7469 7374 6963 616c 2053 6f63 6965  tatistical Socie
+00011780: 7479 2c0a 2020 2020 2020 2020 766f 6c2e  ty,.        vol.
+00011790: 2036 3328 3229 2c20 7061 6765 7320 3332   63(2), pages 32
+000117a0: 352d 3333 382e 2044 4f49 3a20 3130 2e31  5-338. DOI: 10.1
+000117b0: 3131 312f 3134 3637 2d39 3836 382e 3030  111/1467-9868.00
+000117c0: 3238 380a 2020 2020 2020 2020 2222 220a  288.        """.
+000117d0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+000117e0: 6369 7079 2e73 7061 7273 652e 6973 7370  cipy.sparse.issp
+000117f0: 6172 7365 2857 293a 0a20 2020 2020 2020  arse(W):.       
+00011800: 2020 2020 2057 203d 2073 6369 7079 2e73       W = scipy.s
+00011810: 7061 7273 652e 6373 725f 6d61 7472 6978  parse.csr_matrix
+00011820: 2857 290a 2020 2020 2020 2020 7320 3d20  (W).        s = 
+00011830: 6e70 2e61 7361 7272 6179 2857 2e73 756d  np.asarray(W.sum
+00011840: 2861 7869 733d 3029 295b 305d 0a20 2020  (axis=0))[0].   
+00011850: 2020 2020 2044 203d 2073 6369 7079 2e73       D = scipy.s
+00011860: 7061 7273 652e 6469 6167 7328 7329 0a20  parse.diags(s). 
+00011870: 2020 2020 2020 2074 6175 203d 2073 6369         tau = sci
+00011880: 7079 2e73 7061 7273 652e 6373 725f 6d61  py.sparse.csr_ma
+00011890: 7472 6978 2874 6175 290a 2020 2020 2020  trix(tau).      
+000118a0: 2020 616c 7068 6120 3d20 7363 6970 792e    alpha = scipy.
+000118b0: 7370 6172 7365 2e63 7372 5f6d 6174 7269  sparse.csr_matri
+000118c0: 7828 616c 7068 6129 0a0a 2020 2020 2020  x(alpha)..      
+000118d0: 2020 5120 3d20 7461 752e 6d75 6c74 6970    Q = tau.multip
+000118e0: 6c79 2844 202d 2061 6c70 6861 2e6d 756c  ly(D - alpha.mul
+000118f0: 7469 706c 7928 5729 290a 0a20 2020 2020  tiply(W))..     
+00011900: 2020 2070 6572 6d5f 6172 7261 7920 3d20     perm_array = 
+00011910: 7363 6970 792e 7370 6172 7365 2e63 7367  scipy.sparse.csg
+00011920: 7261 7068 2e72 6576 6572 7365 5f63 7574  raph.reverse_cut
+00011930: 6869 6c6c 5f6d 636b 6565 2851 2c20 7379  hill_mckee(Q, sy
+00011940: 6d6d 6574 7269 635f 6d6f 6465 3d54 7275  mmetric_mode=Tru
+00011950: 6529 0a20 2020 2020 2020 2069 6e76 5f70  e).        inv_p
+00011960: 6572 6d20 3d20 6e70 2e61 7267 736f 7274  erm = np.argsort
+00011970: 2870 6572 6d5f 6172 7261 7929 0a0a 2020  (perm_array)..  
+00011980: 2020 2020 2020 5120 3d20 515b 7065 726d        Q = Q[perm
+00011990: 5f61 7272 6179 2c20 3a5d 5b3a 2c20 7065  _array, :][:, pe
+000119a0: 726d 5f61 7272 6179 5d0a 0a20 2020 2020  rm_array]..     
+000119b0: 2020 2051 6220 3d20 512e 6469 6167 6f6e     Qb = Q.diagon
+000119c0: 616c 2829 0a20 2020 2020 2020 2075 203d  al().        u =
+000119d0: 2031 0a20 2020 2020 2020 2077 6869 6c65   1.        while
+000119e0: 206e 702e 636f 756e 745f 6e6f 6e7a 6572   np.count_nonzer
+000119f0: 6f28 512e 6469 6167 6f6e 616c 2875 2929  o(Q.diagonal(u))
+00011a00: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+00011a10: 2020 5162 203d 206e 702e 7673 7461 636b    Qb = np.vstack
+00011a20: 2828 6e70 2e70 6164 2851 2e64 6961 676f  ((np.pad(Q.diago
+00011a30: 6e61 6c28 7529 2c20 2875 2c20 3029 2c20  nal(u), (u, 0), 
+00011a40: 636f 6e73 7461 6e74 5f76 616c 7565 733d  constant_values=
+00011a50: 2830 2c20 3029 292c 2051 6229 290a 2020  (0, 0)), Qb)).  
+00011a60: 2020 2020 2020 2020 2020 7520 2b3d 2031            u += 1
+00011a70: 0a0a 2020 2020 2020 2020 4c20 3d20 7363  ..        L = sc
+00011a80: 6970 792e 6c69 6e61 6c67 2e63 686f 6c65  ipy.linalg.chole
+00011a90: 736b 795f 6261 6e64 6564 2851 622c 206c  sky_banded(Qb, l
+00011aa0: 6f77 6572 3d46 616c 7365 290a 0a20 2020  ower=False)..   
+00011ab0: 2020 2020 2073 697a 6520 3d20 7475 706c       size = tupl
+00011ac0: 6528 7369 7a65 206f 7220 2829 290a 2020  e(size or ()).  
+00011ad0: 2020 2020 2020 6966 2073 697a 653a 0a20        if size:. 
+00011ae0: 2020 2020 2020 2020 2020 206d 7520 3d20             mu = 
+00011af0: 6e70 2e62 726f 6164 6361 7374 5f74 6f28  np.broadcast_to(
+00011b00: 6d75 2c20 7369 7a65 202b 2028 6d75 2e73  mu, size + (mu.s
+00011b10: 6861 7065 5b2d 315d 2c29 290a 2020 2020  hape[-1],)).    
+00011b20: 2020 2020 7a20 3d20 726e 672e 6e6f 726d      z = rng.norm
+00011b30: 616c 2873 697a 653d 6d75 2e73 6861 7065  al(size=mu.shape
+00011b40: 290a 2020 2020 2020 2020 7361 6d70 6c65  ).        sample
+00011b50: 7320 3d20 6e70 2e65 6d70 7479 287a 2e73  s = np.empty(z.s
+00011b60: 6861 7065 290a 2020 2020 2020 2020 666f  hape).        fo
+00011b70: 7220 6964 7820 696e 206e 702e 6e64 696e  r idx in np.ndin
+00011b80: 6465 7828 6d75 2e73 6861 7065 5b3a 2d31  dex(mu.shape[:-1
+00011b90: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+00011ba0: 7361 6d70 6c65 735b 6964 785d 203d 2073  samples[idx] = s
+00011bb0: 6369 7079 2e6c 696e 616c 672e 6368 6f5f  cipy.linalg.cho_
+00011bc0: 736f 6c76 655f 6261 6e64 6564 2828 4c2c  solve_banded((L,
+00011bd0: 2046 616c 7365 292c 207a 5b69 6478 5d29   False), z[idx])
+00011be0: 202b 206d 755b 6964 785d 5b70 6572 6d5f   + mu[idx][perm_
+00011bf0: 6172 7261 795d 0a20 2020 2020 2020 2073  array].        s
+00011c00: 616d 706c 6573 203d 2073 616d 706c 6573  amples = samples
+00011c10: 5b2e 2e2e 2c20 696e 765f 7065 726d 5d0a  [..., inv_perm].
+00011c20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011c30: 616d 706c 6573 0a0a 0a63 6172 203d 2043  amples...car = C
+00011c40: 4152 5256 2829 0a0a 0a63 6c61 7373 2043  ARRV()...class C
+00011c50: 4152 2843 6f6e 7469 6e75 6f75 7329 3a0a  AR(Continuous):.
+00011c60: 2020 2020 7222 2222 0a20 2020 204c 696b      r""".    Lik
+00011c70: 656c 6968 6f6f 6420 666f 7220 6120 636f  elihood for a co
+00011c80: 6e64 6974 696f 6e61 6c20 6175 746f 7265  nditional autore
+00011c90: 6772 6573 7369 6f6e 2e20 5468 6973 2069  gression. This i
+00011ca0: 7320 6120 7370 6563 6961 6c20 6361 7365  s a special case
+00011cb0: 206f 6620 7468 650a 2020 2020 6d75 6c74   of the.    mult
+00011cc0: 6976 6172 6961 7465 206e 6f72 6d61 6c20  ivariate normal 
+00011cd0: 7769 7468 2061 6e20 6164 6a61 6365 6e63  with an adjacenc
+00011ce0: 792d 7374 7275 6374 7572 6564 2063 6f76  y-structured cov
+00011cf0: 6172 6961 6e63 6520 6d61 7472 6978 2e0a  ariance matrix..
+00011d00: 0a20 2020 202e 2e20 6d61 7468 3a3a 0a0a  .    .. math::..
+00011d10: 2020 2020 2020 2066 2878 205c 6d69 6420         f(x \mid 
+00011d20: 572c 205c 616c 7068 612c 205c 7461 7529  W, \alpha, \tau)
+00011d30: 203d 0a20 2020 2020 2020 2020 2020 5c66   =.           \f
+00011d40: 7261 637b 7c54 7c5e 7b31 2f32 7d7d 7b28  rac{|T|^{1/2}}{(
+00011d50: 325c 7069 295e 7b6b 2f32 7d7d 0a20 2020  2\pi)^{k/2}}.   
+00011d60: 2020 2020 2020 2020 5c65 7870 5c6c 6566          \exp\lef
+00011d70: 745c 7b20 2d5c 6672 6163 7b31 7d7b 327d  t\{ -\frac{1}{2}
+00011d80: 2028 782d 5c6d 7529 5e7b 5c70 7269 6d65   (x-\mu)^{\prime
+00011d90: 7d20 545e 7b2d 317d 2028 782d 5c6d 7529  } T^{-1} (x-\mu)
+00011da0: 205c 7269 6768 745c 7d0a 0a20 2020 2077   \right\}..    w
+00011db0: 6865 7265 203a 6d61 7468 3a60 5420 3d20  here :math:`T = 
+00011dc0: 285c 7461 7520 4428 492d 5c61 6c70 6861  (\tau D(I-\alpha
+00011dd0: 2057 2929 5e7b 2d31 7d60 2061 6e64 203a   W))^{-1}` and :
+00011de0: 6d61 7468 3a60 4420 3d20 6469 6167 285c  math:`D = diag(\
+00011df0: 7375 6d5f 6920 575f 7b69 6a7d 2960 2e0a  sum_i W_{ij})`..
+00011e00: 0a20 2020 203d 3d3d 3d3d 3d3d 3d20 203d  .    ========  =
+00011e10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011e20: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 5375  =========.    Su
+00011e30: 7070 6f72 7420 2020 3a6d 6174 683a 6078  pport   :math:`x
+00011e40: 205c 696e 205c 6d61 7468 6262 7b52 7d5e   \in \mathbb{R}^
+00011e50: 6b60 0a20 2020 204d 6561 6e20 2020 2020  k`.    Mean     
+00011e60: 203a 6d61 7468 3a60 5c6d 7520 5c69 6e20   :math:`\mu \in 
+00011e70: 5c6d 6174 6862 627b 527d 5e6b 600a 2020  \mathbb{R}^k`.  
+00011e80: 2020 5661 7269 616e 6365 2020 3a6d 6174    Variance  :mat
+00011e90: 683a 6028 5c74 6175 2044 2849 2d5c 616c  h:`(\tau D(I-\al
+00011ea0: 7068 6120 5729 295e 7b2d 317d 600a 2020  pha W))^{-1}`.  
+00011eb0: 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d    ========  ====
+00011ec0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011ed0: 3d3d 3d3d 3d3d 0a0a 2020 2020 5061 7261  ======..    Para
+00011ee0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00011ef0: 2d2d 2d2d 2d0a 2020 2020 6d75 203a 2074  -----.    mu : t
+00011f00: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
+00011f10: 6f61 740a 2020 2020 2020 2020 5265 616c  oat.        Real
+00011f20: 2d76 616c 7565 6420 6d65 616e 2076 6563  -valued mean vec
+00011f30: 746f 720a 2020 2020 5720 3a20 284d 2c20  tor.    W : (M, 
+00011f40: 4d29 2074 656e 736f 725f 6c69 6b65 206f  M) tensor_like o
+00011f50: 6620 696e 740a 2020 2020 2020 2020 5379  f int.        Sy
+00011f60: 6d6d 6574 7269 6320 6164 6a61 6365 6e63  mmetric adjacenc
+00011f70: 7920 6d61 7472 6978 206f 6620 3173 2061  y matrix of 1s a
+00011f80: 6e64 2030 7320 696e 6469 6361 7469 6e67  nd 0s indicating
+00011f90: 0a20 2020 2020 2020 2061 646a 6163 656e  .        adjacen
+00011fa0: 6379 2062 6574 7765 656e 2065 6c65 6d65  cy between eleme
+00011fb0: 6e74 732e 2049 6620 706f 7373 6962 6c65  nts. If possible
+00011fc0: 2c20 2a57 2a20 6973 2063 6f6e 7665 7274  , *W* is convert
+00011fd0: 6564 0a20 2020 2020 2020 2074 6f20 6120  ed.        to a 
+00011fe0: 7370 6172 7365 206d 6174 7269 782c 2066  sparse matrix, f
+00011ff0: 616c 6c69 6e67 2062 6163 6b20 746f 2061  alling back to a
+00012000: 2064 656e 7365 2076 6172 6961 626c 652e   dense variable.
+00012010: 0a20 2020 2020 2020 203a 6675 6e63 3a60  .        :func:`
+00012020: 7e70 7974 656e 736f 722e 7370 6172 7365  ~pytensor.sparse
+00012030: 2e62 6173 6963 2e61 735f 7370 6172 7365  .basic.as_sparse
+00012040: 5f6f 725f 7465 6e73 6f72 5f76 6172 6961  _or_tensor_varia
+00012050: 626c 6560 2069 730a 2020 2020 2020 2020  ble` is.        
+00012060: 7573 6564 2066 6f72 2074 6869 7320 7370  used for this sp
+00012070: 6172 7365 206f 7220 7465 6e73 6f72 7661  arse or tensorva
+00012080: 7269 6162 6c65 2063 6f6e 7665 7273 696f  riable conversio
+00012090: 6e2e 0a20 2020 2061 6c70 6861 203a 2074  n..    alpha : t
+000120a0: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
+000120b0: 6f61 740a 2020 2020 2020 2020 4175 746f  oat.        Auto
+000120c0: 7265 6772 6573 7369 6f6e 2070 6172 616d  regression param
+000120d0: 6574 6572 2074 616b 696e 6720 7661 6c75  eter taking valu
+000120e0: 6573 2062 6574 7765 656e 202d 3120 616e  es between -1 an
+000120f0: 6420 312e 2056 616c 7565 7320 636c 6f73  d 1. Values clos
+00012100: 6572 2074 6f20 3020 696e 6469 6361 7465  er to 0 indicate
+00012110: 2077 6561 6b65 720a 2020 2020 2020 2020   weaker.        
+00012120: 636f 7272 656c 6174 696f 6e20 616e 6420  correlation and 
+00012130: 7661 6c75 6573 2063 6c6f 7365 7220 746f  values closer to
+00012140: 2031 2069 6e64 6963 6174 6520 6869 6768   1 indicate high
+00012150: 6572 2061 7574 6f63 6f72 7265 6c61 7469  er autocorrelati
+00012160: 6f6e 2e20 466f 7220 6d6f 7374 2075 7365  on. For most use
+00012170: 2063 6173 6573 2c20 7468 650a 2020 2020   cases, the.    
+00012180: 2020 2020 7375 7070 6f72 7420 6f66 2061      support of a
+00012190: 6c70 6861 2073 686f 756c 6420 6265 2072  lpha should be r
+000121a0: 6573 7472 6963 7465 6420 746f 2028 302c  estricted to (0,
+000121b0: 2031 292e 0a20 2020 2074 6175 203a 2074   1)..    tau : t
+000121c0: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
+000121d0: 6f61 740a 2020 2020 2020 2020 506f 7369  oat.        Posi
+000121e0: 7469 7665 2070 7265 6369 7369 6f6e 2076  tive precision v
+000121f0: 6172 6961 626c 6520 636f 6e74 726f 6c6c  ariable controll
+00012200: 696e 6720 7468 6520 7363 616c 6520 6f66  ing the scale of
+00012210: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
+00012220: 6e6f 726d 616c 2076 6172 6961 7465 732e  normal variates.
+00012230: 0a0a 2020 2020 5265 6665 7265 6e63 6573  ..    References
+00012240: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00012250: 2020 2020 2e2e 2020 4a69 6e2c 2058 2e2c      ..  Jin, X.,
+00012260: 2043 6172 6c69 6e2c 2042 2e2c 2042 616e   Carlin, B., Ban
+00012270: 6572 6a65 652c 2053 2e0a 2020 2020 2020  erjee, S..      
+00012280: 2020 2247 656e 6572 616c 697a 6564 2048    "Generalized H
+00012290: 6965 7261 7263 6869 6361 6c20 4d75 6c74  ierarchical Mult
+000122a0: 6976 6172 6961 7465 2043 4152 204d 6f64  ivariate CAR Mod
+000122b0: 656c 7320 666f 7220 4172 6561 6c20 4461  els for Areal Da
+000122c0: 7461 220a 2020 2020 2020 2020 4269 6f6d  ta".        Biom
+000122d0: 6574 7269 6373 2c20 566f 6c2e 2036 312c  etrics, Vol. 61,
+000122e0: 204e 6f2e 2034 2028 4465 632e 2c20 3230   No. 4 (Dec., 20
+000122f0: 3035 292c 2070 702e 2039 3530 2d39 3631  05), pp. 950-961
+00012300: 0a20 2020 2022 2222 0a20 2020 2072 765f  .    """.    rv_
+00012310: 6f70 203d 2063 6172 0a0a 2020 2020 4063  op = car..    @c
+00012320: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00012330: 6566 2064 6973 7428 636c 732c 206d 752c  ef dist(cls, mu,
+00012340: 2057 2c20 616c 7068 612c 2074 6175 2c20   W, alpha, tau, 
+00012350: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00012360: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00012370: 2073 7570 6572 2829 2e64 6973 7428 5b6d   super().dist([m
+00012380: 752c 2057 2c20 616c 7068 612c 2074 6175  u, W, alpha, tau
+00012390: 5d2c 202a 2a6b 7761 7267 7329 0a0a 2020  ], **kwargs)..  
+000123a0: 2020 6465 6620 6d6f 6d65 6e74 2872 762c    def moment(rv,
+000123b0: 2073 697a 652c 206d 752c 2057 2c20 616c   size, mu, W, al
+000123c0: 7068 612c 2074 6175 293a 0a20 2020 2020  pha, tau):.     
+000123d0: 2020 2072 6574 7572 6e20 7074 2e66 756c     return pt.ful
+000123e0: 6c5f 6c69 6b65 2872 762c 206d 7529 0a0a  l_like(rv, mu)..
+000123f0: 2020 2020 6465 6620 6c6f 6770 2876 616c      def logp(val
+00012400: 7565 2c20 6d75 2c20 572c 2061 6c70 6861  ue, mu, W, alpha
+00012410: 2c20 7461 7529 3a0a 2020 2020 2020 2020  , tau):.        
+00012420: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
+00012430: 756c 6174 6520 6c6f 672d 7072 6f62 6162  ulate log-probab
+00012440: 696c 6974 7920 6f66 2061 2043 4152 2d64  ility of a CAR-d
+00012450: 6973 7472 6962 7574 6564 2076 6563 746f  istributed vecto
+00012460: 720a 2020 2020 2020 2020 6174 2073 7065  r.        at spe
+00012470: 6369 6669 6564 2076 616c 7565 2e20 5468  cified value. Th
+00012480: 6973 206c 6f67 2070 726f 6261 6269 6c69  is log probabili
+00012490: 7479 2066 756e 6374 696f 6e20 6469 6666  ty function diff
+000124a0: 6572 7320 6672 6f6d 0a20 2020 2020 2020  ers from.       
+000124b0: 2074 6865 2074 7275 6520 4341 5220 6c6f   the true CAR lo
+000124c0: 6720 6465 6e73 6974 7920 2841 4b41 2061  g density (AKA a
+000124d0: 206d 756c 7469 7661 7269 6174 6520 6e6f   multivariate no
+000124e0: 726d 616c 2077 6974 6820 4341 522d 7374  rmal with CAR-st
+000124f0: 7275 6374 7572 6564 0a20 2020 2020 2020  ructured.       
+00012500: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
+00012510: 6978 2920 6279 2061 6e20 6164 6469 7469  ix) by an additi
+00012520: 7665 2063 6f6e 7374 616e 742e 0a0a 2020  ve constant...  
+00012530: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00012540: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00012550: 2d2d 2d0a 2020 2020 2020 2020 7661 6c75  ---.        valu
+00012560: 653a 2061 7272 6179 0a20 2020 2020 2020  e: array.       
+00012570: 2020 2020 2056 616c 7565 2066 6f72 2077       Value for w
+00012580: 6869 6368 206c 6f67 2d70 726f 6261 6269  hich log-probabi
+00012590: 6c69 7479 2069 7320 6361 6c63 756c 6174  lity is calculat
+000125a0: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+000125b0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+000125c0: 2d2d 2d2d 0a20 2020 2020 2020 2054 656e  ----.        Ten
+000125d0: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
+000125e0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+000125f0: 2073 7061 7273 6520 3d20 6973 696e 7374   sparse = isinst
+00012600: 616e 6365 2857 2c20 2870 7974 656e 736f  ance(W, (pytenso
+00012610: 722e 7370 6172 7365 2e53 7061 7273 6543  r.sparse.SparseC
+00012620: 6f6e 7374 616e 742c 2070 7974 656e 736f  onstant, pytenso
+00012630: 722e 7370 6172 7365 2e53 7061 7273 6556  r.sparse.SparseV
+00012640: 6172 6961 626c 6529 290a 0a20 2020 2020  ariable))..     
+00012650: 2020 2069 6620 7370 6172 7365 3a0a 2020     if sparse:.  
+00012660: 2020 2020 2020 2020 2020 4420 3d20 7370            D = sp
+00012670: 5f73 756d 2857 2c20 6178 6973 3d30 290a  _sum(W, axis=0).
+00012680: 2020 2020 2020 2020 2020 2020 4469 6e76              Dinv
+00012690: 5f73 7172 7420 3d20 7074 2e64 6961 6728  _sqrt = pt.diag(
+000126a0: 3120 2f20 7074 2e73 7172 7428 4429 290a  1 / pt.sqrt(D)).
+000126b0: 2020 2020 2020 2020 2020 2020 4457 4420              DWD 
+000126c0: 3d20 7074 2e64 6f74 2870 7974 656e 736f  = pt.dot(pytenso
+000126d0: 722e 7370 6172 7365 2e64 6f74 2844 696e  r.sparse.dot(Din
+000126e0: 765f 7371 7274 2c20 5729 2c20 4469 6e76  v_sqrt, W), Dinv
+000126f0: 5f73 7172 7429 0a20 2020 2020 2020 2065  _sqrt).        e
+00012700: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00012710: 2044 203d 2057 2e73 756d 2861 7869 733d   D = W.sum(axis=
+00012720: 3029 0a20 2020 2020 2020 2020 2020 2044  0).            D
+00012730: 696e 765f 7371 7274 203d 2070 742e 6469  inv_sqrt = pt.di
+00012740: 6167 2831 202f 2070 742e 7371 7274 2844  ag(1 / pt.sqrt(D
+00012750: 2929 0a20 2020 2020 2020 2020 2020 2044  )).            D
+00012760: 5744 203d 2070 742e 646f 7428 7074 2e64  WD = pt.dot(pt.d
+00012770: 6f74 2844 696e 765f 7371 7274 2c20 5729  ot(Dinv_sqrt, W)
+00012780: 2c20 4469 6e76 5f73 7172 7429 0a20 2020  , Dinv_sqrt).   
+00012790: 2020 2020 206c 616d 203d 2070 742e 736c       lam = pt.sl
+000127a0: 696e 616c 672e 6569 6776 616c 7368 2844  inalg.eigvalsh(D
+000127b0: 5744 2c20 7074 2e65 7965 2844 5744 2e73  WD, pt.eye(DWD.s
+000127c0: 6861 7065 5b30 5d29 290a 0a20 2020 2020  hape[0]))..     
+000127d0: 2020 2064 2c20 5f20 3d20 572e 7368 6170     d, _ = W.shap
+000127e0: 650a 0a20 2020 2020 2020 2069 6620 7661  e..        if va
+000127f0: 6c75 652e 6e64 696d 203d 3d20 313a 0a20  lue.ndim == 1:. 
+00012800: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00012810: 203d 2076 616c 7565 5b4e 6f6e 652c 203a   = value[None, :
+00012820: 5d0a 0a20 2020 2020 2020 206c 6f67 7461  ]..        logta
+00012830: 7520 3d20 6420 2a20 7074 2e6c 6f67 2874  u = d * pt.log(t
+00012840: 6175 292e 7375 6d28 290a 2020 2020 2020  au).sum().      
+00012850: 2020 6c6f 6764 6574 203d 2070 742e 6c6f    logdet = pt.lo
+00012860: 6728 3120 2d20 616c 7068 612e 5420 2a20  g(1 - alpha.T * 
+00012870: 6c61 6d5b 3a2c 204e 6f6e 655d 292e 7375  lam[:, None]).su
+00012880: 6d28 290a 2020 2020 2020 2020 6465 6c74  m().        delt
+00012890: 6120 3d20 7661 6c75 6520 2d20 6d75 0a0a  a = value - mu..
+000128a0: 2020 2020 2020 2020 6966 2073 7061 7273          if spars
+000128b0: 653a 0a20 2020 2020 2020 2020 2020 2057  e:.            W
+000128c0: 6465 6c74 6120 3d20 7079 7465 6e73 6f72  delta = pytensor
+000128d0: 2e73 7061 7273 652e 646f 7428 6465 6c74  .sparse.dot(delt
+000128e0: 612c 2057 290a 2020 2020 2020 2020 656c  a, W).        el
+000128f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012900: 5764 656c 7461 203d 2070 742e 646f 7428  Wdelta = pt.dot(
+00012910: 6465 6c74 612c 2057 290a 0a20 2020 2020  delta, W)..     
+00012920: 2020 2074 6175 5f64 6f74 5f64 656c 7461     tau_dot_delta
+00012930: 203d 2044 5b4e 6f6e 652c 203a 5d20 2a20   = D[None, :] * 
+00012940: 6465 6c74 6120 2d20 616c 7068 6120 2a20  delta - alpha * 
+00012950: 5764 656c 7461 0a20 2020 2020 2020 206c  Wdelta.        l
+00012960: 6f67 7175 6164 203d 2028 7461 7520 2a20  ogquad = (tau * 
+00012970: 6465 6c74 6120 2a20 7461 755f 646f 745f  delta * tau_dot_
+00012980: 6465 6c74 6129 2e73 756d 2861 7869 733d  delta).sum(axis=
+00012990: 2d31 290a 2020 2020 2020 2020 7265 7475  -1).        retu
+000129a0: 726e 2063 6865 636b 5f70 6172 616d 6574  rn check_paramet
+000129b0: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
+000129c0: 2030 2e35 202a 2028 6c6f 6774 6175 202b   0.5 * (logtau +
+000129d0: 206c 6f67 6465 7420 2d20 6c6f 6771 7561   logdet - logqua
+000129e0: 6429 2c0a 2020 2020 2020 2020 2020 2020  d),.            
+000129f0: 2d31 203c 3d20 616c 7068 612c 0a20 2020  -1 <= alpha,.   
+00012a00: 2020 2020 2020 2020 2061 6c70 6861 203c           alpha <
+00012a10: 3d20 312c 0a20 2020 2020 2020 2020 2020  = 1,.           
+00012a20: 2074 6175 203e 2030 2c0a 2020 2020 2020   tau > 0,.      
+00012a30: 2020 2020 2020 6d73 673d 222d 3120 3c3d        msg="-1 <=
+00012a40: 2061 6c70 6861 203c 3d20 312c 2074 6175   alpha <= 1, tau
+00012a50: 203e 2030 222c 0a20 2020 2020 2020 2029   > 0",.        )
+00012a60: 0a0a 0a63 6c61 7373 2053 7469 636b 4272  ...class StickBr
+00012a70: 6561 6b69 6e67 5765 6967 6874 7352 5628  eakingWeightsRV(
+00012a80: 5261 6e64 6f6d 5661 7269 6162 6c65 293a  RandomVariable):
+00012a90: 0a20 2020 206e 616d 6520 3d20 2273 7469  .    name = "sti
+00012aa0: 636b 5f62 7265 616b 696e 675f 7765 6967  ck_breaking_weig
+00012ab0: 6874 7322 0a20 2020 206e 6469 6d5f 7375  hts".    ndim_su
+00012ac0: 7070 203d 2031 0a20 2020 206e 6469 6d73  pp = 1.    ndims
+00012ad0: 5f70 6172 616d 7320 3d20 5b30 2c20 305d  _params = [0, 0]
+00012ae0: 0a20 2020 2064 7479 7065 203d 2022 666c  .    dtype = "fl
+00012af0: 6f61 7458 220a 2020 2020 5f70 7269 6e74  oatX".    _print
+00012b00: 5f6e 616d 6520 3d20 2822 5374 6963 6b42  _name = ("StickB
+00012b10: 7265 616b 696e 6757 6569 6768 7473 222c  reakingWeights",
+00012b20: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
+00012b30: 7b53 7469 636b 4272 6561 6b69 6e67 5765  {StickBreakingWe
+00012b40: 6967 6874 737d 2229 0a0a 2020 2020 6465  ights}")..    de
+00012b50: 6620 6d61 6b65 5f6e 6f64 6528 7365 6c66  f make_node(self
+00012b60: 2c20 726e 672c 2073 697a 652c 2064 7479  , rng, size, dty
+00012b70: 7065 2c20 616c 7068 612c 204b 293a 0a20  pe, alpha, K):. 
+00012b80: 2020 2020 2020 2061 6c70 6861 203d 2070         alpha = p
+00012b90: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00012ba0: 6162 6c65 2861 6c70 6861 290a 2020 2020  able(alpha).    
+00012bb0: 2020 2020 4b20 3d20 7074 2e61 735f 7465      K = pt.as_te
+00012bc0: 6e73 6f72 5f76 6172 6961 626c 6528 696e  nsor_variable(in
+00012bd0: 7458 284b 2929 0a0a 2020 2020 2020 2020  tX(K))..        
+00012be0: 6966 204b 2e6e 6469 6d20 3e20 303a 0a20  if K.ndim > 0:. 
+00012bf0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00012c00: 2056 616c 7565 4572 726f 7228 224b 206d   ValueError("K m
+00012c10: 7573 7420 6265 2061 2073 6361 6c61 722e  ust be a scalar.
+00012c20: 2229 0a0a 2020 2020 2020 2020 7265 7475  ")..        retu
+00012c30: 726e 2073 7570 6572 2829 2e6d 616b 655f  rn super().make_
+00012c40: 6e6f 6465 2872 6e67 2c20 7369 7a65 2c20  node(rng, size, 
+00012c50: 6474 7970 652c 2061 6c70 6861 2c20 4b29  dtype, alpha, K)
+00012c60: 0a0a 2020 2020 6465 6620 5f73 7570 705f  ..    def _supp_
+00012c70: 7368 6170 655f 6672 6f6d 5f70 6172 616d  shape_from_param
+00012c80: 7328 7365 6c66 2c20 6469 7374 5f70 6172  s(self, dist_par
+00012c90: 616d 732c 202a 2a6b 7761 7267 7329 3a0a  ams, **kwargs):.
+00012ca0: 2020 2020 2020 2020 4b20 3d20 6469 7374          K = dist
+00012cb0: 5f70 6172 616d 735b 315d 0a20 2020 2020  _params[1].     
+00012cc0: 2020 2072 6574 7572 6e20 284b 202b 2031     return (K + 1
+00012cd0: 2c29 0a0a 2020 2020 4063 6c61 7373 6d65  ,)..    @classme
+00012ce0: 7468 6f64 0a20 2020 2064 6566 2072 6e67  thod.    def rng
+00012cf0: 5f66 6e28 636c 732c 2072 6e67 2c20 616c  _fn(cls, rng, al
+00012d00: 7068 612c 204b 2c20 7369 7a65 293a 0a20  pha, K, size):. 
+00012d10: 2020 2020 2020 2069 6620 4b20 3c20 303a         if K < 0:
+00012d20: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00012d30: 7365 2056 616c 7565 4572 726f 7228 224b  se ValueError("K
+00012d40: 206e 6565 6473 2074 6f20 6265 2070 6f73   needs to be pos
+00012d50: 6974 6976 652e 2229 0a0a 2020 2020 2020  itive.")..      
+00012d60: 2020 7369 7a65 203d 2074 6f5f 7475 706c    size = to_tupl
+00012d70: 6528 7369 7a65 2920 6966 2073 697a 6520  e(size) if size 
+00012d80: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
+00012d90: 2061 6c70 6861 2e73 6861 7065 0a20 2020   alpha.shape.   
+00012da0: 2020 2020 2073 697a 6520 3d20 7369 7a65       size = size
+00012db0: 202b 2028 4b2c 290a 2020 2020 2020 2020   + (K,).        
+00012dc0: 616c 7068 6120 3d20 616c 7068 615b 2e2e  alpha = alpha[..
+00012dd0: 2e2c 206e 702e 6e65 7761 7869 735d 0a0a  ., np.newaxis]..
+00012de0: 2020 2020 2020 2020 6265 7461 7320 3d20          betas = 
+00012df0: 726e 672e 6265 7461 2831 2c20 616c 7068  rng.beta(1, alph
+00012e00: 612c 2073 697a 653d 7369 7a65 290a 0a20  a, size=size).. 
+00012e10: 2020 2020 2020 2073 7469 636b 7320 3d20         sticks = 
+00012e20: 6e70 2e63 6f6e 6361 7465 6e61 7465 280a  np.concatenate(.
+00012e30: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
+00012e40: 2020 2020 2020 2020 2020 2020 2020 6e70                np
+00012e50: 2e6f 6e65 7328 7368 6170 653d 2873 697a  .ones(shape=(siz
+00012e60: 655b 3a2d 315d 202b 2028 312c 2929 292c  e[:-1] + (1,))),
+00012e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012e80: 206e 702e 6375 6d70 726f 6428 3120 2d20   np.cumprod(1 - 
+00012e90: 6265 7461 735b 2e2e 2e2c 203a 2d31 5d2c  betas[..., :-1],
+00012ea0: 2061 7869 733d 2d31 292c 0a20 2020 2020   axis=-1),.     
+00012eb0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00012ec0: 2020 2020 2020 6178 6973 3d2d 312c 0a20        axis=-1,. 
+00012ed0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00012ee0: 2020 7765 6967 6874 7320 3d20 7374 6963    weights = stic
+00012ef0: 6b73 202a 2062 6574 6173 0a20 2020 2020  ks * betas.     
+00012f00: 2020 2077 6569 6768 7473 203d 206e 702e     weights = np.
+00012f10: 636f 6e63 6174 656e 6174 6528 0a20 2020  concatenate(.   
+00012f20: 2020 2020 2020 2020 2028 7765 6967 6874           (weight
+00012f30: 732c 2031 202d 2077 6569 6768 7473 2e73  s, 1 - weights.s
+00012f40: 756d 2861 7869 733d 2d31 295b 2e2e 2e2c  um(axis=-1)[...,
+00012f50: 206e 702e 6e65 7761 7869 735d 292c 0a20   np.newaxis]),. 
+00012f60: 2020 2020 2020 2020 2020 2061 7869 733d             axis=
+00012f70: 2d31 2c0a 2020 2020 2020 2020 290a 0a20  -1,.        ).. 
+00012f80: 2020 2020 2020 2072 6574 7572 6e20 7765         return we
+00012f90: 6967 6874 730a 0a0a 7374 6963 6b62 7265  ights...stickbre
+00012fa0: 616b 696e 6777 6569 6768 7473 203d 2053  akingweights = S
+00012fb0: 7469 636b 4272 6561 6b69 6e67 5765 6967  tickBreakingWeig
+00012fc0: 6874 7352 5628 290a 0a0a 636c 6173 7320  htsRV()...class 
+00012fd0: 5374 6963 6b42 7265 616b 696e 6757 6569  StickBreakingWei
+00012fe0: 6768 7473 2853 696d 706c 6578 436f 6e74  ghts(SimplexCont
+00012ff0: 696e 756f 7573 293a 0a20 2020 2072 2222  inuous):.    r""
+00013000: 220a 2020 2020 4c69 6b65 6c69 686f 6f64  ".    Likelihood
+00013010: 206f 6620 7472 756e 6361 7465 6420 7374   of truncated st
+00013020: 6963 6b2d 6272 6561 6b69 6e67 2077 6569  ick-breaking wei
+00013030: 6768 7473 2e20 5468 6520 7765 6967 6874  ghts. The weight
+00013040: 7320 6172 6520 6765 6e65 7261 7465 6420  s are generated 
+00013050: 6672 6f6d 2061 0a20 2020 2073 7469 636b  from a.    stick
+00013060: 2d62 7265 616b 696e 6720 7072 6f63 6564  -breaking proced
+00013070: 7563 6520 7768 6572 6520 3a6d 6174 683a  uce where :math:
+00013080: 6078 5f6b 203d 2076 5f6b 205c 7072 6f64  `x_k = v_k \prod
+00013090: 5f7b 5c65 6c6c 203c 206b 7d20 2831 202d  _{\ell < k} (1 -
+000130a0: 2076 5f5c 656c 6c29 6020 666f 720a 2020   v_\ell)` for.  
+000130b0: 2020 3a6d 6174 683a 606b 205c 696e 205c    :math:`k \in \
+000130c0: 7b31 2c20 5c6c 646f 7473 2c20 4b5c 7d60  {1, \ldots, K\}`
+000130d0: 2061 6e64 203a 6d61 7468 3a60 785f 4b20   and :math:`x_K 
+000130e0: 3d20 5c70 726f 645f 7b5c 656c 6c20 3d20  = \prod_{\ell = 
+000130f0: 317d 5e7b 4b7d 2028 3120 2d20 765f 5c65  1}^{K} (1 - v_\e
+00013100: 6c6c 2920 3d20 3120 2d20 5c73 756d 5f7b  ll) = 1 - \sum_{
+00013110: 5c65 6c6c 3d31 7d5e 4b20 785f 5c65 6c6c  \ell=1}^K x_\ell
+00013120: 600a 2020 2020 7769 7468 203a 6d61 7468  `.    with :math
+00013130: 3a60 765f 6b20 5c73 7461 636b 7265 6c7b  :`v_k \stackrel{
+00013140: 5c74 6578 747b 692e 692e 642e 7d7d 7b5c  \text{i.i.d.}}{\
+00013150: 7369 6d7d 205c 7465 7874 7b42 6574 617d  sim} \text{Beta}
+00013160: 2831 2c20 5c61 6c70 6861 2960 2e0a 0a20  (1, \alpha)`... 
+00013170: 2020 202e 2e20 6d61 7468 3a0a 0a20 2020     .. math:..   
+00013180: 2020 2020 2066 285c 6d61 7468 6266 7b78       f(\mathbf{x
+00013190: 7d7c 5c61 6c70 6861 2c20 4b29 203d 0a20  }|\alpha, K) =. 
+000131a0: 2020 2020 2020 2020 2020 2042 2831 2c20             B(1, 
+000131b0: 5c61 6c70 6861 295e 7b2d 4b7d 785f 7b4b  \alpha)^{-K}x_{K
+000131c0: 2b31 7d5e 5c61 6c70 6861 205c 7072 6f64  +1}^\alpha \prod
+000131d0: 5f7b 6b3d 317d 5e7b 4b2b 317d 5c6c 6566  _{k=1}^{K+1}\lef
+000131e0: 745c 7b5c 7375 6d5f 7b6a 3d6b 7d5e 7b4b  t\{\sum_{j=k}^{K
+000131f0: 2b31 7d20 785f 6a5c 7269 6768 745c 7d5e  +1} x_j\right\}^
+00013200: 7b2d 317d 0a0a 2020 2020 3d3d 3d3d 3d3d  {-1}..    ======
+00013210: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
 00013220: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00013230: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00013240: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
-00013250: 2020 2053 7570 706f 7274 2020 203a 6d61     Support   :ma
-00013260: 7468 3a60 785f 6b20 5c69 6e20 2830 2c20  th:`x_k \in (0, 
-00013270: 3129 6020 666f 7220 3a6d 6174 683a 606b  1)` for :math:`k
-00013280: 205c 696e 205c 7b31 2c20 5c6c 646f 7473   \in \{1, \ldots
-00013290: 2c20 4b2b 315c 7d60 0a20 2020 2020 2020  , K+1\}`.       
-000132a0: 2020 2020 2020 2073 7563 6820 7468 6174         such that
-000132b0: 203a 6d61 7468 3a60 5c73 756d 2078 5f6b   :math:`\sum x_k
-000132c0: 203d 2031 600a 2020 2020 4d65 616e 2020   = 1`.    Mean  
-000132d0: 2020 2020 3a6d 6174 683a 605c 6d61 7468      :math:`\math
-000132e0: 6262 7b45 7d5b 785f 6b5d 203d 205c 6466  bb{E}[x_k] = \df
-000132f0: 7261 637b 317d 7b31 202b 205c 616c 7068  rac{1}{1 + \alph
-00013300: 617d 5c6c 6566 7428 5c64 6672 6163 7b5c  a}\left(\dfrac{\
-00013310: 616c 7068 617d 7b31 202b 205c 616c 7068  alpha}{1 + \alph
-00013320: 617d 5c72 6967 6874 295e 7b6b 202d 2031  a}\right)^{k - 1
-00013330: 7d60 0a20 2020 2020 2020 2020 2020 2020  }`.             
-00013340: 2066 6f72 203a 6d61 7468 3a60 6b20 5c69   for :math:`k \i
-00013350: 6e20 5c7b 312c 205c 6c64 6f74 732c 204b  n \{1, \ldots, K
-00013360: 5c7d 6020 616e 6420 3a6d 6174 683a 605c  \}` and :math:`\
-00013370: 6d61 7468 6262 7b45 7d5b 785f 7b4b 2b31  mathbb{E}[x_{K+1
-00013380: 7d5d 203d 205c 6c65 6674 285c 6466 7261  }] = \left(\dfra
-00013390: 637b 5c61 6c70 6861 7d7b 3120 2b20 5c61  c{\alpha}{1 + \a
-000133a0: 6c70 6861 7d5c 7269 6768 7429 5e7b 4b7d  lpha}\right)^{K}
-000133b0: 600a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  `.    ========  
+00013240: 3d3d 3d0a 2020 2020 5375 7070 6f72 7420  ===.    Support 
+00013250: 2020 3a6d 6174 683a 6078 5f6b 205c 696e    :math:`x_k \in
+00013260: 2028 302c 2031 2960 2066 6f72 203a 6d61   (0, 1)` for :ma
+00013270: 7468 3a60 6b20 5c69 6e20 5c7b 312c 205c  th:`k \in \{1, \
+00013280: 6c64 6f74 732c 204b 2b31 5c7d 600a 2020  ldots, K+1\}`.  
+00013290: 2020 2020 2020 2020 2020 2020 7375 6368              such
+000132a0: 2074 6861 7420 3a6d 6174 683a 605c 7375   that :math:`\su
+000132b0: 6d20 785f 6b20 3d20 3160 0a20 2020 204d  m x_k = 1`.    M
+000132c0: 6561 6e20 2020 2020 203a 6d61 7468 3a60  ean      :math:`
+000132d0: 5c6d 6174 6862 627b 457d 5b78 5f6b 5d20  \mathbb{E}[x_k] 
+000132e0: 3d20 5c64 6672 6163 7b31 7d7b 3120 2b20  = \dfrac{1}{1 + 
+000132f0: 5c61 6c70 6861 7d5c 6c65 6674 285c 6466  \alpha}\left(\df
+00013300: 7261 637b 5c61 6c70 6861 7d7b 3120 2b20  rac{\alpha}{1 + 
+00013310: 5c61 6c70 6861 7d5c 7269 6768 7429 5e7b  \alpha}\right)^{
+00013320: 6b20 2d20 317d 600a 2020 2020 2020 2020  k - 1}`.        
+00013330: 2020 2020 2020 666f 7220 3a6d 6174 683a        for :math:
+00013340: 606b 205c 696e 205c 7b31 2c20 5c6c 646f  `k \in \{1, \ldo
+00013350: 7473 2c20 4b5c 7d60 2061 6e64 203a 6d61  ts, K\}` and :ma
+00013360: 7468 3a60 5c6d 6174 6862 627b 457d 5b78  th:`\mathbb{E}[x
+00013370: 5f7b 4b2b 317d 5d20 3d20 5c6c 6566 7428  _{K+1}] = \left(
+00013380: 5c64 6672 6163 7b5c 616c 7068 617d 7b31  \dfrac{\alpha}{1
+00013390: 202b 205c 616c 7068 617d 5c72 6967 6874   + \alpha}\right
+000133a0: 295e 7b4b 7d60 0a20 2020 203d 3d3d 3d3d  )^{K}`.    =====
+000133b0: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
 000133c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000133d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000133e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-000133f0: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
-00013400: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-00013410: 2020 2061 6c70 6861 203a 2074 656e 736f     alpha : tenso
-00013420: 725f 6c69 6b65 206f 6620 666c 6f61 740a  r_like of float.
-00013430: 2020 2020 2020 2020 436f 6e63 656e 7472          Concentr
-00013440: 6174 696f 6e20 7061 7261 6d65 7465 7220  ation parameter 
-00013450: 2861 6c70 6861 203e 2030 292e 0a20 2020  (alpha > 0)..   
-00013460: 204b 203a 2074 656e 736f 725f 6c69 6b65   K : tensor_like
-00013470: 206f 6620 696e 740a 2020 2020 2020 2020   of int.        
-00013480: 5468 6520 6e75 6d62 6572 206f 6620 2273  The number of "s
-00013490: 7469 636b 7322 2074 6f20 6272 6561 6b20  ticks" to break 
-000134a0: 6f66 6620 6672 6f6d 2061 6e20 696e 6974  off from an init
-000134b0: 6961 6c20 6f6e 652d 756e 6974 2073 7469  ial one-unit sti
-000134c0: 636b 2e20 5468 6520 6c65 6e67 7468 206f  ck. The length o
-000134d0: 6620 7468 6520 7765 6967 6874 0a20 2020  f the weight.   
-000134e0: 2020 2020 2076 6563 746f 7220 6973 204b       vector is K
-000134f0: 202b 2031 2c20 7768 6572 6520 7468 6520   + 1, where the 
-00013500: 6c61 7374 2077 6569 6768 7420 6973 206f  last weight is o
-00013510: 6e65 206d 696e 7573 2074 6865 2073 756d  ne minus the sum
-00013520: 206f 6620 616c 6c20 7468 6520 6669 7273   of all the firs
-00013530: 7420 7374 6963 6b73 2e0a 0a20 2020 2052  t sticks...    R
-00013540: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
-00013550: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e 2e20  --------.    .. 
-00013560: 5b31 5d20 4973 6877 6172 616e 2c20 482e  [1] Ishwaran, H.
-00013570: 2c20 2620 4a61 6d65 732c 204c 2e20 462e  , & James, L. F.
-00013580: 2028 3230 3031 292e 2047 6962 6273 2073   (2001). Gibbs s
-00013590: 616d 706c 696e 6720 6d65 7468 6f64 7320  ampling methods 
-000135a0: 666f 7220 7374 6963 6b2d 6272 6561 6b69  for stick-breaki
-000135b0: 6e67 2070 7269 6f72 732e 0a20 2020 2020  ng priors..     
-000135c0: 2020 2020 2020 4a6f 7572 6e61 6c20 6f66        Journal of
-000135d0: 2074 6865 2041 6d65 7269 6361 6e20 5374   the American St
-000135e0: 6174 6973 7469 6361 6c20 4173 736f 6369  atistical Associ
-000135f0: 6174 696f 6e2c 2039 3628 3435 3329 2c20  ation, 96(453), 
-00013600: 3136 312d 3137 332e 0a0a 2020 2020 2e2e  161-173...    ..
-00013610: 205b 325d 204d c3bc 6c6c 6572 2c20 502e   [2] M..ller, P.
-00013620: 2c20 5175 696e 7461 6e61 2c20 462e 2041  , Quintana, F. A
-00013630: 2e2c 204a 6172 612c 2041 2e2c 2026 2048  ., Jara, A., & H
-00013640: 616e 736f 6e2c 2054 2e20 2832 3031 3529  anson, T. (2015)
-00013650: 2e20 4261 7965 7369 616e 206e 6f6e 7061  . Bayesian nonpa
-00013660: 7261 6d65 7472 6963 2064 6174 610a 2020  rametric data.  
-00013670: 2020 2020 2020 2020 2061 6e61 6c79 7369           analysi
-00013680: 732e 204e 6577 2059 6f72 6b3a 2053 7072  s. New York: Spr
-00013690: 696e 6765 722e 0a20 2020 2022 2222 0a20  inger..    """. 
-000136a0: 2020 2072 765f 6f70 203d 2073 7469 636b     rv_op = stick
-000136b0: 6272 6561 6b69 6e67 7765 6967 6874 730a  breakingweights.
-000136c0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-000136d0: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
-000136e0: 6c73 2c20 616c 7068 612c 204b 2c20 2a61  ls, alpha, K, *a
-000136f0: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
-00013700: 2020 2020 2020 2020 616c 7068 6120 3d20          alpha = 
-00013710: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
-00013720: 6961 626c 6528 666c 6f61 7458 2861 6c70  iable(floatX(alp
-00013730: 6861 2929 0a20 2020 2020 2020 204b 203d  ha)).        K =
-00013740: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
-00013750: 7269 6162 6c65 2869 6e74 5828 4b29 290a  riable(intX(K)).
-00013760: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013770: 7375 7065 7228 292e 6469 7374 285b 616c  super().dist([al
-00013780: 7068 612c 204b 5d2c 202a 2a6b 7761 7267  pha, K], **kwarg
-00013790: 7329 0a0a 2020 2020 6465 6620 6d6f 6d65  s)..    def mome
-000137a0: 6e74 2872 762c 2073 697a 652c 2061 6c70  nt(rv, size, alp
-000137b0: 6861 2c20 4b29 3a0a 2020 2020 2020 2020  ha, K):.        
-000137c0: 616c 7068 6120 3d20 616c 7068 615b 2e2e  alpha = alpha[..
-000137d0: 2e2c 206e 702e 6e65 7761 7869 735d 0a20  ., np.newaxis]. 
-000137e0: 2020 2020 2020 206d 6f6d 656e 7420 3d20         moment = 
-000137f0: 2861 6c70 6861 202f 2028 3120 2b20 616c  (alpha / (1 + al
-00013800: 7068 6129 2920 2a2a 2070 742e 6172 616e  pha)) ** pt.aran
-00013810: 6765 284b 290a 2020 2020 2020 2020 6d6f  ge(K).        mo
-00013820: 6d65 6e74 202a 3d20 3120 2f20 2831 202b  ment *= 1 / (1 +
-00013830: 2061 6c70 6861 290a 2020 2020 2020 2020   alpha).        
-00013840: 6d6f 6d65 6e74 203d 2070 742e 636f 6e63  moment = pt.conc
-00013850: 6174 656e 6174 6528 5b6d 6f6d 656e 742c  atenate([moment,
-00013860: 2028 616c 7068 6120 2f20 2831 202b 2061   (alpha / (1 + a
-00013870: 6c70 6861 2929 202a 2a20 4b5d 2c20 6178  lpha)) ** K], ax
-00013880: 6973 3d2d 3129 0a20 2020 2020 2020 2069  is=-1).        i
-00013890: 6620 6e6f 7420 7276 5f73 697a 655f 6973  f not rv_size_is
-000138a0: 5f6e 6f6e 6528 7369 7a65 293a 0a20 2020  _none(size):.   
-000138b0: 2020 2020 2020 2020 206d 6f6d 656e 745f           moment_
-000138c0: 7369 7a65 203d 2070 742e 636f 6e63 6174  size = pt.concat
-000138d0: 656e 6174 6528 0a20 2020 2020 2020 2020  enate(.         
-000138e0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-000138f0: 2020 2020 2020 2020 2020 2020 2073 697a               siz
-00013900: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00013910: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00013920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013930: 204b 202b 2031 2c0a 2020 2020 2020 2020   K + 1,.        
-00013940: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-00013950: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00013960: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00013970: 2020 2020 2020 2020 2020 206d 6f6d 656e             momen
-00013980: 7420 3d20 7074 2e66 756c 6c28 6d6f 6d65  t = pt.full(mome
-00013990: 6e74 5f73 697a 652c 206d 6f6d 656e 7429  nt_size, moment)
-000139a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000139b0: 206d 6f6d 656e 740a 0a20 2020 2064 6566   moment..    def
-000139c0: 206c 6f67 7028 7661 6c75 652c 2061 6c70   logp(value, alp
-000139d0: 6861 2c20 4b29 3a0a 2020 2020 2020 2020  ha, K):.        
-000139e0: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
-000139f0: 756c 6174 6520 6c6f 672d 7072 6f62 6162  ulate log-probab
-00013a00: 696c 6974 7920 6f66 2074 6865 2064 6973  ility of the dis
-00013a10: 7472 6962 7574 696f 6e20 696e 6475 6365  tribution induce
-00013a20: 6420 6672 6f6d 2074 6865 2073 7469 636b  d from the stick
-00013a30: 2d62 7265 616b 696e 6720 7072 6f63 6573  -breaking proces
-00013a40: 730a 2020 2020 2020 2020 6174 2073 7065  s.        at spe
-00013a50: 6369 6669 6564 2076 616c 7565 2e0a 0a20  cified value... 
-00013a60: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
-00013a70: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00013a80: 2d2d 2d2d 0a20 2020 2020 2020 2076 616c  ----.        val
-00013a90: 7565 3a20 6e75 6d65 7269 630a 2020 2020  ue: numeric.    
-00013aa0: 2020 2020 2020 2020 5661 6c75 6520 666f          Value fo
-00013ab0: 7220 7768 6963 6820 6c6f 672d 7072 6f62  r which log-prob
-00013ac0: 6162 696c 6974 7920 6973 2063 616c 6375  ability is calcu
-00013ad0: 6c61 7465 642e 0a0a 2020 2020 2020 2020  lated...        
-00013ae0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
-00013af0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00013b00: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
-00013b10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00013b20: 2020 206c 6f67 7020 3d20 2d70 742e 7375     logp = -pt.su
-00013b30: 6d28 0a20 2020 2020 2020 2020 2020 2070  m(.            p
-00013b40: 742e 6c6f 6728 0a20 2020 2020 2020 2020  t.log(.         
-00013b50: 2020 2020 2020 2070 742e 6375 6d73 756d         pt.cumsum
-00013b60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00013b70: 2020 2020 2020 7661 6c75 655b 2e2e 2e2c        value[...,
-00013b80: 203a 3a2d 315d 2c0a 2020 2020 2020 2020   ::-1],.        
-00013b90: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-00013ba0: 3d2d 312c 0a20 2020 2020 2020 2020 2020  =-1,.           
-00013bb0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00013bc0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00013bd0: 2020 6178 6973 3d2d 312c 0a20 2020 2020    axis=-1,.     
-00013be0: 2020 2029 0a20 2020 2020 2020 206c 6f67     ).        log
-00013bf0: 7020 2b3d 202d 4b20 2a20 6265 7461 6c6e  p += -K * betaln
-00013c00: 2831 2c20 616c 7068 6129 0a20 2020 2020  (1, alpha).     
-00013c10: 2020 206c 6f67 7020 2b3d 2061 6c70 6861     logp += alpha
-00013c20: 202a 2070 742e 6c6f 6728 7661 6c75 655b   * pt.log(value[
-00013c30: 2e2e 2e2c 202d 315d 290a 0a20 2020 2020  ..., -1])..     
-00013c40: 2020 206c 6f67 7020 3d20 7074 2e73 7769     logp = pt.swi
-00013c50: 7463 6828 0a20 2020 2020 2020 2020 2020  tch(.           
-00013c60: 2070 742e 6f72 5f28 0a20 2020 2020 2020   pt.or_(.       
-00013c70: 2020 2020 2020 2020 2070 742e 616e 7928           pt.any(
-00013c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013c90: 2020 2020 2070 742e 616e 645f 2870 742e       pt.and_(pt.
-00013ca0: 6c65 2876 616c 7565 2c20 3029 2c20 7074  le(value, 0), pt
-00013cb0: 2e67 6528 7661 6c75 652c 2031 2929 2c0a  .ge(value, 1)),.
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cd0: 2020 2020 6178 6973 3d2d 312c 0a20 2020      axis=-1,.   
-00013ce0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00013cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d00: 7074 2e6f 725f 280a 2020 2020 2020 2020  pt.or_(.        
-00013d10: 2020 2020 2020 2020 2020 2020 7074 2e62              pt.b
-00013d20: 6974 7769 7365 5f6e 6f74 2870 742e 616c  itwise_not(pt.al
-00013d30: 6c63 6c6f 7365 2876 616c 7565 2e73 756d  lclose(value.sum
-00013d40: 282d 3129 2c20 3129 292c 0a20 2020 2020  (-1), 1)),.     
-00013d50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00013d60: 742e 6e65 7128 7661 6c75 652e 7368 6170  t.neq(value.shap
-00013d70: 655b 2d31 5d2c 204b 202b 2031 292c 0a20  e[-1], K + 1),. 
-00013d80: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00013d90: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
-00013da0: 0a20 2020 2020 2020 2020 2020 202d 6e70  .            -np
-00013db0: 2e69 6e66 2c0a 2020 2020 2020 2020 2020  .inf,.          
-00013dc0: 2020 6c6f 6770 2c0a 2020 2020 2020 2020    logp,.        
-00013dd0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00013de0: 6e20 6368 6563 6b5f 7061 7261 6d65 7465  n check_paramete
-00013df0: 7273 280a 2020 2020 2020 2020 2020 2020  rs(.            
-00013e00: 6c6f 6770 2c0a 2020 2020 2020 2020 2020  logp,.          
-00013e10: 2020 616c 7068 6120 3e20 302c 0a20 2020    alpha > 0,.   
-00013e20: 2020 2020 2020 2020 204b 203e 2030 2c0a           K > 0,.
-00013e30: 2020 2020 2020 2020 2020 2020 6d73 673d              msg=
-00013e40: 2261 6c70 6861 203e 2030 2c20 4b20 3e20  "alpha > 0, K > 
-00013e50: 3022 2c0a 2020 2020 2020 2020 290a 0a0a  0",.        )...
-00013e60: 636c 6173 7320 5a65 726f 5375 6d4e 6f72  class ZeroSumNor
-00013e70: 6d61 6c52 5628 5379 6d62 6f6c 6963 5261  malRV(SymbolicRa
-00013e80: 6e64 6f6d 5661 7269 6162 6c65 293a 0a20  ndomVariable):. 
-00013e90: 2020 2022 2222 5a65 726f 5375 6d4e 6f72     """ZeroSumNor
-00013ea0: 6d61 6c20 7261 6e64 6f6d 2076 6172 6961  mal random varia
-00013eb0: 626c 6522 2222 0a0a 2020 2020 5f70 7269  ble"""..    _pri
-00013ec0: 6e74 5f6e 616d 6520 3d20 2822 5a65 726f  nt_name = ("Zero
-00013ed0: 5375 6d4e 6f72 6d61 6c22 2c20 225c 5c6f  SumNormal", "\\o
-00013ee0: 7065 7261 746f 726e 616d 657b 5a65 726f  peratorname{Zero
-00013ef0: 5375 6d4e 6f72 6d61 6c7d 2229 0a20 2020  SumNormal}").   
-00013f00: 2064 6566 6175 6c74 5f6f 7574 7075 7420   default_output 
-00013f10: 3d20 300a 0a0a 636c 6173 7320 5a65 726f  = 0...class Zero
-00013f20: 5375 6d4e 6f72 6d61 6c28 4469 7374 7269  SumNormal(Distri
-00013f30: 6275 7469 6f6e 293a 0a20 2020 2072 2222  bution):.    r""
-00013f40: 220a 2020 2020 5a65 726f 5375 6d4e 6f72  ".    ZeroSumNor
-00013f50: 6d61 6c20 6469 7374 7269 6275 7469 6f6e  mal distribution
-00013f60: 2c20 692e 6520 4e6f 726d 616c 2064 6973  , i.e Normal dis
-00013f70: 7472 6962 7574 696f 6e20 7768 6572 6520  tribution where 
-00013f80: 6f6e 6520 6f72 0a20 2020 2073 6576 6572  one or.    sever
-00013f90: 616c 2061 7865 7320 6172 6520 636f 6e73  al axes are cons
-00013fa0: 7472 6169 6e65 6420 746f 2073 756d 2074  trained to sum t
-00013fb0: 6f20 7a65 726f 2e0a 2020 2020 4279 2064  o zero..    By d
-00013fc0: 6566 6175 6c74 2c20 7468 6520 6c61 7374  efault, the last
-00013fd0: 2061 7869 7320 6973 2063 6f6e 7374 7261   axis is constra
-00013fe0: 696e 6564 2074 6f20 7375 6d20 746f 207a  ined to sum to z
-00013ff0: 6572 6f2e 0a20 2020 2053 6565 2060 6e5f  ero..    See `n_
-00014000: 7a65 726f 7375 6d5f 6178 6573 6020 6b77  zerosum_axes` kw
-00014010: 6172 6720 666f 7220 6d6f 7265 2064 6574  arg for more det
-00014020: 6169 6c73 2e0a 0a20 2020 202e 2e20 6d61  ails...    .. ma
-00014030: 7468 3a3a 0a0a 2020 2020 2020 2020 5c62  th::..        \b
-00014040: 6567 696e 7b61 6c69 676e 2a7d 0a20 2020  egin{align*}.   
-00014050: 2020 2020 2020 2020 205a 534e 285c 7369           ZSN(\si
-00014060: 676d 6129 203d 204e 205c 4269 6728 2030  gma) = N \Big( 0
-00014070: 2c20 5c73 6967 6d61 5e32 2028 4920 2d20  , \sigma^2 (I - 
-00014080: 5c74 6672 6163 7b31 7d7b 6e7d 4a29 205c  \tfrac{1}{n}J) \
-00014090: 4269 6729 205c 5c0a 2020 2020 2020 2020  Big) \\.        
-000140a0: 2020 2020 5c74 6578 747b 7768 6572 657d      \text{where}
-000140b0: 205c 207e 204a 5f7b 696a 7d20 3d20 3120   \ ~ J_{ij} = 1 
-000140c0: 5c20 7e20 5c74 6578 747b 616e 647d 205c  \ ~ \text{and} \
-000140d0: 5c0a 2020 2020 2020 2020 2020 2020 6e20  \.            n 
-000140e0: 3d20 5c74 6578 747b 6e62 7220 6f66 207a  = \text{nbr of z
-000140f0: 6572 6f2d 7375 6d20 6178 6573 7d0a 2020  ero-sum axes}.  
-00014100: 2020 2020 2020 5c65 6e64 7b61 6c69 676e        \end{align
-00014110: 2a7d 0a0a 2020 2020 5061 7261 6d65 7465  *}..    Paramete
-00014120: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00014130: 2d0a 2020 2020 7369 676d 6120 3a20 7465  -.    sigma : te
-00014140: 6e73 6f72 5f6c 696b 6520 6f66 2066 6c6f  nsor_like of flo
-00014150: 6174 0a20 2020 2020 2020 2053 6361 6c65  at.        Scale
-00014160: 2070 6172 616d 6574 6572 2028 7369 676d   parameter (sigm
-00014170: 6120 3e20 3029 2e0a 2020 2020 2020 2020  a > 0)..        
-00014180: 4974 2773 2061 6374 7561 6c6c 7920 7468  It's actually th
-00014190: 6520 7374 616e 6461 7264 2064 6576 6961  e standard devia
-000141a0: 7469 6f6e 206f 6620 7468 6520 756e 6465  tion of the unde
-000141b0: 726c 7969 6e67 2c20 756e 636f 6e73 7472  rlying, unconstr
-000141c0: 6169 6e65 6420 4e6f 726d 616c 2064 6973  ained Normal dis
-000141d0: 7472 6962 7574 696f 6e2e 0a20 2020 2020  tribution..     
-000141e0: 2020 2044 6566 6175 6c74 7320 746f 2031     Defaults to 1
-000141f0: 2069 6620 6e6f 7420 7370 6563 6966 6965   if not specifie
-00014200: 642e 0a20 2020 2020 2020 2046 6f72 206e  d..        For n
-00014210: 6f77 2c20 6060 7369 676d 6160 6020 6861  ow, ``sigma`` ha
-00014220: 7320 746f 2062 6520 6120 7363 616c 6172  s to be a scalar
-00014230: 2c20 746f 2065 6e73 7572 6520 7468 6520  , to ensure the 
-00014240: 7a65 726f 2d73 756d 2063 6f6e 7374 7261  zero-sum constra
-00014250: 696e 742e 0a20 2020 206e 5f7a 6572 6f73  int..    n_zeros
-00014260: 756d 5f61 7865 733a 2069 6e74 2c20 6465  um_axes: int, de
-00014270: 6661 756c 7473 2074 6f20 310a 2020 2020  faults to 1.    
-00014280: 2020 2020 4e75 6d62 6572 206f 6620 6178      Number of ax
-00014290: 6573 2061 6c6f 6e67 2077 6869 6368 2074  es along which t
-000142a0: 6865 207a 6572 6f2d 7375 6d20 636f 6e73  he zero-sum cons
-000142b0: 7472 6169 6e74 2069 7320 656e 666f 7263  traint is enforc
-000142c0: 6564 2c20 7374 6172 7469 6e67 2066 726f  ed, starting fro
-000142d0: 6d20 7468 6520 7269 6768 746d 6f73 7420  m the rightmost 
-000142e0: 706f 7369 7469 6f6e 2e0a 2020 2020 2020  position..      
-000142f0: 2020 4465 6661 756c 7473 2074 6f20 312c    Defaults to 1,
-00014300: 2069 2e65 2074 6865 2072 6967 6874 6d6f   i.e the rightmo
-00014310: 7374 2061 7869 732e 0a20 2020 207a 6572  st axis..    zer
-00014320: 6f73 756d 5f61 7865 733a 2069 6e74 2c20  osum_axes: int, 
-00014330: 6465 7072 6563 6174 6564 2070 6c65 6173  deprecated pleas
-00014340: 6520 7573 6520 6e5f 7a65 726f 7375 6d5f  e use n_zerosum_
-00014350: 6178 6573 2061 7320 6974 7320 7375 6363  axes as its succ
-00014360: 6573 736f 720a 2020 2020 6469 6d73 3a20  essor.    dims: 
-00014370: 7365 7175 656e 6365 206f 6620 7374 7269  sequence of stri
-00014380: 6e67 732c 206f 7074 696f 6e61 6c0a 2020  ngs, optional.  
-00014390: 2020 2020 2020 4469 6d65 6e73 696f 6e20        Dimension 
-000143a0: 6e61 6d65 7320 6f66 2074 6865 2064 6973  names of the dis
-000143b0: 7472 6962 7574 696f 6e2e 2057 6f72 6b73  tribution. Works
-000143c0: 2074 6865 2073 616d 6520 6173 2066 6f72   the same as for
-000143d0: 206f 7468 6572 2050 794d 4320 6469 7374   other PyMC dist
-000143e0: 7269 6275 7469 6f6e 732e 0a20 2020 2020  ributions..     
-000143f0: 2020 204e 6563 6573 7361 7279 2069 6620     Necessary if 
-00014400: 6060 7368 6170 6560 6020 6973 206e 6f74  ``shape`` is not
-00014410: 2070 6173 7365 642e 0a20 2020 2073 6861   passed..    sha
-00014420: 7065 3a20 7475 706c 6520 6f66 2069 6e74  pe: tuple of int
-00014430: 6567 6572 732c 206f 7074 696f 6e61 6c0a  egers, optional.
-00014440: 2020 2020 2020 2020 5368 6170 6520 6f66          Shape of
-00014450: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
-00014460: 6e2e 2057 6f72 6b73 2074 6865 2073 616d  n. Works the sam
-00014470: 6520 6173 2066 6f72 206f 7468 6572 2050  e as for other P
-00014480: 794d 4320 6469 7374 7269 6275 7469 6f6e  yMC distribution
-00014490: 732e 0a20 2020 2020 2020 204e 6563 6573  s..        Neces
-000144a0: 7361 7279 2069 6620 6060 6469 6d73 6060  sary if ``dims``
-000144b0: 206f 7220 6060 6f62 7365 7276 6564 6060   or ``observed``
-000144c0: 2069 7320 6e6f 7420 7061 7373 6564 2e0a   is not passed..
-000144d0: 0a20 2020 2057 6172 6e69 6e67 730a 2020  .    Warnings.  
-000144e0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2060    --------.    `
-000144f0: 6073 6967 6d61 6060 2068 6173 2074 6f20  `sigma`` has to 
-00014500: 6265 2061 2073 6361 6c61 722c 2074 6f20  be a scalar, to 
-00014510: 656e 7375 7265 2074 6865 207a 6572 6f2d  ensure the zero-
-00014520: 7375 6d20 636f 6e73 7472 6169 6e74 2e0a  sum constraint..
-00014530: 2020 2020 5468 6520 6162 696c 6974 7920      The ability 
-00014540: 746f 2073 7065 6369 6679 2061 2076 6563  to specify a vec
-00014550: 746f 7220 6f66 2060 6073 6967 6d61 6060  tor of ``sigma``
-00014560: 206d 6179 2062 6520 6164 6465 6420 696e   may be added in
-00014570: 2066 7574 7572 6520 7665 7273 696f 6e73   future versions
-00014580: 2e0a 0a20 2020 2060 606e 5f7a 6572 6f73  ...    ``n_zeros
-00014590: 756d 5f61 7865 7360 6020 6861 7320 746f  um_axes`` has to
-000145a0: 2062 6520 3e20 302e 2049 6620 796f 7520   be > 0. If you 
-000145b0: 7761 6e74 2074 6865 2062 6568 6176 696f  want the behavio
-000145c0: 7220 6f66 2060 606e 5f7a 6572 6f73 756d  r of ``n_zerosum
-000145d0: 5f61 7865 7320 3d20 3060 602c 0a20 2020  _axes = 0``,.   
-000145e0: 206a 7573 7420 7573 6520 6060 706d 2e4e   just use ``pm.N
-000145f0: 6f72 6d61 6c60 602e 0a0a 2020 2020 4578  ormal``...    Ex
-00014600: 616d 706c 6573 0a20 2020 202d 2d2d 2d2d  amples.    -----
-00014610: 2d2d 2d0a 2020 2020 4465 6669 6e65 2061  ---.    Define a
-00014620: 2060 5a65 726f 5375 6d4e 6f72 6d61 6c60   `ZeroSumNormal`
-00014630: 2076 6172 6961 626c 652c 2077 6974 6820   variable, with 
-00014640: 6073 6967 6d61 3d31 6020 616e 640a 2020  `sigma=1` and.  
-00014650: 2020 606e 5f7a 6572 6f73 756d 5f61 7865    `n_zerosum_axe
-00014660: 733d 3160 2020 6279 2064 6566 6175 6c74  s=1`  by default
-00014670: 3a3a 0a0a 2020 2020 2020 2020 434f 4f52  ::..        COOR
-00014680: 4453 203d 207b 0a20 2020 2020 2020 2020  DS = {.         
-00014690: 2020 2022 7265 6769 6f6e 7322 3a20 5b22     "regions": ["
-000146a0: 6122 2c20 2262 222c 2022 6322 5d2c 0a20  a", "b", "c"],. 
-000146b0: 2020 2020 2020 2020 2020 2022 616e 7377             "answ
-000146c0: 6572 7322 3a20 5b22 7965 7322 2c20 226e  ers": ["yes", "n
-000146d0: 6f22 2c20 2277 6861 7465 7665 7222 2c20  o", "whatever", 
-000146e0: 2264 6f6e 2774 2075 6e64 6572 7374 616e  "don't understan
-000146f0: 6420 7175 6573 7469 6f6e 225d 2c0a 2020  d question"],.  
-00014700: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00014710: 7769 7468 2070 6d2e 4d6f 6465 6c28 636f  with pm.Model(co
-00014720: 6f72 6473 3d43 4f4f 5244 5329 2061 7320  ords=COORDS) as 
-00014730: 6d3a 0a20 2020 2020 2020 2020 2020 2023  m:.            #
-00014740: 2074 6865 207a 6572 6f20 7375 6d20 6178   the zero sum ax
-00014750: 6973 2077 696c 6c20 6265 2027 616e 7377  is will be 'answ
-00014760: 6572 7327 0a20 2020 2020 2020 2020 2020  ers'.           
-00014770: 2076 203d 2070 6d2e 5a65 726f 5375 6d4e   v = pm.ZeroSumN
-00014780: 6f72 6d61 6c28 2276 222c 2064 696d 733d  ormal("v", dims=
-00014790: 2822 7265 6769 6f6e 7322 2c20 2261 6e73  ("regions", "ans
-000147a0: 7765 7273 2229 290a 0a20 2020 2020 2020  wers"))..       
-000147b0: 2077 6974 6820 706d 2e4d 6f64 656c 2863   with pm.Model(c
-000147c0: 6f6f 7264 733d 434f 4f52 4453 2920 6173  oords=COORDS) as
-000147d0: 206d 3a0a 2020 2020 2020 2020 2020 2020   m:.            
-000147e0: 2320 7468 6520 7a65 726f 2073 756d 2061  # the zero sum a
-000147f0: 7865 7320 7769 6c6c 2062 6520 2761 6e73  xes will be 'ans
-00014800: 7765 7273 2720 616e 6420 2772 6567 696f  wers' and 'regio
-00014810: 6e73 270a 2020 2020 2020 2020 2020 2020  ns'.            
-00014820: 7620 3d20 706d 2e5a 6572 6f53 756d 4e6f  v = pm.ZeroSumNo
-00014830: 726d 616c 2822 7622 2c20 6469 6d73 3d28  rmal("v", dims=(
-00014840: 2272 6567 696f 6e73 222c 2022 616e 7377  "regions", "answ
-00014850: 6572 7322 292c 206e 5f7a 6572 6f73 756d  ers"), n_zerosum
-00014860: 5f61 7865 733d 3229 0a0a 2020 2020 2020  _axes=2)..      
-00014870: 2020 7769 7468 2070 6d2e 4d6f 6465 6c28    with pm.Model(
-00014880: 636f 6f72 6473 3d43 4f4f 5244 5329 2061  coords=COORDS) a
-00014890: 7320 6d3a 0a20 2020 2020 2020 2020 2020  s m:.           
-000148a0: 2023 2074 6865 207a 6572 6f20 7375 6d20   # the zero sum 
-000148b0: 6178 6573 2077 696c 6c20 6265 2074 6865  axes will be the
-000148c0: 206c 6173 7420 7477 6f0a 2020 2020 2020   last two.      
-000148d0: 2020 2020 2020 7620 3d20 706d 2e5a 6572        v = pm.Zer
-000148e0: 6f53 756d 4e6f 726d 616c 2822 7622 2c20  oSumNormal("v", 
-000148f0: 7368 6170 653d 2833 2c20 342c 2035 292c  shape=(3, 4, 5),
-00014900: 206e 5f7a 6572 6f73 756d 5f61 7865 733d   n_zerosum_axes=
-00014910: 3229 0a20 2020 2022 2222 0a20 2020 2072  2).    """.    r
-00014920: 765f 7479 7065 203d 205a 6572 6f53 756d  v_type = ZeroSum
-00014930: 4e6f 726d 616c 5256 0a0a 2020 2020 6465  NormalRV..    de
-00014940: 6620 5f5f 6e65 775f 5f28 0a20 2020 2020  f __new__(.     
-00014950: 2020 2063 6c73 2c20 2a61 7267 732c 207a     cls, *args, z
-00014960: 6572 6f73 756d 5f61 7865 733d 4e6f 6e65  erosum_axes=None
-00014970: 2c20 6e5f 7a65 726f 7375 6d5f 6178 6573  , n_zerosum_axes
-00014980: 3d4e 6f6e 652c 2073 7570 706f 7274 5f73  =None, support_s
-00014990: 6861 7065 3d4e 6f6e 652c 2064 696d 733d  hape=None, dims=
-000149a0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 0a20  None, **kwargs. 
-000149b0: 2020 2029 3a0a 2020 2020 2020 2020 6966     ):.        if
-000149c0: 207a 6572 6f73 756d 5f61 7865 7320 6973   zerosum_axes is
-000149d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000149e0: 2020 2020 2020 206e 5f7a 6572 6f73 756d         n_zerosum
-000149f0: 5f61 7865 7320 3d20 7a65 726f 7375 6d5f  _axes = zerosum_
-00014a00: 6178 6573 0a20 2020 2020 2020 2020 2020  axes.           
-00014a10: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
-00014a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a30: 2254 6865 2027 7a65 726f 7375 6d5f 6178  "The 'zerosum_ax
-00014a40: 6573 2720 7061 7261 6d65 7465 7220 6973  es' parameter is
-00014a50: 2064 6570 7265 6361 7465 642e 2055 7365   deprecated. Use
-00014a60: 2027 6e5f 7a65 726f 7375 6d5f 6178 6573   'n_zerosum_axes
-00014a70: 2720 696e 7374 6561 642e 222c 0a20 2020  ' instead.",.   
-00014a80: 2020 2020 2020 2020 2020 2020 2044 6570               Dep
-00014a90: 7265 6361 7469 6f6e 5761 726e 696e 672c  recationWarning,
-00014aa0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00014ab0: 2020 2020 2020 2069 6620 6469 6d73 2069         if dims i
-00014ac0: 7320 6e6f 7420 4e6f 6e65 206f 7220 6b77  s not None or kw
-00014ad0: 6172 6773 2e67 6574 2822 6f62 7365 7276  args.get("observ
-00014ae0: 6564 2229 2069 7320 6e6f 7420 4e6f 6e65  ed") is not None
-00014af0: 3a0a 2020 2020 2020 2020 2020 2020 6e5f  :.            n_
-00014b00: 7a65 726f 7375 6d5f 6178 6573 203d 2063  zerosum_axes = c
-00014b10: 6c73 2e63 6865 636b 5f7a 6572 6f73 756d  ls.check_zerosum
-00014b20: 5f61 7865 7328 6e5f 7a65 726f 7375 6d5f  _axes(n_zerosum_
-00014b30: 6178 6573 290a 0a20 2020 2020 2020 2020  axes)..         
-00014b40: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
-00014b50: 203d 2067 6574 5f73 7570 706f 7274 5f73   = get_support_s
-00014b60: 6861 7065 280a 2020 2020 2020 2020 2020  hape(.          
-00014b70: 2020 2020 2020 7375 7070 6f72 745f 7368        support_sh
-00014b80: 6170 653d 7375 7070 6f72 745f 7368 6170  ape=support_shap
-00014b90: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00014ba0: 2020 2073 6861 7065 3d4e 6f6e 652c 2020     shape=None,  
-00014bb0: 2320 5368 6170 6520 7769 6c6c 2062 6520  # Shape will be 
-00014bc0: 6368 6563 6b65 6420 696e 2060 636c 732e  checked in `cls.
-00014bd0: 6469 7374 600a 2020 2020 2020 2020 2020  dist`.          
-00014be0: 2020 2020 2020 6469 6d73 3d64 696d 732c        dims=dims,
-00014bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c00: 206f 6273 6572 7665 643d 6b77 6172 6773   observed=kwargs
-00014c10: 2e67 6574 2822 6f62 7365 7276 6564 222c  .get("observed",
-00014c20: 204e 6f6e 6529 2c0a 2020 2020 2020 2020   None),.        
-00014c30: 2020 2020 2020 2020 6e64 696d 5f73 7570          ndim_sup
-00014c40: 703d 6e5f 7a65 726f 7375 6d5f 6178 6573  p=n_zerosum_axes
-00014c50: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00014c60: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014c70: 7375 7065 7228 292e 5f5f 6e65 775f 5f28  super().__new__(
-00014c80: 0a20 2020 2020 2020 2020 2020 2063 6c73  .            cls
-00014c90: 2c0a 2020 2020 2020 2020 2020 2020 2a61  ,.            *a
-00014ca0: 7267 732c 0a20 2020 2020 2020 2020 2020  rgs,.           
-00014cb0: 206e 5f7a 6572 6f73 756d 5f61 7865 733d   n_zerosum_axes=
-00014cc0: 6e5f 7a65 726f 7375 6d5f 6178 6573 2c0a  n_zerosum_axes,.
-00014cd0: 2020 2020 2020 2020 2020 2020 7375 7070              supp
-00014ce0: 6f72 745f 7368 6170 653d 7375 7070 6f72  ort_shape=suppor
-00014cf0: 745f 7368 6170 652c 0a20 2020 2020 2020  t_shape,.       
-00014d00: 2020 2020 2064 696d 733d 6469 6d73 2c0a       dims=dims,.
-00014d10: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
-00014d20: 6172 6773 2c0a 2020 2020 2020 2020 290a  args,.        ).
-00014d30: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00014d40: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
-00014d50: 6c73 2c20 7369 676d 613d 312c 206e 5f7a  ls, sigma=1, n_z
-00014d60: 6572 6f73 756d 5f61 7865 733d 4e6f 6e65  erosum_axes=None
-00014d70: 2c20 7375 7070 6f72 745f 7368 6170 653d  , support_shape=
-00014d80: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-00014d90: 0a20 2020 2020 2020 206e 5f7a 6572 6f73  .        n_zeros
-00014da0: 756d 5f61 7865 7320 3d20 636c 732e 6368  um_axes = cls.ch
-00014db0: 6563 6b5f 7a65 726f 7375 6d5f 6178 6573  eck_zerosum_axes
-00014dc0: 286e 5f7a 6572 6f73 756d 5f61 7865 7329  (n_zerosum_axes)
-00014dd0: 0a0a 2020 2020 2020 2020 7369 676d 6120  ..        sigma 
-00014de0: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-00014df0: 6172 6961 626c 6528 666c 6f61 7458 2873  ariable(floatX(s
-00014e00: 6967 6d61 2929 0a20 2020 2020 2020 2069  igma)).        i
-00014e10: 6620 7369 676d 612e 6e64 696d 203e 2030  f sigma.ndim > 0
-00014e20: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00014e30: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00014e40: 7369 676d 6120 6861 7320 746f 2062 6520  sigma has to be 
-00014e50: 6120 7363 616c 6172 2229 0a0a 2020 2020  a scalar")..    
-00014e60: 2020 2020 7375 7070 6f72 745f 7368 6170      support_shap
-00014e70: 6520 3d20 6765 745f 7375 7070 6f72 745f  e = get_support_
-00014e80: 7368 6170 6528 0a20 2020 2020 2020 2020  shape(.         
-00014e90: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
-00014ea0: 3d73 7570 706f 7274 5f73 6861 7065 2c0a  =support_shape,.
-00014eb0: 2020 2020 2020 2020 2020 2020 7368 6170              shap
-00014ec0: 653d 6b77 6172 6773 2e67 6574 2822 7368  e=kwargs.get("sh
-00014ed0: 6170 6522 292c 0a20 2020 2020 2020 2020  ape"),.         
-00014ee0: 2020 206e 6469 6d5f 7375 7070 3d6e 5f7a     ndim_supp=n_z
-00014ef0: 6572 6f73 756d 5f61 7865 732c 0a20 2020  erosum_axes,.   
-00014f00: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00014f10: 6966 2073 7570 706f 7274 5f73 6861 7065  if support_shape
-00014f20: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00014f30: 2020 2020 2020 6966 206e 5f7a 6572 6f73        if n_zeros
-00014f40: 756d 5f61 7865 7320 3e20 303a 0a20 2020  um_axes > 0:.   
-00014f50: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00014f60: 7365 2056 616c 7565 4572 726f 7228 2259  se ValueError("Y
-00014f70: 6f75 206d 7573 7420 7370 6563 6966 7920  ou must specify 
-00014f80: 6469 6d73 2c20 7368 6170 6520 6f72 2073  dims, shape or s
-00014f90: 7570 706f 7274 5f73 6861 7065 2070 6172  upport_shape par
-00014fa0: 616d 6574 6572 2229 0a20 2020 2020 2020  ameter").       
-00014fb0: 2020 2020 2023 2054 4f44 4f3a 2065 6467       # TODO: edg
-00014fc0: 652d 6361 7365 2064 6f65 736e 2774 2077  e-case doesn't w
-00014fd0: 6f72 6b20 666f 7220 6e6f 772c 2062 6563  ork for now, bec
-00014fe0: 6175 7365 2070 742e 7374 6163 6b20 696e  ause pt.stack in
-00014ff0: 2067 6574 5f73 7570 706f 7274 5f73 6861   get_support_sha
-00015000: 7065 2066 6169 6c73 0a20 2020 2020 2020  pe fails.       
-00015010: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
-00015020: 2020 2020 2020 2020 2023 2020 2020 2073           #     s
-00015030: 7570 706f 7274 5f73 6861 7065 203d 2028  upport_shape = (
-00015040: 2920 2320 6265 6361 7573 6520 6974 2773  ) # because it's
-00015050: 206a 7573 7420 6120 4e6f 726d 616c 2069   just a Normal i
-00015060: 6e20 7468 6174 2063 6173 650a 2020 2020  n that case.    
-00015070: 2020 2020 7375 7070 6f72 745f 7368 6170      support_shap
-00015080: 6520 3d20 7074 2e61 735f 7465 6e73 6f72  e = pt.as_tensor
-00015090: 5f76 6172 6961 626c 6528 696e 7458 2873  _variable(intX(s
-000150a0: 7570 706f 7274 5f73 6861 7065 2929 0a0a  upport_shape))..
-000150b0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
-000150c0: 5f7a 6572 6f73 756d 5f61 7865 7320 3d3d  _zerosum_axes ==
-000150d0: 2070 742e 6765 745f 7665 6374 6f72 5f6c   pt.get_vector_l
-000150e0: 656e 6774 6828 0a20 2020 2020 2020 2020  ength(.         
-000150f0: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
-00015100: 0a20 2020 2020 2020 2029 2c20 2273 7570  .        ), "sup
-00015110: 706f 7274 5f73 6861 7065 2068 6173 2074  port_shape has t
-00015120: 6f20 6265 2061 7320 6c6f 6e67 2061 7320  o be as long as 
-00015130: 6e5f 7a65 726f 7375 6d5f 6178 6573 220a  n_zerosum_axes".
-00015140: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00015150: 7375 7065 7228 292e 6469 7374 280a 2020  super().dist(.  
-00015160: 2020 2020 2020 2020 2020 5b73 6967 6d61            [sigma
-00015170: 5d2c 206e 5f7a 6572 6f73 756d 5f61 7865  ], n_zerosum_axe
-00015180: 733d 6e5f 7a65 726f 7375 6d5f 6178 6573  s=n_zerosum_axes
-00015190: 2c20 7375 7070 6f72 745f 7368 6170 653d  , support_shape=
-000151a0: 7375 7070 6f72 745f 7368 6170 652c 202a  support_shape, *
-000151b0: 2a6b 7761 7267 730a 2020 2020 2020 2020  *kwargs.        
-000151c0: 290a 0a20 2020 2040 636c 6173 736d 6574  )..    @classmet
-000151d0: 686f 640a 2020 2020 6465 6620 6368 6563  hod.    def chec
-000151e0: 6b5f 7a65 726f 7375 6d5f 6178 6573 2863  k_zerosum_axes(c
-000151f0: 6c73 2c20 6e5f 7a65 726f 7375 6d5f 6178  ls, n_zerosum_ax
-00015200: 6573 3a20 4f70 7469 6f6e 616c 5b69 6e74  es: Optional[int
-00015210: 5d29 202d 3e20 696e 743a 0a20 2020 2020  ]) -> int:.     
-00015220: 2020 2069 6620 6e5f 7a65 726f 7375 6d5f     if n_zerosum_
-00015230: 6178 6573 2069 7320 4e6f 6e65 3a0a 2020  axes is None:.  
-00015240: 2020 2020 2020 2020 2020 6e5f 7a65 726f            n_zero
-00015250: 7375 6d5f 6178 6573 203d 2031 0a20 2020  sum_axes = 1.   
-00015260: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00015270: 7374 616e 6365 286e 5f7a 6572 6f73 756d  stance(n_zerosum
-00015280: 5f61 7865 732c 2069 6e74 293a 0a20 2020  _axes, int):.   
-00015290: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-000152a0: 7970 6545 7272 6f72 2822 6e5f 7a65 726f  ypeError("n_zero
-000152b0: 7375 6d5f 6178 6573 2068 6173 2074 6f20  sum_axes has to 
-000152c0: 6265 2061 6e20 696e 7465 6765 7222 290a  be an integer").
-000152d0: 2020 2020 2020 2020 6966 206e 6f74 206e          if not n
-000152e0: 5f7a 6572 6f73 756d 5f61 7865 7320 3e20  _zerosum_axes > 
-000152f0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00015300: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00015310: 226e 5f7a 6572 6f73 756d 5f61 7865 7320  "n_zerosum_axes 
-00015320: 6861 7320 746f 2062 6520 3e20 3022 290a  has to be > 0").
-00015330: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-00015340: 5f7a 6572 6f73 756d 5f61 7865 730a 0a20  _zerosum_axes.. 
-00015350: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00015360: 2020 2020 6465 6620 7276 5f6f 7028 636c      def rv_op(cl
-00015370: 732c 2073 6967 6d61 2c20 6e5f 7a65 726f  s, sigma, n_zero
-00015380: 7375 6d5f 6178 6573 2c20 7375 7070 6f72  sum_axes, suppor
-00015390: 745f 7368 6170 652c 2073 697a 653d 4e6f  t_shape, size=No
-000153a0: 6e65 293a 0a20 2020 2020 2020 2073 6861  ne):.        sha
-000153b0: 7065 203d 2074 6f5f 7475 706c 6528 7369  pe = to_tuple(si
-000153c0: 7a65 2920 2b20 7475 706c 6528 7375 7070  ze) + tuple(supp
-000153d0: 6f72 745f 7368 6170 6529 0a20 2020 2020  ort_shape).     
-000153e0: 2020 206e 6f72 6d61 6c5f 6469 7374 203d     normal_dist =
-000153f0: 2069 676e 6f72 655f 6c6f 6770 726f 6228   ignore_logprob(
-00015400: 706d 2e4e 6f72 6d61 6c2e 6469 7374 2873  pm.Normal.dist(s
-00015410: 6967 6d61 3d73 6967 6d61 2c20 7368 6170  igma=sigma, shap
-00015420: 653d 7368 6170 6529 290a 0a20 2020 2020  e=shape))..     
-00015430: 2020 2069 6620 6e5f 7a65 726f 7375 6d5f     if n_zerosum_
-00015440: 6178 6573 203e 206e 6f72 6d61 6c5f 6469  axes > normal_di
-00015450: 7374 2e6e 6469 6d3a 0a20 2020 2020 2020  st.ndim:.       
-00015460: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00015470: 4572 726f 7228 2253 6861 7065 206f 6620  Error("Shape of 
-00015480: 6469 7374 7269 6275 7469 6f6e 2069 7320  distribution is 
-00015490: 746f 6f20 736d 616c 6c20 666f 7220 7468  too small for th
-000154a0: 6520 6e75 6d62 6572 206f 6620 7a65 726f  e number of zero
-000154b0: 7375 6d20 6178 6573 2229 0a0a 2020 2020  sum axes")..    
-000154c0: 2020 2020 6e6f 726d 616c 5f64 6973 745f      normal_dist_
-000154d0: 2c20 7369 676d 615f 2c20 7375 7070 6f72  , sigma_, suppor
-000154e0: 745f 7368 6170 655f 203d 2028 0a20 2020  t_shape_ = (.   
-000154f0: 2020 2020 2020 2020 206e 6f72 6d61 6c5f           normal_
-00015500: 6469 7374 2e74 7970 6528 292c 0a20 2020  dist.type(),.   
-00015510: 2020 2020 2020 2020 2073 6967 6d61 2e74           sigma.t
-00015520: 7970 6528 292c 0a20 2020 2020 2020 2020  ype(),.         
-00015530: 2020 2073 7570 706f 7274 5f73 6861 7065     support_shape
-00015540: 2e74 7970 6528 292c 0a20 2020 2020 2020  .type(),.       
-00015550: 2029 0a0a 2020 2020 2020 2020 2320 5a65   )..        # Ze
-00015560: 726f 7375 6d2d 6e6f 726d 616c 696e 6720  rosum-normaling 
-00015570: 6973 2061 6368 6965 7665 6420 6279 2073  is achieved by s
-00015580: 7562 7472 6163 7469 6e67 2074 6865 206d  ubtracting the m
-00015590: 6561 6e20 616c 6f6e 6720 7468 6520 6769  ean along the gi
-000155a0: 7665 6e20 6e5f 7a65 726f 7375 6d5f 6178  ven n_zerosum_ax
-000155b0: 6573 0a20 2020 2020 2020 207a 6572 6f73  es.        zeros
-000155c0: 756d 5f72 765f 203d 206e 6f72 6d61 6c5f  um_rv_ = normal_
-000155d0: 6469 7374 5f0a 2020 2020 2020 2020 666f  dist_.        fo
-000155e0: 7220 6178 6973 2069 6e20 7261 6e67 6528  r axis in range(
-000155f0: 6e5f 7a65 726f 7375 6d5f 6178 6573 293a  n_zerosum_axes):
-00015600: 0a20 2020 2020 2020 2020 2020 207a 6572  .            zer
-00015610: 6f73 756d 5f72 765f 202d 3d20 7a65 726f  osum_rv_ -= zero
-00015620: 7375 6d5f 7276 5f2e 6d65 616e 2861 7869  sum_rv_.mean(axi
-00015630: 733d 2d61 7869 7320 2d20 312c 206b 6565  s=-axis - 1, kee
-00015640: 7064 696d 733d 5472 7565 290a 0a20 2020  pdims=True)..   
-00015650: 2020 2020 2072 6574 7572 6e20 5a65 726f       return Zero
-00015660: 5375 6d4e 6f72 6d61 6c52 5628 0a20 2020  SumNormalRV(.   
-00015670: 2020 2020 2020 2020 2069 6e70 7574 733d           inputs=
-00015680: 5b6e 6f72 6d61 6c5f 6469 7374 5f2c 2073  [normal_dist_, s
-00015690: 6967 6d61 5f2c 2073 7570 706f 7274 5f73  igma_, support_s
-000156a0: 6861 7065 5f5d 2c0a 2020 2020 2020 2020  hape_],.        
-000156b0: 2020 2020 6f75 7470 7574 733d 5b7a 6572      outputs=[zer
-000156c0: 6f73 756d 5f72 765f 2c20 7375 7070 6f72  osum_rv_, suppor
-000156d0: 745f 7368 6170 655f 5d2c 0a20 2020 2020  t_shape_],.     
-000156e0: 2020 2020 2020 206e 6469 6d5f 7375 7070         ndim_supp
-000156f0: 3d6e 5f7a 6572 6f73 756d 5f61 7865 732c  =n_zerosum_axes,
-00015700: 0a20 2020 2020 2020 2029 286e 6f72 6d61  .        )(norma
-00015710: 6c5f 6469 7374 2c20 7369 676d 612c 2073  l_dist, sigma, s
-00015720: 7570 706f 7274 5f73 6861 7065 290a 0a0a  upport_shape)...
-00015730: 405f 6368 616e 6765 5f64 6973 745f 7369  @_change_dist_si
-00015740: 7a65 2e72 6567 6973 7465 7228 5a65 726f  ze.register(Zero
-00015750: 5375 6d4e 6f72 6d61 6c52 5629 0a64 6566  SumNormalRV).def
-00015760: 2063 6861 6e67 655f 7a65 726f 7375 6d5f   change_zerosum_
-00015770: 7369 7a65 286f 702c 206e 6f72 6d61 6c5f  size(op, normal_
-00015780: 6469 7374 2c20 6e65 775f 7369 7a65 2c20  dist, new_size, 
-00015790: 6578 7061 6e64 3d46 616c 7365 293a 0a20  expand=False):. 
-000157a0: 2020 206e 6f72 6d61 6c5f 6469 7374 2c20     normal_dist, 
-000157b0: 7369 676d 612c 2073 7570 706f 7274 5f73  sigma, support_s
-000157c0: 6861 7065 203d 206e 6f72 6d61 6c5f 6469  hape = normal_di
-000157d0: 7374 2e6f 776e 6572 2e69 6e70 7574 730a  st.owner.inputs.
-000157e0: 0a20 2020 2069 6620 6578 7061 6e64 3a0a  .    if expand:.
-000157f0: 2020 2020 2020 2020 6f72 6967 696e 616c          original
-00015800: 5f73 6861 7065 203d 2074 7570 6c65 286e  _shape = tuple(n
-00015810: 6f72 6d61 6c5f 6469 7374 2e73 6861 7065  ormal_dist.shape
-00015820: 290a 2020 2020 2020 2020 6f6c 645f 7369  ).        old_si
-00015830: 7a65 203d 206f 7269 6769 6e61 6c5f 7368  ze = original_sh
-00015840: 6170 655b 3a20 6c65 6e28 6f72 6967 696e  ape[: len(origin
-00015850: 616c 5f73 6861 7065 2920 2d20 6f70 2e6e  al_shape) - op.n
-00015860: 6469 6d5f 7375 7070 5d0a 2020 2020 2020  dim_supp].      
-00015870: 2020 6e65 775f 7369 7a65 203d 2074 7570    new_size = tup
-00015880: 6c65 286e 6577 5f73 697a 6529 202b 206f  le(new_size) + o
-00015890: 6c64 5f73 697a 650a 0a20 2020 2072 6574  ld_size..    ret
-000158a0: 7572 6e20 5a65 726f 5375 6d4e 6f72 6d61  urn ZeroSumNorma
-000158b0: 6c2e 7276 5f6f 7028 0a20 2020 2020 2020  l.rv_op(.       
-000158c0: 2073 6967 6d61 3d73 6967 6d61 2c20 6e5f   sigma=sigma, n_
-000158d0: 7a65 726f 7375 6d5f 6178 6573 3d6f 702e  zerosum_axes=op.
-000158e0: 6e64 696d 5f73 7570 702c 2073 7570 706f  ndim_supp, suppo
-000158f0: 7274 5f73 6861 7065 3d73 7570 706f 7274  rt_shape=support
-00015900: 5f73 6861 7065 2c20 7369 7a65 3d6e 6577  _shape, size=new
-00015910: 5f73 697a 650a 2020 2020 290a 0a0a 405f  _size.    )...@_
-00015920: 6d6f 6d65 6e74 2e72 6567 6973 7465 7228  moment.register(
-00015930: 5a65 726f 5375 6d4e 6f72 6d61 6c52 5629  ZeroSumNormalRV)
-00015940: 0a64 6566 207a 6572 6f73 756d 6e6f 726d  .def zerosumnorm
-00015950: 616c 5f6d 6f6d 656e 7428 6f70 2c20 7276  al_moment(op, rv
-00015960: 2c20 2a72 765f 696e 7075 7473 293a 0a20  , *rv_inputs):. 
-00015970: 2020 2072 6574 7572 6e20 7074 2e7a 6572     return pt.zer
-00015980: 6f73 5f6c 696b 6528 7276 290a 0a0a 405f  os_like(rv)...@_
-00015990: 6465 6661 756c 745f 7472 616e 7366 6f72  default_transfor
-000159a0: 6d2e 7265 6769 7374 6572 285a 6572 6f53  m.register(ZeroS
-000159b0: 756d 4e6f 726d 616c 5256 290a 6465 6620  umNormalRV).def 
-000159c0: 7a65 726f 7375 6d5f 6465 6661 756c 745f  zerosum_default_
-000159d0: 7472 616e 7366 6f72 6d28 6f70 2c20 7276  transform(op, rv
-000159e0: 293a 0a20 2020 206e 5f7a 6572 6f73 756d  ):.    n_zerosum
-000159f0: 5f61 7865 7320 3d20 7475 706c 6528 6e70  _axes = tuple(np
-00015a00: 2e61 7261 6e67 6528 2d6f 702e 6e64 696d  .arange(-op.ndim
-00015a10: 5f73 7570 702c 2030 2929 0a20 2020 2072  _supp, 0)).    r
-00015a20: 6574 7572 6e20 5a65 726f 5375 6d54 7261  eturn ZeroSumTra
-00015a30: 6e73 666f 726d 286e 5f7a 6572 6f73 756d  nsform(n_zerosum
-00015a40: 5f61 7865 7329 0a0a 0a40 5f6c 6f67 7072  _axes)...@_logpr
-00015a50: 6f62 2e72 6567 6973 7465 7228 5a65 726f  ob.register(Zero
-00015a60: 5375 6d4e 6f72 6d61 6c52 5629 0a64 6566  SumNormalRV).def
-00015a70: 207a 6572 6f73 756d 6e6f 726d 616c 5f6c   zerosumnormal_l
-00015a80: 6f67 7028 6f70 2c20 7661 6c75 6573 2c20  ogp(op, values, 
-00015a90: 6e6f 726d 616c 5f64 6973 742c 2073 6967  normal_dist, sig
-00015aa0: 6d61 2c20 7375 7070 6f72 745f 7368 6170  ma, support_shap
-00015ab0: 652c 202a 2a6b 7761 7267 7329 3a0a 2020  e, **kwargs):.  
-00015ac0: 2020 2876 616c 7565 2c29 203d 2076 616c    (value,) = val
-00015ad0: 7565 730a 2020 2020 7368 6170 6520 3d20  ues.    shape = 
-00015ae0: 7661 6c75 652e 7368 6170 650a 2020 2020  value.shape.    
-00015af0: 6e5f 7a65 726f 7375 6d5f 6178 6573 203d  n_zerosum_axes =
-00015b00: 206f 702e 6e64 696d 5f73 7570 700a 0a20   op.ndim_supp.. 
-00015b10: 2020 205f 6465 675f 6672 6565 5f73 7570     _deg_free_sup
-00015b20: 706f 7274 5f73 6861 7065 203d 2070 742e  port_shape = pt.
-00015b30: 696e 635f 7375 6274 656e 736f 7228 7368  inc_subtensor(sh
-00015b40: 6170 655b 2d6e 5f7a 6572 6f73 756d 5f61  ape[-n_zerosum_a
-00015b50: 7865 733a 5d2c 202d 3129 0a20 2020 205f  xes:], -1).    _
-00015b60: 6675 6c6c 5f73 697a 6520 3d20 7074 2e70  full_size = pt.p
-00015b70: 726f 6428 7368 6170 6529 0a20 2020 205f  rod(shape).    _
-00015b80: 6465 6772 6565 735f 6f66 5f66 7265 6564  degrees_of_freed
-00015b90: 6f6d 203d 2070 742e 7072 6f64 285f 6465  om = pt.prod(_de
-00015ba0: 675f 6672 6565 5f73 7570 706f 7274 5f73  g_free_support_s
-00015bb0: 6861 7065 290a 0a20 2020 207a 6572 6f73  hape)..    zeros
-00015bc0: 756d 7320 3d20 5b0a 2020 2020 2020 2020  ums = [.        
-00015bd0: 7074 2e61 6c6c 2870 742e 6973 636c 6f73  pt.all(pt.isclos
-00015be0: 6528 7074 2e6d 6561 6e28 7661 6c75 652c  e(pt.mean(value,
-00015bf0: 2061 7869 733d 2d61 7869 7320 2d20 3129   axis=-axis - 1)
-00015c00: 2c20 302c 2061 746f 6c3d 3165 2d39 2929  , 0, atol=1e-9))
-00015c10: 0a20 2020 2020 2020 2066 6f72 2061 7869  .        for axi
-00015c20: 7320 696e 2072 616e 6765 286e 5f7a 6572  s in range(n_zer
-00015c30: 6f73 756d 5f61 7865 7329 0a20 2020 205d  osum_axes).    ]
-00015c40: 0a0a 2020 2020 6f75 7420 3d20 7074 2e73  ..    out = pt.s
-00015c50: 756d 280a 2020 2020 2020 2020 706d 2e6c  um(.        pm.l
-00015c60: 6f67 7028 6e6f 726d 616c 5f64 6973 742c  ogp(normal_dist,
-00015c70: 2076 616c 7565 2920 2a20 5f64 6567 7265   value) * _degre
-00015c80: 6573 5f6f 665f 6672 6565 646f 6d20 2f20  es_of_freedom / 
-00015c90: 5f66 756c 6c5f 7369 7a65 2c0a 2020 2020  _full_size,.    
-00015ca0: 2020 2020 6178 6973 3d74 7570 6c65 286e      axis=tuple(n
-00015cb0: 702e 6172 616e 6765 282d 6e5f 7a65 726f  p.arange(-n_zero
-00015cc0: 7375 6d5f 6178 6573 2c20 3029 292c 0a20  sum_axes, 0)),. 
-00015cd0: 2020 2029 0a0a 2020 2020 7265 7475 726e     )..    return
-00015ce0: 2063 6865 636b 5f70 6172 616d 6574 6572   check_parameter
-00015cf0: 7328 6f75 742c 202a 7a65 726f 7375 6d73  s(out, *zerosums
-00015d00: 2c20 6d73 673d 226d 6561 6e28 7661 6c75  , msg="mean(valu
-00015d10: 652c 2061 7869 733d 6e5f 7a65 726f 7375  e, axis=n_zerosu
-00015d20: 6d5f 6178 6573 2920 3d20 3022 290a       m_axes) = 0").
+000133e0: 3d3d 3d3d 0a0a 2020 2020 5061 7261 6d65  ====..    Parame
+000133f0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00013400: 2d2d 2d0a 2020 2020 616c 7068 6120 3a20  ---.    alpha : 
+00013410: 7465 6e73 6f72 5f6c 696b 6520 6f66 2066  tensor_like of f
+00013420: 6c6f 6174 0a20 2020 2020 2020 2043 6f6e  loat.        Con
+00013430: 6365 6e74 7261 7469 6f6e 2070 6172 616d  centration param
+00013440: 6574 6572 2028 616c 7068 6120 3e20 3029  eter (alpha > 0)
+00013450: 2e0a 2020 2020 4b20 3a20 7465 6e73 6f72  ..    K : tensor
+00013460: 5f6c 696b 6520 6f66 2069 6e74 0a20 2020  _like of int.   
+00013470: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
+00013480: 6f66 2022 7374 6963 6b73 2220 746f 2062  of "sticks" to b
+00013490: 7265 616b 206f 6666 2066 726f 6d20 616e  reak off from an
+000134a0: 2069 6e69 7469 616c 206f 6e65 2d75 6e69   initial one-uni
+000134b0: 7420 7374 6963 6b2e 2054 6865 206c 656e  t stick. The len
+000134c0: 6774 6820 6f66 2074 6865 2077 6569 6768  gth of the weigh
+000134d0: 740a 2020 2020 2020 2020 7665 6374 6f72  t.        vector
+000134e0: 2069 7320 4b20 2b20 312c 2077 6865 7265   is K + 1, where
+000134f0: 2074 6865 206c 6173 7420 7765 6967 6874   the last weight
+00013500: 2069 7320 6f6e 6520 6d69 6e75 7320 7468   is one minus th
+00013510: 6520 7375 6d20 6f66 2061 6c6c 2074 6865  e sum of all the
+00013520: 2066 6972 7374 2073 7469 636b 732e 0a0a   first sticks...
+00013530: 2020 2020 5265 6665 7265 6e63 6573 0a20      References. 
+00013540: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00013550: 2020 2e2e 205b 315d 2049 7368 7761 7261    .. [1] Ishwara
+00013560: 6e2c 2048 2e2c 2026 204a 616d 6573 2c20  n, H., & James, 
+00013570: 4c2e 2046 2e20 2832 3030 3129 2e20 4769  L. F. (2001). Gi
+00013580: 6262 7320 7361 6d70 6c69 6e67 206d 6574  bbs sampling met
+00013590: 686f 6473 2066 6f72 2073 7469 636b 2d62  hods for stick-b
+000135a0: 7265 616b 696e 6720 7072 696f 7273 2e0a  reaking priors..
+000135b0: 2020 2020 2020 2020 2020 204a 6f75 726e             Journ
+000135c0: 616c 206f 6620 7468 6520 416d 6572 6963  al of the Americ
+000135d0: 616e 2053 7461 7469 7374 6963 616c 2041  an Statistical A
+000135e0: 7373 6f63 6961 7469 6f6e 2c20 3936 2834  ssociation, 96(4
+000135f0: 3533 292c 2031 3631 2d31 3733 2e0a 0a20  53), 161-173... 
+00013600: 2020 202e 2e20 5b32 5d20 4dc3 bc6c 6c65     .. [2] M..lle
+00013610: 722c 2050 2e2c 2051 7569 6e74 616e 612c  r, P., Quintana,
+00013620: 2046 2e20 412e 2c20 4a61 7261 2c20 412e   F. A., Jara, A.
+00013630: 2c20 2620 4861 6e73 6f6e 2c20 542e 2028  , & Hanson, T. (
+00013640: 3230 3135 292e 2042 6179 6573 6961 6e20  2015). Bayesian 
+00013650: 6e6f 6e70 6172 616d 6574 7269 6320 6461  nonparametric da
+00013660: 7461 0a20 2020 2020 2020 2020 2020 616e  ta.           an
+00013670: 616c 7973 6973 2e20 4e65 7720 596f 726b  alysis. New York
+00013680: 3a20 5370 7269 6e67 6572 2e0a 2020 2020  : Springer..    
+00013690: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
+000136a0: 7374 6963 6b62 7265 616b 696e 6777 6569  stickbreakingwei
+000136b0: 6768 7473 0a0a 2020 2020 4063 6c61 7373  ghts..    @class
+000136c0: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
+000136d0: 6973 7428 636c 732c 2061 6c70 6861 2c20  ist(cls, alpha, 
+000136e0: 4b2c 202a 6172 6773 2c20 2a2a 6b77 6172  K, *args, **kwar
+000136f0: 6773 293a 0a20 2020 2020 2020 2061 6c70  gs):.        alp
+00013700: 6861 203d 2070 742e 6173 5f74 656e 736f  ha = pt.as_tenso
+00013710: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
+00013720: 5828 616c 7068 6129 290a 2020 2020 2020  X(alpha)).      
+00013730: 2020 4b20 3d20 7074 2e61 735f 7465 6e73    K = pt.as_tens
+00013740: 6f72 5f76 6172 6961 626c 6528 696e 7458  or_variable(intX
+00013750: 284b 2929 0a0a 2020 2020 2020 2020 7265  (K))..        re
+00013760: 7475 726e 2073 7570 6572 2829 2e64 6973  turn super().dis
+00013770: 7428 5b61 6c70 6861 2c20 4b5d 2c20 2a2a  t([alpha, K], **
+00013780: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+00013790: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
+000137a0: 2c20 616c 7068 612c 204b 293a 0a20 2020  , alpha, K):.   
+000137b0: 2020 2020 2061 6c70 6861 203d 2061 6c70       alpha = alp
+000137c0: 6861 5b2e 2e2e 2c20 6e70 2e6e 6577 6178  ha[..., np.newax
+000137d0: 6973 5d0a 2020 2020 2020 2020 6d6f 6d65  is].        mome
+000137e0: 6e74 203d 2028 616c 7068 6120 2f20 2831  nt = (alpha / (1
+000137f0: 202b 2061 6c70 6861 2929 202a 2a20 7074   + alpha)) ** pt
+00013800: 2e61 7261 6e67 6528 4b29 0a20 2020 2020  .arange(K).     
+00013810: 2020 206d 6f6d 656e 7420 2a3d 2031 202f     moment *= 1 /
+00013820: 2028 3120 2b20 616c 7068 6129 0a20 2020   (1 + alpha).   
+00013830: 2020 2020 206d 6f6d 656e 7420 3d20 7074       moment = pt
+00013840: 2e63 6f6e 6361 7465 6e61 7465 285b 6d6f  .concatenate([mo
+00013850: 6d65 6e74 2c20 2861 6c70 6861 202f 2028  ment, (alpha / (
+00013860: 3120 2b20 616c 7068 6129 2920 2a2a 204b  1 + alpha)) ** K
+00013870: 5d2c 2061 7869 733d 2d31 290a 2020 2020  ], axis=-1).    
+00013880: 2020 2020 6966 206e 6f74 2072 765f 7369      if not rv_si
+00013890: 7a65 5f69 735f 6e6f 6e65 2873 697a 6529  ze_is_none(size)
+000138a0: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+000138b0: 6d65 6e74 5f73 697a 6520 3d20 7074 2e63  ment_size = pt.c
+000138c0: 6f6e 6361 7465 6e61 7465 280a 2020 2020  oncatenate(.    
+000138d0: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000138f0: 2020 7369 7a65 2c0a 2020 2020 2020 2020    size,.        
+00013900: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+00013910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013920: 2020 2020 2020 4b20 2b20 312c 0a20 2020        K + 1,.   
+00013930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013940: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+00013950: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00013960: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00013970: 6d6f 6d65 6e74 203d 2070 742e 6675 6c6c  moment = pt.full
+00013980: 286d 6f6d 656e 745f 7369 7a65 2c20 6d6f  (moment_size, mo
+00013990: 6d65 6e74 290a 0a20 2020 2020 2020 2072  ment)..        r
+000139a0: 6574 7572 6e20 6d6f 6d65 6e74 0a0a 2020  eturn moment..  
+000139b0: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
+000139c0: 2c20 616c 7068 612c 204b 293a 0a20 2020  , alpha, K):.   
+000139d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000139e0: 2043 616c 6375 6c61 7465 206c 6f67 2d70   Calculate log-p
+000139f0: 726f 6261 6269 6c69 7479 206f 6620 7468  robability of th
+00013a00: 6520 6469 7374 7269 6275 7469 6f6e 2069  e distribution i
+00013a10: 6e64 7563 6564 2066 726f 6d20 7468 6520  nduced from the 
+00013a20: 7374 6963 6b2d 6272 6561 6b69 6e67 2070  stick-breaking p
+00013a30: 726f 6365 7373 0a20 2020 2020 2020 2061  rocess.        a
+00013a40: 7420 7370 6563 6966 6965 6420 7661 6c75  t specified valu
+00013a50: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
+00013a60: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+00013a70: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00013a80: 2020 7661 6c75 653a 206e 756d 6572 6963    value: numeric
+00013a90: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
+00013aa0: 7565 2066 6f72 2077 6869 6368 206c 6f67  ue for which log
+00013ab0: 2d70 726f 6261 6269 6c69 7479 2069 7320  -probability is 
+00013ac0: 6361 6c63 756c 6174 6564 2e0a 0a20 2020  calculated...   
+00013ad0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
+00013ae0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
+00013af0: 2020 2020 2054 656e 736f 7256 6172 6961       TensorVaria
+00013b00: 626c 650a 2020 2020 2020 2020 2222 220a  ble.        """.
+00013b10: 2020 2020 2020 2020 6c6f 6770 203d 202d          logp = -
+00013b20: 7074 2e73 756d 280a 2020 2020 2020 2020  pt.sum(.        
+00013b30: 2020 2020 7074 2e6c 6f67 280a 2020 2020      pt.log(.    
+00013b40: 2020 2020 2020 2020 2020 2020 7074 2e63              pt.c
+00013b50: 756d 7375 6d28 0a20 2020 2020 2020 2020  umsum(.         
+00013b60: 2020 2020 2020 2020 2020 2076 616c 7565             value
+00013b70: 5b2e 2e2e 2c20 3a3a 2d31 5d2c 0a20 2020  [..., ::-1],.   
+00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b90: 2061 7869 733d 2d31 2c0a 2020 2020 2020   axis=-1,.      
+00013ba0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00013bb0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00013bc0: 2020 2020 2020 2061 7869 733d 2d31 2c0a         axis=-1,.
+00013bd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00013be0: 2020 6c6f 6770 202b 3d20 2d4b 202a 2062    logp += -K * b
+00013bf0: 6574 616c 6e28 312c 2061 6c70 6861 290a  etaln(1, alpha).
+00013c00: 2020 2020 2020 2020 6c6f 6770 202b 3d20          logp += 
+00013c10: 616c 7068 6120 2a20 7074 2e6c 6f67 2876  alpha * pt.log(v
+00013c20: 616c 7565 5b2e 2e2e 2c20 2d31 5d29 0a0a  alue[..., -1])..
+00013c30: 2020 2020 2020 2020 6c6f 6770 203d 2070          logp = p
+00013c40: 742e 7377 6974 6368 280a 2020 2020 2020  t.switch(.      
+00013c50: 2020 2020 2020 7074 2e6f 725f 280a 2020        pt.or_(.  
+00013c60: 2020 2020 2020 2020 2020 2020 2020 7074                pt
+00013c70: 2e61 6e79 280a 2020 2020 2020 2020 2020  .any(.          
+00013c80: 2020 2020 2020 2020 2020 7074 2e61 6e64            pt.and
+00013c90: 5f28 7074 2e6c 6528 7661 6c75 652c 2030  _(pt.le(value, 0
+00013ca0: 292c 2070 742e 6765 2876 616c 7565 2c20  ), pt.ge(value, 
+00013cb0: 3129 292c 0a20 2020 2020 2020 2020 2020  1)),.           
+00013cc0: 2020 2020 2020 2020 2061 7869 733d 2d31           axis=-1
+00013cd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013ce0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00013cf0: 2020 2020 2070 742e 6f72 5f28 0a20 2020       pt.or_(.   
+00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d10: 2070 742e 6269 7477 6973 655f 6e6f 7428   pt.bitwise_not(
+00013d20: 7074 2e61 6c6c 636c 6f73 6528 7661 6c75  pt.allclose(valu
+00013d30: 652e 7375 6d28 2d31 292c 2031 2929 2c0a  e.sum(-1), 1)),.
+00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d50: 2020 2020 7074 2e6e 6571 2876 616c 7565      pt.neq(value
+00013d60: 2e73 6861 7065 5b2d 315d 2c20 4b20 2b20  .shape[-1], K + 
+00013d70: 3129 2c0a 2020 2020 2020 2020 2020 2020  1),.            
+00013d80: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00013d90: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+00013da0: 2020 2d6e 702e 696e 662c 0a20 2020 2020    -np.inf,.     
+00013db0: 2020 2020 2020 206c 6f67 702c 0a20 2020         logp,.   
+00013dc0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00013dd0: 7265 7475 726e 2063 6865 636b 5f70 6172  return check_par
+00013de0: 616d 6574 6572 7328 0a20 2020 2020 2020  ameters(.       
+00013df0: 2020 2020 206c 6f67 702c 0a20 2020 2020       logp,.     
+00013e00: 2020 2020 2020 2061 6c70 6861 203e 2030         alpha > 0
+00013e10: 2c0a 2020 2020 2020 2020 2020 2020 4b20  ,.            K 
+00013e20: 3e20 302c 0a20 2020 2020 2020 2020 2020  > 0,.           
+00013e30: 206d 7367 3d22 616c 7068 6120 3e20 302c   msg="alpha > 0,
+00013e40: 204b 203e 2030 222c 0a20 2020 2020 2020   K > 0",.       
+00013e50: 2029 0a0a 0a63 6c61 7373 205a 6572 6f53   )...class ZeroS
+00013e60: 756d 4e6f 726d 616c 5256 2853 796d 626f  umNormalRV(Symbo
+00013e70: 6c69 6352 616e 646f 6d56 6172 6961 626c  licRandomVariabl
+00013e80: 6529 3a0a 2020 2020 2222 225a 6572 6f53  e):.    """ZeroS
+00013e90: 756d 4e6f 726d 616c 2072 616e 646f 6d20  umNormal random 
+00013ea0: 7661 7269 6162 6c65 2222 220a 0a20 2020  variable"""..   
+00013eb0: 205f 7072 696e 745f 6e61 6d65 203d 2028   _print_name = (
+00013ec0: 225a 6572 6f53 756d 4e6f 726d 616c 222c  "ZeroSumNormal",
+00013ed0: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
+00013ee0: 7b5a 6572 6f53 756d 4e6f 726d 616c 7d22  {ZeroSumNormal}"
+00013ef0: 290a 2020 2020 6465 6661 756c 745f 6f75  ).    default_ou
+00013f00: 7470 7574 203d 2030 0a0a 0a63 6c61 7373  tput = 0...class
+00013f10: 205a 6572 6f53 756d 4e6f 726d 616c 2844   ZeroSumNormal(D
+00013f20: 6973 7472 6962 7574 696f 6e29 3a0a 2020  istribution):.  
+00013f30: 2020 7222 2222 0a20 2020 205a 6572 6f53    r""".    ZeroS
+00013f40: 756d 4e6f 726d 616c 2064 6973 7472 6962  umNormal distrib
+00013f50: 7574 696f 6e2c 2069 2e65 204e 6f72 6d61  ution, i.e Norma
+00013f60: 6c20 6469 7374 7269 6275 7469 6f6e 2077  l distribution w
+00013f70: 6865 7265 206f 6e65 206f 720a 2020 2020  here one or.    
+00013f80: 7365 7665 7261 6c20 6178 6573 2061 7265  several axes are
+00013f90: 2063 6f6e 7374 7261 696e 6564 2074 6f20   constrained to 
+00013fa0: 7375 6d20 746f 207a 6572 6f2e 0a20 2020  sum to zero..   
+00013fb0: 2042 7920 6465 6661 756c 742c 2074 6865   By default, the
+00013fc0: 206c 6173 7420 6178 6973 2069 7320 636f   last axis is co
+00013fd0: 6e73 7472 6169 6e65 6420 746f 2073 756d  nstrained to sum
+00013fe0: 2074 6f20 7a65 726f 2e0a 2020 2020 5365   to zero..    Se
+00013ff0: 6520 606e 5f7a 6572 6f73 756d 5f61 7865  e `n_zerosum_axe
+00014000: 7360 206b 7761 7267 2066 6f72 206d 6f72  s` kwarg for mor
+00014010: 6520 6465 7461 696c 732e 0a0a 2020 2020  e details...    
+00014020: 2e2e 206d 6174 683a 3a0a 0a20 2020 2020  .. math::..     
+00014030: 2020 205c 6265 6769 6e7b 616c 6967 6e2a     \begin{align*
+00014040: 7d0a 2020 2020 2020 2020 2020 2020 5a53  }.            ZS
+00014050: 4e28 5c73 6967 6d61 2920 3d20 4e20 5c42  N(\sigma) = N \B
+00014060: 6967 2820 302c 205c 7369 676d 615e 3220  ig( 0, \sigma^2 
+00014070: 2849 202d 205c 7466 7261 637b 317d 7b6e  (I - \tfrac{1}{n
+00014080: 7d4a 2920 5c42 6967 2920 5c5c 0a20 2020  }J) \Big) \\.   
+00014090: 2020 2020 2020 2020 205c 7465 7874 7b77           \text{w
+000140a0: 6865 7265 7d20 5c20 7e20 4a5f 7b69 6a7d  here} \ ~ J_{ij}
+000140b0: 203d 2031 205c 207e 205c 7465 7874 7b61   = 1 \ ~ \text{a
+000140c0: 6e64 7d20 5c5c 0a20 2020 2020 2020 2020  nd} \\.         
+000140d0: 2020 206e 203d 205c 7465 7874 7b6e 6272     n = \text{nbr
+000140e0: 206f 6620 7a65 726f 2d73 756d 2061 7865   of zero-sum axe
+000140f0: 737d 0a20 2020 2020 2020 205c 656e 647b  s}.        \end{
+00014100: 616c 6967 6e2a 7d0a 0a20 2020 2050 6172  align*}..    Par
+00014110: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00014120: 2d2d 2d2d 2d2d 0a20 2020 2073 6967 6d61  ------.    sigma
+00014130: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+00014140: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
+00014150: 5363 616c 6520 7061 7261 6d65 7465 7220  Scale parameter 
+00014160: 2873 6967 6d61 203e 2030 292e 0a20 2020  (sigma > 0)..   
+00014170: 2020 2020 2049 7427 7320 6163 7475 616c       It's actual
+00014180: 6c79 2074 6865 2073 7461 6e64 6172 6420  ly the standard 
+00014190: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
+000141a0: 2075 6e64 6572 6c79 696e 672c 2075 6e63   underlying, unc
+000141b0: 6f6e 7374 7261 696e 6564 204e 6f72 6d61  onstrained Norma
+000141c0: 6c20 6469 7374 7269 6275 7469 6f6e 2e0a  l distribution..
+000141d0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+000141e0: 2074 6f20 3120 6966 206e 6f74 2073 7065   to 1 if not spe
+000141f0: 6369 6669 6564 2e0a 2020 2020 2020 2020  cified..        
+00014200: 466f 7220 6e6f 772c 2060 6073 6967 6d61  For now, ``sigma
+00014210: 6060 2068 6173 2074 6f20 6265 2061 2073  `` has to be a s
+00014220: 6361 6c61 722c 2074 6f20 656e 7375 7265  calar, to ensure
+00014230: 2074 6865 207a 6572 6f2d 7375 6d20 636f   the zero-sum co
+00014240: 6e73 7472 6169 6e74 2e0a 2020 2020 6e5f  nstraint..    n_
+00014250: 7a65 726f 7375 6d5f 6178 6573 3a20 696e  zerosum_axes: in
+00014260: 742c 2064 6566 6175 6c74 7320 746f 2031  t, defaults to 1
+00014270: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
+00014280: 6f66 2061 7865 7320 616c 6f6e 6720 7768  of axes along wh
+00014290: 6963 6820 7468 6520 7a65 726f 2d73 756d  ich the zero-sum
+000142a0: 2063 6f6e 7374 7261 696e 7420 6973 2065   constraint is e
+000142b0: 6e66 6f72 6365 642c 2073 7461 7274 696e  nforced, startin
+000142c0: 6720 6672 6f6d 2074 6865 2072 6967 6874  g from the right
+000142d0: 6d6f 7374 2070 6f73 6974 696f 6e2e 0a20  most position.. 
+000142e0: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+000142f0: 746f 2031 2c20 692e 6520 7468 6520 7269  to 1, i.e the ri
+00014300: 6768 746d 6f73 7420 6178 6973 2e0a 2020  ghtmost axis..  
+00014310: 2020 7a65 726f 7375 6d5f 6178 6573 3a20    zerosum_axes: 
+00014320: 696e 742c 2064 6570 7265 6361 7465 6420  int, deprecated 
+00014330: 706c 6561 7365 2075 7365 206e 5f7a 6572  please use n_zer
+00014340: 6f73 756d 5f61 7865 7320 6173 2069 7473  osum_axes as its
+00014350: 2073 7563 6365 7373 6f72 0a20 2020 2064   successor.    d
+00014360: 696d 733a 2073 6571 7565 6e63 6520 6f66  ims: sequence of
+00014370: 2073 7472 696e 6773 2c20 6f70 7469 6f6e   strings, option
+00014380: 616c 0a20 2020 2020 2020 2044 696d 656e  al.        Dimen
+00014390: 7369 6f6e 206e 616d 6573 206f 6620 7468  sion names of th
+000143a0: 6520 6469 7374 7269 6275 7469 6f6e 2e20  e distribution. 
+000143b0: 576f 726b 7320 7468 6520 7361 6d65 2061  Works the same a
+000143c0: 7320 666f 7220 6f74 6865 7220 5079 4d43  s for other PyMC
+000143d0: 2064 6973 7472 6962 7574 696f 6e73 2e0a   distributions..
+000143e0: 2020 2020 2020 2020 4e65 6365 7373 6172          Necessar
+000143f0: 7920 6966 2060 6073 6861 7065 6060 2069  y if ``shape`` i
+00014400: 7320 6e6f 7420 7061 7373 6564 2e0a 2020  s not passed..  
+00014410: 2020 7368 6170 653a 2074 7570 6c65 206f    shape: tuple o
+00014420: 6620 696e 7465 6765 7273 2c20 6f70 7469  f integers, opti
+00014430: 6f6e 616c 0a20 2020 2020 2020 2053 6861  onal.        Sha
+00014440: 7065 206f 6620 7468 6520 6469 7374 7269  pe of the distri
+00014450: 6275 7469 6f6e 2e20 576f 726b 7320 7468  bution. Works th
+00014460: 6520 7361 6d65 2061 7320 666f 7220 6f74  e same as for ot
+00014470: 6865 7220 5079 4d43 2064 6973 7472 6962  her PyMC distrib
+00014480: 7574 696f 6e73 2e0a 2020 2020 2020 2020  utions..        
+00014490: 4e65 6365 7373 6172 7920 6966 2060 6064  Necessary if ``d
+000144a0: 696d 7360 6020 6f72 2060 606f 6273 6572  ims`` or ``obser
+000144b0: 7665 6460 6020 6973 206e 6f74 2070 6173  ved`` is not pas
+000144c0: 7365 642e 0a0a 2020 2020 5761 726e 696e  sed...    Warnin
+000144d0: 6773 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  gs.    --------.
+000144e0: 2020 2020 6060 7369 676d 6160 6020 6861      ``sigma`` ha
+000144f0: 7320 746f 2062 6520 6120 7363 616c 6172  s to be a scalar
+00014500: 2c20 746f 2065 6e73 7572 6520 7468 6520  , to ensure the 
+00014510: 7a65 726f 2d73 756d 2063 6f6e 7374 7261  zero-sum constra
+00014520: 696e 742e 0a20 2020 2054 6865 2061 6269  int..    The abi
+00014530: 6c69 7479 2074 6f20 7370 6563 6966 7920  lity to specify 
+00014540: 6120 7665 6374 6f72 206f 6620 6060 7369  a vector of ``si
+00014550: 676d 6160 6020 6d61 7920 6265 2061 6464  gma`` may be add
+00014560: 6564 2069 6e20 6675 7475 7265 2076 6572  ed in future ver
+00014570: 7369 6f6e 732e 0a0a 2020 2020 6060 6e5f  sions...    ``n_
+00014580: 7a65 726f 7375 6d5f 6178 6573 6060 2068  zerosum_axes`` h
+00014590: 6173 2074 6f20 6265 203e 2030 2e20 4966  as to be > 0. If
+000145a0: 2079 6f75 2077 616e 7420 7468 6520 6265   you want the be
+000145b0: 6861 7669 6f72 206f 6620 6060 6e5f 7a65  havior of ``n_ze
+000145c0: 726f 7375 6d5f 6178 6573 203d 2030 6060  rosum_axes = 0``
+000145d0: 2c0a 2020 2020 6a75 7374 2075 7365 2060  ,.    just use `
+000145e0: 6070 6d2e 4e6f 726d 616c 6060 2e0a 0a20  `pm.Normal``... 
+000145f0: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00014600: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6566  --------.    Def
+00014610: 696e 6520 6120 605a 6572 6f53 756d 4e6f  ine a `ZeroSumNo
+00014620: 726d 616c 6020 7661 7269 6162 6c65 2c20  rmal` variable, 
+00014630: 7769 7468 2060 7369 676d 613d 3160 2061  with `sigma=1` a
+00014640: 6e64 0a20 2020 2060 6e5f 7a65 726f 7375  nd.    `n_zerosu
+00014650: 6d5f 6178 6573 3d31 6020 2062 7920 6465  m_axes=1`  by de
+00014660: 6661 756c 743a 3a0a 0a20 2020 2020 2020  fault::..       
+00014670: 2043 4f4f 5244 5320 3d20 7b0a 2020 2020   COORDS = {.    
+00014680: 2020 2020 2020 2020 2272 6567 696f 6e73          "regions
+00014690: 223a 205b 2261 222c 2022 6222 2c20 2263  ": ["a", "b", "c
+000146a0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+000146b0: 2261 6e73 7765 7273 223a 205b 2279 6573  "answers": ["yes
+000146c0: 222c 2022 6e6f 222c 2022 7768 6174 6576  ", "no", "whatev
+000146d0: 6572 222c 2022 646f 6e27 7420 756e 6465  er", "don't unde
+000146e0: 7273 7461 6e64 2071 7565 7374 696f 6e22  rstand question"
+000146f0: 5d2c 0a20 2020 2020 2020 207d 0a20 2020  ],.        }.   
+00014700: 2020 2020 2077 6974 6820 706d 2e4d 6f64       with pm.Mod
+00014710: 656c 2863 6f6f 7264 733d 434f 4f52 4453  el(coords=COORDS
+00014720: 2920 6173 206d 3a0a 2020 2020 2020 2020  ) as m:.        
+00014730: 2020 2020 2320 7468 6520 7a65 726f 2073      # the zero s
+00014740: 756d 2061 7869 7320 7769 6c6c 2062 6520  um axis will be 
+00014750: 2761 6e73 7765 7273 270a 2020 2020 2020  'answers'.      
+00014760: 2020 2020 2020 7620 3d20 706d 2e5a 6572        v = pm.Zer
+00014770: 6f53 756d 4e6f 726d 616c 2822 7622 2c20  oSumNormal("v", 
+00014780: 6469 6d73 3d28 2272 6567 696f 6e73 222c  dims=("regions",
+00014790: 2022 616e 7377 6572 7322 2929 0a0a 2020   "answers"))..  
+000147a0: 2020 2020 2020 7769 7468 2070 6d2e 4d6f        with pm.Mo
+000147b0: 6465 6c28 636f 6f72 6473 3d43 4f4f 5244  del(coords=COORD
+000147c0: 5329 2061 7320 6d3a 0a20 2020 2020 2020  S) as m:.       
+000147d0: 2020 2020 2023 2074 6865 207a 6572 6f20       # the zero 
+000147e0: 7375 6d20 6178 6573 2077 696c 6c20 6265  sum axes will be
+000147f0: 2027 616e 7377 6572 7327 2061 6e64 2027   'answers' and '
+00014800: 7265 6769 6f6e 7327 0a20 2020 2020 2020  regions'.       
+00014810: 2020 2020 2076 203d 2070 6d2e 5a65 726f       v = pm.Zero
+00014820: 5375 6d4e 6f72 6d61 6c28 2276 222c 2064  SumNormal("v", d
+00014830: 696d 733d 2822 7265 6769 6f6e 7322 2c20  ims=("regions", 
+00014840: 2261 6e73 7765 7273 2229 2c20 6e5f 7a65  "answers"), n_ze
+00014850: 726f 7375 6d5f 6178 6573 3d32 290a 0a20  rosum_axes=2).. 
+00014860: 2020 2020 2020 2077 6974 6820 706d 2e4d         with pm.M
+00014870: 6f64 656c 2863 6f6f 7264 733d 434f 4f52  odel(coords=COOR
+00014880: 4453 2920 6173 206d 3a0a 2020 2020 2020  DS) as m:.      
+00014890: 2020 2020 2020 2320 7468 6520 7a65 726f        # the zero
+000148a0: 2073 756d 2061 7865 7320 7769 6c6c 2062   sum axes will b
+000148b0: 6520 7468 6520 6c61 7374 2074 776f 0a20  e the last two. 
+000148c0: 2020 2020 2020 2020 2020 2076 203d 2070             v = p
+000148d0: 6d2e 5a65 726f 5375 6d4e 6f72 6d61 6c28  m.ZeroSumNormal(
+000148e0: 2276 222c 2073 6861 7065 3d28 332c 2034  "v", shape=(3, 4
+000148f0: 2c20 3529 2c20 6e5f 7a65 726f 7375 6d5f  , 5), n_zerosum_
+00014900: 6178 6573 3d32 290a 2020 2020 2222 220a  axes=2).    """.
+00014910: 2020 2020 7276 5f74 7970 6520 3d20 5a65      rv_type = Ze
+00014920: 726f 5375 6d4e 6f72 6d61 6c52 560a 0a20  roSumNormalRV.. 
+00014930: 2020 2064 6566 205f 5f6e 6577 5f5f 280a     def __new__(.
+00014940: 2020 2020 2020 2020 636c 732c 202a 6172          cls, *ar
+00014950: 6773 2c20 7a65 726f 7375 6d5f 6178 6573  gs, zerosum_axes
+00014960: 3d4e 6f6e 652c 206e 5f7a 6572 6f73 756d  =None, n_zerosum
+00014970: 5f61 7865 733d 4e6f 6e65 2c20 7375 7070  _axes=None, supp
+00014980: 6f72 745f 7368 6170 653d 4e6f 6e65 2c20  ort_shape=None, 
+00014990: 6469 6d73 3d4e 6f6e 652c 202a 2a6b 7761  dims=None, **kwa
+000149a0: 7267 730a 2020 2020 293a 0a20 2020 2020  rgs.    ):.     
+000149b0: 2020 2069 6620 7a65 726f 7375 6d5f 6178     if zerosum_ax
+000149c0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+000149d0: 2020 2020 2020 2020 2020 2020 6e5f 7a65              n_ze
+000149e0: 726f 7375 6d5f 6178 6573 203d 207a 6572  rosum_axes = zer
+000149f0: 6f73 756d 5f61 7865 730a 2020 2020 2020  osum_axes.      
+00014a00: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00014a10: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
+00014a20: 2020 2020 2022 5468 6520 277a 6572 6f73       "The 'zeros
+00014a30: 756d 5f61 7865 7327 2070 6172 616d 6574  um_axes' paramet
+00014a40: 6572 2069 7320 6465 7072 6563 6174 6564  er is deprecated
+00014a50: 2e20 5573 6520 276e 5f7a 6572 6f73 756d  . Use 'n_zerosum
+00014a60: 5f61 7865 7327 2069 6e73 7465 6164 2e22  _axes' instead."
+00014a70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00014a80: 2020 4465 7072 6563 6174 696f 6e57 6172    DeprecationWar
+00014a90: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
+00014aa0: 2020 290a 2020 2020 2020 2020 6966 2064    ).        if d
+00014ab0: 696d 7320 6973 206e 6f74 204e 6f6e 6520  ims is not None 
+00014ac0: 6f72 206b 7761 7267 732e 6765 7428 226f  or kwargs.get("o
+00014ad0: 6273 6572 7665 6422 2920 6973 206e 6f74  bserved") is not
+00014ae0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00014af0: 2020 206e 5f7a 6572 6f73 756d 5f61 7865     n_zerosum_axe
+00014b00: 7320 3d20 636c 732e 6368 6563 6b5f 7a65  s = cls.check_ze
+00014b10: 726f 7375 6d5f 6178 6573 286e 5f7a 6572  rosum_axes(n_zer
+00014b20: 6f73 756d 5f61 7865 7329 0a0a 2020 2020  osum_axes)..    
+00014b30: 2020 2020 2020 2020 7375 7070 6f72 745f          support_
+00014b40: 7368 6170 6520 3d20 6765 745f 7375 7070  shape = get_supp
+00014b50: 6f72 745f 7368 6170 6528 0a20 2020 2020  ort_shape(.     
+00014b60: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
+00014b70: 7274 5f73 6861 7065 3d73 7570 706f 7274  rt_shape=support
+00014b80: 5f73 6861 7065 2c0a 2020 2020 2020 2020  _shape,.        
+00014b90: 2020 2020 2020 2020 7368 6170 653d 4e6f          shape=No
+00014ba0: 6e65 2c20 2023 2053 6861 7065 2077 696c  ne,  # Shape wil
+00014bb0: 6c20 6265 2063 6865 636b 6564 2069 6e20  l be checked in 
+00014bc0: 6063 6c73 2e64 6973 7460 0a20 2020 2020  `cls.dist`.     
+00014bd0: 2020 2020 2020 2020 2020 2064 696d 733d             dims=
+00014be0: 6469 6d73 2c0a 2020 2020 2020 2020 2020  dims,.          
+00014bf0: 2020 2020 2020 6f62 7365 7276 6564 3d6b        observed=k
+00014c00: 7761 7267 732e 6765 7428 226f 6273 6572  wargs.get("obser
+00014c10: 7665 6422 2c20 4e6f 6e65 292c 0a20 2020  ved", None),.   
+00014c20: 2020 2020 2020 2020 2020 2020 206e 6469               ndi
+00014c30: 6d5f 7375 7070 3d6e 5f7a 6572 6f73 756d  m_supp=n_zerosum
+00014c40: 5f61 7865 732c 0a20 2020 2020 2020 2020  _axes,.         
+00014c50: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
+00014c60: 7475 726e 2073 7570 6572 2829 2e5f 5f6e  turn super().__n
+00014c70: 6577 5f5f 280a 2020 2020 2020 2020 2020  ew__(.          
+00014c80: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
+00014c90: 2020 202a 6172 6773 2c0a 2020 2020 2020     *args,.      
+00014ca0: 2020 2020 2020 6e5f 7a65 726f 7375 6d5f        n_zerosum_
+00014cb0: 6178 6573 3d6e 5f7a 6572 6f73 756d 5f61  axes=n_zerosum_a
+00014cc0: 7865 732c 0a20 2020 2020 2020 2020 2020  xes,.           
+00014cd0: 2073 7570 706f 7274 5f73 6861 7065 3d73   support_shape=s
+00014ce0: 7570 706f 7274 5f73 6861 7065 2c0a 2020  upport_shape,.  
+00014cf0: 2020 2020 2020 2020 2020 6469 6d73 3d64            dims=d
+00014d00: 696d 732c 0a20 2020 2020 2020 2020 2020  ims,.           
+00014d10: 202a 2a6b 7761 7267 732c 0a20 2020 2020   **kwargs,.     
+00014d20: 2020 2029 0a0a 2020 2020 4063 6c61 7373     )..    @class
+00014d30: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
+00014d40: 6973 7428 636c 732c 2073 6967 6d61 3d31  ist(cls, sigma=1
+00014d50: 2c20 6e5f 7a65 726f 7375 6d5f 6178 6573  , n_zerosum_axes
+00014d60: 3d4e 6f6e 652c 2073 7570 706f 7274 5f73  =None, support_s
+00014d70: 6861 7065 3d4e 6f6e 652c 202a 2a6b 7761  hape=None, **kwa
+00014d80: 7267 7329 3a0a 2020 2020 2020 2020 6e5f  rgs):.        n_
+00014d90: 7a65 726f 7375 6d5f 6178 6573 203d 2063  zerosum_axes = c
+00014da0: 6c73 2e63 6865 636b 5f7a 6572 6f73 756d  ls.check_zerosum
+00014db0: 5f61 7865 7328 6e5f 7a65 726f 7375 6d5f  _axes(n_zerosum_
+00014dc0: 6178 6573 290a 0a20 2020 2020 2020 2073  axes)..        s
+00014dd0: 6967 6d61 203d 2070 742e 6173 5f74 656e  igma = pt.as_ten
+00014de0: 736f 725f 7661 7269 6162 6c65 2866 6c6f  sor_variable(flo
+00014df0: 6174 5828 7369 676d 6129 290a 2020 2020  atX(sigma)).    
+00014e00: 2020 2020 6966 2073 6967 6d61 2e6e 6469      if sigma.ndi
+00014e10: 6d20 3e20 303a 0a20 2020 2020 2020 2020  m > 0:.         
+00014e20: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00014e30: 726f 7228 2273 6967 6d61 2068 6173 2074  ror("sigma has t
+00014e40: 6f20 6265 2061 2073 6361 6c61 7222 290a  o be a scalar").
+00014e50: 0a20 2020 2020 2020 2073 7570 706f 7274  .        support
+00014e60: 5f73 6861 7065 203d 2067 6574 5f73 7570  _shape = get_sup
+00014e70: 706f 7274 5f73 6861 7065 280a 2020 2020  port_shape(.    
+00014e80: 2020 2020 2020 2020 7375 7070 6f72 745f          support_
+00014e90: 7368 6170 653d 7375 7070 6f72 745f 7368  shape=support_sh
+00014ea0: 6170 652c 0a20 2020 2020 2020 2020 2020  ape,.           
+00014eb0: 2073 6861 7065 3d6b 7761 7267 732e 6765   shape=kwargs.ge
+00014ec0: 7428 2273 6861 7065 2229 2c0a 2020 2020  t("shape"),.    
+00014ed0: 2020 2020 2020 2020 6e64 696d 5f73 7570          ndim_sup
+00014ee0: 703d 6e5f 7a65 726f 7375 6d5f 6178 6573  p=n_zerosum_axes
+00014ef0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00014f00: 2020 2020 2069 6620 7375 7070 6f72 745f       if support_
+00014f10: 7368 6170 6520 6973 204e 6f6e 653a 0a20  shape is None:. 
+00014f20: 2020 2020 2020 2020 2020 2069 6620 6e5f             if n_
+00014f30: 7a65 726f 7375 6d5f 6178 6573 203e 2030  zerosum_axes > 0
+00014f40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014f50: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00014f60: 6f72 2822 596f 7520 6d75 7374 2073 7065  or("You must spe
+00014f70: 6369 6679 2064 696d 732c 2073 6861 7065  cify dims, shape
+00014f80: 206f 7220 7375 7070 6f72 745f 7368 6170   or support_shap
+00014f90: 6520 7061 7261 6d65 7465 7222 290a 2020  e parameter").  
+00014fa0: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
+00014fb0: 3a20 6564 6765 2d63 6173 6520 646f 6573  : edge-case does
+00014fc0: 6e27 7420 776f 726b 2066 6f72 206e 6f77  n't work for now
+00014fd0: 2c20 6265 6361 7573 6520 7074 2e73 7461  , because pt.sta
+00014fe0: 636b 2069 6e20 6765 745f 7375 7070 6f72  ck in get_suppor
+00014ff0: 745f 7368 6170 6520 6661 696c 730a 2020  t_shape fails.  
+00015000: 2020 2020 2020 2020 2020 2320 656c 7365            # else
+00015010: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00015020: 2020 2020 7375 7070 6f72 745f 7368 6170      support_shap
+00015030: 6520 3d20 2829 2023 2062 6563 6175 7365  e = () # because
+00015040: 2069 7427 7320 6a75 7374 2061 204e 6f72   it's just a Nor
+00015050: 6d61 6c20 696e 2074 6861 7420 6361 7365  mal in that case
+00015060: 0a20 2020 2020 2020 2073 7570 706f 7274  .        support
+00015070: 5f73 6861 7065 203d 2070 742e 6173 5f74  _shape = pt.as_t
+00015080: 656e 736f 725f 7661 7269 6162 6c65 2869  ensor_variable(i
+00015090: 6e74 5828 7375 7070 6f72 745f 7368 6170  ntX(support_shap
+000150a0: 6529 290a 0a20 2020 2020 2020 2061 7373  e))..        ass
+000150b0: 6572 7420 6e5f 7a65 726f 7375 6d5f 6178  ert n_zerosum_ax
+000150c0: 6573 203d 3d20 7074 2e67 6574 5f76 6563  es == pt.get_vec
+000150d0: 746f 725f 6c65 6e67 7468 280a 2020 2020  tor_length(.    
+000150e0: 2020 2020 2020 2020 7375 7070 6f72 745f          support_
+000150f0: 7368 6170 650a 2020 2020 2020 2020 292c  shape.        ),
+00015100: 2022 7375 7070 6f72 745f 7368 6170 6520   "support_shape 
+00015110: 6861 7320 746f 2062 6520 6173 206c 6f6e  has to be as lon
+00015120: 6720 6173 206e 5f7a 6572 6f73 756d 5f61  g as n_zerosum_a
+00015130: 7865 7322 0a0a 2020 2020 2020 2020 7265  xes"..        re
+00015140: 7475 726e 2073 7570 6572 2829 2e64 6973  turn super().dis
+00015150: 7428 0a20 2020 2020 2020 2020 2020 205b  t(.            [
+00015160: 7369 676d 615d 2c20 6e5f 7a65 726f 7375  sigma], n_zerosu
+00015170: 6d5f 6178 6573 3d6e 5f7a 6572 6f73 756d  m_axes=n_zerosum
+00015180: 5f61 7865 732c 2073 7570 706f 7274 5f73  _axes, support_s
+00015190: 6861 7065 3d73 7570 706f 7274 5f73 6861  hape=support_sha
+000151a0: 7065 2c20 2a2a 6b77 6172 6773 0a20 2020  pe, **kwargs.   
+000151b0: 2020 2020 2029 0a0a 2020 2020 4063 6c61       )..    @cla
+000151c0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+000151d0: 2063 6865 636b 5f7a 6572 6f73 756d 5f61   check_zerosum_a
+000151e0: 7865 7328 636c 732c 206e 5f7a 6572 6f73  xes(cls, n_zeros
+000151f0: 756d 5f61 7865 733a 204f 7074 696f 6e61  um_axes: Optiona
+00015200: 6c5b 696e 745d 2920 2d3e 2069 6e74 3a0a  l[int]) -> int:.
+00015210: 2020 2020 2020 2020 6966 206e 5f7a 6572          if n_zer
+00015220: 6f73 756d 5f61 7865 7320 6973 204e 6f6e  osum_axes is Non
+00015230: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
+00015240: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
+00015250: 310a 2020 2020 2020 2020 6966 206e 6f74  1.        if not
+00015260: 2069 7369 6e73 7461 6e63 6528 6e5f 7a65   isinstance(n_ze
+00015270: 726f 7375 6d5f 6178 6573 2c20 696e 7429  rosum_axes, int)
+00015280: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00015290: 6973 6520 5479 7065 4572 726f 7228 226e  ise TypeError("n
+000152a0: 5f7a 6572 6f73 756d 5f61 7865 7320 6861  _zerosum_axes ha
+000152b0: 7320 746f 2062 6520 616e 2069 6e74 6567  s to be an integ
+000152c0: 6572 2229 0a20 2020 2020 2020 2069 6620  er").        if 
+000152d0: 6e6f 7420 6e5f 7a65 726f 7375 6d5f 6178  not n_zerosum_ax
+000152e0: 6573 203e 2030 3a0a 2020 2020 2020 2020  es > 0:.        
+000152f0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00015300: 7272 6f72 2822 6e5f 7a65 726f 7375 6d5f  rror("n_zerosum_
+00015310: 6178 6573 2068 6173 2074 6f20 6265 203e  axes has to be >
+00015320: 2030 2229 0a20 2020 2020 2020 2072 6574   0").        ret
+00015330: 7572 6e20 6e5f 7a65 726f 7375 6d5f 6178  urn n_zerosum_ax
+00015340: 6573 0a0a 2020 2020 4063 6c61 7373 6d65  es..    @classme
+00015350: 7468 6f64 0a20 2020 2064 6566 2072 765f  thod.    def rv_
+00015360: 6f70 2863 6c73 2c20 7369 676d 612c 206e  op(cls, sigma, n
+00015370: 5f7a 6572 6f73 756d 5f61 7865 732c 2073  _zerosum_axes, s
+00015380: 7570 706f 7274 5f73 6861 7065 2c20 7369  upport_shape, si
+00015390: 7a65 3d4e 6f6e 6529 3a0a 2020 2020 2020  ze=None):.      
+000153a0: 2020 7368 6170 6520 3d20 746f 5f74 7570    shape = to_tup
+000153b0: 6c65 2873 697a 6529 202b 2074 7570 6c65  le(size) + tuple
+000153c0: 2873 7570 706f 7274 5f73 6861 7065 290a  (support_shape).
+000153d0: 2020 2020 2020 2020 6e6f 726d 616c 5f64          normal_d
+000153e0: 6973 7420 3d20 6967 6e6f 7265 5f6c 6f67  ist = ignore_log
+000153f0: 7072 6f62 2870 6d2e 4e6f 726d 616c 2e64  prob(pm.Normal.d
+00015400: 6973 7428 7369 676d 613d 7369 676d 612c  ist(sigma=sigma,
+00015410: 2073 6861 7065 3d73 6861 7065 2929 0a0a   shape=shape))..
+00015420: 2020 2020 2020 2020 6966 206e 5f7a 6572          if n_zer
+00015430: 6f73 756d 5f61 7865 7320 3e20 6e6f 726d  osum_axes > norm
+00015440: 616c 5f64 6973 742e 6e64 696d 3a0a 2020  al_dist.ndim:.  
+00015450: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00015460: 5661 6c75 6545 7272 6f72 2822 5368 6170  ValueError("Shap
+00015470: 6520 6f66 2064 6973 7472 6962 7574 696f  e of distributio
+00015480: 6e20 6973 2074 6f6f 2073 6d61 6c6c 2066  n is too small f
+00015490: 6f72 2074 6865 206e 756d 6265 7220 6f66  or the number of
+000154a0: 207a 6572 6f73 756d 2061 7865 7322 290a   zerosum axes").
+000154b0: 0a20 2020 2020 2020 206e 6f72 6d61 6c5f  .        normal_
+000154c0: 6469 7374 5f2c 2073 6967 6d61 5f2c 2073  dist_, sigma_, s
+000154d0: 7570 706f 7274 5f73 6861 7065 5f20 3d20  upport_shape_ = 
+000154e0: 280a 2020 2020 2020 2020 2020 2020 6e6f  (.            no
+000154f0: 726d 616c 5f64 6973 742e 7479 7065 2829  rmal_dist.type()
+00015500: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
+00015510: 676d 612e 7479 7065 2829 2c0a 2020 2020  gma.type(),.    
+00015520: 2020 2020 2020 2020 7375 7070 6f72 745f          support_
+00015530: 7368 6170 652e 7479 7065 2829 2c0a 2020  shape.type(),.  
+00015540: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00015550: 2023 205a 6572 6f73 756d 2d6e 6f72 6d61   # Zerosum-norma
+00015560: 6c69 6e67 2069 7320 6163 6869 6576 6564  ling is achieved
+00015570: 2062 7920 7375 6274 7261 6374 696e 6720   by subtracting 
+00015580: 7468 6520 6d65 616e 2061 6c6f 6e67 2074  the mean along t
+00015590: 6865 2067 6976 656e 206e 5f7a 6572 6f73  he given n_zeros
+000155a0: 756d 5f61 7865 730a 2020 2020 2020 2020  um_axes.        
+000155b0: 7a65 726f 7375 6d5f 7276 5f20 3d20 6e6f  zerosum_rv_ = no
+000155c0: 726d 616c 5f64 6973 745f 0a20 2020 2020  rmal_dist_.     
+000155d0: 2020 2066 6f72 2061 7869 7320 696e 2072     for axis in r
+000155e0: 616e 6765 286e 5f7a 6572 6f73 756d 5f61  ange(n_zerosum_a
+000155f0: 7865 7329 3a0a 2020 2020 2020 2020 2020  xes):.          
+00015600: 2020 7a65 726f 7375 6d5f 7276 5f20 2d3d    zerosum_rv_ -=
+00015610: 207a 6572 6f73 756d 5f72 765f 2e6d 6561   zerosum_rv_.mea
+00015620: 6e28 6178 6973 3d2d 6178 6973 202d 2031  n(axis=-axis - 1
+00015630: 2c20 6b65 6570 6469 6d73 3d54 7275 6529  , keepdims=True)
+00015640: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00015650: 205a 6572 6f53 756d 4e6f 726d 616c 5256   ZeroSumNormalRV
+00015660: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
+00015670: 7075 7473 3d5b 6e6f 726d 616c 5f64 6973  puts=[normal_dis
+00015680: 745f 2c20 7369 676d 615f 2c20 7375 7070  t_, sigma_, supp
+00015690: 6f72 745f 7368 6170 655f 5d2c 0a20 2020  ort_shape_],.   
+000156a0: 2020 2020 2020 2020 206f 7574 7075 7473           outputs
+000156b0: 3d5b 7a65 726f 7375 6d5f 7276 5f2c 2073  =[zerosum_rv_, s
+000156c0: 7570 706f 7274 5f73 6861 7065 5f5d 2c0a  upport_shape_],.
+000156d0: 2020 2020 2020 2020 2020 2020 6e64 696d              ndim
+000156e0: 5f73 7570 703d 6e5f 7a65 726f 7375 6d5f  _supp=n_zerosum_
+000156f0: 6178 6573 2c0a 2020 2020 2020 2020 2928  axes,.        )(
+00015700: 6e6f 726d 616c 5f64 6973 742c 2073 6967  normal_dist, sig
+00015710: 6d61 2c20 7375 7070 6f72 745f 7368 6170  ma, support_shap
+00015720: 6529 0a0a 0a40 5f63 6861 6e67 655f 6469  e)...@_change_di
+00015730: 7374 5f73 697a 652e 7265 6769 7374 6572  st_size.register
+00015740: 285a 6572 6f53 756d 4e6f 726d 616c 5256  (ZeroSumNormalRV
+00015750: 290a 6465 6620 6368 616e 6765 5f7a 6572  ).def change_zer
+00015760: 6f73 756d 5f73 697a 6528 6f70 2c20 6e6f  osum_size(op, no
+00015770: 726d 616c 5f64 6973 742c 206e 6577 5f73  rmal_dist, new_s
+00015780: 697a 652c 2065 7870 616e 643d 4661 6c73  ize, expand=Fals
+00015790: 6529 3a0a 2020 2020 6e6f 726d 616c 5f64  e):.    normal_d
+000157a0: 6973 742c 2073 6967 6d61 2c20 7375 7070  ist, sigma, supp
+000157b0: 6f72 745f 7368 6170 6520 3d20 6e6f 726d  ort_shape = norm
+000157c0: 616c 5f64 6973 742e 6f77 6e65 722e 696e  al_dist.owner.in
+000157d0: 7075 7473 0a0a 2020 2020 6966 2065 7870  puts..    if exp
+000157e0: 616e 643a 0a20 2020 2020 2020 206f 7269  and:.        ori
+000157f0: 6769 6e61 6c5f 7368 6170 6520 3d20 7475  ginal_shape = tu
+00015800: 706c 6528 6e6f 726d 616c 5f64 6973 742e  ple(normal_dist.
+00015810: 7368 6170 6529 0a20 2020 2020 2020 206f  shape).        o
+00015820: 6c64 5f73 697a 6520 3d20 6f72 6967 696e  ld_size = origin
+00015830: 616c 5f73 6861 7065 5b3a 206c 656e 286f  al_shape[: len(o
+00015840: 7269 6769 6e61 6c5f 7368 6170 6529 202d  riginal_shape) -
+00015850: 206f 702e 6e64 696d 5f73 7570 705d 0a20   op.ndim_supp]. 
+00015860: 2020 2020 2020 206e 6577 5f73 697a 6520         new_size 
+00015870: 3d20 7475 706c 6528 6e65 775f 7369 7a65  = tuple(new_size
+00015880: 2920 2b20 6f6c 645f 7369 7a65 0a0a 2020  ) + old_size..  
+00015890: 2020 7265 7475 726e 205a 6572 6f53 756d    return ZeroSum
+000158a0: 4e6f 726d 616c 2e72 765f 6f70 280a 2020  Normal.rv_op(.  
+000158b0: 2020 2020 2020 7369 676d 613d 7369 676d        sigma=sigm
+000158c0: 612c 206e 5f7a 6572 6f73 756d 5f61 7865  a, n_zerosum_axe
+000158d0: 733d 6f70 2e6e 6469 6d5f 7375 7070 2c20  s=op.ndim_supp, 
+000158e0: 7375 7070 6f72 745f 7368 6170 653d 7375  support_shape=su
+000158f0: 7070 6f72 745f 7368 6170 652c 2073 697a  pport_shape, siz
+00015900: 653d 6e65 775f 7369 7a65 0a20 2020 2029  e=new_size.    )
+00015910: 0a0a 0a40 5f6d 6f6d 656e 742e 7265 6769  ...@_moment.regi
+00015920: 7374 6572 285a 6572 6f53 756d 4e6f 726d  ster(ZeroSumNorm
+00015930: 616c 5256 290a 6465 6620 7a65 726f 7375  alRV).def zerosu
+00015940: 6d6e 6f72 6d61 6c5f 6d6f 6d65 6e74 286f  mnormal_moment(o
+00015950: 702c 2072 762c 202a 7276 5f69 6e70 7574  p, rv, *rv_input
+00015960: 7329 3a0a 2020 2020 7265 7475 726e 2070  s):.    return p
+00015970: 742e 7a65 726f 735f 6c69 6b65 2872 7629  t.zeros_like(rv)
+00015980: 0a0a 0a40 5f64 6566 6175 6c74 5f74 7261  ...@_default_tra
+00015990: 6e73 666f 726d 2e72 6567 6973 7465 7228  nsform.register(
+000159a0: 5a65 726f 5375 6d4e 6f72 6d61 6c52 5629  ZeroSumNormalRV)
+000159b0: 0a64 6566 207a 6572 6f73 756d 5f64 6566  .def zerosum_def
+000159c0: 6175 6c74 5f74 7261 6e73 666f 726d 286f  ault_transform(o
+000159d0: 702c 2072 7629 3a0a 2020 2020 6e5f 7a65  p, rv):.    n_ze
+000159e0: 726f 7375 6d5f 6178 6573 203d 2074 7570  rosum_axes = tup
+000159f0: 6c65 286e 702e 6172 616e 6765 282d 6f70  le(np.arange(-op
+00015a00: 2e6e 6469 6d5f 7375 7070 2c20 3029 290a  .ndim_supp, 0)).
+00015a10: 2020 2020 7265 7475 726e 205a 6572 6f53      return ZeroS
+00015a20: 756d 5472 616e 7366 6f72 6d28 6e5f 7a65  umTransform(n_ze
+00015a30: 726f 7375 6d5f 6178 6573 290a 0a0a 405f  rosum_axes)...@_
+00015a40: 6c6f 6770 726f 622e 7265 6769 7374 6572  logprob.register
+00015a50: 285a 6572 6f53 756d 4e6f 726d 616c 5256  (ZeroSumNormalRV
+00015a60: 290a 6465 6620 7a65 726f 7375 6d6e 6f72  ).def zerosumnor
+00015a70: 6d61 6c5f 6c6f 6770 286f 702c 2076 616c  mal_logp(op, val
+00015a80: 7565 732c 206e 6f72 6d61 6c5f 6469 7374  ues, normal_dist
+00015a90: 2c20 7369 676d 612c 2073 7570 706f 7274  , sigma, support
+00015aa0: 5f73 6861 7065 2c20 2a2a 6b77 6172 6773  _shape, **kwargs
+00015ab0: 293a 0a20 2020 2028 7661 6c75 652c 2920  ):.    (value,) 
+00015ac0: 3d20 7661 6c75 6573 0a20 2020 2073 6861  = values.    sha
+00015ad0: 7065 203d 2076 616c 7565 2e73 6861 7065  pe = value.shape
+00015ae0: 0a20 2020 206e 5f7a 6572 6f73 756d 5f61  .    n_zerosum_a
+00015af0: 7865 7320 3d20 6f70 2e6e 6469 6d5f 7375  xes = op.ndim_su
+00015b00: 7070 0a0a 2020 2020 5f64 6567 5f66 7265  pp..    _deg_fre
+00015b10: 655f 7375 7070 6f72 745f 7368 6170 6520  e_support_shape 
+00015b20: 3d20 7074 2e69 6e63 5f73 7562 7465 6e73  = pt.inc_subtens
+00015b30: 6f72 2873 6861 7065 5b2d 6e5f 7a65 726f  or(shape[-n_zero
+00015b40: 7375 6d5f 6178 6573 3a5d 2c20 2d31 290a  sum_axes:], -1).
+00015b50: 2020 2020 5f66 756c 6c5f 7369 7a65 203d      _full_size =
+00015b60: 2070 742e 7072 6f64 2873 6861 7065 290a   pt.prod(shape).
+00015b70: 2020 2020 5f64 6567 7265 6573 5f6f 665f      _degrees_of_
+00015b80: 6672 6565 646f 6d20 3d20 7074 2e70 726f  freedom = pt.pro
+00015b90: 6428 5f64 6567 5f66 7265 655f 7375 7070  d(_deg_free_supp
+00015ba0: 6f72 745f 7368 6170 6529 0a0a 2020 2020  ort_shape)..    
+00015bb0: 7a65 726f 7375 6d73 203d 205b 0a20 2020  zerosums = [.   
+00015bc0: 2020 2020 2070 742e 616c 6c28 7074 2e69       pt.all(pt.i
+00015bd0: 7363 6c6f 7365 2870 742e 6d65 616e 2876  sclose(pt.mean(v
+00015be0: 616c 7565 2c20 6178 6973 3d2d 6178 6973  alue, axis=-axis
+00015bf0: 202d 2031 292c 2030 2c20 6174 6f6c 3d31   - 1), 0, atol=1
+00015c00: 652d 3929 290a 2020 2020 2020 2020 666f  e-9)).        fo
+00015c10: 7220 6178 6973 2069 6e20 7261 6e67 6528  r axis in range(
+00015c20: 6e5f 7a65 726f 7375 6d5f 6178 6573 290a  n_zerosum_axes).
+00015c30: 2020 2020 5d0a 0a20 2020 206f 7574 203d      ]..    out =
+00015c40: 2070 742e 7375 6d28 0a20 2020 2020 2020   pt.sum(.       
+00015c50: 2070 6d2e 6c6f 6770 286e 6f72 6d61 6c5f   pm.logp(normal_
+00015c60: 6469 7374 2c20 7661 6c75 6529 202a 205f  dist, value) * _
+00015c70: 6465 6772 6565 735f 6f66 5f66 7265 6564  degrees_of_freed
+00015c80: 6f6d 202f 205f 6675 6c6c 5f73 697a 652c  om / _full_size,
+00015c90: 0a20 2020 2020 2020 2061 7869 733d 7475  .        axis=tu
+00015ca0: 706c 6528 6e70 2e61 7261 6e67 6528 2d6e  ple(np.arange(-n
+00015cb0: 5f7a 6572 6f73 756d 5f61 7865 732c 2030  _zerosum_axes, 0
+00015cc0: 2929 2c0a 2020 2020 290a 0a20 2020 2072  )),.    )..    r
+00015cd0: 6574 7572 6e20 6368 6563 6b5f 7061 7261  eturn check_para
+00015ce0: 6d65 7465 7273 286f 7574 2c20 2a7a 6572  meters(out, *zer
+00015cf0: 6f73 756d 732c 206d 7367 3d22 6d65 616e  osums, msg="mean
+00015d00: 2876 616c 7565 2c20 6178 6973 3d6e 5f7a  (value, axis=n_z
+00015d10: 6572 6f73 756d 5f61 7865 7329 203d 2030  erosum_axes) = 0
+00015d20: 2229 0a                                  ").
```

### Comparing `pymc-5.2.0/pymc/distributions/shape_utils.py` & `pymc-5.3.0/pymc/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/simulator.py` & `pymc-5.3.0/pymc/distributions/simulator.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/timeseries.py` & `pymc-5.3.0/pymc/distributions/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 
     Parameters
     ----------
     mu : tensor_like of float, default 0
         innovation drift
     sigma : tensor_like of float, default 1
         sigma > 0, innovation standard deviation.
-    init_dist : Distribution
+    init_dist : unnamed_distribution
         Unnamed univariate distribution of the initial value. Unnamed refers to distributions
         created with the ``.dist()`` API.
 
         .. warning:: init_dist will be cloned, rendering them independent of the ones passed as input.
 
     steps : int, optional
         Number of steps in Gaussian Random Walk (steps > 0). Only needed if shape is not
@@ -313,27 +313,26 @@
 
 
 class MvGaussianRandomWalk(PredefinedRandomWalk):
     r"""Random Walk with Multivariate Normal innovations
 
     Parameters
     ----------
-    mu: tensor_like of float
+    mu : tensor_like of float
         innovation drift
-    cov: tensor_like of float
+    cov : tensor_like of float
         pos def matrix, innovation covariance matrix
-    tau: tensor_like of float
+    tau : tensor_like of float
         pos def matrix, inverse covariance matrix
-    chol: tensor_like of float
+    chol : tensor_like of float
         Cholesky decomposition of covariance matrix
     lower : bool, default=True
         Whether the cholesky fatcor is given as a lower triangular matrix.
-    init_dist: distribution
-        Unnamed multivariate distribution of the initial value. Unnamed refers to distributions
-         created with the ``.dist()`` API.
+    init_dist : unnamed_distribution
+        Unnamed multivariate distribution of the initial value.
 
          .. warning:: init_dist will be cloned, rendering them independent of the ones passed as input.
 
     steps : int, optional
         Number of steps in Random Walk (steps > 0). Only needed if shape is not
         provided.
 
@@ -366,29 +365,28 @@
 
 
 class MvStudentTRandomWalk(PredefinedRandomWalk):
     r"""Multivariate Random Walk with StudentT innovations
 
     Parameters
     ----------
-    nu: int
+    nu : int
         degrees of freedom
-    mu: tensor_like of float
+    mu : tensor_like of float
         innovation drift
-    scale: tensor_like of float
+    scale : tensor_like of float
         pos def matrix, innovation covariance matrix
-    tau: tensor_like of float
+    tau : tensor_like of float
         pos def matrix, inverse covariance matrix
-    chol: tensor_like of float
+    chol : tensor_like of float
         Cholesky decomposition of covariance matrix
     lower : bool, default=True
         Whether the cholesky fatcor is given as a lower triangular matrix.
-    init_dist: distribution
-        Unnamed multivariate distribution of the initial value. Unnamed refers to distributions
-         created with the ``.dist()`` API.
+    init_dist : unnamed_distribution
+        Unnamed multivariate distribution of the initial value.
 
          .. warning:: init_dist will be cloned, rendering them independent of the ones passed as input.
 
     steps : int, optional
         Number of steps in Random Walk (steps > 0). Only needed if shape is not
         provided.
 
@@ -467,17 +465,16 @@
         Standard deviation of innovation (sigma > 0). Only required if
         tau is not specified.
     tau : tensor_like of float, optional
         Precision of innovation (tau > 0).
     constant : bool, default False
         Whether the first element of rho should be used as a constant term in the AR
         process.
-    init_dist : unnamed distribution, optional
-        Scalar or vector distribution for initial values. Unnamed refers to distributions
-        created with the ``.dist()`` API. Distributions should have shape (*shape[:-1], ar_order).
+    init_dist : unnamed_distribution, optional
+        Scalar or vector distribution for initial values. Distributions should have shape (*shape[:-1], ar_order).
         If not, it will be automatically resized. Defaults to pm.Normal.dist(0, 100, shape=...).
 
         .. warning:: init_dist will be cloned, rendering it independent of the one passed as input.
 
     ar_order : int, optional
         Order of the AR process. Inferred from length of the last dimension of rho, if
         possible. ar_order = rho.shape[-1] if constant else rho.shape[-1] - 1
@@ -751,21 +748,21 @@
     .. math::
         \sigma_t^2 = \omega + \alpha_1 * y_{t-1}^2 + \beta_1 * \sigma_{t-1}^2
 
     where \sigma_t^2 (the error variance) follows a ARMA(1, 1) model.
 
     Parameters
     ----------
-    omega: tensor
+    omega : tensor_like of float
         omega > 0, mean variance
-    alpha_1: tensor
+    alpha_1 : tensor_like of float
         alpha_1 >= 0, autoregressive term coefficient
-    beta_1: tensor
+    beta_1 : tensor_like of float
         beta_1 >= 0, alpha_1 + beta_1 < 1, moving average term coefficient
-    initial_vol: tensor
+    initial_vol : tensor_like of float
         initial_vol >= 0, initial volatility, sigma_0
     """
 
     rv_type = GARCH11RV
 
     def __new__(cls, *args, steps=None, **kwargs):
         steps = get_support_shape_1d(
@@ -918,17 +915,16 @@
     ----------
     dt : float
         time step of discretization
     sde_fn : callable
         function returning the drift and diffusion coefficients of SDE
     sde_pars : tuple
         parameters of the SDE, passed as ``*args`` to ``sde_fn``
-    init_dist : unnamed distribution, optional
-        Scalar distribution for initial values. Unnamed refers to distributions created with
-        the ``.dist()`` API. Distributions should have shape (*shape[:-1]).
+    init_dist : unnamed_distribution, optional
+        Scalar distribution for initial values. Distributions should have shape (*shape[:-1]).
         If not, it will be automatically resized. Defaults to pm.Normal.dist(0, 100, shape=...).
 
         .. warning:: init_dist will be cloned, rendering it independent of the one passed as input.
     """
 
     rv_type = EulerMaruyamaRV
```

### Comparing `pymc-5.2.0/pymc/distributions/transforms.py` & `pymc-5.3.0/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/distributions/truncated.py` & `pymc-5.3.0/pymc/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/exceptions.py` & `pymc-5.3.0/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/func_utils.py` & `pymc-5.3.0/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/gp/__init__.py` & `pymc-5.3.0/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/gp/cov.py` & `pymc-5.3.0/pymc/gp/cov.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/gp/gp.py` & `pymc-5.3.0/pymc/gp/gp.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,18 +107,18 @@
     distribution is the GP prior or GP conditional.  This GP implementation
     can be used to implement regression on data that is not normally
     distributed.  For more information on the `prior` and `conditional` methods,
     see their docstrings.
 
     Parameters
     ----------
-    cov_func: None, 2D array, or instance of Covariance
-        The covariance function.  Defaults to zero.
-    mean_func: None, instance of Mean
-        The mean function.  Defaults to zero.
+    mean_func : Mean, default ~pymc.gp.mean.Zero
+        The mean function.
+    cov_func : 2D array-like, or Covariance, default ~pymc.gp.cov.Constant
+        The covariance function.
 
     Examples
     --------
     .. code:: python
 
         # A one dimensional column vector of inputs.
         X = np.linspace(0, 1, 10)[:, None]
@@ -167,26 +167,28 @@
 
         .. math::
 
            f \mid X \sim \text{MvNormal}\left( \mu(X), k(X, X') \right)
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        X: array-like
-            Function input values.
-        reparameterize: bool
+        X : array-like
+            Function input values. If one-dimensional, must be a column
+            vector with shape `(n, 1)`.
+        reparameterize : bool, default True
             Reparameterize the distribution by rotating the random
             variable by the Cholesky factor of the covariance matrix.
-        jitter: scalar
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to distribution constructor.
+            Extra keyword arguments that are passed to :class:`~pymc.MvNormal`
+            distribution constructor.
         """
 
         f = self._build_prior(name, X, reparameterize, jitter, **kwargs)
         self.X = X
         self.f = f
         return f
 
@@ -229,55 +231,58 @@
 
            f_* \mid f, X, X_* \sim \mathcal{GP}\left(
                K(X_*, X) K(X, X)^{-1} f \,,
                K(X_*, X_*) - K(X_*, X) K(X, X)^{-1} K(X, X_*) \right)
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        Xnew: array-like
-            Function input values.
-        given: dict
-            Can optionally take as key value pairs: `X`, `y`,
-            and `gp`.  See the section in the documentation on additive GP
-            models in PyMC for more information.
-        jitter: scalar
+        Xnew : array-like
+            Function input values. If one-dimensional, must be a column
+            vector with shape `(n, 1)`.
+        given : dict, optional
+            Can take as key value pairs: `X`, `y`,
+            and `gp`. See the :ref:`section <additive_gp>` in the documentation
+            on additive GP models in pymc for more information.
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to `MvNormal` distribution
+            Extra keyword arguments that are passed to :class:`~pymc.MvNormal` distribution
             constructor.
         """
         givens = self._get_given_vals(given)
         mu, cov = self._build_conditional(Xnew, *givens, jitter)
         return pm.MvNormal(name, mu=mu, cov=cov, **kwargs)
 
 
 @conditioned_vars(["X", "f", "nu"])
 class TP(Latent):
     r"""
     Student's T process prior.
 
     The usage is nearly identical to that of `gp.Latent`.  The differences
     are that it must be initialized with a degrees of freedom parameter, and
-    TP is not additive.  Given a mean and covariance function, and a degrees of
+    TP is not additive. Given a mean and covariance function, and a degrees of
     freedom parameter, the function :math:`f(x)` is modeled as,
 
     .. math::
 
        f(X) \sim \mathcal{TP}\left( \mu(X), k(X, X'), \nu \right)
 
 
     Parameters
     ----------
-    scale_func : None, 2D array, or instance of Covariance
-        The scale function.  Defaults to zero.
-    mean_func : None, instance of Mean
-        The mean function.  Defaults to zero.
+    mean_func : Mean, default ~pymc.gp.mean.Zero
+        The mean function.
+    scale_func : 2D array-like, or Covariance, default ~pymc.gp.cov.Constant
+        The covariance function.
+    cov_func : 2D array-like, or Covariance, default None
+        Deprecated, previous version of "scale_func"
     nu : float
         The degrees of freedom
 
     References
     ----------
     -   Shah, A., Wilson, A. G., and Ghahramani, Z. (2014).  Student-t
         Processes as Alternatives to Gaussian Processes.  arXiv preprint arXiv:1402.4306.
@@ -316,23 +321,28 @@
         locations `X`.
 
         This is the prior probability over the space
         of functions described by its mean and covariance function.
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        X: array-like
-            Function input values.
-        reparameterize: bool
+        X : array-like
+            Function input values. If one-dimensional, must be a column
+            vector with shape `(n, 1)`.
+        reparameterize : bool, default True
             Reparameterize the distribution by rotating the random
             variable by the Cholesky factor of the covariance matrix.
+        jitter : float, default 1e-6
+            A small correction added to the diagonal of positive semi-definite
+            covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to distribution constructor.
+            Extra keyword arguments that are passed to :class:`~pymc.MvStudentT`
+            distribution constructor.
         """
 
         f = self._build_prior(name, X, reparameterize, jitter, **kwargs)
         self.X = X
         self.f = f
         return f
 
@@ -357,23 +367,24 @@
 
         Given a set of function values `f` that
         the TP prior was over, the conditional distribution over a
         set of new points, `f_*` is
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        Xnew: array-like
-            Function input values.
-        jitter: scalar
+        Xnew : array-like
+            Function input values. If one-dimensional, must be a column
+            vector with shape `(n, 1)`.
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to `MvNormal` distribution
+            Extra keyword arguments that are passed to :class:`~pymc.MvStudentT` distribution
             constructor.
         """
 
         X = self.X
         f = self.f
         nu2, mu, cov = self._build_conditional(Xnew, X, f, jitter)
         return pm.MvStudentT(name, nu=nu2, mu=mu, scale=cov, **kwargs)
@@ -384,22 +395,23 @@
     R"""
     Marginal Gaussian process.
 
     The `gp.Marginal` class is an implementation of the sum of a GP
     prior and additive noise.  It has `marginal_likelihood`, `conditional`
     and `predict` methods.  This GP implementation can be used to
     implement regression on data that is normally distributed.  For more
-    information on the `prior` and `conditional` methods, see their docstrings.
+    information on the `marginal_likelihood`, `conditional`
+    and `predict` methods, see their docstrings.
 
     Parameters
     ----------
-    cov_func: None, 2D array, or instance of Covariance
-        The covariance function.  Defaults to zero.
-    mean_func: None, instance of Mean
-        The mean function.  Defaults to zero.
+    mean_func : Mean, default ~pymc.gp.mean.Zero
+        The mean function.
+    cov_func : 2D array-like, or Covariance, default ~pymc.gp.cov.Constant
+        The covariance function.
 
     Examples
     --------
     .. code:: python
 
         # A one dimensional column vector of inputs.
         X = np.linspace(0, 1, 10)[:, None]
@@ -435,40 +447,42 @@
     def marginal_likelihood(
         self, name, X, y, sigma=None, noise=None, jitter=JITTER_DEFAULT, is_observed=True, **kwargs
     ):
         R"""
         Returns the marginal likelihood distribution, given the input
         locations `X` and the data `y`.
 
-        This is integral over the product of the GP prior and a normal likelihood.
+        This is the integral over the product of the GP prior and a normal likelihood.
 
         .. math::
 
            y \mid X,\theta \sim \int p(y \mid f,\, X,\, \theta) \, p(f \mid X,\, \theta) \, df
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        X: array-like
+        X : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        y: array-like
+        y : array-like
             Data that is the sum of the function with the GP prior and Gaussian
             noise.  Must have shape `(n, )`.
-        sigma: scalar, Variable, or Covariance
+        sigma : float, Variable, or Covariance, default ~pymc.gp.cov.WhiteNoise
             Standard deviation of the Gaussian noise.  Can also be a Covariance for
             non-white noise.
-        noise: scalar, Variable, or Covariance
-            Previous parameterization of `sigma`.
-        jitter: scalar
+        noise : float, Variable, or Covariance, optional
+            Deprecated. Previous parameterization of `sigma`.
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
+        is_observed : bool, default True
+            Deprecated. Whether to set `y` as an `observed` variable in the `model`.
         **kwargs
-            Extra keyword arguments that are passed to `MvNormal` distribution
+            Extra keyword arguments that are passed to :class:`~pymc.MvNormal` distribution
             constructor.
         """
         sigma = _handle_sigma_noise_parameters(sigma=sigma, noise=noise)
 
         noise_func = sigma if isinstance(sigma, Covariance) else pm.gp.cov.WhiteNoise(sigma)
         mu, cov = self._build_marginal_likelihood(X=X, noise_func=noise_func, jitter=jitter)
         self.X = X
@@ -544,31 +558,30 @@
 
            f_* \mid f, X, X_* \sim \mathcal{GP}\left(
                K(X_*, X) [K(X, X) + K_{n}(X, X)]^{-1} f \,,
                K(X_*, X_*) - K(X_*, X) [K(X, X) + K_{n}(X, X)]^{-1} K(X, X_*) \right)
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        Xnew: array-like
+        Xnew : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        pred_noise: bool
+        pred_noise : bool, default False
             Whether or not observation noise is included in the conditional.
-            Default is `False`.
-        given: dict
-            Can optionally take as key value pairs: `X`, `y`, `sigma`,
-            and `gp`.  See the section in the documentation on additive GP
-            models in PyMC for more information.
-        jitter: scalar
+        given : dict, optional
+            Can take key value pairs: `X`, `y`, `sigma`,
+            and `gp`. See the :ref:`section <additive_gp>` in the documentation
+            on additive GP models in pymc for more information.
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to `MvNormal` distribution
+            Extra keyword arguments that are passed to :class:`~pymc.MvNormal` distribution
             constructor.
         """
 
         givens = self._get_given_vals(given)
         mu, cov = self._build_conditional(Xnew, pred_noise, False, *givens, jitter)
         return pm.MvNormal(name, mu=mu, cov=cov, **kwargs)
 
@@ -585,54 +598,60 @@
         R"""
         Return the mean vector and covariance matrix of the conditional
         distribution as numpy arrays, given a `point`, such as the MAP
         estimate or a sample from a `trace`.
 
         Parameters
         ----------
-        Xnew: array-like
+        Xnew : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        point: pymc.model.Point
+        point : pymc.Point, optional
             A specific point to condition on.
-        diag: bool
+        diag : bool, default False
             If `True`, return the diagonal instead of the full covariance
-            matrix.  Default is `False`.
-        pred_noise: bool
+            matrix.
+        pred_noise : bool, default False
             Whether or not observation noise is included in the conditional.
-            Default is `False`.
-        given: dict
-            Same as `conditional` method.
-        jitter: scalar
+        given : dict, optional
+            Can take key value pairs: `X`, `y`, `sigma`,
+            and `gp`. See the :ref:`section <additive_gp>` in the documentation
+            on additive GP models in pymc for more information.
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
+        model : Model, optional
+            Model with the Gaussian Process component for which predictions will
+            be generated. It is optional when inside a with context, otherwise
+            it is required.
         """
         if given is None:
             given = {}
         mu, cov = self._predict_at(Xnew, diag, pred_noise, given, jitter)
         return replace_with_values([mu, cov], replacements=point, model=model)
 
     def _predict_at(self, Xnew, diag=False, pred_noise=False, given=None, jitter=JITTER_DEFAULT):
         R"""
         Return the mean vector and covariance matrix of the conditional
         distribution as symbolic variables.
 
         Parameters
         ----------
-        Xnew: array-like
+        Xnew : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        diag: bool
+        diag : bool, default False
             If `True`, return the diagonal instead of the full covariance
-            matrix.  Default is `False`.
-        pred_noise: bool
+            matrix.
+        pred_noise : bool, default False
             Whether or not observation noise is included in the conditional.
-            Default is `False`.
-        given: dict
-            Same as `conditional` method.
+        given : dict, optional
+            Can take key value pairs: `X`, `y`, `sigma`,
+            and `gp`. See the :ref:`section <additive_gp>` in the documentation
+            on additive GP models in pymc for more information.
         """
         givens = self._get_given_vals(given)
         mu, cov = self._build_conditional(Xnew, pred_noise, diag, *givens, jitter)
         return mu, cov
 
 
 @conditioned_vars(["X", "Xu", "y", "sigma"])
@@ -648,21 +667,20 @@
 
     - DTC: Deterministic Training Conditional
     - FITC: Fully independent Training Conditional
     - VFE: Variational Free Energy
 
     Parameters
     ----------
-    cov_func: None, 2D array, or instance of Covariance
-        The covariance function.  Defaults to zero.
-    mean_func: None, instance of Mean
-        The mean function.  Defaults to zero.
-    approx: string
+    mean_func : Mean, default ~pymc.gp.mean.Zero
+        The mean function.
+    cov_func : 2D array-like, or Covariance, default ~pymc.gp.cov.Constant
+        The covariance function.
+    approx : str, default 'VFE'
         The approximation to use.  Must be one of `VFE`, `FITC` or `DTC`.
-        Default is VFE.
 
     Examples
     --------
     .. code:: python
 
         # A one dimensional column vector of inputs.
         X = np.linspace(0, 1, 10)[:, None]
@@ -752,33 +770,33 @@
         R"""
         Returns the approximate marginal likelihood distribution, given the input
         locations `X`, inducing point locations `Xu`, data `y`, and white noise
         standard deviations `sigma`.
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        X: array-like
+        X : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        Xu: array-like
+        Xu : array-like
             The inducing points.  Must have the same number of columns as `X`.
-        y: array-like
+        y : array-like
             Data that is the sum of the function with the GP prior and Gaussian
             noise.  Must have shape `(n, )`.
-        sigma: scalar, Variable
+        sigma : float, Variable
             Standard deviation of the Gaussian noise.
-        noise: scalar, Variable
-            Previous parameterization of `sigma`
-        jitter: scalar
+        noise : float, Variable, optional
+            Previous parameterization of `sigma`.
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to `MvNormal` distribution
+            Extra keyword arguments that are passed to :class:`~pymc.MvNormal` distribution
             constructor.
         """
 
         self.X = X
         self.Xu = Xu
         self.y = y
 
@@ -844,31 +862,30 @@
     ):
         R"""
         Returns the approximate conditional distribution of the GP evaluated over
         new input locations `Xnew`.
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        Xnew: array-like
+        Xnew : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        pred_noise: bool
+        pred_noise : bool, default False
             Whether or not observation noise is included in the conditional.
-            Default is `False`.
-        given: dict
-            Can optionally take as key value pairs: `X`, `Xu`, `y`, `sigma`,
-            and `gp`.  See the section in the documentation on additive GP
-            models in PyMC for more information.
-        jitter: scalar
+        given : dict, optional
+            Can take key value pairs: `X`, `Xu`, `y`, `sigma`,
+            and `gp`. See the :ref:`section <additive_gp>` in the documentation
+            on additive GP models in pymc for more information.
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to `MvNormal` distribution
+            Extra keyword arguments that are passed to :class:`~pymc.MvNormal` distribution
             constructor.
         """
 
         givens = self._get_given_vals(given)
         mu, cov = self._build_conditional(Xnew, pred_noise, False, *givens, jitter)
         return pm.MvNormal(name, mu=mu, cov=cov, **kwargs)
 
@@ -888,28 +905,27 @@
     R"""
     Latent Gaussian process whose covariance is a tensor product kernel.
 
     The `gp.LatentKron` class is a direct implementation of a GP with a
     Kronecker structured covariance, without reference to any noise or
     specific likelihood.  The GP is constructed with the `prior` method,
     and the conditional GP over new input locations is constructed with
-    the `conditional` method.  `conditional` and method.  For more
+    the `conditional` method. For more
     information on these methods, see their docstrings.  This GP
     implementation can be used to model a Gaussian process whose inputs
     cover evenly spaced grids on more than one dimension.  `LatentKron`
-    is relies on the `KroneckerNormal` distribution, see its docstring
+    relies on the `KroneckerNormal` distribution, see its docstring
     for more information.
 
     Parameters
     ----------
-    cov_funcs: list of Covariance objects
+    mean_func : Mean, default ~pymc.gp.mean.Zero
+        The mean function.
+    cov_funcs : list of Covariance, default [~pymc.gp.cov.Constant]
         The covariance functions that compose the tensor (Kronecker) product.
-        Defaults to [zero].
-    mean_func: None, instance of Mean
-        The mean function.  Defaults to zero.
 
     Examples
     --------
     .. code:: python
 
         # One dimensional column vectors of inputs
         X1 = np.linspace(0, 1, 10)[:, None]
@@ -959,26 +975,26 @@
     def prior(self, name, Xs, jitter=JITTER_DEFAULT, **kwargs):
         """
         Returns the prior distribution evaluated over the input
         locations `Xs`.
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        Xs: list of array-like
+        Xs : list of array-like
             Function input values for each covariance function. Each entry
             must be passable to its respective covariance without error. The
             total covariance function is measured on the full grid
             `cartesian(*Xs)`.
-        jitter: scalar
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to the `KroneckerNormal`
+            Extra keyword arguments that are passed to the :class:`~pymc.KroneckerNormal`
             distribution constructor.
         """
         if len(Xs) != len(self.cov_funcs):
             raise ValueError("Must provide a covariance function for each X")
 
         f = self._build_prior(name, Xs, jitter, **kwargs)
         self.Xs = Xs
@@ -1020,24 +1036,24 @@
         The distribution returned by `conditional` does not have a
         Kronecker structure regardless of whether the input points lie
         on a full grid.  Therefore, `Xnew` does not need to have grid
         structure.
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        Xnew: array-like
+        Xnew : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        jitter: scalar
+        jitter : float, default 1e-6
             A small correction added to the diagonal of positive semi-definite
             covariance matrices to ensure numerical stability.
         **kwargs
-            Extra keyword arguments that are passed to `MvNormal` distribution
+            Extra keyword arguments that are passed to :class:`~pymc.MvNormal` distribution
             constructor.
         """
         mu, cov = self._build_conditional(Xnew, jitter)
         return pm.MvNormal(name, mu=mu, cov=cov, **kwargs)
 
 
 @conditioned_vars(["Xs", "y", "sigma"])
@@ -1049,23 +1065,23 @@
     Kronecker GP prior and additive white noise. It has
     `marginal_likelihood`, `conditional` and `predict` methods. This GP
     implementation can be used to efficiently implement regression on
     data that are normally distributed with a tensor product kernel and
     are measured on a full grid of inputs: `cartesian(*Xs)`.
     `MarginalKron` is based on the `KroneckerNormal` distribution, see
     its docstring for more information. For more information on the
-    `prior` and `conditional` methods, see their docstrings.
+    `marginal_likelihood`, `conditional` and `predict` methods,
+    see their docstrings.
 
     Parameters
     ----------
-    cov_funcs: list of Covariance objects
+    mean_func : Mean, default ~pymc.gp.mean.Zero
+        The mean function.
+    cov_funcs : list of Covariance, default [~pymc.gp.cov.Constant]
         The covariance functions that compose the tensor (Kronecker) product.
-        Defaults to [zero].
-    mean_func: None, instance of Mean
-        The mean function.  Defaults to zero.
 
     Examples
     --------
     .. code:: python
 
         # One dimensional column vectors of inputs
         X1 = np.linspace(0, 1, 10)[:, None]
@@ -1127,31 +1143,30 @@
     def marginal_likelihood(self, name, Xs, y, sigma, is_observed=True, **kwargs):
         """
         Returns the marginal likelihood distribution, given the input
         locations `cartesian(*Xs)` and the data `y`.
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        Xs: list of array-like
+        Xs : list of array-like
             Function input values for each covariance function. Each entry
             must be passable to its respective covariance without error. The
             total covariance function is measured on the full grid
             `cartesian(*Xs)`.
-        y: array-like
+        y : array-like
             Data that is the sum of the function with the GP prior and Gaussian
             noise.  Must have shape `(n, )`.
-        sigma: scalar, Variable
+        sigma : float, Variable
             Standard deviation of the white Gaussian noise.
-        is_observed: bool
-            Whether to set `y` as an `observed` variable in the `model`.
-            Default is `True`.
+        is_observed : bool, default True
+            Deprecated. Whether to set `y` as an `observed` variable in the `model`.
         **kwargs
-            Extra keyword arguments that are passed to `KroneckerNormal`
+            Extra keyword arguments that are passed to :class:`~pymc.KroneckerNormal`
             distribution constructor.
         """
         self._check_inputs(Xs, y)
         mu, covs = self._build_marginal_likelihood(Xs)
         self.Xs = Xs
         self.y = y
         self.sigma = sigma
@@ -1222,64 +1237,65 @@
         The distribution returned by `conditional` does not have a
         Kronecker structure regardless of whether the input points lie
         on a full grid.  Therefore, `Xnew` does not need to have grid
         structure.
 
         Parameters
         ----------
-        name: string
+        name : str
             Name of the random variable
-        Xnew: array-like
+        Xnew : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        pred_noise: bool
+        pred_noise : bool, default False
             Whether or not observation noise is included in the conditional.
-            Default is `False`.
         **kwargs
-            Extra keyword arguments that are passed to `MvNormal` distribution
+            Extra keyword arguments that are passed to :class:`~pymc.MvNormal` distribution
             constructor.
         """
         mu, cov = self._build_conditional(Xnew, diag, pred_noise)
         return pm.MvNormal(name, mu=mu, cov=cov, **kwargs)
 
     def predict(self, Xnew, point=None, diag=False, pred_noise=False, model=None):
         R"""
         Return the mean vector and covariance matrix of the conditional
         distribution as numpy arrays, given a `point`, such as the MAP
         estimate or a sample from a `trace`.
 
         Parameters
         ----------
-        Xnew: array-like
+        Xnew : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        point: pymc.model.Point
+        point : pymc.Point, optional
             A specific point to condition on.
-        diag: bool
+        diag : bool, default False
             If `True`, return the diagonal instead of the full covariance
-            matrix.  Default is `False`.
-        pred_noise: bool
+            matrix.
+        pred_noise : bool, default False
             Whether or not observation noise is included in the conditional.
-            Default is `False`.
+        model : Model, optional
+            Model with the Gaussian Process component for which predictions will
+            be generated. It is optional when inside a with context, otherwise
+            it is required.
         """
         mu, cov = self._predict_at(Xnew, diag, pred_noise)
         return replace_with_values([mu, cov], replacements=point, model=model)
 
     def _predict_at(self, Xnew, diag=False, pred_noise=False):
         R"""
         Return the mean vector and covariance matrix of the conditional
         distribution as symbolic variables.
 
         Parameters
         ----------
-        Xnew: array-like
+        Xnew : array-like
             Function input values.  If one-dimensional, must be a column
             vector with shape `(n, 1)`.
-        diag: bool
+        diag : bool, default False
             If `True`, return the diagonal instead of the full covariance
-            matrix.  Default is `False`.
-        pred_noise: bool
+            matrix.
+        pred_noise : bool, default False
             Whether or not observation noise is included in the conditional.
-            Default is `False`.
         """
         mu, cov = self._build_conditional(Xnew, diag, pred_noise)
         return mu, cov
```

### Comparing `pymc-5.2.0/pymc/gp/hsgp_approx.py` & `pymc-5.3.0/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/gp/mean.py` & `pymc-5.3.0/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/gp/util.py` & `pymc-5.3.0/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/initial_point.py` & `pymc-5.3.0/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/__init__.py` & `pymc-5.3.0/pymc/logprob/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/abstract.py` & `pymc-5.3.0/pymc/logprob/abstract.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/basic.py` & `pymc-5.3.0/pymc/logprob/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,48 +61,87 @@
 from pymc.logprob.rewriting import construct_ir_fgraph
 from pymc.logprob.transforms import RVTransform, TransformValuesRewrite
 from pymc.logprob.utils import rvs_to_value_vars
 
 TensorLike: TypeAlias = Union[Variable, float, np.ndarray]
 
 
-def logp(rv: TensorVariable, value: TensorLike, **kwargs) -> TensorVariable:
+def _warn_rvs_in_inferred_graph(graph: Sequence[TensorVariable]):
+    """Issue warning if any RVs are found in graph.
+
+    RVs are usually an (implicit) conditional input of the derived probability expression,
+    and meant to be replaced by respective value variables before evaluation.
+    However, when the IR graph is built, any non-input nodes (including RVs) are cloned,
+    breaking the link with the original ones.
+    This makes it impossible (or difficult) to replace it by the respective values afterward,
+    so we instruct users to do it beforehand.
+    """
+    from pymc.testing import assert_no_rvs
+
+    try:
+        assert_no_rvs(graph)
+    except AssertionError:
+        warnings.warn(
+            "RandomVariables were found in the derived graph. "
+            "These variables are a clone and do not match the original ones on identity.\n"
+            "If you are deriving a quantity that depends on model RVs, use `model.replace_rvs_by_values` first. For example: "
+            "`logp(model.replace_rvs_by_values([rv])[0], value)`",
+            stacklevel=3,
+        )
+
+
+def logp(
+    rv: TensorVariable, value: TensorLike, warn_missing_rvs: bool = True, **kwargs
+) -> TensorVariable:
     """Return the log-probability graph of a Random Variable"""
 
     value = pt.as_tensor_variable(value, dtype=rv.dtype)
     try:
         return _logprob_helper(rv, value, **kwargs)
     except NotImplementedError:
         fgraph, _, _ = construct_ir_fgraph({rv: value})
         [(ir_rv, ir_value)] = fgraph.preserve_rv_mappings.rv_values.items()
-        return _logprob_helper(ir_rv, ir_value, **kwargs)
+        expr = _logprob_helper(ir_rv, ir_value, **kwargs)
+        if warn_missing_rvs:
+            _warn_rvs_in_inferred_graph(expr)
+        return expr
 
 
-def logcdf(rv: TensorVariable, value: TensorLike, **kwargs) -> TensorVariable:
+def logcdf(
+    rv: TensorVariable, value: TensorLike, warn_missing_rvs: bool = True, **kwargs
+) -> TensorVariable:
     """Create a graph for the log-CDF of a Random Variable."""
     value = pt.as_tensor_variable(value, dtype=rv.dtype)
     try:
         return _logcdf_helper(rv, value, **kwargs)
     except NotImplementedError:
         # Try to rewrite rv
         fgraph, rv_values, _ = construct_ir_fgraph({rv: value})
         [ir_rv] = fgraph.outputs
-        return _logcdf_helper(ir_rv, value, **kwargs)
+        expr = _logcdf_helper(ir_rv, value, **kwargs)
+        if warn_missing_rvs:
+            _warn_rvs_in_inferred_graph(expr)
+        return expr
 
 
-def icdf(rv: TensorVariable, value: TensorLike, **kwargs) -> TensorVariable:
+def icdf(
+    rv: TensorVariable, value: TensorLike, warn_missing_rvs: bool = True, **kwargs
+) -> TensorVariable:
     """Create a graph for the inverse CDF of a  Random Variable."""
-    value = pt.as_tensor_variable(value, dtype=rv.dtype)
+    value = pt.as_tensor_variable(value, dtype="floatX")
     try:
         return _icdf_helper(rv, value, **kwargs)
     except NotImplementedError:
         # Try to rewrite rv
         fgraph, rv_values, _ = construct_ir_fgraph({rv: value})
         [ir_rv] = fgraph.outputs
-        return _icdf_helper(ir_rv, value, **kwargs)
+        expr = _icdf_helper(ir_rv, value, **kwargs)
+        if warn_missing_rvs:
+            _warn_rvs_in_inferred_graph(expr)
+        return expr
 
 
 def factorized_joint_logprob(
     rv_values: Dict[TensorVariable, TensorVariable],
     warn_missing_rvs: bool = True,
     ir_rewriter: Optional[GraphRewriter] = None,
     extra_rewrites: Optional[Union[GraphRewriter, NodeRewriter]] = None,
@@ -211,15 +250,16 @@
         if not outputs:
             continue
 
         if any(o not in updated_rv_values for o in outputs):
             if warn_missing_rvs:
                 warnings.warn(
                     "Found a random variable that was neither among the observations "
-                    f"nor the conditioned variables: {node.outputs}"
+                    f"nor the conditioned variables: {outputs}.\n"
+                    "This variables is a clone and does not match the original one on identity."
                 )
             continue
 
         q_value_vars = [replacements[q_rv_var] for q_rv_var in outputs]
 
         if not q_value_vars:
             continue
```

### Comparing `pymc-5.2.0/pymc/logprob/censoring.py` & `pymc-5.3.0/pymc/logprob/censoring.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/checks.py` & `pymc-5.3.0/pymc/logprob/checks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/cumsum.py` & `pymc-5.3.0/pymc/logprob/cumsum.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/mixture.py` & `pymc-5.3.0/pymc/logprob/mixture.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/rewriting.py` & `pymc-5.3.0/pymc/logprob/rewriting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/scan.py` & `pymc-5.3.0/pymc/logprob/scan.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/tensor.py` & `pymc-5.3.0/pymc/logprob/tensor.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/logprob/transforms.py` & `pymc-5.3.0/pymc/logprob/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,15 +604,15 @@
         transform = AbsTransform()
     elif isinstance(scalar_op, Pow):
         # We only allow for the base to be measurable
         if measurable_input_idx != 0:
             return None
         try:
             (power,) = other_inputs
-            power = pt.get_scalar_constant_value(power).item()
+            power = pt.get_underlying_scalar_constant_value(power).item()
         # Power needs to be a constant
         except NotScalarConstantError:
             return None
         transform_inputs = (measurable_input, power)
         transform = PowerTransform(power=power)
     elif isinstance(scalar_op, Add):
         transform_inputs = (measurable_input, pt.add(*other_inputs))
```

### Comparing `pymc-5.2.0/pymc/logprob/utils.py` & `pymc-5.3.0/pymc/logprob/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/math.py` & `pymc-5.3.0/pymc/math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/model.py` & `pymc-5.3.0/pymc/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,27 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import functools
+import sys
 import threading
 import types
 import warnings
 
 from sys import modules
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     List,
+    Literal,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
@@ -35,21 +37,23 @@
 
 import numpy as np
 import pytensor
 import pytensor.sparse as sparse
 import pytensor.tensor as pt
 import scipy.sparse as sps
 
+from pytensor.compile import DeepCopyOp, get_mode
 from pytensor.compile.sharedvalue import SharedVariable
 from pytensor.graph.basic import Constant, Variable, graph_inputs
 from pytensor.graph.fg import FunctionGraph
 from pytensor.scalar import Cast
 from pytensor.tensor.elemwise import Elemwise
 from pytensor.tensor.random.op import RandomVariable
 from pytensor.tensor.random.rewriting import local_subtensor_rv_lift
+from pytensor.tensor.random.type import RandomType
 from pytensor.tensor.sharedvar import ScalarSharedVariable
 from pytensor.tensor.var import TensorConstant, TensorVariable
 
 from pymc.blocking import DictToArrayBijection, RaveledVars
 from pymc.data import GenTensorVariable, is_minibatch
 from pymc.distributions.transforms import _default_transform
 from pymc.exceptions import (
@@ -57,14 +61,15 @@
     ImputationWarning,
     SamplingError,
     ShapeError,
     ShapeWarning,
 )
 from pymc.initial_point import make_initial_point_fn
 from pymc.logprob.basic import joint_logp
+from pymc.logprob.utils import ParameterValueError
 from pymc.pytensorf import (
     PointFunc,
     SeedSequenceSeed,
     compile_pymc,
     convert_observed_data,
     gradient,
     hessian,
@@ -1434,15 +1439,15 @@
             # Now, we lift the non-missing observed values and produce a new
             # `rv_var` that contains only those.
             #
             # The end result is two disjoint distributions: one for the missing
             # values, and another for the non-missing values.
 
             antimask_idx = (~mask).nonzero()
-            nonmissing_data = pt.as_tensor_variable(data[antimask_idx])
+            nonmissing_data = pt.as_tensor_variable(data[antimask_idx].data)
             unmasked_rv_var = rv_var[antimask_idx]
             unmasked_rv_var = unmasked_rv_var.owner.clone().default_output()
 
             fgraph = FunctionGraph(
                 [i for i in graph_inputs((unmasked_rv_var,)) if not isinstance(i, Constant)],
                 [unmasked_rv_var],
                 clone=False,
@@ -1775,15 +1780,16 @@
 
             initial_eval = self.point_logps(point=elem)
 
             if not all(np.isfinite(v) for v in initial_eval.values()):
                 raise SamplingError(
                     "Initial evaluation of model at starting point failed!\n"
                     f"Starting values:\n{elem}\n\n"
-                    f"Logp initial evaluation results:\n{initial_eval}"
+                    f"Logp initial evaluation results:\n{initial_eval}\n"
+                    "You can call `model.debug()` for more details."
                 )
 
     def point_logps(self, point=None, round_vals=2):
         """Computes the log probability of `point` for all random variables in the model.
 
         Parameters
         ----------
@@ -1807,14 +1813,160 @@
             factor.name: np.round(np.asarray(factor_logp), round_vals)
             for factor, factor_logp in zip(
                 factors,
                 self.compile_fn(factor_logps_fn)(point),
             )
         }
 
+    def debug(
+        self,
+        point: Optional[Dict[str, np.ndarray]] = None,
+        fn: Literal["logp", "dlogp", "random"] = "logp",
+        verbose: bool = False,
+    ):
+        """Debug model function at point.
+
+        The method will evaluate the `fn` for each variable at a time.
+        When an evaluation fails or produces a non-finite value we print:
+         1. The graph of the parameters
+         2. The value of the parameters (if those can be evaluated)
+         3. The output of `fn` (if it can be evaluated)
+
+        This function should help to quickly narrow down invalid parametrizations.
+
+        Parameters
+        ----------
+        point : Point
+            Point at which model function should be evaluated
+        fn : str, default "logp"
+            Function to be used for debugging. Can be one of [logp, dlogp, random].
+        verbose : bool, default False
+            Whether to show a more verbose PyTensor output when function cannot be evaluated
+        """
+        print_ = functools.partial(print, file=sys.stdout)
+
+        def first_line(exc):
+            return exc.args[0].split("\n")[0]
+
+        def debug_parameters(rv):
+            if isinstance(rv.owner.op, RandomVariable):
+                inputs = rv.owner.inputs[3:]
+            else:
+                inputs = [inp for inp in rv.owner.inputs if not isinstance(inp.type, RandomType)]
+            rv_inputs = pytensor.function(
+                self.value_vars,
+                self.replace_rvs_by_values(inputs),
+                on_unused_input="ignore",
+                mode=get_mode(None).excluding("inplace", "fusion"),
+            )
+
+            print_(f"The variable {rv} has the following parameters:")
+            # done and used_ids are used to keep the same ids across distinct dprint calls
+            done = {}
+            used_ids = {}
+            for i, out in enumerate(rv_inputs.maker.fgraph.outputs):
+                print_(f"{i}: ", end=""),
+                # Don't print useless deepcopys
+                if out.owner and isinstance(out.owner.op, DeepCopyOp):
+                    out = out.owner.inputs[0]
+                pytensor.dprint(out, print_type=True, done=done, used_ids=used_ids)
+
+            try:
+                print_("The parameters evaluate to:")
+                for i, rv_input_eval in enumerate(rv_inputs(**point)):
+                    print_(f"{i}: {rv_input_eval}")
+            except Exception as exc:
+                print_(
+                    f"The parameters of the variable {rv} cannot be evaluated: {first_line(exc)}"
+                )
+                if verbose:
+                    print_(exc, "\n")
+
+        if fn not in ("logp", "dlogp", "random"):
+            raise ValueError(f"fn must be one of [logp, dlogp, random], got {fn}")
+
+        if point is None:
+            point = self.initial_point()
+        print_(f"point={point}\n")
+
+        rvs_to_check = list(self.basic_RVs)
+        if fn in ("logp", "dlogp"):
+            rvs_to_check += [self.replace_rvs_by_values(p) for p in self.potentials]
+
+        found_problem = False
+        for rv in rvs_to_check:
+            if fn == "logp":
+                rv_fn = pytensor.function(
+                    self.value_vars, self.logp(vars=rv, sum=False)[0], on_unused_input="ignore"
+                )
+            elif fn == "dlogp":
+                rv_fn = pytensor.function(
+                    self.value_vars, self.dlogp(vars=rv), on_unused_input="ignore"
+                )
+            else:
+                [rv_inputs_replaced] = replace_rvs_by_values(
+                    [rv],
+                    # Don't include itself, or the function will just the the value variable
+                    rvs_to_values={
+                        rv_key: value
+                        for rv_key, value in self.rvs_to_values.items()
+                        if rv_key is not rv
+                    },
+                    rvs_to_transforms=self.rvs_to_transforms,
+                )
+                rv_fn = pytensor.function(
+                    self.value_vars, rv_inputs_replaced, on_unused_input="ignore"
+                )
+
+            try:
+                rv_fn_eval = rv_fn(**point)
+            except ParameterValueError as exc:
+                found_problem = True
+                debug_parameters(rv)
+                print_(
+                    f"This does not respect one of the following constraints: {first_line(exc)}\n"
+                )
+                if verbose:
+                    print_(exc)
+            except Exception as exc:
+                found_problem = True
+                debug_parameters(rv)
+                print_(
+                    f"The variable {rv} {fn} method raised the following exception: {first_line(exc)}\n"
+                )
+                if verbose:
+                    print_(exc)
+            else:
+                if not np.all(np.isfinite(rv_fn_eval)):
+                    found_problem = True
+                    debug_parameters(rv)
+                    if fn == "random" or rv is self.potentials:
+                        print_("This combination seems able to generate non-finite values")
+                    else:
+                        # Find which values are associated with non-finite evaluation
+                        values = self.rvs_to_values[rv]
+                        if rv in self.observed_RVs:
+                            values = values.eval()
+                        else:
+                            values = point[values.name]
+
+                        observed = " observed " if rv in self.observed_RVs else " "
+                        print_(
+                            f"Some of the{observed}values of variable {rv} are associated with a non-finite {fn}:"
+                        )
+                        mask = ~np.isfinite(rv_fn_eval)
+                        for value, fn_eval in zip(values[mask], rv_fn_eval[mask]):
+                            print_(f" value = {value} -> {fn} = {fn_eval}")
+                        print_()
+
+        if not found_problem:
+            print_("No problems found")
+        elif not verbose:
+            print_("You can set `verbose=True` for more details")
+
 
 # this is really disgusting, but it breaks a self-loop: I can't pass Model
 # itself as context class init arg.
 Model._context_class = Model
 
 
 class BlockModelAccess(Model):
```

### Comparing `pymc-5.2.0/pymc/model_graph.py` & `pymc-5.3.0/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/ode/__init__.py` & `pymc-5.3.0/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/ode/ode.py` & `pymc-5.3.0/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/ode/utils.py` & `pymc-5.3.0/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/plots/__init__.py` & `pymc-5.3.0/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/printing.py` & `pymc-5.3.0/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/pytensorf.py` & `pymc-5.3.0/pymc/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/sampling/__init__.py` & `pymc-5.3.0/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/sampling/forward.py` & `pymc-5.3.0/pymc/sampling/forward.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/sampling/jax.py` & `pymc-5.3.0/pymc/sampling/jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/sampling/mcmc.py` & `pymc-5.3.0/pymc/sampling/mcmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/sampling/parallel.py` & `pymc-5.3.0/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/sampling/population.py` & `pymc-5.3.0/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/sampling_jax.py` & `pymc-5.3.0/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/smc/__init__.py` & `pymc-5.3.0/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/smc/kernels.py` & `pymc-5.3.0/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/smc/sampling.py` & `pymc-5.3.0/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/stats/__init__.py` & `pymc-5.3.0/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/stats/convergence.py` & `pymc-5.3.0/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/stats/log_likelihood.py` & `pymc-5.3.0/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/__init__.py` & `pymc-5.3.0/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/arraystep.py` & `pymc-5.3.0/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/compound.py` & `pymc-5.3.0/pymc/step_methods/compound.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/hmc/__init__.py` & `pymc-5.3.0/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.3.0/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/hmc/hmc.py` & `pymc-5.3.0/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/hmc/integration.py` & `pymc-5.3.0/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/hmc/nuts.py` & `pymc-5.3.0/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.3.0/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/metropolis.py` & `pymc-5.3.0/pymc/step_methods/metropolis.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/slicer.py` & `pymc-5.3.0/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/step_methods/step_sizes.py` & `pymc-5.3.0/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/testing.py` & `pymc-5.3.0/pymc/testing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/tuning/__init__.py` & `pymc-5.3.0/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/tuning/scaling.py` & `pymc-5.3.0/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/tuning/starting.py` & `pymc-5.3.0/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/util.py` & `pymc-5.3.0/pymc/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/__init__.py` & `pymc-5.3.0/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/approximations.py` & `pymc-5.3.0/pymc/variational/approximations.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/callbacks.py` & `pymc-5.3.0/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/inference.py` & `pymc-5.3.0/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/minibatch_rv.py` & `pymc-5.3.0/pymc/variational/minibatch_rv.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/operators.py` & `pymc-5.3.0/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/opvi.py` & `pymc-5.3.0/pymc/variational/opvi.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/stein.py` & `pymc-5.3.0/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/test_functions.py` & `pymc-5.3.0/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/variational/updates.py` & `pymc-5.3.0/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc/vartypes.py` & `pymc-5.3.0/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/pymc.egg-info/PKG-INFO` & `pymc-5.3.0/pymc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.2.0
+Version: 5.3.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
@@ -165,21 +165,21 @@
            :target: https://mybinder.org/v2/gh/pymc-devs/pymc/main?filepath=%2Fdocs%2Fsource%2Fnotebooks
         .. |Build Status| image:: https://github.com/pymc-devs/pymc/workflows/pytest/badge.svg
            :target: https://github.com/pymc-devs/pymc/actions
         .. |Coverage| image:: https://codecov.io/gh/pymc-devs/pymc/branch/main/graph/badge.svg
            :target: https://codecov.io/gh/pymc-devs/pymc
         .. |Dockerhub| image:: https://img.shields.io/docker/automated/pymc/pymc.svg
            :target: https://hub.docker.com/r/pymc/pymc
-        .. |NumFOCUS| image:: https://www.numfocus.org/wp-content/uploads/2017/03/1457562110.png
-           :target: http://www.numfocus.org/
         .. |NumFOCUS_badge| image:: https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A
            :target: http://www.numfocus.org/
-        .. |PyMCLabs| image:: https://raw.githubusercontent.com/pymc-devs/pymc/main/docs/logos/sponsors/pymc-labs.png
+        .. |NumFOCUS| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_numfocus.png?raw=true
+           :target: http://www.numfocus.org/
+        .. |PyMCLabs| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_pymc_labs.png?raw=true
            :target: https://pymc-labs.io
-        .. |Mistplay| image:: https://github.com/pymc-devs/pymcon_web_series_website/blob/main/static/images/sponsors_logos/mistplay_label_dark.png?raw=true
+        .. |Mistplay| image:: https://github.com/pymc-devs/brand/blob/main/sponsors/sponsor_logos/sponsor_mistplay.png?raw=true
            :target: https://www.mistplay.com/
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pymc-5.2.0/pymc.egg-info/SOURCES.txt` & `pymc-5.3.0/pymc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/scripts/docker_container.sh` & `pymc-5.3.0/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/setup.py` & `pymc-5.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.2.0/versioneer.py` & `pymc-5.3.0/versioneer.py`

 * *Files identical despite different names*

