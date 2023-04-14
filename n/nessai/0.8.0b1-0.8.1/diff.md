# Comparing `tmp/nessai-0.8.0b1.tar.gz` & `tmp/nessai-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessai-0.8.0b1.tar", last modified: Mon Feb 20 16:30:07 2023, max compression
+gzip compressed data, was "nessai-0.8.1.tar", last modified: Fri Apr 14 10:22:16 2023, max compression
```

## Comparing `nessai-0.8.0b1.tar` & `nessai-0.8.1.tar`

### file list

```diff
@@ -1,226 +1,226 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.997073 nessai-0.8.0b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.969072 nessai-0.8.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.973072 nessai-0.8.0b1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.973072 nessai-0.8.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.github/workflows/compatibility-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-20 16:29:54.000000 nessai-0.8.0b1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35941 2023-02-20 16:29:54.000000 nessai-0.8.0b1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-20 16:29:54.000000 nessai-0.8.0b1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-20 16:29:54.000000 nessai-0.8.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-02-20 16:30:06.997073 nessai-0.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-02-20 16:29:54.000000 nessai-0.8.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-20 16:29:54.000000 nessai-0.8.0b1/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.977073 nessai-0.8.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.977073 nessai-0.8.0b1/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/assets/insertion_indices.png
--rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/assets/logXlogL.png
--rw-r--r--   0 runner    (1001) docker     (123)    70482 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/assets/posterior_distribution.png
--rw-r--r--   0 runner    (1001) docker     (123)   159636 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/assets/state.png
--rw-r--r--   0 runner    (1001) docker     (123)    20221 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/assets/trace.png
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/bilby-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/further-details.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/gaussian-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/gravitational-wave-inference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/normalising-flows-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/parallelisation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/reparameterisations.rst
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/running-the-sampler.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-02-20 16:29:54.000000 nessai-0.8.0b1/docs/sampler-configuration.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.977073 nessai-0.8.0b1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/2d_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/augmented_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/bilby_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/bilby_unbounded_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/corner_plot_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/eggbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.977073 nessai-0.8.0b1/examples/gw/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/gw/basic_gw_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/gw/calibration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/gw/full_gw_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/half_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/parallelisation_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/reparameterisations_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-20 16:29:54.000000 nessai-0.8.0b1/examples/unbounded_prior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.981073 nessai-0.8.0b1/nessai/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/evidence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.981073 nessai-0.8.0b1/nessai/flowmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flowmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flowmodel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flowmodel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flowmodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.981073 nessai-0.8.0b1/nessai/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/realnvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/flowsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.981073 nessai-0.8.0b1/nessai/gw/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/gw/proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/gw/reparameterisations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/gw/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/livepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/nestedsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18724 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/priors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.985073 nessai-0.8.0b1/nessai/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/proposal/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/proposal/augmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/proposal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    57643 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/proposal/flowproposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/proposal/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/proposal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.985073 nessai-0.8.0b1/nessai/reparameterisations/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/reparameterisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/reparameterisations/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/reparameterisations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/reparameterisations/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/reparameterisations/null.py
--rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/reparameterisations/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/reparameterisations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.985073 nessai-0.8.0b1/nessai/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/samplers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    47635 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/samplers/nestedsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.985073 nessai-0.8.0b1/nessai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/bilbyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-02-20 16:29:54.000000 nessai-0.8.0b1/nessai/utils/torchutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.981073 nessai-0.8.0b1/nessai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-02-20 16:30:06.000000 nessai-0.8.0b1/nessai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-02-20 16:30:06.000000 nessai-0.8.0b1/nessai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 16:30:06.000000 nessai-0.8.0b1/nessai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-20 16:30:06.000000 nessai-0.8.0b1/nessai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-20 16:30:06.000000 nessai-0.8.0b1/nessai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-20 16:29:54.000000 nessai-0.8.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-20 16:29:54.000000 nessai-0.8.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-02-20 16:30:06.997073 nessai-0.8.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-20 16:29:54.000000 nessai-0.8.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.989073 nessai-0.8.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_bilby_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_deprecation_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_evidence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.989073 nessai-0.8.0b1/tests/test_flowmodel/
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flowmodel/test_flowmodel_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flowmodel/test_flowmodel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.989073 nessai-0.8.0b1/tests/test_flows/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flows/test_base_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flows/test_distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flows/test_flow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flows/test_included_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flows/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flows/test_specific_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    21368 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_flowsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.989073 nessai-0.8.0b1/tests/test_gw/
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_gw/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_gw/test_distance_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_gw/test_gw_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_gw/test_gw_reparameterisations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_gw/test_reparameterisation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_livepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_priors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.989073 nessai-0.8.0b1/tests/test_proposal/
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_augmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_base_proposal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.989073 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    22764 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_proposal/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.993073 nessai-0.8.0b1/tests/test_reparameterisations/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_angle_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_base_reparameterisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_get_reparameterisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_null.py
--rw-r--r--   0 runner    (1001) docker     (123)    36520 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_rescale_to_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_scale_and_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_reparameterisations/test_to_cartesian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.993073 nessai-0.8.0b1/tests/test_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_base_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.993073 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_core_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_flow_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_general_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_live_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_manage_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_ns_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_proposal_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_yield_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 16:30:06.997073 nessai-0.8.0b1/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_bilbyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_distance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_distribution_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_hist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_indices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_rescaling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_sampling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_sorting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_stats_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_structures_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_threading_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_utils/test_torchtutils_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-20 16:29:54.000000 nessai-0.8.0b1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.907367 nessai-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.847367 nessai-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.855367 nessai-0.8.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.859367 nessai-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/compatibility-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-14 10:22:03.000000 nessai-0.8.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-14 10:22:03.000000 nessai-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-14 10:22:03.000000 nessai-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-14 10:22:03.000000 nessai-0.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    38342 2023-04-14 10:22:03.000000 nessai-0.8.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-14 10:22:03.000000 nessai-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-14 10:22:03.000000 nessai-0.8.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-14 10:22:16.907367 nessai-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-14 10:22:03.000000 nessai-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-14 10:22:03.000000 nessai-0.8.1/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.863367 nessai-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.863367 nessai-0.8.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/insertion_indices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/logXlogL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70482 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/posterior_distribution.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159636 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/state.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20221 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/assets/trace.png
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/bilby-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/further-details.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/gaussian-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/gravitational-wave-inference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/normalising-flows-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/parallelisation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/reparameterisations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/running-the-sampler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-14 10:22:03.000000 nessai-0.8.1/docs/sampler-configuration.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.867367 nessai-0.8.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/2d_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/augmented_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/bilby_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/bilby_unbounded_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/corner_plot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/eggbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.867367 nessai-0.8.1/examples/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/gw/basic_gw_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/gw/calibration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/gw/full_gw_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/half_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/parallelisation_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/reparameterisations_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-14 10:22:03.000000 nessai-0.8.1/examples/unbounded_prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.871367 nessai-0.8.1/nessai/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/evidence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.875367 nessai-0.8.1/nessai/flowmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowmodel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowmodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.875367 nessai-0.8.1/nessai/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/nsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/realnvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/flowsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.879367 nessai-0.8.1/nessai/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/gw/proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/gw/reparameterisations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/gw/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/livepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/nestedsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.879367 nessai-0.8.1/nessai/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/augmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57696 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/flowproposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/proposal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.883367 nessai-0.8.1/nessai/reparameterisations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/reparameterisations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.883367 nessai-0.8.1/nessai/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/samplers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47635 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/samplers/nestedsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.887367 nessai-0.8.1/nessai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/bilbyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-14 10:22:03.000000 nessai-0.8.1/nessai/utils/torchutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.871367 nessai-0.8.1/nessai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 10:22:16.000000 nessai-0.8.1/nessai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-14 10:22:03.000000 nessai-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 10:22:03.000000 nessai-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-14 10:22:16.911367 nessai-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 10:22:03.000000 nessai-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.891367 nessai-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_bilby_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_deprecation_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_evidence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.891367 nessai-0.8.1/tests/test_flowmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flowmodel/test_flowmodel_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flowmodel/test_flowmodel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.891367 nessai-0.8.1/tests/test_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_base_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_flow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_included_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flows/test_specific_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21368 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_flowsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.895367 nessai-0.8.1/tests/test_gw/
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/test_distance_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/test_gw_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/test_gw_reparameterisations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_gw/test_reparameterisation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_livepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.895367 nessai-0.8.1/tests/test_proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_augmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_base_proposal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.899367 nessai-0.8.1/tests/test_proposal/test_flowproposal/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_proposal/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.899367 nessai-0.8.1/tests/test_reparameterisations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_angle_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_base_reparameterisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_get_reparameterisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36520 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_rescale_to_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_scale_and_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_reparameterisations/test_to_cartesian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.899367 nessai-0.8.1/tests/test_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_base_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.903367 nessai-0.8.1/tests/test_samplers/test_nested_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_core_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_flow_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_general_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_live_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_manage_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_ns_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_proposal_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_yield_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15119 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 10:22:16.907367 nessai-0.8.1/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_bilbyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_distance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_distribution_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_hist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_indices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_rescaling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_sampling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_sorting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_stats_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_structures_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_threading_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_utils/test_torchtutils_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-14 10:22:03.000000 nessai-0.8.1/tests/test_version.py
```

### Comparing `nessai-0.8.0b1/.github/ISSUE_TEMPLATE/feature_request.md` & `nessai-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/.github/workflows/compatibility-tests.yml` & `nessai-0.8.1/.github/workflows/compatibility-tests.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/.github/workflows/integration-tests.yml` & `nessai-0.8.1/.github/workflows/integration-tests.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/.github/workflows/lint.yml` & `nessai-0.8.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/.github/workflows/publish-to-pypi.yml` & `nessai-0.8.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/.github/workflows/tests.yml` & `nessai-0.8.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/.gitignore` & `nessai-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/.pre-commit-config.yaml` & `nessai-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/CHANGELOG.md` & `nessai-0.8.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,58 +3,68 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.8.1]
+
+### Fixed
+
+- Fix incorrect sign in delta phase reparameterisation ([#292](https://github.com/mj-will/nessai/pull/292))
+- Remove maximum scipy version ([#295](https://github.com/mj-will/nessai/pull/295))
+- Specify three quantiles in default corner kwargs as required by corner 2.2.2 ([#298](https://github.com/mj-will/nessai/pull/298))
+
+## [0.8.0]
+
 ### Added
 
-- Add `DeltaPhaseReparameterisation` for GW analyses.
-- Add `nessai.utils.sorting`.
-- Add `log_posterior_weights` and `effective_n_posterior_samples` to the integral state object.
-- Add a check for the multiprocessing start method when using `n_pool`.
+- Add `DeltaPhaseReparameterisation` for GW analyses. ([#244](https://github.com/mj-will/nessai/pull/244))
+- Add `nessai.utils.sorting`. ([#244](https://github.com/mj-will/nessai/pull/244))
+- Add `log_posterior_weights` and `effective_n_posterior_samples` to the integral state object. ([#248](https://github.com/mj-will/nessai/pull/248))
+- Add a check for the multiprocessing start method when using `n_pool`. ([#250](https://github.com/mj-will/nessai/pull/250))
 - Add option to reverse reparameterisations in `FlowProposal`.
-- Add `disable_vectorisation` to `FlowSampler`.
-- Add `likelihood_chunksize` which allows the user to limit how many points are passed to a vectorised likelihood function at once.
-- Add `allow_multi_valued_likelihood` which allows for multi-valued likelihoods, e.g. that include numerical integration.
-- Add `parameters` keyword argument to `nessai.plot.plot_trace` and pass additional keyword arguments to the plotting function.
-- Add option to construct live points without non-sampling parameters.
-- Add option to use a different estimate of the shrinkage. Default remains unchanged.
-- Add `ScaleAndShift` reparameterisation which includes Z-score normalisation.
-- Add option to specify default result file extension.
+- Add `disable_vectorisation` to `FlowSampler`. ([#254](https://github.com/mj-will/nessai/pull/254))
+- Add `likelihood_chunksize` which allows the user to limit how many points are passed to a vectorised likelihood function at once. ([#256](https://github.com/mj-will/nessai/pull/256))
+- Add `allow_multi_valued_likelihood` which allows for multi-valued likelihoods, e.g. that include numerical integration. ([#257](https://github.com/mj-will/nessai/pull/257))
+- Add `parameters` keyword argument to `nessai.plot.plot_trace` and pass additional keyword arguments to the plotting function. ([#259](https://github.com/mj-will/nessai/pull/259))
+- Add option to construct live points without non-sampling parameters. ([#266](https://github.com/mj-will/nessai/pull/266))
+- Add option to use a different estimate of the shrinkage. Default remains unchanged. ([#248](https://github.com/mj-will/nessai/pull/248), [#269](https://github.com/mj-will/nessai/pull/269))
+- Add `ScaleAndShift` reparameterisation which includes Z-score normalisation. ([#273](https://github.com/mj-will/nessai/pull/273))
+- Add option to specify default result file extension. ([#274](https://github.com/mj-will/nessai/pull/274))
 
 ### Changed
 
-- Refactor `nessai.reparameterisations` into a submodule.
-- Use `torch.inference_mode` instead of `torch.no_grad`.
-- Changed `CombinedReparameterisations` to sort and add reparameterisations based on their requirements.
-- Refactor `nessai.evidence._NSIntegralState` to inherit from a base class.
-- Revert default logging level to `INFO`
-- Rework logging statements to reduce the amount of information printed by default.
-- Refactor `nessai.proposal.FlowProposal.verify_rescaling` to be stricter.
-- Truth input in `nessai.plot.corner_plot` can now be an iterable or a dictionary.
-- Tweak how the prior volume is computed for the final nested sample. This will also change the evidence and posterior weights.
-- Stricter handling of keyword arguments passed to `NestedSampler`. Unknown keyword arguments will now raise an error.
-- Rework `nessai.config` to have `config.livepoints` and `config.plot` which contain global settings. Some of the setting names have also changed.
-- `Rescale` reparameterisation is now an alias for `ScaleAndShift`.
-- Change the default result file extension to `hdf5`, old result file format can be recovered by setting it to `json`.
-- Optimisations to `FlowProposal.populate`, including changes to `Model.in_bounds` and how sampling from the latent prior is handled.
-- Add a maximum figure size (`nessai.config.plotting.max_figsize`) to prevent very large trace plots when the number of dimensions is very high.
+- Refactor `nessai.reparameterisations` into a submodule. ([#241](https://github.com/mj-will/nessai/pull/241))
+- Use `torch.inference_mode` instead of `torch.no_grad`. ([#245](https://github.com/mj-will/nessai/pull/245))
+- Changed `CombinedReparameterisations` to sort and add reparameterisations based on their requirements. ([#244](https://github.com/mj-will/nessai/pull/244), [#253](https://github.com/mj-will/nessai/pull/253))
+- Refactor `nessai.evidence._NSIntegralState` to inherit from a base class. ([#248](https://github.com/mj-will/nessai/pull/248))
+- Revert default logging level to `INFO`. ([#249](https://github.com/mj-will/nessai/pull/249))
+- Rework logging statements to reduce the amount of information printed by default. ([#249](https://github.com/mj-will/nessai/pull/249))
+- Refactor `nessai.proposal.FlowProposal.verify_rescaling` to be stricter. ([#253](https://github.com/mj-will/nessai/pull/253))
+- Truth input in `nessai.plot.corner_plot` can now be an iterable or a dictionary. ([#255](https://github.com/mj-will/nessai/pull/255))
+- Tweak how the prior volume is computed for the final nested sample. This will also change the evidence and posterior weights. ([#248](https://github.com/mj-will/nessai/pull/248), [#269](https://github.com/mj-will/nessai/pull/269))
+- Stricter handling of keyword arguments passed to `NestedSampler`. Unknown keyword arguments will now raise an error. ([#270](https://github.com/mj-will/nessai/pull/270))
+- Rework `nessai.config` to have `config.livepoints` and `config.plot` which contain global settings. Some of the setting names have also changed. ([#272](https://github.com/mj-will/nessai/pull/272))
+- `Rescale` reparameterisation is now an alias for `ScaleAndShift`. ([#273](https://github.com/mj-will/nessai/pull/273))
+- Change the default result file extension to `hdf5`, old result file format can be recovered by setting it to `json`. ([#274](https://github.com/mj-will/nessai/pull/274))
+- Optimisations to `FlowProposal.populate`, including changes to `Model.in_bounds` and how sampling from the latent prior is handled. ([#277](https://github.com/mj-will/nessai/pull/277))
+- Add a maximum figure size (`nessai.config.plotting.max_figsize`) to prevent very large trace plots when the number of dimensions is very high. ([#282](https://github.com/mj-will/nessai/pull/282))
 
 ### Fixed
 
-- Fix a bug where setting the livepoint precision (e.g. `f16`) did not work.
-- Fix plotting failing when sampling large number of parameters.
+- Fix a bug where setting the livepoint precision (e.g. `f16`) did not work. ([#272](https://github.com/mj-will/nessai/pull/272))
+- Fix plotting failing when sampling large number of parameters. ([#281](https://github.com/mj-will/nessai/pull/281), [#282](https://github.com/mj-will/nessai/pull/282))
 
 ### Removed
 
-- Removed `nessai._NSIntegralState.reset`
-- Removed `nessai.gw.legacy`
-- Removed support for changing the variance of the latent distribution via `draw_latent_kwargs` from `FlowProposal`.
+- Removed `nessai._NSIntegralState.reset`. ([#248](https://github.com/mj-will/nessai/pull/248))
+- Removed `nessai.gw.legacy`. ([#267](https://github.com/mj-will/nessai/pull/267))
+- Removed support for changing the variance of the latent distribution via `draw_latent_kwargs` from `FlowProposal`. ([#277](https://github.com/mj-will/nessai/pull/277))
 
 ## [0.7.1]
 
 ### Fixed
 
 - Fix bug that led to the multiprocessing pool not being used when resuming. ([#261](https://github.com/mj-will/nessai/pull/261))
 
@@ -483,15 +493,17 @@
 
 - Fix a bug where `maximum_uninformed` did not have the expected behaviour.
 
 ### Deprecated
 
 - Original `GWFlowProposal` method renamed to `LegacyGWFlowProposal`. Will be removed in the next release.
 
-[Unreleased]: https://github.com/mj-will/nessai/compare/v0.7.1...HEAD
+[Unreleased]: https://github.com/mj-will/nessai/compare/v0.8.1...HEAD
+[0.8.1]: https://github.com/mj-will/nessai/compare/v0.8.0...v0.8.1
+[0.8.0]: https://github.com/mj-will/nessai/compare/v0.7.1...v0.8.0
 [0.7.1]: https://github.com/mj-will/nessai/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/mj-will/nessai/compare/v0.6.0...v0.7.0
 [0.6.0]: https://github.com/mj-will/nessai/compare/v0.5.1...v0.6.0
 [0.5.1]: https://github.com/mj-will/nessai/compare/v0.5.0...v0.5.1
 [0.5.0]: https://github.com/mj-will/nessai/compare/v0.4.0...v0.5.0
 [0.4.0]: https://github.com/mj-will/nessai/compare/v0.3.3...v0.4.0
 [0.3.3]: https://github.com/mj-will/nessai/compare/v0.3.2...v0.3.3
```

### Comparing `nessai-0.8.0b1/CONTRIBUTING.md` & `nessai-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/LICENSE.md` & `nessai-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/PKG-INFO` & `nessai-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai
-Version: 0.8.0b1
+Version: 0.8.1
 Summary: Nessai: Nested Sampling with Artificial Intelligence
 Home-page: https://github.com/mj-will/nessai
 Author: Michael J. Williams
 Author-email: m.williams.4@research.gla.ac.uk
 Project-URL: Documentation, https://nessai.readthedocs.io/
 Keywords: nested sampling,normalising flows,machine learning
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nessai-0.8.0b1/README.md` & `nessai-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/Makefile` & `nessai-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/assets/insertion_indices.png` & `nessai-0.8.1/docs/assets/insertion_indices.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/assets/logXlogL.png` & `nessai-0.8.1/docs/assets/logXlogL.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/assets/posterior_distribution.png` & `nessai-0.8.1/docs/assets/posterior_distribution.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/assets/state.png` & `nessai-0.8.1/docs/assets/state.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/assets/trace.png` & `nessai-0.8.1/docs/assets/trace.png`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/conf.py` & `nessai-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/further-details.rst` & `nessai-0.8.1/docs/further-details.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/gaussian-example.rst` & `nessai-0.8.1/docs/gaussian-example.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/gravitational-wave-inference.rst` & `nessai-0.8.1/docs/gravitational-wave-inference.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/index.rst` & `nessai-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/installation.rst` & `nessai-0.8.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/normalising-flows-configuration.rst` & `nessai-0.8.1/docs/normalising-flows-configuration.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/parallelisation.rst` & `nessai-0.8.1/docs/parallelisation.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/reparameterisations.rst` & `nessai-0.8.1/docs/reparameterisations.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/running-the-sampler.rst` & `nessai-0.8.1/docs/running-the-sampler.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/docs/sampler-configuration.rst` & `nessai-0.8.1/docs/sampler-configuration.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/2d_gaussian.py` & `nessai-0.8.1/examples/2d_gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/augmented_example.py` & `nessai-0.8.1/examples/augmented_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/bilby_example.py` & `nessai-0.8.1/examples/bilby_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/bilby_unbounded_priors.py` & `nessai-0.8.1/examples/bilby_unbounded_priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/corner_plot_example.py` & `nessai-0.8.1/examples/corner_plot_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/eggbox.py` & `nessai-0.8.1/examples/eggbox.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/gw/basic_gw_example.py` & `nessai-0.8.1/examples/gw/basic_gw_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/gw/calibration_example.py` & `nessai-0.8.1/examples/gw/calibration_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/gw/full_gw_example.py` & `nessai-0.8.1/examples/gw/full_gw_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/half_gaussian.py` & `nessai-0.8.1/examples/half_gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/parallelisation_example.py` & `nessai-0.8.1/examples/parallelisation_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/reparameterisations_example.py` & `nessai-0.8.1/examples/reparameterisations_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/rosenbrock.py` & `nessai-0.8.1/examples/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/examples/unbounded_prior.py` & `nessai-0.8.1/examples/unbounded_prior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/__init__.py` & `nessai-0.8.1/nessai/__init__.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/config.py` & `nessai-0.8.1/nessai/config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/evidence.py` & `nessai-0.8.1/nessai/evidence.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flowmodel/base.py` & `nessai-0.8.1/nessai/flowmodel/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flowmodel/config.py` & `nessai-0.8.1/nessai/flowmodel/config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flowmodel/utils.py` & `nessai-0.8.1/nessai/flowmodel/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flows/base.py` & `nessai-0.8.1/nessai/flows/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flows/distributions.py` & `nessai-0.8.1/nessai/flows/distributions.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flows/maf.py` & `nessai-0.8.1/nessai/flows/maf.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flows/nets.py` & `nessai-0.8.1/nessai/flows/nets.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flows/nsf.py` & `nessai-0.8.1/nessai/flows/nsf.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flows/realnvp.py` & `nessai-0.8.1/nessai/flows/realnvp.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flows/transforms.py` & `nessai-0.8.1/nessai/flows/transforms.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flows/utils.py` & `nessai-0.8.1/nessai/flows/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/flowsampler.py` & `nessai-0.8.1/nessai/flowsampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/gw/proposal.py` & `nessai-0.8.1/nessai/gw/proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/gw/reparameterisations.py` & `nessai-0.8.1/nessai/gw/reparameterisations.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
         -------
         x, x_prime : structured arrays
             Update version of the x and x_prime arrays
         log_j : array_like
             Updated log Jacobian determinant
         """
         x_prime[self.prime_parameters[0]] = (
-            x[self.parameters[0]] - np.sign(np.cos(x["theta_jn"])) * x["psi"]
+            x[self.parameters[0]] + np.sign(np.cos(x["theta_jn"])) * x["psi"]
         )
         return x, x_prime, log_j
 
     def inverse_reparameterise(self, x, x_prime, log_j, **kwargs):
         """
         Apply the reparameterisation to convert from x-space
         to x'-space
@@ -204,15 +204,15 @@
         x, x_prime : structured arrays
             Update version of the x and x_prime arrays
         log_j : array_like
             Updated log Jacobian determinant
         """
         x[self.parameters[0]] = np.mod(
             x_prime[self.prime_parameters[0]]
-            + np.sign(np.cos(x["theta_jn"])) * x["psi"],
+            - np.sign(np.cos(x["theta_jn"])) * x["psi"],
             2 * np.pi,
         )
         return x, x_prime, log_j
 
 
 default_gw = {
     "distance": (
```

### Comparing `nessai-0.8.0b1/nessai/gw/utils.py` & `nessai-0.8.1/nessai/gw/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/livepoint.py` & `nessai-0.8.1/nessai/livepoint.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/model.py` & `nessai-0.8.1/nessai/model.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/plot.py` & `nessai-0.8.1/nessai/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,15 +568,15 @@
     import corner
 
     default_kwargs = dict(
         bins=32,
         smooth=0.9,
         color=config.plotting.base_colour,
         truth_color=config.plotting.highlight_colour,
-        quantiles=[0.16, 0.84],
+        quantiles=[0.16, 0.5, 0.84],
         levels=(1 - np.exp(-0.5), 1 - np.exp(-2), 1 - np.exp(-9 / 2.0)),
         plot_density=True,
         plot_datapoints=True,
         fill_contours=True,
         show_titles=True,
         hist_kwargs=dict(density=True),
     )
```

### Comparing `nessai-0.8.0b1/nessai/posterior.py` & `nessai-0.8.1/nessai/posterior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/priors.py` & `nessai-0.8.1/nessai/priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/proposal/analytic.py` & `nessai-0.8.1/nessai/proposal/analytic.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/proposal/augmented.py` & `nessai-0.8.1/nessai/proposal/augmented.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/proposal/base.py` & `nessai-0.8.1/nessai/proposal/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/proposal/flowproposal.py` & `nessai-0.8.1/nessai/proposal/flowproposal.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,15 +654,16 @@
                     ]
                 }
 
             logger.info(f"Adding {rc.__name__} with config: {default_config}")
             r = rc(prior_bounds=prior_bounds, **default_config)
             self._reparameterisation.add_reparameterisations(r)
 
-        self.add_default_reparameterisations()
+        if self.use_default_reparameterisations:
+            self.add_default_reparameterisations()
 
         other_params = [
             n
             for n in self.model.names
             if n not in self._reparameterisation.parameters
         ]
         if other_params:
```

### Comparing `nessai-0.8.0b1/nessai/proposal/rejection.py` & `nessai-0.8.1/nessai/proposal/rejection.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/proposal/utils.py` & `nessai-0.8.1/nessai/proposal/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/reparameterisations/__init__.py` & `nessai-0.8.1/nessai/reparameterisations/__init__.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/reparameterisations/angle.py` & `nessai-0.8.1/nessai/reparameterisations/angle.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/reparameterisations/base.py` & `nessai-0.8.1/nessai/reparameterisations/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/reparameterisations/combined.py` & `nessai-0.8.1/nessai/reparameterisations/combined.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/reparameterisations/null.py` & `nessai-0.8.1/nessai/reparameterisations/null.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/reparameterisations/rescale.py` & `nessai-0.8.1/nessai/reparameterisations/rescale.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/reparameterisations/utils.py` & `nessai-0.8.1/nessai/reparameterisations/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/samplers/base.py` & `nessai-0.8.1/nessai/samplers/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/samplers/nestedsampler.py` & `nessai-0.8.1/nessai/samplers/nestedsampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/__init__.py` & `nessai-0.8.1/nessai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/bilbyutils.py` & `nessai-0.8.1/nessai/utils/bilbyutils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/distance.py` & `nessai-0.8.1/nessai/utils/distance.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/distributions.py` & `nessai-0.8.1/nessai/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/hist.py` & `nessai-0.8.1/nessai/utils/hist.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/indices.py` & `nessai-0.8.1/nessai/utils/indices.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/io.py` & `nessai-0.8.1/nessai/utils/io.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/logging.py` & `nessai-0.8.1/nessai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/multiprocessing.py` & `nessai-0.8.1/nessai/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/rescaling.py` & `nessai-0.8.1/nessai/utils/rescaling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/sampling.py` & `nessai-0.8.1/nessai/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/sorting.py` & `nessai-0.8.1/nessai/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/stats.py` & `nessai-0.8.1/nessai/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/structures.py` & `nessai-0.8.1/nessai/utils/structures.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/testing.py` & `nessai-0.8.1/nessai/utils/testing.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/threading.py` & `nessai-0.8.1/nessai/utils/threading.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai/utils/torchutils.py` & `nessai-0.8.1/nessai/utils/torchutils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/nessai.egg-info/PKG-INFO` & `nessai-0.8.1/nessai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai
-Version: 0.8.0b1
+Version: 0.8.1
 Summary: Nessai: Nested Sampling with Artificial Intelligence
 Home-page: https://github.com/mj-will/nessai
 Author: Michael J. Williams
 Author-email: m.williams.4@research.gla.ac.uk
 Project-URL: Documentation, https://nessai.readthedocs.io/
 Keywords: nested sampling,normalising flows,machine learning
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `nessai-0.8.0b1/nessai.egg-info/SOURCES.txt` & `nessai-0.8.1/nessai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/pyproject.toml` & `nessai-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/setup.cfg` & `nessai-0.8.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 packages = find:
 python requires = >=3.7
 install_requires = 
 	numpy>=1.9
 	pandas
 	matplotlib>=2.0
 	seaborn
-	scipy>=0.16,<1.10
+	scipy>=0.16
 	torch>=1.11.0
 	tqdm
 	glasflow
 	h5py>=3.0
 
 [options.extras_require]
 test =
```

### Comparing `nessai-0.8.0b1/tests/conftest.py` & `nessai-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_bilby_compatibility.py` & `nessai-0.8.1/tests/test_bilby_compatibility.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_config.py` & `nessai-0.8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_deprecation_warnings.py` & `nessai-0.8.1/tests/test_deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_evidence.py` & `nessai-0.8.1/tests/test_evidence.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flowmodel/test_flowmodel_base.py` & `nessai-0.8.1/tests/test_flowmodel/test_flowmodel_base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flowmodel/test_flowmodel_utils.py` & `nessai-0.8.1/tests/test_flowmodel/test_flowmodel_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flows/test_base_flow.py` & `nessai-0.8.1/tests/test_flows/test_base_flow.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flows/test_distributions.py` & `nessai-0.8.1/tests/test_flows/test_distributions.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flows/test_flow_utils.py` & `nessai-0.8.1/tests/test_flows/test_flow_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flows/test_included_flows.py` & `nessai-0.8.1/tests/test_flows/test_included_flows.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flows/test_nets.py` & `nessai-0.8.1/tests/test_flows/test_nets.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flows/test_specific_flows.py` & `nessai-0.8.1/tests/test_flows/test_specific_flows.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_flowsampler.py` & `nessai-0.8.1/tests/test_flowsampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_gw/conftest.py` & `nessai-0.8.1/tests/test_gw/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_gw/test_distance_converters.py` & `nessai-0.8.1/tests/test_gw/test_distance_converters.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_gw/test_gw_proposal.py` & `nessai-0.8.1/tests/test_gw/test_gw_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_gw/test_gw_reparameterisations.py` & `nessai-0.8.1/tests/test_gw/test_gw_reparameterisations.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         x_out,
         x_prime_out,
         log_j_out,
     ) = DeltaPhaseReparameterisation.reparameterise(
         delta_phase_reparam, x, x_prime, log_j
     )
     assert x_out == x
-    assert x_prime_out["delta_phase"] == 0.5
+    assert x_prime_out["delta_phase"] == 1.5
     assert log_j_out == 0
 
 
 def test_delta_phase_inverse_reparameterise(delta_phase_reparam):
     """Assert the correct value is returned"""
     delta_phase_reparam.parameters = ["phase"]
     delta_phase_reparam.prime_parameters = ["delta_phase"]
@@ -172,15 +172,15 @@
         x_out,
         x_prime_out,
         log_j_out,
     ) = DeltaPhaseReparameterisation.inverse_reparameterise(
         delta_phase_reparam, x, x_prime, log_j
     )
     assert x_prime_out == x_prime
-    assert x["phase"] == 1.0
+    assert x["phase"] == 0.0
     assert log_j_out == 0
 
 
 @pytest.mark.integration_test
 def test_delta_phase_inverse_invertible():
     """Assert the reparameterisation is invertible"""
     n = 10
@@ -199,13 +199,19 @@
     x_prime = empty_structured_array(
         n, names=["delta_phase", "theta_jn", "psi"]
     )
     x_prime["psi"] = x["psi"]
     x_prime["theta_jn"] = x["theta_jn"]
     log_j = np.zeros(n)
     x_f, x_prime_f, log_j_f = reparam.reparameterise(x, x_prime, log_j)
+
+    x_in = x_f.copy()
+    x_in["phase"] = np.nan
+
     assert_structured_arrays_equal(x_f, x)
     np.testing.assert_array_equal(log_j_f, log_j)
-    x_i, x_prime_i, log_j_i = reparam.reparameterise(x_f, x_prime_f, log_j_f)
+    x_i, x_prime_i, log_j_i = reparam.inverse_reparameterise(
+        x_in, x_prime_f.copy(), log_j_f.copy()
+    )
     assert_structured_arrays_equal(x_prime_i, x_prime_f)
-    assert_structured_arrays_equal(x_i, x)
+    assert_structured_arrays_equal(x_i, x, rtol=1e-15)
     np.testing.assert_array_equal(log_j_i, log_j_f)
```

### Comparing `nessai-0.8.0b1/tests/test_gw/test_reparameterisation_integration.py` & `nessai-0.8.1/tests/test_gw/test_reparameterisation_integration.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_livepoint.py` & `nessai-0.8.1/tests/test_livepoint.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_model.py` & `nessai-0.8.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_plot.py` & `nessai-0.8.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_posterior.py` & `nessai-0.8.1/tests/test_posterior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_priors.py` & `nessai-0.8.1/tests/test_priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_analytic.py` & `nessai-0.8.1/tests/test_proposal/test_analytic.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_augmented.py` & `nessai-0.8.1/tests/test_proposal/test_augmented.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_base_proposal.py` & `nessai-0.8.1/tests/test_proposal/test_base_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_population.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_population.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py` & `nessai-0.8.1/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,21 @@
 def test_get_reparamaterisation(mocked_fn, proposal):
     """Make sure the underlying function is called"""
     FlowProposal.get_reparameterisation(proposal, "angle")
     assert mocked_fn.called_once_with("angle")
 
 
 @pytest.mark.parametrize("reverse_order", [False, True])
+@pytest.mark.parametrize("use_default_reparameterisations", [False, True])
 def test_configure_reparameterisations_dict(
-    proposal, dummy_cmb_rc, dummy_rc, reverse_order
+    proposal,
+    dummy_cmb_rc,
+    dummy_rc,
+    reverse_order,
+    use_default_reparameterisations,
 ):
     """Test configuration for reparameterisations dictionary.
 
     Also tests to make sure boundary inversion is set and if the
     `reverse_reparameterisation` is correctly set.
     """
     dummy_rc.return_value = "r"
@@ -69,25 +74,31 @@
     proposal.get_reparameterisation = MagicMock(
         return_value=(dummy_rc, {"boundary_inversion": True})
     )
     proposal.model = MagicMock()
     proposal.model.bounds = {"x": [-1, 1], "y": [-1, 1]}
     proposal.model.names = ["x"]
     proposal.reverse_reparameterisations = reverse_order
+    proposal.use_default_reparameterisations = use_default_reparameterisations
 
     with patch(
         "nessai.proposal.flowproposal.CombinedReparameterisation",
         return_value=dummy_cmb_rc,
     ) as mocked_class:
         FlowProposal.configure_reparameterisations(
             proposal, {"x": {"reparameterisation": "default"}}
         )
 
     proposal.get_reparameterisation.assert_called_once_with("default")
-    proposal.add_default_reparameterisations.assert_called_once()
+
+    if use_default_reparameterisations:
+        proposal.add_default_reparameterisations.assert_called_once()
+    else:
+        proposal.add_default_reparameterisations.assert_not_called()
+
     dummy_rc.assert_called_once_with(
         prior_bounds={"x": [-1, 1]}, parameters="x", boundary_inversion=True
     )
     mocked_class.assert_called_once_with(reverse_order=reverse_order)
     # fmt: off
     proposal._reparameterisation.add_reparameterisations \
         .assert_called_once_with("r")
@@ -129,15 +140,15 @@
     ) as mocked_class:
         FlowProposal.configure_reparameterisations(
             proposal,
             {"x": {"reparameterisation": "default", "parameters": ["y"]}},
         )
 
     proposal.get_reparameterisation.assert_called_once_with("default")
-    proposal.add_default_reparameterisations.assert_called_once()
+    proposal.add_default_reparameterisations.assert_not_called()
     dummy_rc.assert_called_once_with(
         prior_bounds={"x": [-1, 1], "y": [-1, 1]},
         parameters=["y", "x"],
     )
     mocked_class.assert_called_once()
     # fmt: off
     proposal._reparameterisation.add_reparameterisations \
@@ -209,15 +220,15 @@
     proposal.add_default_reparameterisations = MagicMock()
     proposal.get_reparameterisation = get_reparameterisation
     proposal.model.bounds = {"x": [-1, 1], "y": [-1, 1]}
     proposal.model.names = ["x", "y"]
     proposal.fallback_reparameterisation = None
     FlowProposal.configure_reparameterisations(proposal, {"x": "default"})
 
-    proposal.add_default_reparameterisations.assert_called_once()
+    proposal.add_default_reparameterisations.assert_not_called()
     assert proposal.rescaled_names == ["x_prime", "y"]
     assert proposal.rescale_parameters == ["x"]
     assert proposal._reparameterisation.parameters == ["x", "y"]
     assert proposal._reparameterisation.prime_parameters == ["x_prime", "y"]
     assert mocked_class.called_once
 
 
@@ -229,15 +240,15 @@
     proposal.model.bounds = {"x": [-1, 1], "y": [-1, 1]}
     proposal.model.names = ["x", "y"]
     proposal.fallback_reparameterisation = None
     FlowProposal.configure_reparameterisations(
         proposal, {"default": {"parameters": ["x"]}}
     )
 
-    proposal.add_default_reparameterisations.assert_called_once()
+    proposal.add_default_reparameterisations.assert_not_called()
     assert proposal.rescaled_names == ["x_prime", "y"]
     assert proposal.rescale_parameters == ["x"]
     assert proposal._reparameterisation.parameters == ["x", "y"]
     assert proposal._reparameterisation.prime_parameters == ["x_prime", "y"]
     assert mocked_class.called_once
 
 
@@ -246,15 +257,15 @@
     """Test configuration when input is None"""
     proposal.add_default_reparameterisations = MagicMock()
     proposal.get_reparameterisation = get_reparameterisation
     proposal.model.bounds = {"x": [-1, 1], "y": [-1, 1]}
     proposal.model.names = ["x", "y"]
     proposal.fallback_reparameterisation = None
     FlowProposal.configure_reparameterisations(proposal, None)
-    proposal.add_default_reparameterisations.assert_called_once()
+    proposal.add_default_reparameterisations.assert_not_called()
     assert proposal.rescaled_names == ["x", "y"]
 
     assert proposal.rescale_parameters == []
     assert proposal._reparameterisation.parameters == ["x", "y"]
     assert proposal._reparameterisation.prime_parameters == ["x", "y"]
     assert all(
         [
@@ -270,15 +281,15 @@
     """Test configuration when input is None"""
     proposal.add_default_reparameterisations = MagicMock()
     proposal.get_reparameterisation = get_reparameterisation
     proposal.model.bounds = {"x": [-1, 1], "y": [-1, 1]}
     proposal.model.names = ["x", "y"]
     proposal.fallback_reparameterisation = "default"
     FlowProposal.configure_reparameterisations(proposal, None)
-    proposal.add_default_reparameterisations.assert_called_once()
+    proposal.add_default_reparameterisations.assert_not_called()
     assert proposal.rescaled_names == ["x_prime", "y_prime"]
 
     assert proposal.rescale_parameters == ["x", "y"]
     assert proposal._reparameterisation.parameters == ["x", "y"]
     assert proposal._reparameterisation.prime_parameters == [
         "x_prime",
         "y_prime",
```

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_rejection.py` & `nessai-0.8.1/tests/test_proposal/test_rejection.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_proposal/test_utils.py` & `nessai-0.8.1/tests/test_proposal/test_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/conftest.py` & `nessai-0.8.1/tests/test_reparameterisations/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_angle.py` & `nessai-0.8.1/tests/test_reparameterisations/test_angle.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_angle_pair.py` & `nessai-0.8.1/tests/test_reparameterisations/test_angle_pair.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_base_reparameterisation.py` & `nessai-0.8.1/tests/test_reparameterisations/test_base_reparameterisation.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_combined.py` & `nessai-0.8.1/tests/test_reparameterisations/test_combined.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_get_reparameterisation.py` & `nessai-0.8.1/tests/test_reparameterisations/test_get_reparameterisation.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_null.py` & `nessai-0.8.1/tests/test_reparameterisations/test_null.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_rescale_to_bounds.py` & `nessai-0.8.1/tests/test_reparameterisations/test_rescale_to_bounds.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_scale_and_shift.py` & `nessai-0.8.1/tests/test_reparameterisations/test_scale_and_shift.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_reparameterisations/test_to_cartesian.py` & `nessai-0.8.1/tests/test_reparameterisations/test_to_cartesian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_base_sampler.py` & `nessai-0.8.1/tests/test_samplers/test_base_sampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_core_sampling.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_core_sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_flow_proposal.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_flow_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_general_config.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_general_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_live_points.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_live_points.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_manage_state.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_manage_state.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_ns_plotting.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_ns_plotting.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_properties.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_properties.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_proposal_config.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_proposal_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_resume.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_resume.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_samplers/test_nested_sampler/test_yield_sample.py` & `nessai-0.8.1/tests/test_samplers/test_nested_sampler/test_yield_sample.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_sampling.py` & `nessai-0.8.1/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_bilbyutils.py` & `nessai-0.8.1/tests/test_utils/test_bilbyutils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_distance_utils.py` & `nessai-0.8.1/tests/test_utils/test_distance_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_distribution_utils.py` & `nessai-0.8.1/tests/test_utils/test_distribution_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_hist_utils.py` & `nessai-0.8.1/tests/test_utils/test_hist_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_indices_utils.py` & `nessai-0.8.1/tests/test_utils/test_indices_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_io_utils.py` & `nessai-0.8.1/tests/test_utils/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_logging_utils.py` & `nessai-0.8.1/tests/test_utils/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_multiprocessing_utils.py` & `nessai-0.8.1/tests/test_utils/test_multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_rescaling_utils.py` & `nessai-0.8.1/tests/test_utils/test_rescaling_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_sampling_utils.py` & `nessai-0.8.1/tests/test_utils/test_sampling_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_sorting_utils.py` & `nessai-0.8.1/tests/test_utils/test_sorting_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_stats_utils.py` & `nessai-0.8.1/tests/test_utils/test_stats_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_structures_utils.py` & `nessai-0.8.1/tests/test_utils/test_structures_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_testing_utils.py` & `nessai-0.8.1/tests/test_utils/test_testing_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_threading_utils.py` & `nessai-0.8.1/tests/test_utils/test_threading_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_utils/test_torchtutils_utils.py` & `nessai-0.8.1/tests/test_utils/test_torchtutils_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.8.0b1/tests/test_version.py` & `nessai-0.8.1/tests/test_version.py`

 * *Files identical despite different names*

