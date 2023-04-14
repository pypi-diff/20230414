# Comparing `tmp/gpytorch-1.9.0.tar.gz` & `tmp/gpytorch-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpytorch-1.9.0.tar", last modified: Tue Aug 30 14:17:19 2022, max compression
+gzip compressed data, was "gpytorch-1.9.1.tar", last modified: Wed Jan  4 22:55:09 2023, max compression
```

## Comparing `gpytorch-1.9.0.tar` & `gpytorch-1.9.1.tar`

### file list

```diff
@@ -1,467 +1,470 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.111927 gpytorch-1.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.063926 gpytorch-1.9.0/.conda/
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.059925 gpytorch-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.063926 gpytorch-1.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.github/ISSUE_TEMPLATE/---bug-report.md
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.github/ISSUE_TEMPLATE/---documentation-examples.md
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.github/ISSUE_TEMPLATE/---feature-request.md
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.github/ISSUE_TEMPLATE/---refactor.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.063926 gpytorch-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.github/workflows/run_test_suite.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-08-30 14:17:04.000000 gpytorch-1.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-08-30 14:17:04.000000 gpytorch-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6847 2022-08-30 14:17:19.115927 gpytorch-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5361 2022-08-30 14:17:04.000000 gpytorch-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.063926 gpytorch-1.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.067926 gpytorch-1.9.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.067926 gpytorch-1.9.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/beta_features.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6835 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/constraints.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/distributions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/functions.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3357 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/kernels.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/likelihoods.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/marginal_log_likelihoods.rst
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/means.rst
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1669 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/module.rst
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/optim.rst
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/priors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/settings.rst
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6850 2022-08-30 14:17:04.000000 gpytorch-1.9.0/docs/source/variational.rst
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-30 14:17:04.000000 gpytorch-1.9.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.067926 gpytorch-1.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.067926 gpytorch-1.9.0/examples/00_Basic_Usage/
--rw-r--r--   0 runner    (1001) docker     (121)    17334 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/00_Basic_Usage/Hyperparameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    69079 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/00_Basic_Usage/Implementing_a_custom_Kernel.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    55633 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/00_Basic_Usage/Metrics.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/00_Basic_Usage/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12161 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/00_Basic_Usage/Saving_and_Loading_Models.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/00_Basic_Usage/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.071926 gpytorch-1.9.0/examples/01_Exact_GPs/
--rw-r--r--   0 runner    (1001) docker     (121)    73485 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/01_Exact_GPs/GP_Regression_DistributionalKernel.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    27158 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/01_Exact_GPs/GP_Regression_Fully_Bayesian.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   169145 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/01_Exact_GPs/GP_Regression_on_Classification_Labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/01_Exact_GPs/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/01_Exact_GPs/Simple_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   328148 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/01_Exact_GPs/Spectral_Delta_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    24340 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/01_Exact_GPs/Spectral_Mixture_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/01_Exact_GPs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.071926 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/
--rw-r--r--   0 runner    (1001) docker     (121)    12304 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Exact_GP_Posterior_Sampling_with_CIQ.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    41944 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Grid_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    63975 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/KISSGP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9537 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/KeOps_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4405 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9659 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/SGPR_Regression_CUDA.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    11843 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Scalable_Kernel_Interpolation_for_Products_CUDA.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    31783 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Simple_GP_Regression_CUDA.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    19699 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Simple_GP_Regression_With_LOVE_Fast_Variances_and_Sampling.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    14398 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Simple_MultiGPU_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4405 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.071926 gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/
--rw-r--r--   0 runner    (1001) docker     (121)    43803 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/Batch_Independent_Multioutput_GP.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    41271 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/Hadamard_Multitask_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    43250 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/ModelList_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    40526 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/Multitask_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.071926 gpytorch-1.9.0/examples/045_GPLVM/
--rw-r--r--   0 runner    (1001) docker     (121)    65872 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/045_GPLVM/Gaussian_Process_Latent_Variable_Models_with_Stochastic_Variational_Inference.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/045_GPLVM/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/045_GPLVM/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.075926 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/
--rw-r--r--   0 runner    (1001) docker     (121)    64175 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/Approximate_GP_Objective_Functions.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    36880 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/GP_Regression_with_Uncertain_Inputs.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    17417 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/Modifying_the_variational_strategy_and_distribution.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    14534 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/Natural_Gradient_Descent.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    21316 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/Non_Gaussian_Likelihoods.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    71492 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/PolyaGamma_Binary_Classification.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10580 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/SVGP_CIQ.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    86959 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/SVGP_Multitask_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    13727 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/SVGP_Regression_CUDA.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    31427 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/VNNGP.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3489 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.075926 gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/
--rw-r--r--   0 runner    (1001) docker     (121)    76380 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/DGP_Multitask_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    18846 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/Deep_Gaussian_Processes.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    19995 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/Deep_Sigma_Point_Processes.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.075926 gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    15805 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/Deep_Kernel_Learning_DenseNet_CIFAR_Tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    11188 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/KISSGP_Deep_Kernel_Regression_CUDA.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/densenet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.079926 gpytorch-1.9.0/examples/07_Pyro_Integration/
--rw-r--r--   0 runner    (1001) docker     (121)   282137 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/07_Pyro_Integration/Clustered_Multitask_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    81543 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/07_Pyro_Integration/Cox_Process_Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    33420 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/07_Pyro_Integration/Pyro_GPyTorch_High_Level.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    82188 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/07_Pyro_Integration/Pyro_GPyTorch_Low_Level.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/07_Pyro_Integration/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/07_Pyro_Integration/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.079926 gpytorch-1.9.0/examples/08_Advanced_Usage/
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)   144728 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/SVGP_Model_Updating.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    74956 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/Simple_Batch_Mode_GP_Regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   102267 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/Simple_GP_Regression_Derivative_Information_1d.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    77503 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/Simple_GP_Regression_Derivative_Information_2d.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6719 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/TorchScript_Exact_Models.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     8940 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/TorchScript_Variational_Models.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2924 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)  1040259 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/08_Advanced_Usage/svgp_elevators.pt
--rw-r--r--   0 runner    (1001) docker     (121)    42604 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-08-30 14:17:04.000000 gpytorch-1.9.0/examples/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.079926 gpytorch-1.9.0/gpytorch/
--rw-r--r--   0 runner    (1001) docker     (121)    12380 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.083926 gpytorch-1.9.0/gpytorch/constraints/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8483 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.083926 gpytorch-1.9.0/gpytorch/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/distributions/delta.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    13906 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/distributions/multitask_multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)    14673 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/distributions/multivariate_normal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.083926 gpytorch-1.9.0/gpytorch/functions/
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/functions/_log_normal_cdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/functions/matern_covariance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/functions/rbf_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.087926 gpytorch-1.9.0/gpytorch/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)     2235 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2359 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/additive_structure_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7380 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/arc_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4000 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/cosine_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7133 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/cylindrical_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/distributional_input_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/gaussian_symmetrized_kl_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     9076 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/grid_interpolation_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7431 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/grid_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3659 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/index_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5437 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/inducing_point_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.087926 gpytorch-1.9.0/gpytorch/kernels/keops/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/keops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/keops/keops_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4388 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/keops/matern_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2441 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/keops/rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    21641 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/lcm_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/linear_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4926 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/matern_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/multi_device_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2555 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/multitask_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4961 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/newton_girard_additive_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6197 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/periodic_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5174 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/piecewise_polynomial_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/polynomial_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/polynomial_kernel_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)     3267 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/product_structure_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3848 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5654 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/rbf_kernel_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)     5960 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/rff_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3751 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/rq_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/scale_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5147 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/spectral_delta_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    16478 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/kernels/spectral_mixture_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.087926 gpytorch-1.9.0/gpytorch/lazy/
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17166 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/lazy/lazy_evaluated_kernel_tensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/lazy/lazy_tensor.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/lazy/non_lazy_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.087926 gpytorch-1.9.0/gpytorch/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2138 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/bernoulli_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/beta_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)    15402 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/gaussian_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/laplace_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)    16079 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/likelihood_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    12771 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/multitask_gaussian_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     7453 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/noise_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3512 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/softmax_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/likelihoods/student_t_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.087926 gpytorch-1.9.0/gpytorch/means/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/means/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4520 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/means/constant_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/means/constant_mean_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/means/linear_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/means/mean.py
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/means/multitask_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/means/zero_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.087926 gpytorch-1.9.0/gpytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2447 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.091926 gpytorch-1.9.0/gpytorch/mlls/
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3383 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/_approximate_mll.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/added_loss_term.py
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/deep_approximate_mll.py
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/deep_predictive_log_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/exact_marginal_log_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     4506 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/gamma_robust_variational_elbo.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/inducing_point_kernel_added_loss_term.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/kl_gaussian_added_loss_term.py
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/leave_one_out_pseudo_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/marginal_log_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/noise_model_added_loss_term.py
--rw-r--r--   0 runner    (1001) docker     (121)     3892 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/predictive_log_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/sum_marginal_log_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     3900 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/mlls/variational_elbo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.091926 gpytorch-1.9.0/gpytorch/models/
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5284 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/approximate_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.091926 gpytorch-1.9.0/gpytorch/models/deep_gps/
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/deep_gps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6472 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/deep_gps/deep_gp.py
--rw-r--r--   0 runner    (1001) docker     (121)     5073 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/deep_gps/dspp.py
--rw-r--r--   0 runner    (1001) docker     (121)    16129 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/exact_gp.py
--rw-r--r--   0 runner    (1001) docker     (121)    38047 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/exact_prediction_strategies.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/gp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.091926 gpytorch-1.9.0/gpytorch/models/gplvm/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/gplvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/gplvm/bayesian_gplvm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3476 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/gplvm/latent_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3306 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/model_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.091926 gpytorch-1.9.0/gpytorch/models/pyro/
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/pyro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/pyro/_pyro_mixin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4639 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/models/pyro/pyro_gp.py
--rw-r--r--   0 runner    (1001) docker     (121)    25687 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/module.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.091926 gpytorch-1.9.0/gpytorch/optim/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/optim/ngd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.095926 gpytorch-1.9.0/gpytorch/priors/
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/priors/horseshoe_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     6819 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/priors/lkj_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)      892 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/priors/prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     3265 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/priors/smoothed_box_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/priors/torch_priors.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/priors/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/priors/wishart_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)    11628 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.095926 gpytorch-1.9.0/gpytorch/test/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6762 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/test/base_kernel_test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     4346 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/test/base_likelihood_test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     1437 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/test/base_mean_test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     2623 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/test/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     6405 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/test/model_test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16499 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/test/variational_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.095926 gpytorch-1.9.0/gpytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/broadcasting.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/cholesky.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/getitem.py
--rw-r--r--   0 runner    (1001) docker     (121)     6362 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     9276 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/lanczos.py
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/memoize.py
--rw-r--r--   0 runner    (1001) docker     (121)     9351 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/permutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3290 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/quadrature.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/sparse.py
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/toeplitz.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.099927 gpytorch-1.9.0/gpytorch/variational/
--rw-r--r--   0 runner    (1001) docker     (121)     2146 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/_variational_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    15175 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/additive_grid_interpolation_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)    11774 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/batch_decoupled_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/cholesky_variational_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    14696 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/ciq_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/delta_variational_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     4850 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/grid_interpolation_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5091 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/independent_multitask_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)    11046 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/lmc_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/mean_field_variational_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     6276 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/natural_variational_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)    17867 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/nearest_neighbor_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4657 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/orthogonally_decoupled_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5378 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/tril_natural_variational_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     9207 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/unwhitened_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)    11491 2022-08-30 14:17:04.000000 gpytorch-1.9.0/gpytorch/variational/variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-30 14:17:18.000000 gpytorch-1.9.0/gpytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.083926 gpytorch-1.9.0/gpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6847 2022-08-30 14:17:18.000000 gpytorch-1.9.0/gpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    16700 2022-08-30 14:17:18.000000 gpytorch-1.9.0/gpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-30 14:17:18.000000 gpytorch-1.9.0/gpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-08-30 14:17:18.000000 gpytorch-1.9.0/gpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-30 14:17:18.000000 gpytorch-1.9.0/gpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-08-30 14:17:04.000000 gpytorch-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-30 14:17:04.000000 gpytorch-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-08-30 14:17:19.115927 gpytorch-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-08-30 14:17:04.000000 gpytorch-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.099927 gpytorch-1.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.099927 gpytorch-1.9.0/test/constraints/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7488 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/constraints/test_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.099927 gpytorch-1.9.0/test/distributions/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/distributions/test_delta.py
--rw-r--r--   0 runner    (1001) docker     (121)    16246 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/distributions/test_multitask_multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (121)    17954 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/distributions/test_multivariate_normal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.103927 gpytorch-1.9.0/test/examples/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4688 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/old_variational_strategy_model.pth
--rw-r--r--   0 runner    (1001) docker     (121)     3302 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_batch_decoupled_ppgpr_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     9805 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_batch_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     7688 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_batch_multitask_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     7182 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_batch_svgp_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3711 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_decoupled_svgp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     5001 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_dspp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     7308 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_fixed_noise_fanatasy_updates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4497 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_grid_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_hadamard_multitask_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     4000 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_independent_multitask_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_additive_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     3589 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_additive_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     5348 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_dkl_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3160 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_gp_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     6402 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_kronecker_product_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_kronecker_product_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3480 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_multiplicative_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     4522 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_variational_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     6800 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kissgp_white_noise_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kronecker_multitask_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_kronecker_multitask_ski_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3972 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_lcm_kernel_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     7956 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_lmc_svgp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3108 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_model_list_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)    17894 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_pyro_integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     3356 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_rff_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_sgpr_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     2766 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_simple_gp_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)    21070 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_simple_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_spectral_mixture_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3517 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_svgp_gp_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     6067 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_svgp_gp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_unwhitened_svgp_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     6731 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/examples/test_white_noise_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.103927 gpytorch-1.9.0/test/functions/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/functions/test_log_normal_cdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/functions/test_matern_covariance.py
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/functions/test_rbf_covariance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.107927 gpytorch-1.9.0/test/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.107927 gpytorch-1.9.0/test/kernels/keops/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/keops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2569 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/keops/test_matern_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/keops/test_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    15284 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_additive_and_product_kernels.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_arc_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4350 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_cosine_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_cylindrical_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_gaussian_symmetrized_kl_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_grid_interpolation_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_grid_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_index_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_inducing_point_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3660 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_linear_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7304 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_matern_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7048 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_newton_girard_additive_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3982 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_periodic_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3636 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_piecewise_polynomial_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4717 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_polynomial_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_polynomial_kernel_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)     8936 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_rbf_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2716 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_rbf_kernel_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)     6245 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_rff_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     9482 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_rq_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_scale_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_spectral_delta_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5939 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/kernels/test_spectral_mixture_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.107927 gpytorch-1.9.0/test/lazy/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8715 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/lazy/test_lazy_evaluated_kernel_tensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5583 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/lazy/test_lazy_tensor_deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.107927 gpytorch-1.9.0/test/likelihoods/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/test_bernoulli_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/test_beta_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     8231 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/test_gaussian_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     3353 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/test_general_multitask_gaussian_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     1831 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/test_laplace_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     2497 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/test_multitask_gaussian_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/test_softmax_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/likelihoods/test_student_t_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.107927 gpytorch-1.9.0/test/means/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/means/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/means/test_constant_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/means/test_constant_mean_grad.py
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/means/test_linear_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)     1941 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/means/test_multitask_mean.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/means/test_zero_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.107927 gpytorch-1.9.0/test/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8041 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.111927 gpytorch-1.9.0/test/mlls/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/mlls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/mlls/test_exact_marginal_log_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (121)     3017 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/mlls/test_leave_one_out_pseudo_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.111927 gpytorch-1.9.0/test/models/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11152 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/models/test_exact_gp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/models/test_model_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/models/test_variational_gp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.111927 gpytorch-1.9.0/test/optim/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1444 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/optim/test_ngd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.111927 gpytorch-1.9.0/test/priors/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4194 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/priors/test_gamma_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/priors/test_half_cauchy_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     2665 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/priors/test_horseshoe_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)    10980 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/priors/test_lkj_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     5023 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/priors/test_multivariate_normal_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/priors/test_normal_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     4348 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/priors/test_smoothed_box_prior.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/test_module.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.111927 gpytorch-1.9.0/test/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1027 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/utils/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     7534 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/utils/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5509 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/utils/test_nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/utils/test_quadrature.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:19.111927 gpytorch-1.9.0/test/variational/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7720 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_batch_decoupled_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_ciq_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_grid_interpolation_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7223 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_independent_multitask_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     8866 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_lmc_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6386 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_natural_variational_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_nearest_neighbor_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2516 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_orthogonally_decoupled_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3269 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_unwhitened_variational_strategy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3726 2022-08-30 14:17:04.000000 gpytorch-1.9.0/test/variational/test_variational_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.901913 gpytorch-1.9.1/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.897913 gpytorch-1.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.901913 gpytorch-1.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.github/ISSUE_TEMPLATE/---bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.github/ISSUE_TEMPLATE/---documentation-examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.github/ISSUE_TEMPLATE/---feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.github/ISSUE_TEMPLATE/---refactor.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.901913 gpytorch-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.github/workflows/run_test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-04 22:55:01.000000 gpytorch-1.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-04 22:55:01.000000 gpytorch-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-01-04 22:55:09.945915 gpytorch-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-01-04 22:55:01.000000 gpytorch-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.901913 gpytorch-1.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.905913 gpytorch-1.9.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.905913 gpytorch-1.9.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/beta_features.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/constraints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/distributions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/kernels.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/likelihoods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/marginal_log_likelihoods.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/means.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/optim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/priors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-01-04 22:55:01.000000 gpytorch-1.9.1/docs/source/variational.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-04 22:55:01.000000 gpytorch-1.9.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.905913 gpytorch-1.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.905913 gpytorch-1.9.1/examples/00_Basic_Usage/
+-rw-r--r--   0 runner    (1001) docker     (123)    17334 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/00_Basic_Usage/Hyperparameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    69079 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/00_Basic_Usage/Implementing_a_custom_Kernel.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    55633 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/00_Basic_Usage/Metrics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/00_Basic_Usage/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/00_Basic_Usage/Saving_and_Loading_Models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/00_Basic_Usage/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.905913 gpytorch-1.9.1/examples/01_Exact_GPs/
+-rw-r--r--   0 runner    (1001) docker     (123)    93992 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/01_Exact_GPs/GP_Regression_DistributionalKernel.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27158 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/01_Exact_GPs/GP_Regression_Fully_Bayesian.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   169145 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/01_Exact_GPs/GP_Regression_on_Classification_Labels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/01_Exact_GPs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    36113 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/01_Exact_GPs/Simple_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   328148 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/01_Exact_GPs/Spectral_Delta_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/01_Exact_GPs/Spectral_Mixture_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/01_Exact_GPs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.909913 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Exact_GP_Posterior_Sampling_with_CIQ.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Grid_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    63975 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/KISSGP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/KeOps_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/SGPR_Regression_CUDA.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Scalable_Kernel_Interpolation_for_Products_CUDA.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31783 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Simple_GP_Regression_CUDA.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Simple_GP_Regression_With_LOVE_Fast_Variances_and_Sampling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14398 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Simple_MultiGPU_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.909913 gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/
+-rw-r--r--   0 runner    (1001) docker     (123)    43803 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/Batch_Independent_Multioutput_GP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    41271 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/Hadamard_Multitask_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    43250 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/ModelList_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    40977 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/Multitask_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.909913 gpytorch-1.9.1/examples/045_GPLVM/
+-rw-r--r--   0 runner    (1001) docker     (123)    65872 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/045_GPLVM/Gaussian_Process_Latent_Variable_Models_with_Stochastic_Variational_Inference.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/045_GPLVM/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/045_GPLVM/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.909913 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/
+-rw-r--r--   0 runner    (1001) docker     (123)    64175 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/Approximate_GP_Objective_Functions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    36880 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/GP_Regression_with_Uncertain_Inputs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17417 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/Modifying_the_variational_strategy_and_distribution.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/Natural_Gradient_Descent.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21316 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/Non_Gaussian_Likelihoods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    71492 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/PolyaGamma_Binary_Classification.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/SVGP_CIQ.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    86959 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/SVGP_Multitask_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/SVGP_Regression_CUDA.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31427 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/VNNGP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.913913 gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/
+-rw-r--r--   0 runner    (1001) docker     (123)    76380 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/DGP_Multitask_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18846 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/Deep_Gaussian_Processes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19995 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/Deep_Sigma_Point_Processes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.913913 gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/Deep_Kernel_Learning_DenseNet_CIFAR_Tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/KISSGP_Deep_Kernel_Regression_CUDA.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.913913 gpytorch-1.9.1/examples/07_Pyro_Integration/
+-rw-r--r--   0 runner    (1001) docker     (123)   282137 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/07_Pyro_Integration/Clustered_Multitask_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    81543 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/07_Pyro_Integration/Cox_Process_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    33420 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/07_Pyro_Integration/Pyro_GPyTorch_High_Level.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    82188 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/07_Pyro_Integration/Pyro_GPyTorch_Low_Level.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/07_Pyro_Integration/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/07_Pyro_Integration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.913913 gpytorch-1.9.1/examples/08_Advanced_Usage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   144728 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/SVGP_Model_Updating.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    74956 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/Simple_Batch_Mode_GP_Regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   102267 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/Simple_GP_Regression_Derivative_Information_1d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    77503 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/Simple_GP_Regression_Derivative_Information_2d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/TorchScript_Exact_Models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/TorchScript_Variational_Models.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  1040259 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/08_Advanced_Usage/svgp_elevators.pt
+-rw-r--r--   0 runner    (1001) docker     (123)    42604 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-01-04 22:55:01.000000 gpytorch-1.9.1/examples/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.917913 gpytorch-1.9.1/gpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.917913 gpytorch-1.9.1/gpytorch/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.917913 gpytorch-1.9.1/gpytorch/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/distributions/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14188 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/distributions/multitask_multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18714 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/distributions/multivariate_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.917913 gpytorch-1.9.1/gpytorch/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/functions/_log_normal_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/functions/matern_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/functions/rbf_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.921913 gpytorch-1.9.1/gpytorch/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/additive_structure_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/arc_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/cosine_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/cylindrical_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/distributional_input_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/gaussian_symmetrized_kl_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/grid_interpolation_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/grid_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/index_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/inducing_point_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.921913 gpytorch-1.9.1/gpytorch/kernels/keops/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/keops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/keops/keops_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/keops/matern_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/keops/rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28648 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/lcm_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/linear_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/matern_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/multi_device_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/multitask_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/newton_girard_additive_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/periodic_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/piecewise_polynomial_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/polynomial_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/polynomial_kernel_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/product_structure_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/rbf_kernel_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/rff_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/rq_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/scale_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/spectral_delta_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16478 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/kernels/spectral_mixture_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.921913 gpytorch-1.9.1/gpytorch/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/lazy/lazy_evaluated_kernel_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/lazy/lazy_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/lazy/non_lazy_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.925914 gpytorch-1.9.1/gpytorch/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/bernoulli_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/beta_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15402 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/gaussian_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/laplace_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16079 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/likelihood_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12981 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/multitask_gaussian_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/noise_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/softmax_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/likelihoods/student_t_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.925914 gpytorch-1.9.1/gpytorch/means/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/means/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/means/constant_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/means/constant_mean_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/means/linear_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/means/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/means/multitask_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/means/zero_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.925914 gpytorch-1.9.1/gpytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.925914 gpytorch-1.9.1/gpytorch/mlls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/_approximate_mll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/added_loss_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/deep_approximate_mll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/deep_predictive_log_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/exact_marginal_log_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/gamma_robust_variational_elbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/inducing_point_kernel_added_loss_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/kl_gaussian_added_loss_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/leave_one_out_pseudo_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/marginal_log_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/noise_model_added_loss_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/predictive_log_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/sum_marginal_log_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/mlls/variational_elbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.925914 gpytorch-1.9.1/gpytorch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/approximate_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.925914 gpytorch-1.9.1/gpytorch/models/deep_gps/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/deep_gps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/deep_gps/deep_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/deep_gps/dspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/exact_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38061 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/exact_prediction_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/gp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.929914 gpytorch-1.9.1/gpytorch/models/gplvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/gplvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/gplvm/bayesian_gplvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/gplvm/latent_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/model_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.929914 gpytorch-1.9.1/gpytorch/models/pyro/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/pyro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/pyro/_pyro_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/models/pyro/pyro_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25741 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.929914 gpytorch-1.9.1/gpytorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/optim/ngd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.929914 gpytorch-1.9.1/gpytorch/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/priors/horseshoe_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/priors/lkj_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/priors/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/priors/smoothed_box_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/priors/torch_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/priors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/priors/wishart_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.929914 gpytorch-1.9.1/gpytorch/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8291 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/test/base_kernel_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/test/base_likelihood_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/test/base_mean_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/test/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/test/model_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16499 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/test/variational_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.933914 gpytorch-1.9.1/gpytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/broadcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/lanczos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/permutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/toeplitz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.933914 gpytorch-1.9.1/gpytorch/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/_variational_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15389 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/additive_grid_interpolation_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/batch_decoupled_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/cholesky_variational_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/ciq_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/delta_variational_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/grid_interpolation_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/independent_multitask_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/lmc_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/mean_field_variational_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/natural_variational_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/nearest_neighbor_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/orthogonally_decoupled_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/tril_natural_variational_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/unwhitened_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-01-04 22:55:01.000000 gpytorch-1.9.1/gpytorch/variational/variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-04 22:55:09.000000 gpytorch-1.9.1/gpytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.917913 gpytorch-1.9.1/gpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-01-04 22:55:09.000000 gpytorch-1.9.1/gpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-01-04 22:55:09.000000 gpytorch-1.9.1/gpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 22:55:09.000000 gpytorch-1.9.1/gpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-01-04 22:55:09.000000 gpytorch-1.9.1/gpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-04 22:55:09.000000 gpytorch-1.9.1/gpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-01-04 22:55:01.000000 gpytorch-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-04 22:55:01.000000 gpytorch-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-01-04 22:55:09.949915 gpytorch-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-01-04 22:55:01.000000 gpytorch-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.933914 gpytorch-1.9.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.933914 gpytorch-1.9.1/test/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/constraints/test_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.933914 gpytorch-1.9.1/test/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/distributions/test_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/distributions/test_multitask_multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17954 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/distributions/test_multivariate_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.941914 gpytorch-1.9.1/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/old_variational_strategy_model.pth
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_batch_decoupled_ppgpr_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_batch_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_batch_multitask_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_batch_svgp_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_decoupled_svgp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_dspp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_fixed_noise_fanatasy_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_grid_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_hadamard_multitask_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_independent_multitask_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_additive_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_additive_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_dkl_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_gp_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_kronecker_product_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_kronecker_product_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_multiplicative_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_variational_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kissgp_white_noise_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kronecker_multitask_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kronecker_multitask_sgpr_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_kronecker_multitask_ski_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_lcm_kernel_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_lmc_svgp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_model_list_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_pyro_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_rff_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_sgpr_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_simple_gp_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_simple_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_spectral_mixture_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_svgp_gp_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_svgp_gp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_unwhitened_svgp_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/examples/test_white_noise_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.941914 gpytorch-1.9.1/test/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/functions/test_log_normal_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/functions/test_matern_covariance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/functions/test_rbf_covariance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.941914 gpytorch-1.9.1/test/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.941914 gpytorch-1.9.1/test/kernels/keops/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/keops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/keops/test_matern_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/keops/test_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_additive_and_product_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_arc_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_cosine_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_cylindrical_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_gaussian_symmetrized_kl_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_grid_interpolation_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_grid_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_index_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_inducing_point_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_linear_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_matern_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_newton_girard_additive_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_periodic_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_piecewise_polynomial_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_polynomial_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_polynomial_kernel_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_rbf_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_rbf_kernel_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_rff_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_rq_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_scale_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_spectral_delta_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/kernels/test_spectral_mixture_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.941914 gpytorch-1.9.1/test/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/lazy/test_lazy_evaluated_kernel_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/lazy/test_lazy_tensor_deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.941914 gpytorch-1.9.1/test/likelihoods/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/test_bernoulli_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/test_beta_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/test_gaussian_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/test_general_multitask_gaussian_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/test_laplace_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/test_multitask_gaussian_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/test_softmax_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/likelihoods/test_student_t_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/test/means/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/means/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/means/test_constant_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/means/test_constant_mean_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/means/test_linear_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/means/test_multitask_mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/means/test_zero_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/test/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/test/mlls/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/mlls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/mlls/test_exact_marginal_log_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/mlls/test_inducing_point_kernel_added_loss_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/mlls/test_leave_one_out_pseudo_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/test/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/models/test_exact_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/models/test_model_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/models/test_variational_gp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/test/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/optim/test_ngd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/test/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/test_gamma_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/test_half_cauchy_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/test_half_normal_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/test_horseshoe_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/test_lkj_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/test_multivariate_normal_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/test_normal_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/priors/test_smoothed_box_prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/utils/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/utils/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/utils/test_nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/utils/test_quadrature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:09.945915 gpytorch-1.9.1/test/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_batch_decoupled_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_ciq_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_grid_interpolation_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_independent_multitask_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_lmc_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_natural_variational_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_nearest_neighbor_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_orthogonally_decoupled_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_unwhitened_variational_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-01-04 22:55:01.000000 gpytorch-1.9.1/test/variational/test_variational_strategy.py
```

### Comparing `gpytorch-1.9.0/.conda/meta.yaml` & `gpytorch-1.9.1/.conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/.github/ISSUE_TEMPLATE/---bug-report.md` & `gpytorch-1.9.1/.github/ISSUE_TEMPLATE/---bug-report.md`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/.github/ISSUE_TEMPLATE/---documentation-examples.md` & `gpytorch-1.9.1/.github/ISSUE_TEMPLATE/---documentation-examples.md`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/.github/ISSUE_TEMPLATE/---feature-request.md` & `gpytorch-1.9.1/.github/ISSUE_TEMPLATE/---feature-request.md`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/.github/workflows/deploy.yml` & `gpytorch-1.9.1/.github/workflows/deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     - uses: conda-incubator/setup-miniconda@v2
       with:
         auto-update-conda: false
         python-version: "3.8"
     - name: Install dependencies
       run: |
         conda install -y anaconda-client conda-build
+        conda install linear_operator -c gpytorch
         pip install setuptools_scm
     - name: Build and publish
       run: |
         conda config --set anaconda_upload yes
         conda config --append channels pytorch
         /usr/share/miniconda/bin/anaconda login --username ${{ secrets.CONDA_USERNAME }} --password ${{ secrets.CONDA_PASSWORD }}
         python -m setuptools_scm
```

### Comparing `gpytorch-1.9.0/.github/workflows/run_test_suite.yml` & `gpytorch-1.9.1/.github/workflows/run_test_suite.yml`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
   run_unit_tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         pytorch-version: ["master", "stable"]
         extras: ["with-extras", "no-extras"]
+        exclude:  # Currently pyro does not support the torch 2.0.0 beta
+          - pytorch-version: "master"
+            extras: "with-extras"
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
         python-version: "3.8"
     - name: Install dependencies
```

### Comparing `gpytorch-1.9.0/.gitignore` & `gpytorch-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/.pre-commit-config.yaml` & `gpytorch-1.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/.readthedocs.yml` & `gpytorch-1.9.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/LICENSE` & `gpytorch-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/PKG-INFO` & `gpytorch-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpytorch
-Version: 1.9.0
+Version: 1.9.1
 Summary: An implementation of Gaussian Processes in Pytorch
 Home-page: https://gpytorch.ai
 Author: Jake Gardner, Geoff Pleiss
 Author-email: jrg365@cornell.edu, gpleiss@gmail.com
 License: MIT
 Project-URL: Documentation, https://gpytorch.readthedocs.io
 Project-URL: Source, https://github.com/cornellius-gp/gpytorch/
@@ -40,14 +40,15 @@
         (To use packages globally but install GPyTorch as a user-only package, use `pip install --user` above.)
         
         #### Latest (unstable) version
         
         To upgrade to the latest (unstable) version, run
         
         ```bash
+        pip install --upgrade git+https://github.com/cornellius-gp/linear_operator.git
         pip install --upgrade git+https://github.com/cornellius-gp/gpytorch.git
         ```
         
         #### ArchLinux Package
         Note: Experimental AUR package. For most users, we recommend installation by conda or pip.
         
         GPyTorch is also available on the [ArchLinux User Repository](https://wiki.archlinux.org/index.php/Arch_User_Repository) (AUR).
```

### Comparing `gpytorch-1.9.0/README.md` & `gpytorch-1.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 (To use packages globally but install GPyTorch as a user-only package, use `pip install --user` above.)
 
 #### Latest (unstable) version
 
 To upgrade to the latest (unstable) version, run
 
 ```bash
+pip install --upgrade git+https://github.com/cornellius-gp/linear_operator.git
 pip install --upgrade git+https://github.com/cornellius-gp/gpytorch.git
 ```
 
 #### ArchLinux Package
 Note: Experimental AUR package. For most users, we recommend installation by conda or pip.
 
 GPyTorch is also available on the [ArchLinux User Repository](https://wiki.archlinux.org/index.php/Arch_User_Repository) (AUR).
```

### Comparing `gpytorch-1.9.0/docs/Makefile` & `gpytorch-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/constraints.rst` & `gpytorch-1.9.1/docs/source/constraints.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/distributions.rst` & `gpytorch-1.9.1/docs/source/distributions.rst`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 
 MultivariateNormal
 -----------------------------
 
 .. autoclass:: MultivariateNormal
    :members:
+   :special-members: __getitem__
 
 
 MultitaskMultivariateNormal
 ----------------------------------
 
 .. autoclass:: MultitaskMultivariateNormal
    :members:
```

### Comparing `gpytorch-1.9.0/docs/source/functions.rst` & `gpytorch-1.9.1/docs/source/functions.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/index.rst` & `gpytorch-1.9.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/kernels.rst` & `gpytorch-1.9.1/docs/source/kernels.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 Kernel
 ----------------
 
 .. autoclass:: Kernel
    :members:
+   :special-members: __call__, __getitem__
 
 Standard Kernels
 -----------------------------
 
 :hidden:`CosineKernel`
 ~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `gpytorch-1.9.0/docs/source/likelihoods.rst` & `gpytorch-1.9.1/docs/source/likelihoods.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/marginal_log_likelihoods.rst` & `gpytorch-1.9.1/docs/source/marginal_log_likelihoods.rst`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
 :hidden:`LeaveOneOutPseudoLikelihood`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: LeaveOneOutPseudoLikelihood
    :members:
 
+
 Approximate GP Inference
 -----------------------------------
 
 These are MLLs for use with :obj:`~gpytorch.models.ApproximateGP` modules. They are designed for
 when exact inference is intractable (either when the likelihood is non-Gaussian likelihood, or when
 there is too much data for an ExactGP model).
 
@@ -69,7 +70,26 @@
    :members:
 
 :hidden:`DeepApproximateMLL`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: DeepApproximateMLL
    :members:
+
+
+Modifications to Objective Functions
+---------------------------------------
+
+.. autoclass:: AddedLossTerm
+   :members:
+
+:hidden:`InducingPointKernelAddedLossTerm`
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: InducingPointKernelAddedLossTerm
+   :members:
+
+:hidden:`KLGaussianAddedLossTerm`
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: KLGaussianAddedLossTerm
+   :members:
```

### Comparing `gpytorch-1.9.0/docs/source/means.rst` & `gpytorch-1.9.1/docs/source/means.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/metrics.rst` & `gpytorch-1.9.1/docs/source/metrics.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/models.rst` & `gpytorch-1.9.1/docs/source/models.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/priors.rst` & `gpytorch-1.9.1/docs/source/priors.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/utils.rst` & `gpytorch-1.9.1/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/docs/source/variational.rst` & `gpytorch-1.9.1/docs/source/variational.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/00_Basic_Usage/Hyperparameters.ipynb` & `gpytorch-1.9.1/examples/00_Basic_Usage/Hyperparameters.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/00_Basic_Usage/Implementing_a_custom_Kernel.ipynb` & `gpytorch-1.9.1/examples/00_Basic_Usage/Implementing_a_custom_Kernel.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/00_Basic_Usage/Metrics.ipynb` & `gpytorch-1.9.1/examples/00_Basic_Usage/Metrics.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/00_Basic_Usage/README.rst` & `gpytorch-1.9.1/examples/00_Basic_Usage/README.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/00_Basic_Usage/Saving_and_Loading_Models.ipynb` & `gpytorch-1.9.1/examples/00_Basic_Usage/Saving_and_Loading_Models.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/00_Basic_Usage/index.rst` & `gpytorch-1.9.1/examples/00_Basic_Usage/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/01_Exact_GPs/GP_Regression_DistributionalKernel.ipynb` & `gpytorch-1.9.1/examples/08_Advanced_Usage/Simple_GP_Regression_Derivative_Information_2d.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8161230587988401%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# GPyTorch regression with derivative information in "*

 * *            "2d\\n'), (2, '## Introduction\\n'), (3, 'In this notebook, we show how to train a GP "*

 * *            'regression model in GPyTorch of a 2-dimensional function given function values and '*

 * *            'derivative observations. We consider modeling the Franke function where the values '*

 * *            'and derivatives are contaminated with independent $\\\\mathcal{N}(0, 0.5)$ '*

 * *            "distributed noi […]*

```diff
@@ -1,804 +1,360 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# GP Regression with Uncertain Inputs\n",
+                "# GPyTorch regression with derivative information in 2d\n",
                 "\n",
                 "## Introduction\n",
-                "\n",
-                "In this notebook, we're going to demonstrate one way of dealing with uncertainty in our training data. Let's say that we're collecting training data that models the following function.\n",
-                "\n",
-                "$$\n",
-                "\\begin{align}\n",
-                "y &= \\sin(2\\pi x) + \\epsilon \\\\\n",
-                "  \\epsilon &\\sim \\mathcal{N}(0, 0.2) \n",
-                "\\end{align}\n",
-                "$$\n",
-                "\n",
-                "However, now assume that we're a bit uncertain about our features. In particular, we're going to assume that every `x_i` value is not a point but a distribution instead. E.g.\n",
-                "\n",
-                "$$ x_i \\sim \\mathcal{N}(\\mu_i, \\sigma_i). $$"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "### Using a distributional kernel to deal with uncertain inputs\n",
-                "\n",
-                "Rather than using a variational method (see the GP Regression with Uncertian Inputs tutorial in the variational examples), if we explicitly know the type of uncertainty in our inputs we can pass that into our kernel.\n",
-                "\n",
-                "More specifically, assuming Gaussian inputs, we will compute the symmetrized KL divergence between the Gaussian inputs.\n",
-                "\n"
+                "In this notebook, we show how to train a GP regression model in GPyTorch of a 2-dimensional function given function values and derivative observations. We consider modeling the Franke function where the values and derivatives are contaminated with independent $\\mathcal{N}(0, 0.5)$ distributed noise."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import math\n",
                 "import torch\n",
-                "import tqdm\n",
                 "import gpytorch\n",
+                "import math\n",
+                "from matplotlib import cm\n",
                 "from matplotlib import pyplot as plt\n",
+                "import numpy as np\n",
                 "\n",
                 "%matplotlib inline\n",
                 "%load_ext autoreload\n",
                 "%autoreload 2"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Franke function\n",
+                "The following is a vectorized implementation of the 2-dimensional Franke function (https://www.sfu.ca/~ssurjano/franke2d.html)"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Training data is 100 points in [0,1] inclusive regularly spaced\n",
-                "train_x_mean = torch.linspace(0, 1, 20)\n",
-                "# We'll assume the variance shrinks the closer we get to 1\n",
-                "train_x_stdv = torch.linspace(0.03, 0.01, 20)\n",
-                "\n",
-                "# True function is sin(2*pi*x) with Gaussian noise\n",
-                "train_y = torch.sin(train_x_mean * (2 * math.pi)) + torch.randn(train_x_mean.size()) * 0.2"
+                "def franke(X, Y):\n",
+                "    term1 = .75*torch.exp(-((9*X - 2).pow(2) + (9*Y - 2).pow(2))/4)\n",
+                "    term2 = .75*torch.exp(-((9*X + 1).pow(2))/49 - (9*Y + 1)/10)\n",
+                "    term3 = .5*torch.exp(-((9*X - 7).pow(2) + (9*Y - 3).pow(2))/4)\n",
+                "    term4 = .2*torch.exp(-(9*X - 4).pow(2) - (9*Y - 7).pow(2))\n",
+                "    \n",
+                "    f = term1 + term2 + term3 - term4\n",
+                "    dfx = -2*(9*X - 2)*9/4 * term1 - 2*(9*X + 1)*9/49 * term2 + \\\n",
+                "          -2*(9*X - 7)*9/4 * term3 + 2*(9*X - 4)*9 * term4\n",
+                "    dfy = -2*(9*Y - 2)*9/4 * term1 - 9/10 * term2 + \\\n",
+                "          -2*(9*Y - 3)*9/4 * term3 + 2*(9*Y - 7)*9 * term4\n",
+                "    \n",
+                "    return f, dfx, dfy"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To effectively pass in the training distributional data, we will need to stack the mean and log variances."
+                "## Setting up the training data\n",
+                "We use a grid with 100 points in $[0,1] \\times [0,1]$ with 10 uniformly distributed points per dimension."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
-                "train_x_distributional = torch.stack((train_x_mean, (train_x_stdv**2).log()), dim=1)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "<matplotlib.legend.Legend at 0x7fc3069399d0>"
-                        ]
-                    },
-                    "execution_count": 4,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                },
-                {
-                    "data": {
-                        "image/png": "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\n",
-                        "text/plain": [
-                            "<Figure size 576x216 with 1 Axes>"
-                        ]
-                    },
-                    "metadata": {
-                        "needs_background": "light"
-                    },
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "f, ax = plt.subplots(1, 1, figsize=(8, 3))\n",
-                "ax.errorbar(train_x_mean, train_y, xerr=(train_x_stdv * 2), fmt=\"k*\", label=\"Train Data\")\n",
-                "ax.legend()"
+                "xv, yv = torch.meshgrid(torch.linspace(0, 1, 10), torch.linspace(0, 1, 10), indexing=\"ij\")\n",
+                "train_x = torch.cat((\n",
+                "    xv.contiguous().view(xv.numel(), 1), \n",
+                "    yv.contiguous().view(yv.numel(), 1)),\n",
+                "    dim=1\n",
+                ")\n",
+                "\n",
+                "f, dfx, dfy = franke(train_x[:, 0], train_x[:, 1])\n",
+                "train_y = torch.stack([f, dfx, dfy], -1).squeeze(1)\n",
+                "\n",
+                "train_y += 0.05 * torch.randn(train_y.size()) # Add noise to both values and gradients"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We train the hyperparameters of the resulting distributional GP via type-II gradient descent, as is standard in many settings. We could also do fully Bayesian inference."
+                "## Setting up the model\n",
+                "A GP prior on the function values implies a multi-output GP prior on the function values and the partial derivatives, see 9.4 in http://www.gaussianprocess.org/gpml/chapters/RW9.pdf for more details. This allows using a `MultitaskMultivariateNormal` and `MultitaskGaussianLikelihood` to train a GP model from both function values and gradients. The resulting RBF kernel that models the covariance between the values and partial derivatives has been implemented in `RBFKernelGrad` and the extension of a constant mean is implemented in `ConstantMeanGrad`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
+            "execution_count": 4,
+            "metadata": {
+                "scrolled": true
+            },
             "outputs": [],
             "source": [
-                "from gpytorch.models import ExactGP\n",
-                "from gpytorch.kernels import GaussianSymmetrizedKLKernel, ScaleKernel\n",
-                "from gpytorch.means import ConstantMean\n",
-                "\n",
-                "class ExactGPModel(ExactGP):\n",
+                "class GPModelWithDerivatives(gpytorch.models.ExactGP):\n",
                 "    def __init__(self, train_x, train_y, likelihood):\n",
-                "        super(ExactGPModel, self).__init__(train_x, train_y, likelihood)\n",
-                "        self.mean_module = ConstantMean()\n",
-                "        self.covar_module = ScaleKernel(GaussianSymmetrizedKLKernel())\n",
+                "        super(GPModelWithDerivatives, self).__init__(train_x, train_y, likelihood)\n",
+                "        self.mean_module = gpytorch.means.ConstantMeanGrad()\n",
+                "        self.base_kernel = gpytorch.kernels.RBFKernelGrad(ard_num_dims=2)\n",
+                "        self.covar_module = gpytorch.kernels.ScaleKernel(self.base_kernel)\n",
                 "        \n",
                 "    def forward(self, x):\n",
                 "        mean_x = self.mean_module(x)\n",
                 "        covar_x = self.covar_module(x)\n",
-                "        return gpytorch.distributions.MultivariateNormal(mean_x, covar_x)\n",
+                "        return gpytorch.distributions.MultitaskMultivariateNormal(mean_x, covar_x)\n",
                 "\n",
-                "# initialize likelihood and model\n",
-                "likelihood = gpytorch.likelihoods.GaussianLikelihood()\n",
-                "model = ExactGPModel(train_x_distributional, train_y, likelihood)"
+                "likelihood = gpytorch.likelihoods.MultitaskGaussianLikelihood(num_tasks=3)  # Value + x-derivative + y-derivative\n",
+                "model = GPModelWithDerivatives(train_x, train_y, likelihood)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The model training is similar to training a standard GP regression model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Iter 1/500 - Loss: 1.274   lengthscale: 0.693   noise: 0.693\n",
-                        "Iter 2/500 - Loss: 1.242   lengthscale: 0.826   noise: 0.576\n",
-                        "Iter 3/500 - Loss: 1.173   lengthscale: 0.955   noise: 0.475\n",
-                        "Iter 4/500 - Loss: 1.141   lengthscale: 1.102   noise: 0.389\n",
-                        "Iter 5/500 - Loss: 1.121   lengthscale: 1.266   noise: 0.317\n",
-                        "Iter 6/500 - Loss: 1.097   lengthscale: 1.442   noise: 0.261\n",
-                        "Iter 7/500 - Loss: 1.093   lengthscale: 1.621   noise: 0.220\n",
-                        "Iter 8/500 - Loss: 1.112   lengthscale: 1.801   noise: 0.192\n",
-                        "Iter 9/500 - Loss: 1.112   lengthscale: 1.988   noise: 0.177\n",
-                        "Iter 10/500 - Loss: 1.095   lengthscale: 2.188   noise: 0.172\n",
-                        "Iter 11/500 - Loss: 1.081   lengthscale: 2.401   noise: 0.172\n",
-                        "Iter 12/500 - Loss: 1.068   lengthscale: 2.624   noise: 0.177\n",
-                        "Iter 13/500 - Loss: 1.049   lengthscale: 2.856   noise: 0.183\n",
-                        "Iter 14/500 - Loss: 1.031   lengthscale: 3.095   noise: 0.188\n",
-                        "Iter 15/500 - Loss: 1.020   lengthscale: 3.340   noise: 0.191\n",
-                        "Iter 16/500 - Loss: 1.014   lengthscale: 3.589   noise: 0.189\n",
-                        "Iter 17/500 - Loss: 1.007   lengthscale: 3.842   noise: 0.183\n",
-                        "Iter 18/500 - Loss: 0.997   lengthscale: 4.098   noise: 0.173\n",
-                        "Iter 19/500 - Loss: 0.983   lengthscale: 4.356   noise: 0.159\n",
-                        "Iter 20/500 - Loss: 0.968   lengthscale: 4.616   noise: 0.144\n",
-                        "Iter 21/500 - Loss: 0.951   lengthscale: 4.877   noise: 0.128\n",
-                        "Iter 22/500 - Loss: 0.933   lengthscale: 5.139   noise: 0.112\n",
-                        "Iter 23/500 - Loss: 0.913   lengthscale: 5.402   noise: 0.097\n",
-                        "Iter 24/500 - Loss: 0.891   lengthscale: 5.667   noise: 0.083\n",
-                        "Iter 25/500 - Loss: 0.870   lengthscale: 5.933   noise: 0.070\n",
-                        "Iter 26/500 - Loss: 0.850   lengthscale: 6.202   noise: 0.059\n",
-                        "Iter 27/500 - Loss: 0.832   lengthscale: 6.474   noise: 0.050\n",
-                        "Iter 28/500 - Loss: 0.814   lengthscale: 6.748   noise: 0.042\n",
-                        "Iter 29/500 - Loss: 0.794   lengthscale: 7.025   noise: 0.035\n",
-                        "Iter 30/500 - Loss: 0.775   lengthscale: 7.304   noise: 0.029\n",
-                        "Iter 31/500 - Loss: 0.756   lengthscale: 7.586   noise: 0.024\n",
-                        "Iter 32/500 - Loss: 0.737   lengthscale: 7.868   noise: 0.020\n",
-                        "Iter 33/500 - Loss: 0.719   lengthscale: 8.152   noise: 0.017\n",
-                        "Iter 34/500 - Loss: 0.701   lengthscale: 8.437   noise: 0.014\n",
-                        "Iter 35/500 - Loss: 0.684   lengthscale: 8.722   noise: 0.012\n",
-                        "Iter 36/500 - Loss: 0.668   lengthscale: 9.007   noise: 0.010\n",
-                        "Iter 37/500 - Loss: 0.653   lengthscale: 9.291   noise: 0.008\n",
-                        "Iter 38/500 - Loss: 0.637   lengthscale: 9.575   noise: 0.007\n",
-                        "Iter 39/500 - Loss: 0.621   lengthscale: 9.859   noise: 0.006\n",
-                        "Iter 40/500 - Loss: 0.606   lengthscale: 10.142   noise: 0.005\n",
-                        "Iter 41/500 - Loss: 0.591   lengthscale: 10.424   noise: 0.005\n",
-                        "Iter 42/500 - Loss: 0.577   lengthscale: 10.705   noise: 0.004\n",
-                        "Iter 43/500 - Loss: 0.564   lengthscale: 10.985   noise: 0.003\n",
-                        "Iter 44/500 - Loss: 0.551   lengthscale: 11.263   noise: 0.003\n",
-                        "Iter 45/500 - Loss: 0.539   lengthscale: 11.540   noise: 0.003\n",
-                        "Iter 46/500 - Loss: 0.526   lengthscale: 11.815   noise: 0.002\n",
-                        "Iter 47/500 - Loss: 0.514   lengthscale: 12.088   noise: 0.002\n",
-                        "Iter 48/500 - Loss: 0.503   lengthscale: 12.359   noise: 0.002\n",
-                        "Iter 49/500 - Loss: 0.492   lengthscale: 12.627   noise: 0.002\n",
-                        "Iter 50/500 - Loss: 0.482   lengthscale: 12.892   noise: 0.001\n",
-                        "Iter 51/500 - Loss: 0.472   lengthscale: 13.154   noise: 0.001\n",
-                        "Iter 52/500 - Loss: 0.462   lengthscale: 13.412   noise: 0.001\n",
-                        "Iter 53/500 - Loss: 0.453   lengthscale: 13.668   noise: 0.001\n",
-                        "Iter 54/500 - Loss: 0.445   lengthscale: 13.919   noise: 0.001\n",
-                        "Iter 55/500 - Loss: 0.437   lengthscale: 14.167   noise: 0.001\n",
-                        "Iter 56/500 - Loss: 0.429   lengthscale: 14.410   noise: 0.001\n",
-                        "Iter 57/500 - Loss: 0.422   lengthscale: 14.649   noise: 0.001\n",
-                        "Iter 58/500 - Loss: 0.415   lengthscale: 14.883   noise: 0.001\n",
-                        "Iter 59/500 - Loss: 0.409   lengthscale: 15.111   noise: 0.001\n",
-                        "Iter 60/500 - Loss: 0.403   lengthscale: 15.335   noise: 0.001\n",
-                        "Iter 61/500 - Loss: 0.398   lengthscale: 15.552   noise: 0.001\n",
-                        "Iter 62/500 - Loss: 0.393   lengthscale: 15.764   noise: 0.001\n",
-                        "Iter 63/500 - Loss: 0.389   lengthscale: 15.970   noise: 0.001\n",
-                        "Iter 64/500 - Loss: 0.385   lengthscale: 16.170   noise: 0.000\n",
-                        "Iter 65/500 - Loss: 0.381   lengthscale: 16.363   noise: 0.000\n",
-                        "Iter 66/500 - Loss: 0.378   lengthscale: 16.551   noise: 0.000\n",
-                        "Iter 67/500 - Loss: 0.375   lengthscale: 16.731   noise: 0.000\n",
-                        "Iter 68/500 - Loss: 0.373   lengthscale: 16.905   noise: 0.000\n",
-                        "Iter 69/500 - Loss: 0.371   lengthscale: 17.072   noise: 0.000\n",
-                        "Iter 70/500 - Loss: 0.369   lengthscale: 17.231   noise: 0.000\n",
-                        "Iter 71/500 - Loss: 0.367   lengthscale: 17.383   noise: 0.000\n",
-                        "Iter 72/500 - Loss: 0.366   lengthscale: 17.527   noise: 0.000\n",
-                        "Iter 73/500 - Loss: 0.365   lengthscale: 17.662   noise: 0.000\n",
-                        "Iter 74/500 - Loss: 0.364   lengthscale: 17.791   noise: 0.000\n",
-                        "Iter 75/500 - Loss: 0.363   lengthscale: 17.911   noise: 0.000\n",
-                        "Iter 76/500 - Loss: 0.363   lengthscale: 18.024   noise: 0.000\n",
-                        "Iter 77/500 - Loss: 0.362   lengthscale: 18.129   noise: 0.000\n",
-                        "Iter 78/500 - Loss: 0.362   lengthscale: 18.227   noise: 0.000\n",
-                        "Iter 79/500 - Loss: 0.362   lengthscale: 18.317   noise: 0.000\n",
-                        "Iter 80/500 - Loss: 0.362   lengthscale: 18.400   noise: 0.000\n",
-                        "Iter 81/500 - Loss: 0.362   lengthscale: 18.477   noise: 0.000\n",
-                        "Iter 82/500 - Loss: 0.362   lengthscale: 18.546   noise: 0.000\n",
-                        "Iter 83/500 - Loss: 0.362   lengthscale: 18.608   noise: 0.000\n",
-                        "Iter 84/500 - Loss: 0.362   lengthscale: 18.664   noise: 0.000\n",
-                        "Iter 85/500 - Loss: 0.362   lengthscale: 18.712   noise: 0.000\n",
-                        "Iter 86/500 - Loss: 0.362   lengthscale: 18.755   noise: 0.000\n",
-                        "Iter 87/500 - Loss: 0.362   lengthscale: 18.791   noise: 0.000\n",
-                        "Iter 88/500 - Loss: 0.362   lengthscale: 18.822   noise: 0.000\n",
-                        "Iter 89/500 - Loss: 0.362   lengthscale: 18.848   noise: 0.000\n",
-                        "Iter 90/500 - Loss: 0.363   lengthscale: 18.868   noise: 0.000\n",
-                        "Iter 91/500 - Loss: 0.363   lengthscale: 18.884   noise: 0.000\n",
-                        "Iter 92/500 - Loss: 0.363   lengthscale: 18.896   noise: 0.000\n",
-                        "Iter 93/500 - Loss: 0.363   lengthscale: 18.904   noise: 0.000\n",
-                        "Iter 94/500 - Loss: 0.363   lengthscale: 18.909   noise: 0.000\n",
-                        "Iter 95/500 - Loss: 0.363   lengthscale: 18.910   noise: 0.000\n",
-                        "Iter 96/500 - Loss: 0.363   lengthscale: 18.907   noise: 0.000\n",
-                        "Iter 97/500 - Loss: 0.363   lengthscale: 18.902   noise: 0.000\n",
-                        "Iter 98/500 - Loss: 0.363   lengthscale: 18.894   noise: 0.000\n",
-                        "Iter 99/500 - Loss: 0.362   lengthscale: 18.884   noise: 0.000\n",
-                        "Iter 100/500 - Loss: 0.362   lengthscale: 18.873   noise: 0.000\n",
-                        "Iter 101/500 - Loss: 0.362   lengthscale: 18.859   noise: 0.000\n",
-                        "Iter 102/500 - Loss: 0.362   lengthscale: 18.844   noise: 0.000\n",
-                        "Iter 103/500 - Loss: 0.362   lengthscale: 18.828   noise: 0.000\n",
-                        "Iter 104/500 - Loss: 0.362   lengthscale: 18.811   noise: 0.000\n",
-                        "Iter 105/500 - Loss: 0.362   lengthscale: 18.794   noise: 0.000\n",
-                        "Iter 106/500 - Loss: 0.362   lengthscale: 18.776   noise: 0.000\n",
-                        "Iter 107/500 - Loss: 0.362   lengthscale: 18.758   noise: 0.000\n",
-                        "Iter 108/500 - Loss: 0.362   lengthscale: 18.740   noise: 0.000\n",
-                        "Iter 109/500 - Loss: 0.362   lengthscale: 18.722   noise: 0.000\n",
-                        "Iter 110/500 - Loss: 0.362   lengthscale: 18.704   noise: 0.000\n",
-                        "Iter 111/500 - Loss: 0.362   lengthscale: 18.687   noise: 0.000\n",
-                        "Iter 112/500 - Loss: 0.362   lengthscale: 18.670   noise: 0.000\n",
-                        "Iter 113/500 - Loss: 0.362   lengthscale: 18.653   noise: 0.000\n",
-                        "Iter 114/500 - Loss: 0.362   lengthscale: 18.638   noise: 0.000\n",
-                        "Iter 115/500 - Loss: 0.362   lengthscale: 18.622   noise: 0.000\n",
-                        "Iter 116/500 - Loss: 0.362   lengthscale: 18.608   noise: 0.000\n",
-                        "Iter 117/500 - Loss: 0.362   lengthscale: 18.595   noise: 0.000\n",
-                        "Iter 118/500 - Loss: 0.362   lengthscale: 18.583   noise: 0.000\n",
-                        "Iter 119/500 - Loss: 0.362   lengthscale: 18.572   noise: 0.000\n",
-                        "Iter 120/500 - Loss: 0.362   lengthscale: 18.561   noise: 0.000\n",
-                        "Iter 121/500 - Loss: 0.362   lengthscale: 18.552   noise: 0.000\n",
-                        "Iter 122/500 - Loss: 0.362   lengthscale: 18.543   noise: 0.000\n",
-                        "Iter 123/500 - Loss: 0.362   lengthscale: 18.536   noise: 0.000\n",
-                        "Iter 124/500 - Loss: 0.362   lengthscale: 18.529   noise: 0.000\n",
-                        "Iter 125/500 - Loss: 0.362   lengthscale: 18.524   noise: 0.000\n",
-                        "Iter 126/500 - Loss: 0.362   lengthscale: 18.519   noise: 0.000\n",
-                        "Iter 127/500 - Loss: 0.362   lengthscale: 18.516   noise: 0.000\n",
-                        "Iter 128/500 - Loss: 0.362   lengthscale: 18.513   noise: 0.000\n",
-                        "Iter 129/500 - Loss: 0.362   lengthscale: 18.511   noise: 0.000\n",
-                        "Iter 130/500 - Loss: 0.362   lengthscale: 18.510   noise: 0.000\n",
-                        "Iter 131/500 - Loss: 0.362   lengthscale: 18.509   noise: 0.000\n",
-                        "Iter 132/500 - Loss: 0.362   lengthscale: 18.510   noise: 0.000\n",
-                        "Iter 133/500 - Loss: 0.362   lengthscale: 18.511   noise: 0.000\n",
-                        "Iter 134/500 - Loss: 0.362   lengthscale: 18.512   noise: 0.000\n",
-                        "Iter 135/500 - Loss: 0.362   lengthscale: 18.514   noise: 0.000\n",
-                        "Iter 136/500 - Loss: 0.362   lengthscale: 18.517   noise: 0.000\n",
-                        "Iter 137/500 - Loss: 0.362   lengthscale: 18.520   noise: 0.000\n",
-                        "Iter 138/500 - Loss: 0.362   lengthscale: 18.524   noise: 0.000\n",
-                        "Iter 139/500 - Loss: 0.362   lengthscale: 18.528   noise: 0.000\n",
-                        "Iter 140/500 - Loss: 0.362   lengthscale: 18.532   noise: 0.000\n",
-                        "Iter 141/500 - Loss: 0.362   lengthscale: 18.537   noise: 0.000\n",
-                        "Iter 142/500 - Loss: 0.362   lengthscale: 18.542   noise: 0.000\n",
-                        "Iter 143/500 - Loss: 0.362   lengthscale: 18.547   noise: 0.000\n",
-                        "Iter 144/500 - Loss: 0.362   lengthscale: 18.552   noise: 0.000\n",
-                        "Iter 145/500 - Loss: 0.362   lengthscale: 18.558   noise: 0.000\n",
-                        "Iter 146/500 - Loss: 0.362   lengthscale: 18.563   noise: 0.000\n",
-                        "Iter 147/500 - Loss: 0.362   lengthscale: 18.569   noise: 0.000\n",
-                        "Iter 148/500 - Loss: 0.362   lengthscale: 18.574   noise: 0.000\n",
-                        "Iter 149/500 - Loss: 0.362   lengthscale: 18.580   noise: 0.000\n",
-                        "Iter 150/500 - Loss: 0.362   lengthscale: 18.586   noise: 0.000\n",
-                        "Iter 151/500 - Loss: 0.362   lengthscale: 18.592   noise: 0.000\n",
-                        "Iter 152/500 - Loss: 0.362   lengthscale: 18.597   noise: 0.000\n",
-                        "Iter 153/500 - Loss: 0.362   lengthscale: 18.603   noise: 0.000\n",
-                        "Iter 154/500 - Loss: 0.362   lengthscale: 18.608   noise: 0.000\n",
-                        "Iter 155/500 - Loss: 0.362   lengthscale: 18.614   noise: 0.000\n",
-                        "Iter 156/500 - Loss: 0.362   lengthscale: 18.619   noise: 0.000\n",
-                        "Iter 157/500 - Loss: 0.362   lengthscale: 18.625   noise: 0.000\n",
-                        "Iter 158/500 - Loss: 0.362   lengthscale: 18.630   noise: 0.000\n",
-                        "Iter 159/500 - Loss: 0.362   lengthscale: 18.635   noise: 0.000\n",
-                        "Iter 160/500 - Loss: 0.362   lengthscale: 18.640   noise: 0.000\n",
-                        "Iter 161/500 - Loss: 0.362   lengthscale: 18.645   noise: 0.000\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Iter 162/500 - Loss: 0.362   lengthscale: 18.650   noise: 0.000\n",
-                        "Iter 163/500 - Loss: 0.362   lengthscale: 18.655   noise: 0.000\n",
-                        "Iter 164/500 - Loss: 0.362   lengthscale: 18.659   noise: 0.000\n",
-                        "Iter 165/500 - Loss: 0.361   lengthscale: 18.664   noise: 0.000\n",
-                        "Iter 166/500 - Loss: 0.361   lengthscale: 18.669   noise: 0.000\n",
-                        "Iter 167/500 - Loss: 0.361   lengthscale: 18.673   noise: 0.000\n",
-                        "Iter 168/500 - Loss: 0.361   lengthscale: 18.678   noise: 0.000\n",
-                        "Iter 169/500 - Loss: 0.361   lengthscale: 18.682   noise: 0.000\n",
-                        "Iter 170/500 - Loss: 0.361   lengthscale: 18.686   noise: 0.000\n",
-                        "Iter 171/500 - Loss: 0.361   lengthscale: 18.691   noise: 0.000\n",
-                        "Iter 172/500 - Loss: 0.361   lengthscale: 18.695   noise: 0.000\n",
-                        "Iter 173/500 - Loss: 0.361   lengthscale: 18.699   noise: 0.000\n",
-                        "Iter 174/500 - Loss: 0.361   lengthscale: 18.704   noise: 0.000\n",
-                        "Iter 175/500 - Loss: 0.361   lengthscale: 18.708   noise: 0.000\n",
-                        "Iter 176/500 - Loss: 0.361   lengthscale: 18.713   noise: 0.000\n",
-                        "Iter 177/500 - Loss: 0.361   lengthscale: 18.717   noise: 0.000\n",
-                        "Iter 178/500 - Loss: 0.361   lengthscale: 18.721   noise: 0.000\n",
-                        "Iter 179/500 - Loss: 0.361   lengthscale: 18.726   noise: 0.000\n",
-                        "Iter 180/500 - Loss: 0.361   lengthscale: 18.731   noise: 0.000\n",
-                        "Iter 181/500 - Loss: 0.361   lengthscale: 18.735   noise: 0.000\n",
-                        "Iter 182/500 - Loss: 0.361   lengthscale: 18.740   noise: 0.000\n",
-                        "Iter 183/500 - Loss: 0.361   lengthscale: 18.745   noise: 0.000\n",
-                        "Iter 184/500 - Loss: 0.361   lengthscale: 18.750   noise: 0.000\n",
-                        "Iter 185/500 - Loss: 0.361   lengthscale: 18.755   noise: 0.000\n",
-                        "Iter 186/500 - Loss: 0.361   lengthscale: 18.760   noise: 0.000\n",
-                        "Iter 187/500 - Loss: 0.361   lengthscale: 18.765   noise: 0.000\n",
-                        "Iter 188/500 - Loss: 0.361   lengthscale: 18.771   noise: 0.000\n",
-                        "Iter 189/500 - Loss: 0.361   lengthscale: 18.776   noise: 0.000\n",
-                        "Iter 190/500 - Loss: 0.361   lengthscale: 18.782   noise: 0.000\n",
-                        "Iter 191/500 - Loss: 0.361   lengthscale: 18.788   noise: 0.000\n",
-                        "Iter 192/500 - Loss: 0.361   lengthscale: 18.794   noise: 0.000\n",
-                        "Iter 193/500 - Loss: 0.361   lengthscale: 18.800   noise: 0.000\n",
-                        "Iter 194/500 - Loss: 0.361   lengthscale: 18.806   noise: 0.000\n",
-                        "Iter 195/500 - Loss: 0.361   lengthscale: 18.813   noise: 0.000\n",
-                        "Iter 196/500 - Loss: 0.361   lengthscale: 18.820   noise: 0.000\n",
-                        "Iter 197/500 - Loss: 0.361   lengthscale: 18.827   noise: 0.000\n",
-                        "Iter 198/500 - Loss: 0.361   lengthscale: 18.834   noise: 0.000\n",
-                        "Iter 199/500 - Loss: 0.361   lengthscale: 18.841   noise: 0.000\n",
-                        "Iter 200/500 - Loss: 0.361   lengthscale: 18.848   noise: 0.000\n",
-                        "Iter 201/500 - Loss: 0.361   lengthscale: 18.856   noise: 0.000\n",
-                        "Iter 202/500 - Loss: 0.361   lengthscale: 18.863   noise: 0.000\n",
-                        "Iter 203/500 - Loss: 0.361   lengthscale: 18.871   noise: 0.000\n",
-                        "Iter 204/500 - Loss: 0.361   lengthscale: 18.880   noise: 0.000\n",
-                        "Iter 205/500 - Loss: 0.361   lengthscale: 18.888   noise: 0.000\n",
-                        "Iter 206/500 - Loss: 0.361   lengthscale: 18.897   noise: 0.001\n",
-                        "Iter 207/500 - Loss: 0.361   lengthscale: 18.905   noise: 0.001\n",
-                        "Iter 208/500 - Loss: 0.361   lengthscale: 18.914   noise: 0.001\n",
-                        "Iter 209/500 - Loss: 0.361   lengthscale: 18.924   noise: 0.001\n",
-                        "Iter 210/500 - Loss: 0.361   lengthscale: 18.933   noise: 0.001\n",
-                        "Iter 211/500 - Loss: 0.361   lengthscale: 18.943   noise: 0.001\n",
-                        "Iter 212/500 - Loss: 0.361   lengthscale: 18.953   noise: 0.001\n",
-                        "Iter 213/500 - Loss: 0.361   lengthscale: 18.963   noise: 0.001\n",
-                        "Iter 214/500 - Loss: 0.361   lengthscale: 18.974   noise: 0.001\n",
-                        "Iter 215/500 - Loss: 0.361   lengthscale: 18.985   noise: 0.001\n",
-                        "Iter 216/500 - Loss: 0.361   lengthscale: 18.996   noise: 0.001\n",
-                        "Iter 217/500 - Loss: 0.361   lengthscale: 19.007   noise: 0.001\n",
-                        "Iter 218/500 - Loss: 0.361   lengthscale: 19.019   noise: 0.001\n",
-                        "Iter 219/500 - Loss: 0.361   lengthscale: 19.030   noise: 0.001\n",
-                        "Iter 220/500 - Loss: 0.361   lengthscale: 19.043   noise: 0.001\n",
-                        "Iter 221/500 - Loss: 0.360   lengthscale: 19.055   noise: 0.001\n",
-                        "Iter 222/500 - Loss: 0.360   lengthscale: 19.068   noise: 0.001\n",
-                        "Iter 223/500 - Loss: 0.360   lengthscale: 19.081   noise: 0.001\n",
-                        "Iter 224/500 - Loss: 0.360   lengthscale: 19.095   noise: 0.001\n",
-                        "Iter 225/500 - Loss: 0.360   lengthscale: 19.109   noise: 0.001\n",
-                        "Iter 226/500 - Loss: 0.360   lengthscale: 19.123   noise: 0.001\n",
-                        "Iter 227/500 - Loss: 0.360   lengthscale: 19.138   noise: 0.001\n",
-                        "Iter 228/500 - Loss: 0.360   lengthscale: 19.153   noise: 0.001\n",
-                        "Iter 229/500 - Loss: 0.360   lengthscale: 19.169   noise: 0.001\n",
-                        "Iter 230/500 - Loss: 0.360   lengthscale: 19.185   noise: 0.001\n",
-                        "Iter 231/500 - Loss: 0.360   lengthscale: 19.202   noise: 0.001\n",
-                        "Iter 232/500 - Loss: 0.360   lengthscale: 19.219   noise: 0.001\n",
-                        "Iter 233/500 - Loss: 0.360   lengthscale: 19.236   noise: 0.001\n",
-                        "Iter 234/500 - Loss: 0.360   lengthscale: 19.254   noise: 0.001\n",
-                        "Iter 235/500 - Loss: 0.360   lengthscale: 19.273   noise: 0.001\n",
-                        "Iter 236/500 - Loss: 0.360   lengthscale: 19.292   noise: 0.001\n",
-                        "Iter 237/500 - Loss: 0.360   lengthscale: 19.311   noise: 0.001\n",
-                        "Iter 238/500 - Loss: 0.359   lengthscale: 19.332   noise: 0.001\n",
-                        "Iter 239/500 - Loss: 0.359   lengthscale: 19.353   noise: 0.001\n",
-                        "Iter 240/500 - Loss: 0.359   lengthscale: 19.374   noise: 0.001\n",
-                        "Iter 241/500 - Loss: 0.359   lengthscale: 19.396   noise: 0.001\n",
-                        "Iter 242/500 - Loss: 0.359   lengthscale: 19.419   noise: 0.001\n",
-                        "Iter 243/500 - Loss: 0.359   lengthscale: 19.443   noise: 0.001\n",
-                        "Iter 244/500 - Loss: 0.359   lengthscale: 19.467   noise: 0.001\n",
-                        "Iter 245/500 - Loss: 0.359   lengthscale: 19.492   noise: 0.001\n",
-                        "Iter 246/500 - Loss: 0.359   lengthscale: 19.518   noise: 0.001\n",
-                        "Iter 247/500 - Loss: 0.358   lengthscale: 19.545   noise: 0.001\n",
-                        "Iter 248/500 - Loss: 0.358   lengthscale: 19.572   noise: 0.001\n",
-                        "Iter 249/500 - Loss: 0.358   lengthscale: 19.600   noise: 0.001\n",
-                        "Iter 250/500 - Loss: 0.358   lengthscale: 19.630   noise: 0.001\n",
-                        "Iter 251/500 - Loss: 0.358   lengthscale: 19.660   noise: 0.001\n",
-                        "Iter 252/500 - Loss: 0.358   lengthscale: 19.690   noise: 0.001\n",
-                        "Iter 253/500 - Loss: 0.358   lengthscale: 19.722   noise: 0.001\n",
-                        "Iter 254/500 - Loss: 0.357   lengthscale: 19.755   noise: 0.001\n",
-                        "Iter 255/500 - Loss: 0.357   lengthscale: 19.789   noise: 0.001\n",
-                        "Iter 256/500 - Loss: 0.357   lengthscale: 19.823   noise: 0.001\n",
-                        "Iter 257/500 - Loss: 0.357   lengthscale: 19.859   noise: 0.001\n",
-                        "Iter 258/500 - Loss: 0.357   lengthscale: 19.896   noise: 0.001\n",
-                        "Iter 259/500 - Loss: 0.357   lengthscale: 19.933   noise: 0.001\n",
-                        "Iter 260/500 - Loss: 0.356   lengthscale: 19.972   noise: 0.001\n",
-                        "Iter 261/500 - Loss: 0.356   lengthscale: 20.012   noise: 0.001\n",
-                        "Iter 262/500 - Loss: 0.356   lengthscale: 20.052   noise: 0.001\n",
-                        "Iter 263/500 - Loss: 0.356   lengthscale: 20.094   noise: 0.002\n",
-                        "Iter 264/500 - Loss: 0.356   lengthscale: 20.136   noise: 0.002\n",
-                        "Iter 265/500 - Loss: 0.355   lengthscale: 20.179   noise: 0.002\n",
-                        "Iter 266/500 - Loss: 0.355   lengthscale: 20.224   noise: 0.002\n",
-                        "Iter 267/500 - Loss: 0.355   lengthscale: 20.269   noise: 0.002\n",
-                        "Iter 268/500 - Loss: 0.355   lengthscale: 20.315   noise: 0.002\n",
-                        "Iter 269/500 - Loss: 0.355   lengthscale: 20.362   noise: 0.002\n",
-                        "Iter 270/500 - Loss: 0.354   lengthscale: 20.409   noise: 0.002\n",
-                        "Iter 271/500 - Loss: 0.354   lengthscale: 20.458   noise: 0.002\n",
-                        "Iter 272/500 - Loss: 0.354   lengthscale: 20.507   noise: 0.002\n",
-                        "Iter 273/500 - Loss: 0.354   lengthscale: 20.557   noise: 0.002\n",
-                        "Iter 274/500 - Loss: 0.354   lengthscale: 20.607   noise: 0.002\n",
-                        "Iter 275/500 - Loss: 0.353   lengthscale: 20.658   noise: 0.002\n",
-                        "Iter 276/500 - Loss: 0.353   lengthscale: 20.709   noise: 0.002\n",
-                        "Iter 277/500 - Loss: 0.353   lengthscale: 20.761   noise: 0.002\n",
-                        "Iter 278/500 - Loss: 0.353   lengthscale: 20.813   noise: 0.002\n",
-                        "Iter 279/500 - Loss: 0.353   lengthscale: 20.866   noise: 0.002\n",
-                        "Iter 280/500 - Loss: 0.352   lengthscale: 20.919   noise: 0.002\n",
-                        "Iter 281/500 - Loss: 0.352   lengthscale: 20.972   noise: 0.002\n",
-                        "Iter 282/500 - Loss: 0.352   lengthscale: 21.025   noise: 0.002\n",
-                        "Iter 283/500 - Loss: 0.352   lengthscale: 21.078   noise: 0.002\n",
-                        "Iter 284/500 - Loss: 0.352   lengthscale: 21.132   noise: 0.002\n",
-                        "Iter 285/500 - Loss: 0.352   lengthscale: 21.185   noise: 0.002\n",
-                        "Iter 286/500 - Loss: 0.351   lengthscale: 21.239   noise: 0.003\n",
-                        "Iter 287/500 - Loss: 0.351   lengthscale: 21.292   noise: 0.003\n",
-                        "Iter 288/500 - Loss: 0.351   lengthscale: 21.345   noise: 0.003\n",
-                        "Iter 289/500 - Loss: 0.351   lengthscale: 21.398   noise: 0.003\n",
-                        "Iter 290/500 - Loss: 0.351   lengthscale: 21.451   noise: 0.003\n",
-                        "Iter 291/500 - Loss: 0.350   lengthscale: 21.504   noise: 0.003\n",
-                        "Iter 292/500 - Loss: 0.350   lengthscale: 21.556   noise: 0.003\n",
-                        "Iter 293/500 - Loss: 0.350   lengthscale: 21.608   noise: 0.003\n",
-                        "Iter 294/500 - Loss: 0.350   lengthscale: 21.661   noise: 0.003\n",
-                        "Iter 295/500 - Loss: 0.350   lengthscale: 21.712   noise: 0.003\n",
-                        "Iter 296/500 - Loss: 0.350   lengthscale: 21.764   noise: 0.003\n",
-                        "Iter 297/500 - Loss: 0.349   lengthscale: 21.815   noise: 0.003\n",
-                        "Iter 298/500 - Loss: 0.349   lengthscale: 21.867   noise: 0.003\n",
-                        "Iter 299/500 - Loss: 0.349   lengthscale: 21.918   noise: 0.003\n",
-                        "Iter 300/500 - Loss: 0.349   lengthscale: 21.968   noise: 0.003\n",
-                        "Iter 301/500 - Loss: 0.349   lengthscale: 22.019   noise: 0.003\n",
-                        "Iter 302/500 - Loss: 0.349   lengthscale: 22.070   noise: 0.003\n",
-                        "Iter 303/500 - Loss: 0.348   lengthscale: 22.120   noise: 0.003\n",
-                        "Iter 304/500 - Loss: 0.348   lengthscale: 22.170   noise: 0.003\n",
-                        "Iter 305/500 - Loss: 0.348   lengthscale: 22.220   noise: 0.003\n",
-                        "Iter 306/500 - Loss: 0.348   lengthscale: 22.270   noise: 0.003\n",
-                        "Iter 307/500 - Loss: 0.348   lengthscale: 22.320   noise: 0.003\n",
-                        "Iter 308/500 - Loss: 0.348   lengthscale: 22.370   noise: 0.003\n",
-                        "Iter 309/500 - Loss: 0.347   lengthscale: 22.419   noise: 0.004\n",
-                        "Iter 310/500 - Loss: 0.347   lengthscale: 22.469   noise: 0.004\n",
-                        "Iter 311/500 - Loss: 0.347   lengthscale: 22.519   noise: 0.004\n",
-                        "Iter 312/500 - Loss: 0.347   lengthscale: 22.568   noise: 0.004\n",
-                        "Iter 313/500 - Loss: 0.347   lengthscale: 22.618   noise: 0.004\n",
-                        "Iter 314/500 - Loss: 0.347   lengthscale: 22.668   noise: 0.004\n",
-                        "Iter 315/500 - Loss: 0.347   lengthscale: 22.717   noise: 0.004\n",
-                        "Iter 316/500 - Loss: 0.346   lengthscale: 22.767   noise: 0.004\n",
-                        "Iter 317/500 - Loss: 0.346   lengthscale: 22.817   noise: 0.004\n",
-                        "Iter 318/500 - Loss: 0.346   lengthscale: 22.867   noise: 0.004\n",
-                        "Iter 319/500 - Loss: 0.346   lengthscale: 22.916   noise: 0.004\n",
-                        "Iter 320/500 - Loss: 0.346   lengthscale: 22.966   noise: 0.004\n",
-                        "Iter 321/500 - Loss: 0.346   lengthscale: 23.016   noise: 0.004\n",
-                        "Iter 322/500 - Loss: 0.346   lengthscale: 23.066   noise: 0.004\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Iter 323/500 - Loss: 0.345   lengthscale: 23.116   noise: 0.004\n",
-                        "Iter 324/500 - Loss: 0.345   lengthscale: 23.166   noise: 0.004\n",
-                        "Iter 325/500 - Loss: 0.345   lengthscale: 23.217   noise: 0.004\n",
-                        "Iter 326/500 - Loss: 0.345   lengthscale: 23.267   noise: 0.004\n",
-                        "Iter 327/500 - Loss: 0.345   lengthscale: 23.318   noise: 0.004\n",
-                        "Iter 328/500 - Loss: 0.345   lengthscale: 23.369   noise: 0.004\n",
-                        "Iter 329/500 - Loss: 0.344   lengthscale: 23.420   noise: 0.005\n",
-                        "Iter 330/500 - Loss: 0.344   lengthscale: 23.471   noise: 0.005\n",
-                        "Iter 331/500 - Loss: 0.344   lengthscale: 23.523   noise: 0.005\n",
-                        "Iter 332/500 - Loss: 0.344   lengthscale: 23.574   noise: 0.005\n",
-                        "Iter 333/500 - Loss: 0.344   lengthscale: 23.626   noise: 0.005\n",
-                        "Iter 334/500 - Loss: 0.344   lengthscale: 23.679   noise: 0.005\n",
-                        "Iter 335/500 - Loss: 0.343   lengthscale: 23.731   noise: 0.005\n",
-                        "Iter 336/500 - Loss: 0.343   lengthscale: 23.784   noise: 0.005\n",
-                        "Iter 337/500 - Loss: 0.343   lengthscale: 23.837   noise: 0.005\n",
-                        "Iter 338/500 - Loss: 0.343   lengthscale: 23.891   noise: 0.005\n",
-                        "Iter 339/500 - Loss: 0.343   lengthscale: 23.945   noise: 0.005\n",
-                        "Iter 340/500 - Loss: 0.343   lengthscale: 23.999   noise: 0.005\n",
-                        "Iter 341/500 - Loss: 0.342   lengthscale: 24.053   noise: 0.005\n",
-                        "Iter 342/500 - Loss: 0.342   lengthscale: 24.108   noise: 0.005\n",
-                        "Iter 343/500 - Loss: 0.342   lengthscale: 24.164   noise: 0.005\n",
-                        "Iter 344/500 - Loss: 0.342   lengthscale: 24.219   noise: 0.005\n",
-                        "Iter 345/500 - Loss: 0.342   lengthscale: 24.276   noise: 0.005\n",
-                        "Iter 346/500 - Loss: 0.341   lengthscale: 24.332   noise: 0.005\n",
-                        "Iter 347/500 - Loss: 0.341   lengthscale: 24.389   noise: 0.006\n",
-                        "Iter 348/500 - Loss: 0.341   lengthscale: 24.447   noise: 0.006\n",
-                        "Iter 349/500 - Loss: 0.341   lengthscale: 24.505   noise: 0.006\n",
-                        "Iter 350/500 - Loss: 0.341   lengthscale: 24.563   noise: 0.006\n",
-                        "Iter 351/500 - Loss: 0.340   lengthscale: 24.622   noise: 0.006\n",
-                        "Iter 352/500 - Loss: 0.340   lengthscale: 24.681   noise: 0.006\n",
-                        "Iter 353/500 - Loss: 0.340   lengthscale: 24.741   noise: 0.006\n",
-                        "Iter 354/500 - Loss: 0.340   lengthscale: 24.801   noise: 0.006\n",
-                        "Iter 355/500 - Loss: 0.340   lengthscale: 24.862   noise: 0.006\n",
-                        "Iter 356/500 - Loss: 0.339   lengthscale: 24.924   noise: 0.006\n",
-                        "Iter 357/500 - Loss: 0.339   lengthscale: 24.985   noise: 0.006\n",
-                        "Iter 358/500 - Loss: 0.339   lengthscale: 25.048   noise: 0.006\n",
-                        "Iter 359/500 - Loss: 0.339   lengthscale: 25.111   noise: 0.006\n",
-                        "Iter 360/500 - Loss: 0.338   lengthscale: 25.174   noise: 0.006\n",
-                        "Iter 361/500 - Loss: 0.338   lengthscale: 25.239   noise: 0.006\n",
-                        "Iter 362/500 - Loss: 0.338   lengthscale: 25.303   noise: 0.006\n",
-                        "Iter 363/500 - Loss: 0.338   lengthscale: 25.369   noise: 0.007\n",
-                        "Iter 364/500 - Loss: 0.337   lengthscale: 25.435   noise: 0.007\n",
-                        "Iter 365/500 - Loss: 0.337   lengthscale: 25.501   noise: 0.007\n",
-                        "Iter 366/500 - Loss: 0.337   lengthscale: 25.568   noise: 0.007\n",
-                        "Iter 367/500 - Loss: 0.337   lengthscale: 25.636   noise: 0.007\n",
-                        "Iter 368/500 - Loss: 0.336   lengthscale: 25.704   noise: 0.007\n",
-                        "Iter 369/500 - Loss: 0.336   lengthscale: 25.773   noise: 0.007\n",
-                        "Iter 370/500 - Loss: 0.336   lengthscale: 25.842   noise: 0.007\n",
-                        "Iter 371/500 - Loss: 0.335   lengthscale: 25.913   noise: 0.007\n",
-                        "Iter 372/500 - Loss: 0.335   lengthscale: 25.983   noise: 0.007\n",
-                        "Iter 373/500 - Loss: 0.335   lengthscale: 26.055   noise: 0.007\n",
-                        "Iter 374/500 - Loss: 0.335   lengthscale: 26.127   noise: 0.007\n",
-                        "Iter 375/500 - Loss: 0.334   lengthscale: 26.199   noise: 0.007\n",
-                        "Iter 376/500 - Loss: 0.334   lengthscale: 26.273   noise: 0.007\n",
-                        "Iter 377/500 - Loss: 0.334   lengthscale: 26.347   noise: 0.007\n",
-                        "Iter 378/500 - Loss: 0.333   lengthscale: 26.421   noise: 0.008\n",
-                        "Iter 379/500 - Loss: 0.333   lengthscale: 26.496   noise: 0.008\n",
-                        "Iter 380/500 - Loss: 0.333   lengthscale: 26.572   noise: 0.008\n",
-                        "Iter 381/500 - Loss: 0.332   lengthscale: 26.649   noise: 0.008\n",
-                        "Iter 382/500 - Loss: 0.332   lengthscale: 26.726   noise: 0.008\n",
-                        "Iter 383/500 - Loss: 0.332   lengthscale: 26.804   noise: 0.008\n",
-                        "Iter 384/500 - Loss: 0.331   lengthscale: 26.882   noise: 0.008\n",
-                        "Iter 385/500 - Loss: 0.331   lengthscale: 26.961   noise: 0.008\n",
-                        "Iter 386/500 - Loss: 0.331   lengthscale: 27.041   noise: 0.008\n",
-                        "Iter 387/500 - Loss: 0.330   lengthscale: 27.121   noise: 0.008\n",
-                        "Iter 388/500 - Loss: 0.330   lengthscale: 27.202   noise: 0.008\n",
-                        "Iter 389/500 - Loss: 0.330   lengthscale: 27.284   noise: 0.008\n",
-                        "Iter 390/500 - Loss: 0.329   lengthscale: 27.366   noise: 0.008\n",
-                        "Iter 391/500 - Loss: 0.329   lengthscale: 27.449   noise: 0.008\n",
-                        "Iter 392/500 - Loss: 0.328   lengthscale: 27.532   noise: 0.008\n",
-                        "Iter 393/500 - Loss: 0.328   lengthscale: 27.616   noise: 0.009\n",
-                        "Iter 394/500 - Loss: 0.328   lengthscale: 27.701   noise: 0.009\n",
-                        "Iter 395/500 - Loss: 0.327   lengthscale: 27.786   noise: 0.009\n",
-                        "Iter 396/500 - Loss: 0.327   lengthscale: 27.872   noise: 0.009\n",
-                        "Iter 397/500 - Loss: 0.326   lengthscale: 27.959   noise: 0.009\n",
-                        "Iter 398/500 - Loss: 0.326   lengthscale: 28.046   noise: 0.009\n",
-                        "Iter 399/500 - Loss: 0.326   lengthscale: 28.133   noise: 0.009\n",
-                        "Iter 400/500 - Loss: 0.325   lengthscale: 28.222   noise: 0.009\n",
-                        "Iter 401/500 - Loss: 0.325   lengthscale: 28.311   noise: 0.009\n",
-                        "Iter 402/500 - Loss: 0.324   lengthscale: 28.400   noise: 0.009\n",
-                        "Iter 403/500 - Loss: 0.324   lengthscale: 28.490   noise: 0.009\n",
-                        "Iter 404/500 - Loss: 0.323   lengthscale: 28.580   noise: 0.009\n",
-                        "Iter 405/500 - Loss: 0.323   lengthscale: 28.672   noise: 0.009\n",
-                        "Iter 406/500 - Loss: 0.323   lengthscale: 28.763   noise: 0.009\n",
-                        "Iter 407/500 - Loss: 0.322   lengthscale: 28.855   noise: 0.009\n",
-                        "Iter 408/500 - Loss: 0.322   lengthscale: 28.948   noise: 0.010\n",
-                        "Iter 409/500 - Loss: 0.321   lengthscale: 29.041   noise: 0.010\n",
-                        "Iter 410/500 - Loss: 0.321   lengthscale: 29.135   noise: 0.010\n",
-                        "Iter 411/500 - Loss: 0.320   lengthscale: 29.229   noise: 0.010\n",
-                        "Iter 412/500 - Loss: 0.320   lengthscale: 29.324   noise: 0.010\n",
-                        "Iter 413/500 - Loss: 0.319   lengthscale: 29.419   noise: 0.010\n",
-                        "Iter 414/500 - Loss: 0.319   lengthscale: 29.515   noise: 0.010\n",
-                        "Iter 415/500 - Loss: 0.318   lengthscale: 29.611   noise: 0.010\n",
-                        "Iter 416/500 - Loss: 0.318   lengthscale: 29.708   noise: 0.010\n",
-                        "Iter 417/500 - Loss: 0.317   lengthscale: 29.805   noise: 0.010\n",
-                        "Iter 418/500 - Loss: 0.317   lengthscale: 29.903   noise: 0.010\n",
-                        "Iter 419/500 - Loss: 0.316   lengthscale: 30.001   noise: 0.010\n",
-                        "Iter 420/500 - Loss: 0.316   lengthscale: 30.099   noise: 0.010\n",
-                        "Iter 421/500 - Loss: 0.315   lengthscale: 30.198   noise: 0.010\n",
-                        "Iter 422/500 - Loss: 0.315   lengthscale: 30.297   noise: 0.010\n",
-                        "Iter 423/500 - Loss: 0.314   lengthscale: 30.397   noise: 0.010\n",
-                        "Iter 424/500 - Loss: 0.314   lengthscale: 30.497   noise: 0.010\n",
-                        "Iter 425/500 - Loss: 0.313   lengthscale: 30.598   noise: 0.011\n",
-                        "Iter 426/500 - Loss: 0.313   lengthscale: 30.699   noise: 0.011\n",
-                        "Iter 427/500 - Loss: 0.312   lengthscale: 30.800   noise: 0.011\n",
-                        "Iter 428/500 - Loss: 0.312   lengthscale: 30.901   noise: 0.011\n",
-                        "Iter 429/500 - Loss: 0.311   lengthscale: 31.003   noise: 0.011\n",
-                        "Iter 430/500 - Loss: 0.311   lengthscale: 31.106   noise: 0.011\n",
-                        "Iter 431/500 - Loss: 0.310   lengthscale: 31.209   noise: 0.011\n",
-                        "Iter 432/500 - Loss: 0.310   lengthscale: 31.312   noise: 0.011\n",
-                        "Iter 433/500 - Loss: 0.309   lengthscale: 31.415   noise: 0.011\n",
-                        "Iter 434/500 - Loss: 0.309   lengthscale: 31.519   noise: 0.011\n",
-                        "Iter 435/500 - Loss: 0.308   lengthscale: 31.623   noise: 0.011\n",
-                        "Iter 436/500 - Loss: 0.308   lengthscale: 31.727   noise: 0.011\n",
-                        "Iter 437/500 - Loss: 0.307   lengthscale: 31.832   noise: 0.011\n",
-                        "Iter 438/500 - Loss: 0.306   lengthscale: 31.936   noise: 0.011\n",
-                        "Iter 439/500 - Loss: 0.306   lengthscale: 32.042   noise: 0.011\n",
-                        "Iter 440/500 - Loss: 0.305   lengthscale: 32.147   noise: 0.011\n",
-                        "Iter 441/500 - Loss: 0.305   lengthscale: 32.253   noise: 0.011\n",
-                        "Iter 442/500 - Loss: 0.304   lengthscale: 32.359   noise: 0.011\n",
-                        "Iter 443/500 - Loss: 0.304   lengthscale: 32.465   noise: 0.011\n",
-                        "Iter 444/500 - Loss: 0.303   lengthscale: 32.571   noise: 0.012\n",
-                        "Iter 445/500 - Loss: 0.303   lengthscale: 32.678   noise: 0.012\n",
-                        "Iter 446/500 - Loss: 0.302   lengthscale: 32.785   noise: 0.012\n",
-                        "Iter 447/500 - Loss: 0.301   lengthscale: 32.892   noise: 0.012\n",
-                        "Iter 448/500 - Loss: 0.301   lengthscale: 32.999   noise: 0.012\n",
-                        "Iter 449/500 - Loss: 0.300   lengthscale: 33.106   noise: 0.012\n",
-                        "Iter 450/500 - Loss: 0.300   lengthscale: 33.214   noise: 0.012\n",
-                        "Iter 451/500 - Loss: 0.299   lengthscale: 33.322   noise: 0.012\n",
-                        "Iter 452/500 - Loss: 0.299   lengthscale: 33.430   noise: 0.012\n",
-                        "Iter 453/500 - Loss: 0.298   lengthscale: 33.538   noise: 0.012\n",
-                        "Iter 454/500 - Loss: 0.298   lengthscale: 33.646   noise: 0.012\n",
-                        "Iter 455/500 - Loss: 0.297   lengthscale: 33.755   noise: 0.012\n",
-                        "Iter 456/500 - Loss: 0.296   lengthscale: 33.863   noise: 0.012\n",
-                        "Iter 457/500 - Loss: 0.296   lengthscale: 33.972   noise: 0.012\n",
-                        "Iter 458/500 - Loss: 0.295   lengthscale: 34.081   noise: 0.012\n",
-                        "Iter 459/500 - Loss: 0.295   lengthscale: 34.190   noise: 0.012\n",
-                        "Iter 460/500 - Loss: 0.294   lengthscale: 34.299   noise: 0.012\n",
-                        "Iter 461/500 - Loss: 0.294   lengthscale: 34.408   noise: 0.012\n",
-                        "Iter 462/500 - Loss: 0.293   lengthscale: 34.517   noise: 0.012\n",
-                        "Iter 463/500 - Loss: 0.292   lengthscale: 34.626   noise: 0.012\n",
-                        "Iter 464/500 - Loss: 0.292   lengthscale: 34.736   noise: 0.012\n",
-                        "Iter 465/500 - Loss: 0.291   lengthscale: 34.845   noise: 0.012\n",
-                        "Iter 466/500 - Loss: 0.291   lengthscale: 34.955   noise: 0.012\n",
-                        "Iter 467/500 - Loss: 0.290   lengthscale: 35.064   noise: 0.012\n",
-                        "Iter 468/500 - Loss: 0.290   lengthscale: 35.174   noise: 0.012\n",
-                        "Iter 469/500 - Loss: 0.289   lengthscale: 35.284   noise: 0.013\n"
-                    ]
-                },
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Iter 470/500 - Loss: 0.289   lengthscale: 35.394   noise: 0.013\n",
-                        "Iter 471/500 - Loss: 0.288   lengthscale: 35.503   noise: 0.013\n",
-                        "Iter 472/500 - Loss: 0.287   lengthscale: 35.613   noise: 0.013\n",
-                        "Iter 473/500 - Loss: 0.287   lengthscale: 35.723   noise: 0.013\n",
-                        "Iter 474/500 - Loss: 0.286   lengthscale: 35.833   noise: 0.013\n",
-                        "Iter 475/500 - Loss: 0.286   lengthscale: 35.943   noise: 0.013\n",
-                        "Iter 476/500 - Loss: 0.285   lengthscale: 36.052   noise: 0.013\n",
-                        "Iter 477/500 - Loss: 0.285   lengthscale: 36.162   noise: 0.013\n",
-                        "Iter 478/500 - Loss: 0.284   lengthscale: 36.272   noise: 0.013\n",
-                        "Iter 479/500 - Loss: 0.284   lengthscale: 36.382   noise: 0.013\n",
-                        "Iter 480/500 - Loss: 0.283   lengthscale: 36.491   noise: 0.013\n",
-                        "Iter 481/500 - Loss: 0.282   lengthscale: 36.601   noise: 0.013\n",
-                        "Iter 482/500 - Loss: 0.282   lengthscale: 36.711   noise: 0.013\n",
-                        "Iter 483/500 - Loss: 0.281   lengthscale: 36.821   noise: 0.013\n",
-                        "Iter 484/500 - Loss: 0.281   lengthscale: 36.930   noise: 0.013\n",
-                        "Iter 485/500 - Loss: 0.280   lengthscale: 37.040   noise: 0.013\n",
-                        "Iter 486/500 - Loss: 0.280   lengthscale: 37.149   noise: 0.013\n",
-                        "Iter 487/500 - Loss: 0.279   lengthscale: 37.259   noise: 0.013\n",
-                        "Iter 488/500 - Loss: 0.279   lengthscale: 37.368   noise: 0.013\n",
-                        "Iter 489/500 - Loss: 0.278   lengthscale: 37.477   noise: 0.013\n",
-                        "Iter 490/500 - Loss: 0.278   lengthscale: 37.586   noise: 0.013\n",
-                        "Iter 491/500 - Loss: 0.277   lengthscale: 37.695   noise: 0.013\n",
-                        "Iter 492/500 - Loss: 0.276   lengthscale: 37.804   noise: 0.013\n",
-                        "Iter 493/500 - Loss: 0.276   lengthscale: 37.913   noise: 0.013\n",
-                        "Iter 494/500 - Loss: 0.275   lengthscale: 38.022   noise: 0.013\n",
-                        "Iter 495/500 - Loss: 0.275   lengthscale: 38.131   noise: 0.013\n",
-                        "Iter 496/500 - Loss: 0.274   lengthscale: 38.239   noise: 0.013\n",
-                        "Iter 497/500 - Loss: 0.274   lengthscale: 38.348   noise: 0.013\n",
-                        "Iter 498/500 - Loss: 0.273   lengthscale: 38.456   noise: 0.013\n",
-                        "Iter 499/500 - Loss: 0.273   lengthscale: 38.564   noise: 0.013\n",
-                        "Iter 500/500 - Loss: 0.272   lengthscale: 38.672   noise: 0.013\n"
+                        "Iter 1/100 - Loss: 128.629   lengthscales: 0.693, 0.693   noise: 0.693\n",
+                        "Iter 2/100 - Loss: 127.182   lengthscales: 0.668, 0.668   noise: 0.668\n",
+                        "Iter 3/100 - Loss: 125.838   lengthscales: 0.644, 0.645   noise: 0.644\n",
+                        "Iter 4/100 - Loss: 123.982   lengthscales: 0.624, 0.621   noise: 0.621\n",
+                        "Iter 5/100 - Loss: 122.799   lengthscales: 0.604, 0.598   noise: 0.598\n",
+                        "Iter 6/100 - Loss: 120.909   lengthscales: 0.583, 0.576   noise: 0.576\n",
+                        "Iter 7/100 - Loss: 119.255   lengthscales: 0.562, 0.555   noise: 0.554\n",
+                        "Iter 8/100 - Loss: 117.506   lengthscales: 0.542, 0.534   noise: 0.533\n",
+                        "Iter 9/100 - Loss: 116.083   lengthscales: 0.522, 0.513   noise: 0.513\n",
+                        "Iter 10/100 - Loss: 113.978   lengthscales: 0.502, 0.493   noise: 0.493\n",
+                        "Iter 11/100 - Loss: 112.242   lengthscales: 0.482, 0.474   noise: 0.473\n",
+                        "Iter 12/100 - Loss: 110.389   lengthscales: 0.463, 0.455   noise: 0.455\n",
+                        "Iter 13/100 - Loss: 108.644   lengthscales: 0.444, 0.436   noise: 0.436\n",
+                        "Iter 14/100 - Loss: 107.660   lengthscales: 0.426, 0.418   noise: 0.419\n",
+                        "Iter 15/100 - Loss: 104.480   lengthscales: 0.408, 0.402   noise: 0.401\n",
+                        "Iter 16/100 - Loss: 103.058   lengthscales: 0.391, 0.387   noise: 0.385\n",
+                        "Iter 17/100 - Loss: 101.174   lengthscales: 0.374, 0.373   noise: 0.369\n",
+                        "Iter 18/100 - Loss: 98.379   lengthscales: 0.358, 0.361   noise: 0.353\n",
+                        "Iter 19/100 - Loss: 96.482   lengthscales: 0.343, 0.352   noise: 0.338\n",
+                        "Iter 20/100 - Loss: 95.282   lengthscales: 0.327, 0.344   noise: 0.323\n",
+                        "Iter 21/100 - Loss: 92.911   lengthscales: 0.313, 0.339   noise: 0.309\n",
+                        "Iter 22/100 - Loss: 89.532   lengthscales: 0.300, 0.335   noise: 0.295\n",
+                        "Iter 23/100 - Loss: 89.324   lengthscales: 0.288, 0.332   noise: 0.282\n",
+                        "Iter 24/100 - Loss: 86.490   lengthscales: 0.279, 0.329   noise: 0.269\n",
+                        "Iter 25/100 - Loss: 85.546   lengthscales: 0.272, 0.328   noise: 0.257\n",
+                        "Iter 26/100 - Loss: 83.578   lengthscales: 0.268, 0.327   noise: 0.245\n",
+                        "Iter 27/100 - Loss: 81.732   lengthscales: 0.265, 0.326   noise: 0.234\n",
+                        "Iter 28/100 - Loss: 79.472   lengthscales: 0.265, 0.326   noise: 0.223\n",
+                        "Iter 29/100 - Loss: 77.669   lengthscales: 0.267, 0.327   noise: 0.212\n",
+                        "Iter 30/100 - Loss: 75.215   lengthscales: 0.269, 0.329   noise: 0.202\n",
+                        "Iter 31/100 - Loss: 73.676   lengthscales: 0.272, 0.329   noise: 0.193\n",
+                        "Iter 32/100 - Loss: 70.514   lengthscales: 0.276, 0.328   noise: 0.183\n",
+                        "Iter 33/100 - Loss: 69.765   lengthscales: 0.280, 0.325   noise: 0.175\n",
+                        "Iter 34/100 - Loss: 68.525   lengthscales: 0.284, 0.320   noise: 0.166\n",
+                        "Iter 35/100 - Loss: 66.181   lengthscales: 0.287, 0.314   noise: 0.158\n",
+                        "Iter 36/100 - Loss: 62.446   lengthscales: 0.288, 0.307   noise: 0.150\n",
+                        "Iter 37/100 - Loss: 62.009   lengthscales: 0.287, 0.299   noise: 0.143\n",
+                        "Iter 38/100 - Loss: 58.204   lengthscales: 0.284, 0.290   noise: 0.136\n",
+                        "Iter 39/100 - Loss: 57.167   lengthscales: 0.280, 0.281   noise: 0.130\n",
+                        "Iter 40/100 - Loss: 54.072   lengthscales: 0.274, 0.271   noise: 0.123\n",
+                        "Iter 41/100 - Loss: 51.696   lengthscales: 0.268, 0.261   noise: 0.117\n",
+                        "Iter 42/100 - Loss: 49.792   lengthscales: 0.261, 0.253   noise: 0.111\n",
+                        "Iter 43/100 - Loss: 46.250   lengthscales: 0.255, 0.246   noise: 0.106\n",
+                        "Iter 44/100 - Loss: 47.110   lengthscales: 0.250, 0.241   noise: 0.101\n",
+                        "Iter 45/100 - Loss: 45.541   lengthscales: 0.248, 0.237   noise: 0.096\n",
+                        "Iter 46/100 - Loss: 41.711   lengthscales: 0.246, 0.237   noise: 0.091\n",
+                        "Iter 47/100 - Loss: 40.852   lengthscales: 0.245, 0.237   noise: 0.086\n",
+                        "Iter 48/100 - Loss: 39.588   lengthscales: 0.244, 0.239   noise: 0.082\n",
+                        "Iter 49/100 - Loss: 36.817   lengthscales: 0.244, 0.241   noise: 0.078\n",
+                        "Iter 50/100 - Loss: 34.773   lengthscales: 0.244, 0.244   noise: 0.074\n",
+                        "Iter 51/100 - Loss: 31.050   lengthscales: 0.243, 0.247   noise: 0.070\n",
+                        "Iter 52/100 - Loss: 28.448   lengthscales: 0.242, 0.248   noise: 0.067\n",
+                        "Iter 53/100 - Loss: 29.796   lengthscales: 0.241, 0.246   noise: 0.063\n",
+                        "Iter 54/100 - Loss: 25.501   lengthscales: 0.239, 0.243   noise: 0.060\n",
+                        "Iter 55/100 - Loss: 28.542   lengthscales: 0.237, 0.238   noise: 0.057\n",
+                        "Iter 56/100 - Loss: 23.089   lengthscales: 0.236, 0.231   noise: 0.054\n",
+                        "Iter 57/100 - Loss: 19.792   lengthscales: 0.235, 0.225   noise: 0.051\n",
+                        "Iter 58/100 - Loss: 20.285   lengthscales: 0.235, 0.219   noise: 0.049\n",
+                        "Iter 59/100 - Loss: 16.047   lengthscales: 0.234, 0.214   noise: 0.046\n",
+                        "Iter 60/100 - Loss: 15.160   lengthscales: 0.234, 0.211   noise: 0.044\n",
+                        "Iter 61/100 - Loss: 13.038   lengthscales: 0.232, 0.209   noise: 0.042\n",
+                        "Iter 62/100 - Loss: 13.928   lengthscales: 0.230, 0.209   noise: 0.040\n",
+                        "Iter 63/100 - Loss: 9.312   lengthscales: 0.227, 0.210   noise: 0.038\n",
+                        "Iter 64/100 - Loss: 7.950   lengthscales: 0.223, 0.212   noise: 0.036\n",
+                        "Iter 65/100 - Loss: 3.461   lengthscales: 0.220, 0.215   noise: 0.034\n",
+                        "Iter 66/100 - Loss: 5.609   lengthscales: 0.217, 0.217   noise: 0.033\n",
+                        "Iter 67/100 - Loss: 2.204   lengthscales: 0.214, 0.218   noise: 0.031\n",
+                        "Iter 68/100 - Loss: 0.597   lengthscales: 0.212, 0.219   noise: 0.029\n",
+                        "Iter 69/100 - Loss: -1.111   lengthscales: 0.211, 0.217   noise: 0.028\n",
+                        "Iter 70/100 - Loss: -2.389   lengthscales: 0.209, 0.214   noise: 0.027\n",
+                        "Iter 71/100 - Loss: -3.256   lengthscales: 0.208, 0.210   noise: 0.025\n",
+                        "Iter 72/100 - Loss: -4.180   lengthscales: 0.209, 0.207   noise: 0.024\n",
+                        "Iter 73/100 - Loss: -6.345   lengthscales: 0.209, 0.205   noise: 0.023\n",
+                        "Iter 74/100 - Loss: -10.216   lengthscales: 0.210, 0.204   noise: 0.022\n",
+                        "Iter 75/100 - Loss: -11.749   lengthscales: 0.209, 0.204   noise: 0.021\n",
+                        "Iter 76/100 - Loss: -10.651   lengthscales: 0.208, 0.204   noise: 0.020\n",
+                        "Iter 77/100 - Loss: -12.092   lengthscales: 0.207, 0.205   noise: 0.019\n",
+                        "Iter 78/100 - Loss: -14.908   lengthscales: 0.204, 0.206   noise: 0.018\n",
+                        "Iter 79/100 - Loss: -16.482   lengthscales: 0.202, 0.208   noise: 0.017\n",
+                        "Iter 80/100 - Loss: -17.962   lengthscales: 0.199, 0.207   noise: 0.016\n",
+                        "Iter 81/100 - Loss: -23.044   lengthscales: 0.198, 0.207   noise: 0.016\n",
+                        "Iter 82/100 - Loss: -20.867   lengthscales: 0.196, 0.205   noise: 0.015\n",
+                        "Iter 83/100 - Loss: -20.908   lengthscales: 0.195, 0.203   noise: 0.014\n",
+                        "Iter 84/100 - Loss: -25.210   lengthscales: 0.193, 0.201   noise: 0.013\n",
+                        "Iter 85/100 - Loss: -24.521   lengthscales: 0.193, 0.199   noise: 0.013\n",
+                        "Iter 86/100 - Loss: -25.571   lengthscales: 0.193, 0.199   noise: 0.012\n",
+                        "Iter 87/100 - Loss: -26.477   lengthscales: 0.194, 0.199   noise: 0.012\n",
+                        "Iter 88/100 - Loss: -26.940   lengthscales: 0.195, 0.200   noise: 0.011\n",
+                        "Iter 89/100 - Loss: -27.446   lengthscales: 0.196, 0.199   noise: 0.011\n",
+                        "Iter 90/100 - Loss: -30.484   lengthscales: 0.196, 0.198   noise: 0.010\n",
+                        "Iter 91/100 - Loss: -29.450   lengthscales: 0.194, 0.196   noise: 0.010\n",
+                        "Iter 92/100 - Loss: -28.761   lengthscales: 0.192, 0.198   noise: 0.009\n",
+                        "Iter 93/100 - Loss: -34.818   lengthscales: 0.189, 0.200   noise: 0.009\n",
+                        "Iter 94/100 - Loss: -39.531   lengthscales: 0.186, 0.203   noise: 0.009\n",
+                        "Iter 95/100 - Loss: -38.291   lengthscales: 0.184, 0.202   noise: 0.008\n",
+                        "Iter 96/100 - Loss: -38.961   lengthscales: 0.182, 0.200   noise: 0.008\n",
+                        "Iter 97/100 - Loss: -41.103   lengthscales: 0.180, 0.197   noise: 0.007\n",
+                        "Iter 98/100 - Loss: -42.563   lengthscales: 0.179, 0.194   noise: 0.007\n",
+                        "Iter 99/100 - Loss: -42.571   lengthscales: 0.179, 0.191   noise: 0.007\n",
+                        "Iter 100/100 - Loss: -37.692   lengthscales: 0.179, 0.191   noise: 0.007\n"
                     ]
                 }
             ],
             "source": [
                 "# this is for running the notebook in our testing framework\n",
                 "import os\n",
                 "smoke_test = ('CI' in os.environ)\n",
-                "training_iter = 2 if smoke_test else 500\n",
+                "training_iter = 2 if smoke_test else 50\n",
                 "\n",
                 "\n",
                 "# Find optimal model hyperparameters\n",
                 "model.train()\n",
                 "likelihood.train()\n",
                 "\n",
                 "# Use the adam optimizer\n",
-                "optimizer = torch.optim.Adam(model.parameters(), lr=0.25)  # Includes GaussianLikelihood parameters\n",
+                "optimizer = torch.optim.Adam(model.parameters(), lr=0.05)  # Includes GaussianLikelihood parameters\n",
                 "\n",
                 "# \"Loss\" for GPs - the marginal log likelihood\n",
                 "mll = gpytorch.mlls.ExactMarginalLogLikelihood(likelihood, model)\n",
                 "\n",
                 "for i in range(training_iter):\n",
-                "    # Zero gradients from previous iteration\n",
                 "    optimizer.zero_grad()\n",
-                "    # Output from model\n",
-                "    output = model(train_x_distributional)\n",
-                "    # Calc loss and backprop gradients\n",
+                "    output = model(train_x)\n",
                 "    loss = -mll(output, train_y)\n",
                 "    loss.backward()\n",
-                "    print('Iter %d/%d - Loss: %.3f   lengthscale: %.3f   noise: %.3f' % (\n",
+                "    print(\"Iter %d/%d - Loss: %.3f   lengthscales: %.3f, %.3f   noise: %.3f\" % (\n",
                 "        i + 1, training_iter, loss.item(),\n",
-                "        model.covar_module.base_kernel.lengthscale.item(),\n",
+                "        model.covar_module.base_kernel.lengthscale.squeeze()[0],\n",
+                "        model.covar_module.base_kernel.lengthscale.squeeze()[1],\n",
                 "        model.likelihood.noise.item()\n",
                 "    ))\n",
                 "    optimizer.step()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now, we test predictions. For simplicity, we will assume a fixed variance of $0.01.$"
+                "Model predictions are also similar to GP regression with only function values, but we need more CG iterations to get accurate estimates of the predictive variance"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAeIAAADGCAYAAAAOo4M3AAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADh0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uMy4xLjMsIGh0dHA6Ly9tYXRwbG90bGliLm9yZy+AADFEAAAgAElEQVR4nO3deXic1Xnw/++ZfR/tsmTZeJO8yFjyisEGm50QFxogL/A2hJC2FAiUtCW/NCWJSRPStKUhbQOkNKHZCDgQUgiBF0zAgAETL9jGNt4ty7Jl7RrNvp7fHyML20iyLI00I+n+XNdzzfbMM2ceaeaes91Haa0RQgghRHYYsl0AIYQQYjyTQCyEEEJkkQRiIYQQIoskEAshhBBZJIFYCCGEyCIJxEIIIUQWDTkQK6VsSqk/KqW2KaV2KqW+lYmCCSGEEOOBGuo8YqWUApxa64BSygysB+7VWm/IRAGFEEKIscw01APodCQPdN80d2+SJUQIIYQYgIz0ESuljEqprUAzsFZr/X4mjiuEEEKMdUOuEQNorZNArVIqD/itUmqu1nrHyfsopW4HbgdwOp0LZ82alYmXFkIIIXLe5s2bW7XWxb09NuQ+4k8cUKnVQFBr/VBf+yxatEhv2rQpo68rhBBC5Cql1Gat9aLeHsvEqOni7powSik7cBmwe6jHFUIIIcaDTDRNlwE/U0oZSQf2X2utX8zAcYUQQogxLxOjprcD8zNQFiGEEGLcychgLSGEEJkVj8dpaGggEolkuyjiLNhsNioqKjCbzQN+jgRiIYTIQQ0NDbjdbqZMmUI6b5LIdVpr2traaGhoYOrUqQN+nuSaFkKIHBSJRCgsLJQgPIoopSgsLDzrVgwJxEIIkaMkCI8+g/mbSSAWQgjRq4aGBq699loqKyuZPn069957L7FYDICf/vSn3H333Vku4Se5XK5e7zcajdTW1lJdXU1NTQ3f//73SaVS/R6rrq6OX/3qV8NRzFNIIBZCCPEJWmuuu+46/vRP/5R9+/axd+9eAoEA999//7C9ZiKRGLZj2+12tm7dys6dO1m7di0vvfQS3/pW/4sFSiAWQgiRNa+//jo2m43bbrsNSNcoH374YZ544glCoRAAR44c4aqrrmLmzJk9QS0YDPLpT3+ampoa5s6dy5o1awDYvHkzK1asYOHChVx55ZU0NjYCsHLlSv7hH/6BFStW8OCDDzJlypSemmooFGLSpEnE43EOHDjAVVddxcKFC7nwwgvZvTudN+rQoUOcf/75LF68mG984xsDem8lJSU8/vjj/PCHP0RrTV1dHRdeeCELFixgwYIFvPvuuwD8/d//PW+//Ta1tbU8/PDDfe43VDJqWgghctyXvwxbt2b2mLW18IMf9P34zp07Wbhw4Sn3eTweJk+ezP79+wH44x//yI4dO3A4HCxevJhPf/rTHD58mPLycn7/+98D4PP5iMfj3HPPPTz//PMUFxezZs0a7r//fp544gkAOjs7efPNNwHYsmULb775JhdffDG/+93vuPLKKzGbzdx+++386Ec/orKykvfff5+77rqL119/nXvvvZc777yTz3/+8zzyyCMDfv/Tpk0jlUrR3NxMSUkJa9euxWazsW/fPm6++WY2bdrE9773PR566CFefDGdoyoUCvW631BJIBZCCPEJWuteBx6dfP/ll19OYWEhANdddx3r16/n6quv5r777uOrX/0qq1at4sILL2THjh3s2LGDyy+/HIBkMklZWVnPMW+88cZTrq9Zs4aLL76Yp59+mrvuuotAIMC7777LZz/72Z79otEoAO+88w6/+c1vALjlllv46le/elbvEdJztu+++262bt2K0Whk7969ve4/0P3OlgRiIYTIcf3VXIdLdXV1T4A7oauriyNHjjB9+nQ2b978iUCtlKKqqorNmzfz0ksv8bWvfY0rrriCz3zmM1RXV/Pee+/1+lpOp7Pn+jXXXMPXvvY12tvb2bx5M5dccgnBYJC8vDy29tEsMJiRygcPHsRoNFJSUsK3vvUtSktL2bZtG6lUCpvN1utzHn744QHtd7akj1gIIcQnXHrppYRCIX7+858D6Vrs3/3d3/GFL3wBh8MBwNq1a2lvbyccDvO///u/LFu2jGPHjuFwOPjc5z7Hfffdx5YtW5g5cyYtLS09gTgej7Nz585eX9flcrFkyRLuvfdeVq1ahdFoxOPxMHXqVJ555hkgXZPdtm0bAMuWLePpp58G4MknnxzQe2tpaeGOO+7g7rvvRimFz+ejrKwMg8HAL37xC5LJJAButxu/39/zvL72GyoJxEIIIT5BKcVvf/tbnnnmGSorK6mqqsJms/Hd7363Z5/ly5dzyy23UFtby/XXX8+iRYv48MMPWbJkCbW1tTz44IN8/etfx2Kx8Oyzz/LVr36Vmpoaamtr+x3odOONN/LLX/7ylCbrJ598kp/85CfU1NRQXV3N888/D8C///u/88gjj7B48WJ8Pl+fxwyHwz3Tly677DKuuOIKVq9eDcBdd93Fz372M5YuXcrevXt7aujz5s3DZDJRU1PDww8/3Od+Q5Xx9YgHQtYjFkKI/n300UfMnj0728UQg9Db325Y1yMWQgghxOBJIBZCCCGySAKxEEIIkUUSiIUQQogskkAshBBCZNGQA7FSapJS6g2l1EdKqZ1KqXszUTAhhBBiPMhEjTgB/J3WejawFPiSUmpOBo4rhBAii5RS3HLLLT23E4kExcXFrFq1KoulGnuGnOJSa90INHZf9yulPgImAruGemwhhBBpD6/NTF7jE/7m8qoz7uN0OtmxYwfhcBi73c7atWuZOHFiRsshMtxHrJSaAswH3s/kcYUQQmTHpz71qZ6VlJ566iluvvnmnseCwSBf/OIXWbx4MfPnz+/JdtXXcoHr1q1j5cqV3HDDDcyaNYs/+7M/IxtJpXJNxgKxUsoF/Ab4sta6q5fHb1dKbVJKbWppacnUywohhBhGN910E08//TSRSITt27dz3nnn9Tz24IMPcskll7Bx40beeOMNvvKVrxAMBnuWFdyyZQtr1qzhr//6r3ue88EHH/CDH/yAXbt2cfDgQd55551svK2ckpHVl5RSZtJB+Emt9XO97aO1fhx4HNIpLjPxukIIIYbXvHnzqKur46mnnuLqq68+5bFXX32VF154gYceegiASCRCfX095eXlfS4XuGTJEioqKgCora2lrq6O5cuXj9wbykFDDsQqvf7UT4CPtNbfH3qRhBBC5JJrrrmG++67j3Xr1tHW1tZzv9aa3/zmN8ycOfOU/R944IE+lwu0Wq09141GI4lEYvjfQI7LRNP0MuAW4BKl1Nbu7eozPUkIIcTo8MUvfpFvfvObnHvuuafcf+WVV/Kf//mfPf28H3zwATB8ywWOVUMOxFrr9VprpbWep7Wu7d5eykThhBBCZF9FRQX33vvJFBHf+MY3iMfjzJs3j7lz5/KNb3wD6HtZQdE7WQZRCCFykCyDOHrJMohCCCHEKCKBWAghhMgiCcRCCCFEFkkgFkIIIbJIArEQQgiRRRKIhRBCiCySQCyEEKJPx48f56abbmL69OnMmTOHq6+++pSUlQP19ttvU11dTW1tLUePHuWGG27odb+VK1cy3qa3ZiTXtBCDEUukiCaSxBIpYskUyZQmlYKU1iS1RmtNsvu21mAwgFEpDAaFQanu62A0KEwGA1azAavJgNVkzPZbEyIrGhsbuemmm1izZg0TJkwY8vG01nzmM5/h1ltv5emnnwZg69atNDU1UVV15mUUT/bkk09y3333cdtttwHw7LPPDrl8Y4UEYpExqZQmEEsQjKY3fyRBMJokEE0QiiWIxNOBN5pIEY2nSA1TMhmDUqcEZavJgNNqxGU147KZcFlNuLsvHRYj6XTpQox+3/72t1m/fj3/+I//yKOPPjrk473xxhuYzWbuuOOOnvtqa2vRWvOVr3yFl19+GaUUX//617nxxhtZt24dDzzwAEVFRezYsYOFCxfyy1/+kp/85Cf8+te/5pVXXuG1117jwQcfZNWqVT1rHd92223s2rWL2bNnEw6He17r1VdfZfXq1USjUaZPn87//M//4HK5mDJlCrfeeiu/+93viMfjPPPMM8yaNYtAIMA999zDpk2bUEqxevVqrr/++j6PkyskEIuzkkxpOkMxOkJxfOEYHcE4HaEYnaE4wViCXFhaNKU14ViScCwJxPvd12hQuKwm8hxm8p0WCp0W8h0WCpwWnFb5eIjctnLlSiDd7JtKpXruf+yxx3jssccwGAxceOGFrFu3blDHPxFMT/fcc8+xdetWtm3bRmtrK4sXL+aiiy4C0vmmd+7cSXl5OcuWLeOdd97hL/7iL1i/fj2rVq3ihhtuoK6u7pSyOhwOtm/fzvbt21mwYAEAra2tfOc73+G1117D6XTyz//8z3z/+9/nm9/8JgBFRUVs2bKFRx99lIceeogf//jHfPvb38br9fLhhx8C0NHRccbj5AL5phF98oXjtPijNPsjtPijtAVi+COJYavJZkMypfGF4/jCcQ63hU55zGo2UOCwUOiyUuK2MsFro8hlxWiQGrTILUuWLOHgwYO0traSSqUwGAwUFRUxffr0YXm99evXc/PNN2M0GiktLWXFihVs3LgRj8dz1sscvvXWWz3rFc+bN4958+YBsGHDBnbt2sWyZcsAiMVinH/++T3Pu+666wBYuHAhzz2XXn33tdde62lCB8jPz+fFF1/s9zi5QAKxAMAXitPYFaa5K0qzP0qLP0okPr5XTInGUzT6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\n",
+                        "image/png": "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\n",
                         "text/plain": [
-                            "<Figure size 576x216 with 1 Axes>"
+                            "<Figure size 1008x720 with 6 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "# Get into evaluation (predictive posterior) mode\n",
+                "# Set into eval mode\n",
                 "model.eval()\n",
                 "likelihood.eval()\n",
                 "\n",
-                "# Test points are regularly spaced along [0,1]\n",
-                "# Make predictions by feeding model through likelihood\n",
-                "with torch.no_grad(), gpytorch.settings.fast_pred_var():\n",
-                "    test_x = torch.linspace(0, 1, 51)\n",
-                "    test_x_distributional = torch.stack((test_x, (1e-2 * torch.ones_like(test_x)).log()), dim=1)\n",
-                "    observed_pred = likelihood(model(test_x_distributional))\n",
-                "\n",
-                "with torch.no_grad():\n",
-                "    # Initialize plot\n",
-                "    f, ax = plt.subplots(1, 1, figsize=(8, 3))\n",
-                "\n",
-                "    # Get upper and lower confidence bounds\n",
-                "    lower, upper = observed_pred.confidence_region()\n",
-                "    # Plot training data as black stars\n",
-                "    ax.errorbar(train_x_mean.numpy(), train_y.numpy(), xerr=train_x_stdv, fmt='k*')\n",
-                "    # Plot predictive means as blue line\n",
-                "    ax.plot(test_x.numpy(), observed_pred.mean.numpy(), 'b')\n",
-                "    # Shade between the lower and upper confidence bounds\n",
-                "    ax.fill_between(test_x.numpy(), lower.numpy(), upper.numpy(), alpha=0.5)\n",
-                "    ax.set_ylim([-3, 3])\n",
-                "    ax.legend(['Observed Data', 'Mean', 'Confidence'])"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "As a final note, we've made it very easy to extend the distributional kernel class by exposing a generic `DistributionalInputKernel` class that takes as input any distance function over probability distributions."
+                "# Initialize plots\n",
+                "fig, ax = plt.subplots(2, 3, figsize=(14, 10))\n",
+                "\n",
+                "# Test points\n",
+                "n1, n2 = 50, 50\n",
+                "xv, yv = torch.meshgrid(torch.linspace(0, 1, n1), torch.linspace(0, 1, n2), indexing=\"ij\")\n",
+                "f, dfx, dfy = franke(xv, yv)\n",
+                "\n",
+                "# Make predictions\n",
+                "with torch.no_grad(), gpytorch.settings.fast_computations(log_prob=False, covar_root_decomposition=False):\n",
+                "    test_x = torch.stack([xv.reshape(n1*n2, 1), yv.reshape(n1*n2, 1)], -1).squeeze(1)\n",
+                "    predictions = likelihood(model(test_x))\n",
+                "    mean = predictions.mean\n",
+                "\n",
+                "extent = (xv.min(), xv.max(), yv.max(), yv.min())\n",
+                "ax[0, 0].imshow(f, extent=extent, cmap=cm.jet)\n",
+                "ax[0, 0].set_title('True values')\n",
+                "ax[0, 1].imshow(dfx, extent=extent, cmap=cm.jet)\n",
+                "ax[0, 1].set_title('True x-derivatives')\n",
+                "ax[0, 2].imshow(dfy, extent=extent, cmap=cm.jet)\n",
+                "ax[0, 2].set_title('True y-derivatives')\n",
+                "\n",
+                "ax[1, 0].imshow(mean[:, 0].detach().numpy().reshape(n1, n2), extent=extent, cmap=cm.jet)\n",
+                "ax[1, 0].set_title('Predicted values')\n",
+                "ax[1, 1].imshow(mean[:, 1].detach().numpy().reshape(n1, n2), extent=extent, cmap=cm.jet)\n",
+                "ax[1, 1].set_title('Predicted x-derivatives')\n",
+                "ax[1, 2].imshow(mean[:, 2].detach().numpy().reshape(n1, n2), extent=extent, cmap=cm.jet)\n",
+                "ax[1, 2].set_title('Predicted y-derivatives')\n",
+                "\n",
+                "None"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.0"
+            "version": "3.7.3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `gpytorch-1.9.0/examples/01_Exact_GPs/GP_Regression_Fully_Bayesian.ipynb` & `gpytorch-1.9.1/examples/01_Exact_GPs/GP_Regression_Fully_Bayesian.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/01_Exact_GPs/GP_Regression_on_Classification_Labels.ipynb` & `gpytorch-1.9.1/examples/01_Exact_GPs/GP_Regression_on_Classification_Labels.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/01_Exact_GPs/README.rst` & `gpytorch-1.9.1/examples/01_Exact_GPs/README.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/01_Exact_GPs/Simple_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/01_Exact_GPs/Simple_GP_Regression.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9532738095238096%*

 * *Differences: {"'cells'": "{9: {'source': {insert: [(4, 'Just as a user defined GP model returns a "*

 * *            '`MultivariateNormal` containing the prior mean and covariance from forward, a trained '*

 * *            'GP model in eval mode returns a `MultivariateNormal` containing the posterior mean '*

 * *            "and covariance.\\n'), (5, '\\n'), (6, 'If we denote a test point (`test_x`) as `x*` "*

 * *            'with the true output being `y*`, then `model(test_x)` returns the model posterior '*

 * *            'distribution `p(f […]*

```diff
@@ -263,22 +263,37 @@
                 "        model.covar_module.base_kernel.lengthscale.item(),\n",
                 "        model.likelihood.noise.item()\n",
                 "    ))\n",
                 "    optimizer.step()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Make predictions with the model\n",
                 "\n",
                 "In the next cell, we make predictions with the model. To do this, we simply put the model and likelihood in eval mode, and call both modules on the test data.\n",
                 "\n",
-                "Just as a user defined GP model returns a `MultivariateNormal` containing the prior mean and covariance from forward, a trained GP model in eval mode returns a `MultivariateNormal` containing the posterior mean and covariance. Thus, getting the predictive mean and variance, and then sampling functions from the GP at the given test points could be accomplished with calls like:\n",
+                "Just as a user defined GP model returns a `MultivariateNormal` containing the prior mean and covariance from forward, a trained GP model in eval mode returns a `MultivariateNormal` containing the posterior mean and covariance.\n",
+                "\n",
+                "If we denote a test point (`test_x`) as `x*` with the true output being `y*`, then `model(test_x)` returns the model posterior distribution `p(f* | x*, X, y)`, for training data `X, y`. This posterior is the distribution over the function we are trying to model, and thus quantifies our model uncertainty.\n",
+                "\n",
+                "In contrast, `likelihood(model(test_x))` gives us the posterior predictive distribution `p(y* | x*, X, y)` which is the probability distribution over the predicted output value. Recall in our problem setup \n",
+                "\n",
+                "$$\n",
+                "\\begin{align}\n",
+                "y &= \\sin(2\\pi x) + \\epsilon\n",
+                "\\end{align}\n",
+                "$$\n",
+                "\n",
+                "where \ud835\udf16 is the likelihood noise for each observation. By including the _likelihood noise_ which is the noise in your observation (e.g. due to noisy sensor), the prediction is over the observed value of the test point.\n",
+                "\n",
+                "Thus, getting the predictive mean and variance, and then sampling functions from the GP at the given test points could be accomplished with calls like:\n",
                 "\n",
                 "```python\n",
                 "f_preds = model(test_x)\n",
                 "y_preds = likelihood(model(test_x))\n",
                 "\n",
                 "f_mean = f_preds.mean\n",
                 "f_var = f_preds.variance\n",
@@ -320,15 +335,15 @@
             "execution_count": 12,
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAQAAAADDCAYAAABtec/IAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDMuMC4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvOIA7rQAAIABJREFUeJztnXl4U2X2+D/ZmnRPW2gLZWtBAUFtaVDBDWhRAdcKwvh1dGYQdAac34wOKqOizig4IoM7DoI6DuJWRR3BhUVFBISUFsGhsrSUrXub7k2z3N8fadI0TdrQpm1K3s/z8JDe9eTm3nPPe96zyCRJQiAQBCby3hZAIBD0HkIBCAQBjFAAAkEAIxSAQBDACAUgEAQwyq4eQKfTpTd/nKrX6x/q6vEEAkHP0SULoPnhn6XX67cA43Q63TjfiCUQCHoCma/iAHQ63TG9Xj/cJwcTCAQ9gk98ADqd7kHgHl8cSyAQ9By+tAA+BObp9XqDu/UPP/ywCDkUCHqJZ555RuZueZecgPYxv16v3wfkAfOBZz1t/+STT3Z4zJKSEmJjY7siVrfj7zL6u3zg/zL6u3zgvYyPP/64x3VdHQKkA9HNn7XYlIBAIOgjdFUBrAaSdDrdfAC9Xp/ZdZEEAkFP0aUhQPN4f7WPZBEECGazmZqaGmpqavDXbFSr1Up1dXVvi9EurjLKZDLUajXx8fEold492l0OBBIIzpaioiIiIyOJiYlBJnPrm+p1TCYTKpWqt8VoF1cZJUnCYDBQVFTEoEGDvDqGCAUW9DhGo5GIiIhef/izs7PJzs7u9vMYDAY+/vjjbj+PTCZDq9ViNBq93kcoAEGPI0mS1w9/YWEh6enpFBUVdfp82dnZrFmzhq1bt7JmzRry8my+6sjISDIzu99tpdVq3Z4nOzub0aNH8/HHH/Pxxx+zYsUKh2zuaG+dHZlMdlbDKjEEEPg1y5YtY+fOnSxdupQXX3zxrPc3GAwsX76c9evXO5bdfvvtrF+/nujo6Hb29C1RUVFtlqWkpJCYmEhGRoZj2fTp09m0aVObbfPy8li7di1PP/20T+USCkDgl2i1WhobGx1/r169mtWrV6PRaDAY3MaauSUzM5MpU6a0WhYVFcXWrVtJTU0lOzubrVu3kpOTw9y5c8nKygIgKyuLmTNnsm3bNqKjo0lMTCQ/P5/MzEwSExMZOXIkX375JevXr2fBggU88MADAK22T0xMZO3atSQnJ7Nv3z6vv7f9Tb9t2zYApkyZQk5ODvn5+WRnZxMZGcm2bduwWCxMnTqVpKQkr6+HK2IIIPBLDh06xOzZswkODgYgODiYOXPmkJube9bHqqqq8rguJSWFtLQ0kpOTWbt2LTk5OWzbto3Jkyfz6KOPkpqa6nj4p0yZQlRUFE8//TR33nmn4xgZGRkkJSW12f6RRx7hlltuIS0tjcTExLOSOSkpiejoaKKjo9mwYQNTpkwhMTGRlJSUNuu6glAAAr9kwIABREREYDQa0Wg0DsdhfHz8WR1nypQpjre6nfz8fNLS0lotsw8HbrnlFubOncuKFStoamoiMjKSlJQUhxWh1WpbHXvFihWkpqY6lrluf7YYDAaSkpJYsWIFkZGRJCcnO5aDbShgX3fxxRe3WtcZxBBA4LeUlJQwb9485s6dy9q1azvlCExKSmLRokWsWbOGxMREcnJyePnllx3rDQZDqyGA3WSfPHkyU6dOZe3atY63r90ENxgMaLVaZs6cySOPPOJQCk899VSr7R944AE2bNhAcnKyY9+UlBTHubOzs8nPz3fMEOTn5ztks5+vqqqKvLw8KisrMRgM5OfnO9ZVVFSQl5dHfn5+q+OeDT5LBuqIhx9+WBK5AD2Dv8t39OhRhg4d6tfz7H0xDsDO0aNHGTFihOPvxx9/3GMykBgCCAQBjFAAAkEAIxSAQBDACAUgEAQwQgEIBAGMUAACQQAjFIDgnCY7O5sJEya0yvrLy8trsyxQEYFAgl5Fo1H75DiNje5TYFNSUhyBQK+88gpgCw22h9UGOkIBCM55IiMjPa7Ly8trlcDjmmiTn5/PihUreOCBB9i2bZvPs/F6my4PAXQ63fzmf//whUCCwKKx0eiTfx2RkZHBmjVr2oTjuibwuCbapKWlodVqSUtL61LMvb/ii9ZgW/R6vb04aHpH+wgEvUFaWpojvdYV5wQed4k27nL5zxW6agEkYSsNDraS4J1PTBYIuoHs7GzWrl1LXl6e401vLwWWnZ3tSODZunUrFRUVDktg//795OXlsWnTJvLz8x1JN+ea47CrVYGdKwKPA97vmjgCgW9JSUlxVAOyF+1ISUnh0KFDjm2cx/X24homk4lZs2YBtgpCgNtKPX0dnzgBmzsE7WvuEOSRkpKSDo/VF8ZZ/i6jv8tntVqxWCy9LUa7+Lt84FlGq9Xq1bMGvpsFSNfr9Q91tJG3Kar+nMpqx99l9Gf5qqurUSgUfp9u6+/ygXsZ5XK517+/T2YB9Hr9s82fhRNQIOhD+GIW4B86ne6YTqer9JFMAoGgh+iqE3ALcO7OkQgEHjAYDGzbtq1VSe++iIgEFPQ6L31zrEv73zd5eLvrs7OzycrKclTmPZuIvhUrVpCcnExOTo5jFgFamn0IBSAQ+DHuGoN426bLYDBQUVFBWlqa2yYi50KAkFAAgnOazMzMVmW7wRYPYM8BSExMpKqqisjIyFYx/0888QRZWVnk5+ezdetWHn30UXbt2oXBYGjT7MM1n6CioqJN/oC9s49dluTk5Fb79FZikkgHFgQc9iYed999N2lpaWRmZrqN+bdHDqalpTFu3DgAt80+XPMJ3B1rxYoVzJ07l4yMDKZMmdJmn95CWACCc5qZM2fyhz/8odWyrVu3Ajjq+xsMhi7H/EdGRpKUlORQCu6OZR9G2PsIuO7TGwgFIDin0Wq1rRqDVFVVkZyczFNPPUVmZibR0dFkZGSQn5/fKuY/JyeH6upqRyOQffv2kZ2d7bbZh2tDENdj2fdbvny5463vuo9zx6GeRDQG6QT+LqO/yycag/gG0RhEIBB0CaEABIIARigAQY8jk8noqaFnoCFJEjKZW2vfLcIJ2AGFhYX8+te/Zt26dW1aUxvqTRTXGKluMFFrNFPXZKHOaMZiBbkMZDKQy2RoVAoiNErCNUoig1X0CwsiMti/x5fdiVqtprq6mpiYmLO6WQXtI0kSBoMBtdr7QqtCAXTAsmXL2LlzJ0uXLuWJZc+RV1ZP7olKGg7X02jqfM54mFrJgEgNA7UaEmNCCdcEzk8RHx9PQUEBVVVVfmsJWK1W5HL/NpBdZZTJZKjV6jYvqvYInLvuLNFqtTQ2Njr+Xr16NatXr0apCuLRd3cQGmq7dNUVpaxb9hfuWPwcEdH9vT5+rdHMkZJajpTUsp1y4iPVnB8bxojYMEKCFD7/Pv6EUqkkPDzcr2cq/H0mBXwjo3+ruF7CYpXYuF3PhKk3olJrAFCpNaRMnsHit75ute2W9as4/nMWW9av6vT5JCQKqxr574+H0E28mne+PUBhVWPHOwoEXURYAE40ma3sP1XFgdPV1DXJkFQazE1GlEFqzE1GNCFhRET3p66ujsU3pmA2NTn23bXxfXZtfB+lKohln3WucOSW9avI/zmLNS89R8XCJcRHaBg3REtSvxAxVhZ0C0IB0PLgZ5+swmhuGdfXGiq4bPpsLps+i92bPqSmssyxbvFbX/P568s5uGsrJmMjKrWGsRPTuP7uRWd9/o6USUyomonDoxkWE9K1LyoQuBDQQwCLVWLfCQP/3n2C3fkVrR5+gLsee4GMhY8xMGkUGQsf467HXnCsi4jujzoktI2FAPDqors4fSyXVxfdRXVFaYdyLH7ra1ImzfA43Mg/eYpp117Dm1v3U1ztuQlGYWEh6enpXheEFAgCVgHkl9Wxfs9JfjhWflbe/OqKUt5ccg+nj+Xy0/dfMy7tRu5buZ7Lps+mprLc4RN499kHvfYNeFImdqei/Zhvv/pPPsw6zZZDJTQ0tZXZPmPx/PPPe38hBAGNTxRAc1nwPkFlfROf/VTI5weKMDSYqK4odfum9rR8y/pVnDiUw7vPPkhDbRVBag0Dk0ax9+uPObhzC7s2vo8kSRSfOIYkSeza+D6Lpo1h8Y1t872dz2Efbjgrk8U3prBo2hjHMXdtfJ+/TLuAmy8Zwbo9J8ktqgFsMxYajYbVq1djtVpZt24dGo2m1xJMBH2HLvsAmguD/gtovy5TL2O1SmSdMLC3oBKLtWXu2dmLn7FwicflruP04hO2Mlb28bpcoSQ0MprG+losTtspVEFoQsKYv/T1NjI5n8N5eJGx8DHApiA8+RkaTRY2Hyoht6iGPdkHePqJR/nss89oaGhAo9Fw880388wzz/juAgrOSbqsAPR6/RadTpfnC2G6i+JqI9t+KaWstmX87Mnx5op9uUKpImXSDA7s3IK5qeU4yiA1F16ejlyuIGvrF0A8yNQgmUEGFpOJuqpydm/6wKFgOnL6OccWtDc0ADhZ2UBxtRyLUoPRaESjsf0fERFxVgEhgsDknJ4FMFus/Hi8kuyTbSPOPHnxr771d3yX+Ybbt+7md15tfrtHAONANgFzk47sb4YBCUCc7eD2UzmdctfGYnZtPI5MdoKrbs3l9JHVHD/0GuYmQ5sZBGfLoL2ZCDtNFiu5+ae5JuN2/vrnBbz+2qsUFxf7+GoKzkV6VAH0ZGuw8joT2/OqqGwwu12vUIcgb36rKlVBmJuMKFQatPGD2yyXKzWUnInhSM4MNGHP0FAzBFC0esBtWIBigjQy1MHhNNbXYzKagX7YlEMcknQp32UCLAOeBJkek3EzTU3lLPvNNW0sAwClKohrf3s/E2++k8yVj1B0qoDwqH6tzjzz/qW2fcoU3HHvnxg9uL9fzwb4e/syf5cPfCNjjyqAnmgNZrVK7Dtp4MeCWqxyNaGhrRMjnM1rY211m7draGioY/nI1N/y9bpGftquI2vzQGAsAHKFlYFJDQwd1cDgUQ0c/OEVDu58G4WqEqu5gdS028hYuISPXnqSH7/4ELlSg8UUw5gJv2PsxPmcOhxM1tZKGusTQZoITOTnHyBu6NMoFJmUnHoac9OxVpZBaGgoX725ghOHctj5yb9b+Stc2V1YjzpayaXDovw6gMjfQ239XT7ouozn1BCgqsHE5kMl7YbRduR4s1pg/DVr+eG/0bz1tzDH+jCtmbETqxk7sYa4xFK00S1BOQd/2MuEGVe2MdPbmu87OX/cFPZ89RcWvf4cqiAT+T+HcPCHcA7sjKC4IBz4LfBrZPKPMBmXowkJc2sZtBd1KCGx93glhVWNXDM6llD1OfUzC3xIl0uC6XS6mcDrwDy9Xp/pabvuLgmWW1TDd4fLaLJY3a53dbzZsT9ElSVl/GvxDqzmP1NZEmxbF2QlZVIVuvQqhl1Qj7w5R6euro7Q0NCzlhHg45f/xu5NH3DZ9NtavcXNTTJy9WFseDWf6orLQbKdLCRiPzfeIyd3z2J+3t3WL+EuAanoVAEfv7CEOxY/x4D4AVw7JpYEbXCn5O0u/D3Zxt/lA+9lbK8kmC9mATIBjw9+d2M0Wfj2SBmHi2tbLXfN0vPk9Jv+20Xs/TqST1/rh7HhKgCi45uYeH0F468xEBLuXqGcLR15/pVBEmMn1jB2Yj8qS46x49MYfvxCS331xby3HMKjn8Vk/B3KoBy3swHOfPfh2lZTmJ/kFHLliBguGhTpk+8iOHfo07bhGUMjXx8qoabR1Gad6zy+a7SdyWikrmoKT9+ZgM2DD/A/4Akqij7iy38rufrWziX1uONscgeiYs3cMK+YqbeXsvuLKL75MIaaiguA3SSOOUVo5ApqKg+2PUcHSqak1sik8/qhVARsAKjAhT6pAKxWiT0FlegLDG2n99p5CEaNv4rLps9mRPJcPn0tnsP7bE49dfBpzKZHsZjfRqUOYuzEaZ1K6mmP9sJ9PdUU0IRamTSznEunVfLth/3YviGaI9mDUCj/yeTbyjA1laEKavn+diVjj1VwVTKHCmuorDMxbWwcYcIvIKAP5gJUNZj4KPsMe49Xuq0m4ymxZuHKd6muNGM2LeedZWlUl48lJNzMLQsKSb76L1gt/0YZpOrQvO4s1RWlbnMHoOOaAsGhVqb9poSH1hxFN9WAxSxjy/r+rPxDEsd+anFG2pWMxdTkMXCoqLqRD/Sn200qEgQOfUoB/K+wmvf2nqKo2rOX39Ob9os38zhx6B32fj0ICZh4QwUPrT3KxOsrqasuaxOH72u2rF/VKncgY+Fj5O7d3ibW3zlvwDUfQdvfzOz7z/D75ceJHWyk9LSa1x4axrpnomios/2UtYYKUq/JaPe71DWZ+Tj7DEdKatusEwQWfcIOrG+y8M0vpeSV1Xm1vfP028qFC9i1MQO4rXntTiTrvfz4RS6F+Rdzx+LnWk0Hpt9+L+uW/YXqilKfWAHtDUk68gt4ylPoN7CAkPDbGZi0gDN5t7L/uwEUHIrhV385w12PveCYpbBPbbrDbLXy1c8lVNQ1cWli2863gsDA7y2AY6W2tF1vH36w5fHfsuAxio5fgkJxGNvDXwssRBmUTsrkISRfPc2t2e2LEl/OtJfr78laWfaba9q1DJ769RSO/28XZ/LuAC4G9mAoCWLVg0PYuDYWs8m74B8JiT3HK/ny52LMHqZPBec2fmsB1BnNbD9aztFOmKn1NXKemH0ASZrVvORL4B7gBOYmyP5mo2PbjpKAOirxJZPJCA1SEKZWEqpWEqpWoJDJkLCVaZYGRbInRmtzyrkZl7uL9fdkGRzYsZlF08a4SHAYuJz4Yf+muOBXfJvZj0P6EO585AyakNNeFSw9UlJLTaOZGRfGn/MFSQWt8UsF8POZan441rZCjzf8khXKBysHIkmjkCvqkcnux2L+FzK5gvNTr0StCaHgUA71NVVeJwFBS1zBvCUrGRoTyfmDY4iPUBMbrkbVwbTaq+Za5s+fz9y5c3n99TWcOH2Gy4fHcKaqkflPvuz4ns4muzvLwFUxAMjkcpAsJI75jFv/OIF3n02g+HgIL/4xkSGjNrodQrijqLqRD7JOc+NF8USHBp31dRf0TfxOAXz9SyWVZu/Ecp4+Cw6LZdMbsez4NAaAYRfUo419iP3frUYZpMZiaiI6dmCrGH3nhyth+CiP03RhaiXffbqW4z/vI3/z29zx2GPExnpfbOP991ssjJdeetHxeRw2K6Go2sjhYluJ8Ibm6kTuLAPnIYNMJkeSrFx4eTqhEdHUVJYxbHQDf345jyWzDmBsmMWR7P8HKNi18QFHSvMz/81p9zpmmq1cNyaWIdGi/mAg4HcKoLTOhNLLOWr7eP2zf31KyamlFOZpkCskrr2zhEm3lvOfpbluU2k9pdg6L//xiw+x1lXy6M3jMBpbpsxef/11Xn/9dTQajU+ysWQyGQMiNQyI1HDliBhOGRo4eKaG3yx50THN6WwZuJPdeb0m1Mqf/xXGB8tf5dSRucBC4FJgJslXJ7d7He2Wwmc/FXH1ef24MCGiy99P4N/4XXvwlV8eRKluP269tWd9LvAiEAIcYeDwvzP3b3M77cEPCVIydmA4YwdGEKpWUlhYyMMPP+yothMcHMy1117L888/360FN6oaTOScquJQYQ2mDhx0roFEdXV1fPnGc+zedAz4EEgESoFZwHcOv0ZH+RHJg7VcMTy6WzIK/T3W3t/lA9/kAvj9LIA7Fr/1NRddMQuZ/ENgDRBCVNw2kq9+jMK8dZ3y4IcEKbnqvH7cddlgLk2MdmTQDRgwgIiIiFbVdsLCwrq92k5ksIqrz+vHbyYMQTc0CmU7barczVzUGipITRvEiOQFwFdAf2ALg85bxcNv2qoNd1SNOOekgY0Hi2kyixmCcxW/GwI4Y3+z3XTvYj59bZnjDVdVNphf9r2IZI0HaoA/UFm8jsrmIjhn06RDo1KQOkTLhQkRHp15JSUlzJs3j7lz57J27VoKCgp8+0U7kG9CUjQXJkSw53gl/yuscQwNvGlO8tFLT3I0ZwYy+TIk6yJOHbmXz/5VRFX5rdz5yNIOS47ll9XxcfYZrr8wnrAA6l8YKPj1L+pcYrvkZB6b31lF3JDn+XxNHBazjJCI49z2p8Ps21bKz7tVyORytzHw7pDLZFw0KJJLh0URpGzfEHJ24r3wwgu9UmknTK1kysj+JA+K5Puj5ZyoqPc4XTjl9gWO/WoNFUyYMYvLpg/n8zUvcnT/fH76Ph54jk9XreLoflt48lW33Omx5FhprZEPsk4z48J44iK87zwr6D4KyuvxRYK3XyoA9xV4tezeNBuwmd4Tb6jg+rsbUAUN4pcsLRazLSPQ05vMmSHRIVw5IqZPTndFhwZx08UD+KW4lu+PKNy+wZ3LhTlHOeYf/BWS9Q3gM2ACP+1IAPazb+t/mfPA0najIO3hw+mj+3NebBiC3sFildiZV8FPp6qYdUHXfwe/9AHYx6bKIPvb5lIgG7gFMDB01N8pzL+WJTOTHRFzdmwVe2VuY+DD1Eqmj43nposH9MmH35mRcWHccelgZI3VTPAyj8F2XQcBlwC7gCHAD0jS9SyaNoan7pjSbhSkPXx4j4dELEH3UtVgInPfaXJOGqgqL2XWrFkUFRV16Zh+aQG0zHebQPYXkJYCKmAPMJuC3OPNW8pImTTDbfCO8xtMhowLBoZzxfCYDs39voRGpeCbTZ9wsqKeLbmlDEwaBdgqFrnDfl2hGEjD1s7h18AG4CEk6TmgfR+KhMSP+RWU1TaRPqr/OXU9/Zlfimv59pdSR8WrzetXsWfPHpYuXcqLL77Ywd6e8atfr7CwkNV/nUd1RSmGUgva/nqQlgMqVOpXgSuA4057SGR/uxGTsdGj6R8ZrOLm5AFMGXnu3qyDo0P41fhBXpnmNp/AHC684krgTuCv2G6D5cjkawGlx1bo0JKhmP1LPh9ln6G6oW0xFoHvMJosfPlzMV//r5gmi9WpW9R7SJLE6tWru9QFyq+eiGXLlnH8UA7vPbeZI9mrMJSmEBxm4bePnyA17TvAhEzWIrJKrSGyXxyp6Te5NYEvTIjkV+MHMSjKv+rhdQcalYLrxsQxdXQsQe2EJtsbnkpWKxNmzOHPr+g4f9xKoBHJ+jtksq8xGYM9+lCcpxzLao28n3WaU5UN3fjNApeTlQ28u/dUq7Rt16nb4OBg5syZQ25ubqfO4YvWYDMBAzBOr9c/25ljaLVaGhsbAQXwN45k299K27n/1Xi0/c3s3Wx7c9VWVXBgx9fIZDaP/wWXTnLEudsj4kKClKSN6h+Q7bRHxYejGhPN3mIrpbWti344Bww5OwfnPT2KVQ/+hZOHn8JknIwm9ABlhYtb7dvelKPxvzlcPjyalMGiF6EvMFms7M6vZP/JKiSX5hPO4eBqtbrLXaC6ZAHYm4Lq9fotgKGzTUIPHTrETTfNA74FHsXWceMJYApP3zmSxTemtHlz/enlD906vZL6hXL7+EEB+fDbCdcomTluIGMHtg7lbS/V+ffP/oFFq0uIH9ZIY10Cp4++Qf7BFsupvaAhSZLYcbScTSJoqMsUVjXy3t5T5Jw0tHn47diGcbP59NNPmTdvXpe6QHXVApgNbG7+nAekA/vO9iADBgwgJkaJLZz3FPB/wPZmp951rebz3dXyB1DIZVwxIoaLEkTlWwClQs7kkf0ZqA0m9byEVv0MPTn5omLNLHjuOO88k0CuPpx/LR7KDfN/Yf/2O73qU3istJaKuiamj43r87MsPY3ZYmWXh7e+K3c99gIymYwLLghj0qRJXTpvVxWAFqhw+jumvY3bC6A5cyafW25Zx8GCPI7s2+4w8RUqDQp1iEfPNkCkRsmkYZHEqIw9EqTj722jnOWLksGXW77jwcee4Kdd3zge4NGXTuaaO//o9rrOWpTLV28NYc8XcXzy6mjgeja99RJ1VeWkXpOBbuot6DdvoLK0uM3+dXV1vPFdFZcNDef8/p59L33pGnY3Z6qM7DxeQ7XRfRs7d8hkMgwG77f3hN+0Bvvkk08ASJ00jQkz5rRp1+WJUfHhXH1evx738Pt7ooizfLGxsSSPSCB7e5MjNTosIpL4QUM97r9vyxBgPvA88DhZm9cDv0Opkpj9p78xfExKq+2d/Quh0f3JLjFTi8Tk8/uhVrkvMtKXrmF30GiysONoOYeKmkCpJlTpOcrSNeFLJpOh1YZ1WcauPjUGwF5QTgt0uZrmHQ8vJ2PhY47Cmc4mvzMKuYzJI/vbvN7n6PSeLykvK2PevHmseu9zrwqf2sb8+SiUM7HlW9yOXLGD3z35MdC2YKk7/8KRklre1Z9ut1VboJJbVMO6H09yqKim1XLX62rH9frWGBTs39/1YVZXLYD3AV3z5yRgSxeP5xXhGhXTxsSJuPSzwDmf4TJdClsOlWK2enbY2b3NVsuHKJSTsZg/wmrR8dbfyljwzyp2b7TdkE/9egqS03Fc/Qs1jbYy7qlDtFwyLAqF3H+blfYEpTVGvjtS5lEputZmcD/7EgSsZMCASPbvtxDRhbINXVIAer1+n85GOmDQ6/Vn7QA8W4bGhHDN6Fg0HsxKQcecFxtGhEbFxgNF1DV5HkfWGipAJsNizsIWPryBpsaJrPyDBmgAJHAJCXaXiCVJEvqCSvLK6kgf1Z+4CE23fC9/xmiysDu/kgNnqt33s/AwzapQqpyiXeORyV5HktIBGDGikbo6WZcUQJdtZ71ev1qv12/R6/Wru3qs9pAhY/ywKG64MF48/D4gLkLNbboEYsM9W1F3PfYCj/5nW/P0XzUwBZn8XSAM+BR4BGWQhpiBQ5DJZB0mYlXUNbF2834uuWIShUWdn7rqS1isEjknq3j7x5P8dLrKYw7FwpXvEhoZ7ch/UQapCY2M5o8vvEdQcBgm4++Bg7aHX1bBTffmsm5dKQMGdE2+PjF4DlLImTY2jssSu6c6TaASplaSkTKQEe2EELcuXQ6S9f8Ii1wOWIGnMDf9G4s5yOvGKpvXv8qBrB/50+P/4Fip96Xe+yJHS2p5Z89Jvj9aRqOp/QK3P37xAXVVFa2mWeuqKtj2/k5++v5x4J9AKOqQz0EaTcnJJ/HFo+CXyUDOaINRN6zWAAAT/0lEQVRVzLhQVKrtLlQKOdddEMvuYBX6gkq327jWITy4azmjdBJ5B/9MU+NtNNamMmmWleg4kyM2o013ZlcT94tMxgzORBWk5kRRKVEh587vW1Bez57jle12sLLjriybLWYjCFjM/u1/bf58Cvg9xvrPAdi18T2GDHmvy7Up/doCGBoTwm2pCeLh72ZkMhkTkqJJHxWL3M1rxR6FaZ+ZWfLOt8z9+/X88YUC+iUYaawfzgv3JZKrb5mudfVauzNxUybP4OE3v2L9nlN8d7iM2rOYB/dHCsrr+TDrNJ/9VOjVww9tIyyVQWrCo24A2T5s0bBB9Bu4id8v30fKJKlVJObNN9/c6RwAO36rAFIGa7nhwniPc8gC3zN6QDg3Jw9ArfTumscNaeI3j+sJDttBfY2SN5YM4aEZmSyaNrZNV6MX7pvVysS1mJocvgKrJPHT6Sr+s/skO46W09B09v0gegurVWLngaNcfNlVrPv2J68ffPt0H7T0gFCoYjA3PUdN5ScgjQGOApM4L+VtksaOaBOJ6YvalH6nABQyGemjYrliRIwY7/cCCdpgZqUORBus8mr7Hz59iYbaqxl8vm2a0WpdAmxEJmvtBJSklqlCT0VbzFYr2ScNvL37BN8fLafKj1ONm8xW9p0w8PaPJ3nkib9zeP/esypG62wh1RoqGJn6DMGhJ7CVcbeSMPwT7lt5kAkzBjiuk30odt/K9UyYMZuysrbl284Wv/MBTD1fy+gB4b0tRkATFRLErNQENh0s5rTBfaqv69j15OE5wFpgPTANScrCltPxPf0GDqGqvKRN3UJPkYhNFis5Jw3sP1lFYr8QLh4U6Rcp3ZIkccrQyM4DR/nbA7+nIPenDouyutJ2um878AK2ku0w6LwGZv3pDAOTzgdAG9tSpq11HswSbjsXS4LFhHr35hF0LxqVgpsuHsDoePfK2N3YNSr2ZxSqCdjKjQ0GviF2yH+oKCltt26hJyQk8srq2JBzhrd3n2BXXgXltW37GHQnkiRRXN3IrrwK/r37JJ/knOG1F54j72AWF191Xbtl1d3RUu4uBNvbPheYhUpt4Yb5Rdy3Mp+BSS2JW75uVuuK31kAAv9BIZeRPjoWbYiK3XmVrbLUXDsbW0xNBGmCsZqPoVBNxWJaDCym5MQdwFD6JfyVX//1zx4rD3fEydNnWLbQNqswbHACSf1CSdBqiI/Q+DwUvL7JQkFlIwcqSikor3cES7m+vbO2fub47E0xWrBdN1PTRZibHgfGAxAVt5ffPxtJVGyLE9Sbku++QCgAQYfohkahDVax2SV8uO304FbH38/fNwvJugVYB1xJ2emNrFxwPwrlxzzz3+x2szvd4RoiW1HXhL7AVt49NlxNfKQGbbCKqBAV0aFBXnU5Nlms1DSaqW40Y6g3UVzTSFGVkepGE3V1dYSGtvZBuCvDHhIeyYjky9otq95yvRR88VYsB3cuBSA8qp6BSa+iUn9FVGzrnBdPJd/bK3XfGYQCEHjFiNgwwl3Ch11rMzjXZ3j0P9v4/PXlHNh5KeamF4EMYA1DRz1LZUkZQR4SPDuMH3B5E1oliaLqxjbed6VcTpBSjrr5n0Iuw2KVMFkkLFYrRrPV0Yj1bDi6/8dWwxl3FalcsZhh18YovvpPLI11ChRKiasyykmbU4o6eDowvc0+rhaWN9ZFZ/A7H4Cg9yksLCQ9Pb1Nyem4CDW3pSbQP6zjJCz7DWwxnUGhuh34FUpVNXkHo1lx73D2fNkfq9PzZ58W2/TGP1uNeTtqX+YJs9VKfZOZyvomiqobOW1ooKi6kfI6I4YGU6ce/i3rV1FTWUbskCTuW7mecVNuZP/3X7XJ3LMjSXBwZzgr7h3Op68NoLFOwUhdLQ+sOsb035agDm6/8Iez1985wlKGjPN91JtBWACCNixbtoydO3e6LTkdplFy67iBbM0tbVWs0h2uQ4TK4rko1Ws5+EMEm9YMY/+3Ddz8hyKGjW5wZBXmH7Tt6/ym1029+azehK5WRFdp06im4BgrF9zaXKBWcgxLnDnxi4bP18SRf9Bm6iiDTpCxoBrdVLnXIbzuql8NigpmYlIMcRFqnxS/EQpA4KClOKuN1atXO8pOO4ebqhRyrhsTR7+woDbOQWfc3cCSdIoDP4Tzyap+nD4azCv3JwJvAv2A1jd0yuQZXH/3Ija88pTbdu6ecPUXdBXX8bgde2yDs7JauPJ/bHozksNZtlmOkAgzsYP+w/H/3cvJw7cw/prOyRMdEsTlI2J8XutSDAEEDg4dOsTs2bMJDrbNuXdUclo3NIoZF8a1W4bcFZkMLrqihhHJdwNPI5OZgN8Cx4C/A5HI5HJkMpnjTe8aiuypSExLzfzWUYiLb0xxu72n4huuuI7HAfoNHNJqWDJy/EKGX3yK5xcOb37464F/UF8dw/H//Q5ocsizaPpYxzk7kiFIIeeKETHM6aZCt0IBCBy4a4XeUcnpxH6hzEpNINrLZB77Q5q9bT3wKJJ0AbZehWHYKkLnEzt4LRdfdVu742t3D4672ITQyGjue/5dt8fwdo69uqKUn763NVG1ReHNwWKxYDIakStnYDJ+zC97X+IXfX9sdRL+ia0+zsNAteM4KnVz6nTzuduTQYaMUfHh3HHpYFIGa7utkIpQAIJW2Fuhb9++3euS09GhtsjB9tKK7bj2fVSpTxHZbz4jdQ8xeGQJEEVxwW848MMa6qv/ysY1H7o9jrsHx53nvK6qgt2bPmgtgwdL4eEbknl10V2cPpbLm0vuaVXurKG2iiC1hoFJo7j+7iUEh91PcFgBVvPnwDRk8kYuve4UYyfMQ6V+BChueeCbB/0mYyPlZ060Oqc7ayUmVE1GykCmjo4lVN29o3ThAxC0wrUVurcEKeVMGxNHToSGH46VY/VQ+KJldqDJZSrtLqCMh66/A6tlCRbzFcAi9n1jYd83G5DLV7Pss+d55Jb2pwXtVYzaK4N+8VXXkbX1M+RyBVarxTHHLpcr2Lftv4529K3LncnYtfEMuzbuxha2e7/t+8SYuPyGCi6dZsBiLuL5hV85FJDJ2EhVaRHj0m5k3JQb2PDy3ygvOoVktdqy/rQx1BjKHS3tL7o8nSf+vpS0lATkPVQ6TVgAAp+SPDiSW5IHEt7Om6vWUEHqNRlup9IeefsRUiY9g0J1JfAOtsIjM7Fav+bpO89jXNoxzh/3Z5RB7qcFW1cxar0NwKJpYxwRfNbmeUiTsZHsbzaStfUzW+jviWNIkoRklQNXAc9iy8zbDvwOCGfo6HrmLDrN4jePMGV2OaERljbThHFDRmA2NRGk1nB+ygRGJF8GktQqctJZEV40LJ6pqef32MMPPrIAdDrduJ6oByjoGwzUapgzfhDbfil1W/XnrsdeaI60CyVIo6GhpsrhsW+xEDYCO4BFwL3AHVRXJLHny0HYxtj3I5Nvx2TcCoQSHtUy3ecpiMbVmy+TKzg/dSJqTQgFh3KorarFYjofWzv6q4DrgCgnyU+SMFzP/z18If0HtVghnqYJ7dgtEJlM1iZy8qobf8X9C+5l00fvdLnVd2fwRW/AdGx9pod3XRzBuYJGpWD62HgOnK5mx9HyNhWIn/rVFR5N+VHjryI17SZqqyo4sm8nVuvjKIOWkXTh74mKvZ+srRrMTYOQrLcDt5P9DRzJNhI31EzsICOxg5s4k3ceF1y2hHFTruDnXRuoLCnCahmAJCVhMp5AoeyPxTyQ+qobiIiaisVSgsU0BGiddShXHCFuaC5X3BjJycOvUWsopf+g9sN23Zn3rm3rZ/1xCc88909Sh2hRKuRce9Ul3fI7dESXFYBer9+i0+nyfCGM4NzjwoQIErQaNh8qoaSmZVz+/179hG3vvOI21t3+kHz00pNIkrXZZDYSE3+GjIXVZCysprigimM/hbJ9wwkqi0dQa4im1qDm2H57jPFTAPy8C2wd6+DpOwFsgU2W5rybk4dt/+xvelXQCRSqfYREHGbIyDOYm352TDtecu2jbr+jp8QoZ/PeOXgpqV8oV4yIIdLLmgvdSY86Ab2JXPL3llHg/zL6o3xXD1ZxoNBE9ularJKEKjgMefPDoVQFuW0DZygr8diK7MX/52x2y4AhwGjk8rGkpC2iqjSIxnolxnoFjfUKTE1yVEFWlCoryiAr6mArkf2MRMU1cTL3MwoOfUTy5IHcvGABkEBjYwwajc2H4E3ikqusuXu+ayO70mLk0iHhDNLKMdZUUlLT4WHbP6cPfme/aQ3Wme16E3+X0R/li4+DcSOa2JJbQn5RBcba6jYRfs5t4OY++Yrjs70VmT3Md+HKd/ku8w0nC6KYsRPHcv3d1xMR7V26sevYPecbyPnm3yhVQTz67o52W9K54k5WOxdcrGP8MC0XJUT6fD6/q79zhwpAp9PNd7M4r7kluEBwVsSEBTFrXALfHTQT/eTLGM02T7ynTDpX7PP/P37xQZez5TpKue1qToFcJuOiQZGMH6r1214WHSqA7m74IQg85HIZY+JDuHRUDDvzysktrO2wJba7tGAAmUzOfSvXd6rQSHspt3V1dZ3OKZAh47y4UC5LjPaLcX57+GIWYKbtP91MvV6f6QOZBAFCSJCC9FGxjB0QwY5j5e02EW3vbR0R3d9rC8IV14zFmsqyTlfjkSFjRGwolwyL6jOl7H0xC5AJiAdf0GniIzXMHJdAQXk9u/MrWs0W2PGmQEZnTHZ3GYvVFaVsWLWMX/Z+51U1HplMxnmxoYwf2ncefDsiElDgNwyNCWG2bhDTx8YTF962gainAhl2PCXWeJv1Z8fbajxqpYLUIVp+c9kQrr0grs89/CByAQR+yPD+oQzvH0phVSP7T1VxtLQOSZLcvq2h4wKadsWw6Y1/UlF8xisLoc7N0MBOXLiG0QPCGRkX5vOCpD2NUAACv2VApIYBkRpqG80cKqrhcEktFXVty4J78g8c2LGZRdPGOLaz5wA8dccUnt10oN1zz3nwWcc0YMbCxwhTKxkZF8ao+PA++ab3hFAAAr8nTKNk/LAoxg+Lory2icMlteSX1VNR14SE1GHsf/a3G1sdT5KsLJo2pl2nngwZceEahsYEMywmlNjwoHOyU5VQAII+RUxYEBPCopmQFE1Dk4UzVY2cMjTwXq2BidfP4ZLrZjpMdrtiANt0ob2ElzunnlqpIDY8iLgIDXERahTGGoYmdK3vXl9AKABBnyU4SOHwF/zwtc28rzWaqcyYQk2jCaPZymdNNVw/+04MFeXs2LwRmVyOucnIsPh+3HblWCI0SsI1qjZ9BEpKzq5vQV9FKADBOUWYWkmYWok9q2/z5xsAmD17Nvfccw9z585l7dq1FBUVcZ6PSmv3ZYQCEAQEna10dK7Tt+cwBAJBlxAKQCAIYIQCEAgCGKEABIIARigAgSCAEQpAIAhghAIQCAIYoQAEggBGKACBIIARCkAgCGCEAhAIAhhfFAW1lw0frtfrH+rq8QQCQc/RJQuguS/glubS4UnNfwsEgj5CV4cASdgbr0Fe898CgaCP0KUhgEvTkHHA+562BdEbsKfwd/nA/2X0d/nAj3oD6nS6ccA+vV6/r73tRG/AnsPf5QP/l9Hf5QP/6Q2YLhyAAkHfo8u9AXU63Xy9Xv9s8+d00TRUIOg7+GIW4B86ne6YTqer9JFMAoGgh+iqE3ALEOUjWQQCQQ8jIgEFggBGKACBIIARCkAgCGCEAhAIAhihAASCAEYoAIEggBEKQCAIYIQCEAgCGKEABIIARigAgSCAEQpAIAhghAIQCAIYoQAEggBGKACBIIARCkAgCGCEAhAIAhihAASCAEYoAIEggPFFazB7Y5CpojKwQNC38EVR0FnNtQHHNfcHEAgEfQRfFAW1lwFP6qgxiEAg8C981RnoQeCejrZ7/PHHfXE6gUDgI2SSJPnkQDqd7kNgnl6v9/+magKBAOhiazD7mL/Z9M8D5gPP+lZEgUDQXXS1NVg6YB/3a4G9vhBKIBD0DF0aAuh0Oi1wW/OfqXq9vkM/gEAg8B985gMQ9A46nW4mYADG2Zu0etjuwfbWC/wfnU43ztNMm7f3gSs+mQXoLB0J3dkv1YPy2f0jw3sjCMrJB7NFp9MlebpBmuM1ptIL/hkvruE4IAlAr9dn9rB4dhm8vQ+TOuqW3V00/4b/Aoa7WefVfeCOXgsFdhYaMLgGEXW03g/kSwe2NN8QSU4RkT3JbGw3JticsL0hg0e8/A0XNz/4Sb0RSOblfZjXvD6vt4Ld7Of3sLrT90Fv5gJ0JHRv39wdnT/JaVle8989jRaocPo7xnWD5rfBFtflPUS717D5zboXQK/XP9tLgWTe3Gf/aP7fX4PdOrwPPNGbCqAjoTv9pXxEu+fX6/WrnczBcYC+pwQ7S6J78dwd/YbjgRidTjeuOZisN+jod96H7c1f6bLdOYHIBuwizSbhvl56MxhoecC1QLnzyl5++3tLuf3aNVsEfkXzTJcBWAa8rtPpesPS64h274P26E0F0JHQnf5SPsLb86f3Yhbk+7QMPZJozstovmnBNq6e2eysjO6F8WtH17CclnGtAZtF0NN0JON8YFmzc3Ae4DdKyul3dnsfeENvKoCObt5Ofykf0ZF86HS6+XavcW84AZ3enOmAwckK2dq8PtPJs651c4jupqNrmOm0vrcCyTr8ne00X8teCXVvto50LlaS/Xf2dB90SK/GATS/mfJwml7R6XRZer0+1dN6f5Gv+WJ/iG1cGE1LWrTACS9/4wpgfG9ZUl7I+GDz+ujemgbsLkQgkEAQwAgnoEAQwAgFIBAEMEIBCAQBjFAAAkEAIxSAQBDACAUgEAQwQgEIBAHM/wcVyBgkKNumfgAAAABJRU5ErkJggg==\n",
+                        "image/png": "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",
                         "text/plain": [
                             "<Figure size 288x216 with 1 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -347,39 +362,37 @@
                 "    # Plot predictive means as blue line\n",
                 "    ax.plot(test_x.numpy(), observed_pred.mean.numpy(), 'b')\n",
                 "    # Shade between the lower and upper confidence bounds\n",
                 "    ax.fill_between(test_x.numpy(), lower.numpy(), upper.numpy(), alpha=0.5)\n",
                 "    ax.set_ylim([-3, 3])\n",
                 "    ax.legend(['Observed Data', 'Mean', 'Confidence'])"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "anaconda-cloud": {},
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python 3.9.12 64-bit ('3.9.12')",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.0"
+            "version": "3.9.12"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "8a61b873b964ebeec997f3785d4891e85789cfba4e32a225b1d76f494e6c6489"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `gpytorch-1.9.0/examples/01_Exact_GPs/Spectral_Delta_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/01_Exact_GPs/Spectral_Delta_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/01_Exact_GPs/Spectral_Mixture_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/01_Exact_GPs/Spectral_Mixture_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/01_Exact_GPs/index.rst` & `gpytorch-1.9.1/examples/01_Exact_GPs/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Exact_GP_Posterior_Sampling_with_CIQ.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Exact_GP_Posterior_Sampling_with_CIQ.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Grid_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Grid_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/KISSGP_Regression.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/KISSGP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/KeOps_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/KeOps_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/README.rst` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/README.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/SGPR_Regression_CUDA.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/SGPR_Regression_CUDA.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Scalable_Kernel_Interpolation_for_Products_CUDA.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Scalable_Kernel_Interpolation_for_Products_CUDA.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Simple_GP_Regression_CUDA.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Simple_GP_Regression_CUDA.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Simple_GP_Regression_With_LOVE_Fast_Variances_and_Sampling.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Simple_GP_Regression_With_LOVE_Fast_Variances_and_Sampling.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/Simple_MultiGPU_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/Simple_MultiGPU_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/02_Scalable_Exact_GPs/index.rst` & `gpytorch-1.9.1/examples/02_Scalable_Exact_GPs/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/Batch_Independent_Multioutput_GP.ipynb` & `gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/Batch_Independent_Multioutput_GP.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/Hadamard_Multitask_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/Hadamard_Multitask_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/ModelList_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/ModelList_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/Multitask_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/Multitask_GP_Regression.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868483946608947%*

 * *Differences: {"'cells'": "{1: {'execution_count': 1, 'outputs': []}, 3: {'execution_count': 2}, 5: "*

 * *            "{'execution_count': 3}, 7: {'execution_count': 4, 'outputs': {0: {'text': ['Iter 1/50 "*

 * *            "- Loss: 1.220\\n', 'Iter 2/50 - Loss: 1.180\\n', 'Iter 3/50 - Loss: 1.138\\n', 'Iter "*

 * *            "4/50 - Loss: 1.096\\n', 'Iter 5/50 - Loss: 1.054\\n', 'Iter 6/50 - Loss: 1.013\\n', "*

 * *            "'Iter 7/50 - Loss: 0.972\\n', 'Iter 8/50 - Loss: 0.932\\n', 'Iter 9/50 - Loss: "*

 * *            "0.892\\n', 'Iter  […]*

```diff
@@ -17,26 +17,17 @@
                 "\n",
                 "where $k_\\text{inputs}$ is a standard kernel (e.g. RBF) that operates on the inputs.\n",
                 "$k_\\text{task}$ is a lookup table containing inter-task covariance."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 1,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "The autoreload extension is already loaded. To reload it, use:\n",
-                        "  %reload_ext autoreload\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "import math\n",
                 "import torch\n",
                 "import gpytorch\n",
                 "from matplotlib import pyplot as plt\n",
                 "\n",
                 "%matplotlib inline\n",
@@ -55,15 +46,15 @@
                 "We'll have two functions - a sine function (y1) and a cosine function (y2).\n",
                 "\n",
                 "For MTGPs, our `train_targets` will actually have two dimensions: with the second dimension corresponding to the different tasks."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "train_x = torch.linspace(0, 1, 100)\n",
                 "\n",
                 "train_y = torch.stack([\n",
                 "    torch.sin(train_x * (2 * math.pi)) + torch.randn(train_x.size()) * 0.2,\n",
@@ -85,15 +76,15 @@
                 "3. We're using a `MultitaskMultivariateNormal` and `MultitaskGaussianLikelihood`. This allows us to deal with the predictions/outputs in a nice way. For example, when we call MultitaskMultivariateNormal.mean, we get a `n x num_tasks` matrix back.\n",
                 "\n",
                 "You may also notice that we don't use a ScaleKernel, since the MultitaskKernel will do some scaling for us. (This way we're not overparameterizing the kernel.)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "class MultitaskGPModel(gpytorch.models.ExactGP):\n",
                 "    def __init__(self, train_x, train_y, likelihood):\n",
                 "        super(MultitaskGPModel, self).__init__(train_x, train_y, likelihood)\n",
                 "        self.mean_module = gpytorch.means.MultitaskMean(\n",
@@ -118,73 +109,73 @@
             "metadata": {},
             "source": [
                 "### Train the model hyperparameters"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 4,
             "metadata": {
                 "scrolled": false
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Iter 1/50 - Loss: 47.568\n",
-                        "Iter 2/50 - Loss: 42.590\n",
-                        "Iter 3/50 - Loss: 37.327\n",
-                        "Iter 4/50 - Loss: 32.383\n",
-                        "Iter 5/50 - Loss: 27.693\n",
-                        "Iter 6/50 - Loss: 22.967\n",
-                        "Iter 7/50 - Loss: 18.709\n",
-                        "Iter 8/50 - Loss: 13.625\n",
-                        "Iter 9/50 - Loss: 9.454\n",
-                        "Iter 10/50 - Loss: 3.937\n",
-                        "Iter 11/50 - Loss: -0.266\n",
-                        "Iter 12/50 - Loss: -5.492\n",
-                        "Iter 13/50 - Loss: -9.174\n",
-                        "Iter 14/50 - Loss: -14.201\n",
-                        "Iter 15/50 - Loss: -17.646\n",
-                        "Iter 16/50 - Loss: -23.065\n",
-                        "Iter 17/50 - Loss: -27.227\n",
-                        "Iter 18/50 - Loss: -31.771\n",
-                        "Iter 19/50 - Loss: -35.461\n",
-                        "Iter 20/50 - Loss: -40.396\n",
-                        "Iter 21/50 - Loss: -43.209\n",
-                        "Iter 22/50 - Loss: -48.011\n",
-                        "Iter 23/50 - Loss: -52.596\n",
-                        "Iter 24/50 - Loss: -55.427\n",
-                        "Iter 25/50 - Loss: -58.277\n",
-                        "Iter 26/50 - Loss: -62.170\n",
-                        "Iter 27/50 - Loss: -66.251\n",
-                        "Iter 28/50 - Loss: -68.859\n",
-                        "Iter 29/50 - Loss: -71.799\n",
-                        "Iter 30/50 - Loss: -74.687\n",
-                        "Iter 31/50 - Loss: -77.924\n",
-                        "Iter 32/50 - Loss: -80.209\n",
-                        "Iter 33/50 - Loss: -82.885\n",
-                        "Iter 34/50 - Loss: -85.627\n",
-                        "Iter 35/50 - Loss: -87.761\n",
-                        "Iter 36/50 - Loss: -88.781\n",
-                        "Iter 37/50 - Loss: -88.784\n",
-                        "Iter 38/50 - Loss: -90.362\n",
-                        "Iter 39/50 - Loss: -92.546\n",
-                        "Iter 40/50 - Loss: -92.249\n",
-                        "Iter 41/50 - Loss: -93.311\n",
-                        "Iter 42/50 - Loss: -92.987\n",
-                        "Iter 43/50 - Loss: -93.307\n",
-                        "Iter 44/50 - Loss: -93.322\n",
-                        "Iter 45/50 - Loss: -92.269\n",
-                        "Iter 46/50 - Loss: -91.461\n",
-                        "Iter 47/50 - Loss: -90.908\n",
-                        "Iter 48/50 - Loss: -92.142\n",
-                        "Iter 49/50 - Loss: -93.466\n",
-                        "Iter 50/50 - Loss: -90.492\n"
+                        "Iter 1/50 - Loss: 1.220\n",
+                        "Iter 2/50 - Loss: 1.180\n",
+                        "Iter 3/50 - Loss: 1.138\n",
+                        "Iter 4/50 - Loss: 1.096\n",
+                        "Iter 5/50 - Loss: 1.054\n",
+                        "Iter 6/50 - Loss: 1.013\n",
+                        "Iter 7/50 - Loss: 0.972\n",
+                        "Iter 8/50 - Loss: 0.932\n",
+                        "Iter 9/50 - Loss: 0.892\n",
+                        "Iter 10/50 - Loss: 0.854\n",
+                        "Iter 11/50 - Loss: 0.815\n",
+                        "Iter 12/50 - Loss: 0.777\n",
+                        "Iter 13/50 - Loss: 0.739\n",
+                        "Iter 14/50 - Loss: 0.700\n",
+                        "Iter 15/50 - Loss: 0.660\n",
+                        "Iter 16/50 - Loss: 0.620\n",
+                        "Iter 17/50 - Loss: 0.579\n",
+                        "Iter 18/50 - Loss: 0.538\n",
+                        "Iter 19/50 - Loss: 0.497\n",
+                        "Iter 20/50 - Loss: 0.456\n",
+                        "Iter 21/50 - Loss: 0.415\n",
+                        "Iter 22/50 - Loss: 0.376\n",
+                        "Iter 23/50 - Loss: 0.338\n",
+                        "Iter 24/50 - Loss: 0.301\n",
+                        "Iter 25/50 - Loss: 0.265\n",
+                        "Iter 26/50 - Loss: 0.231\n",
+                        "Iter 27/50 - Loss: 0.197\n",
+                        "Iter 28/50 - Loss: 0.165\n",
+                        "Iter 29/50 - Loss: 0.134\n",
+                        "Iter 30/50 - Loss: 0.104\n",
+                        "Iter 31/50 - Loss: 0.076\n",
+                        "Iter 32/50 - Loss: 0.050\n",
+                        "Iter 33/50 - Loss: 0.027\n",
+                        "Iter 34/50 - Loss: 0.006\n",
+                        "Iter 35/50 - Loss: -0.012\n",
+                        "Iter 36/50 - Loss: -0.027\n",
+                        "Iter 37/50 - Loss: -0.040\n",
+                        "Iter 38/50 - Loss: -0.051\n",
+                        "Iter 39/50 - Loss: -0.059\n",
+                        "Iter 40/50 - Loss: -0.065\n",
+                        "Iter 41/50 - Loss: -0.068\n",
+                        "Iter 42/50 - Loss: -0.070\n",
+                        "Iter 43/50 - Loss: -0.069\n",
+                        "Iter 44/50 - Loss: -0.068\n",
+                        "Iter 45/50 - Loss: -0.066\n",
+                        "Iter 46/50 - Loss: -0.063\n",
+                        "Iter 47/50 - Loss: -0.060\n",
+                        "Iter 48/50 - Loss: -0.057\n",
+                        "Iter 49/50 - Loss: -0.055\n",
+                        "Iter 50/50 - Loss: -0.053\n"
                     ]
                 }
             ],
             "source": [
                 "# this is for running the notebook in our testing framework\n",
                 "import os\n",
                 "smoke_test = ('CI' in os.environ)\n",
@@ -215,22 +206,22 @@
             "metadata": {},
             "source": [
                 "### Make predictions with the model"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 5,
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 576x216 with 2 Axes>"
                         ]
                     },
                     "metadata": {
                         "needs_background": "light"
                     },
@@ -278,37 +269,35 @@
                 "\n",
                 "None"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "collapsed": true
-            },
+            "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "anaconda-cloud": {},
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.7.3"
+            "version": "3.8.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 1
 }
```

### Comparing `gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/README.rst` & `gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/README.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/03_Multitask_Exact_GPs/index.rst` & `gpytorch-1.9.1/examples/03_Multitask_Exact_GPs/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/045_GPLVM/Gaussian_Process_Latent_Variable_Models_with_Stochastic_Variational_Inference.ipynb` & `gpytorch-1.9.1/examples/045_GPLVM/Gaussian_Process_Latent_Variable_Models_with_Stochastic_Variational_Inference.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/Approximate_GP_Objective_Functions.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/Approximate_GP_Objective_Functions.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/GP_Regression_with_Uncertain_Inputs.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/GP_Regression_with_Uncertain_Inputs.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/Modifying_the_variational_strategy_and_distribution.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/Modifying_the_variational_strategy_and_distribution.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/Natural_Gradient_Descent.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/Natural_Gradient_Descent.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/Non_Gaussian_Likelihoods.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/Non_Gaussian_Likelihoods.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/PolyaGamma_Binary_Classification.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/PolyaGamma_Binary_Classification.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/README.rst` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/README.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/SVGP_CIQ.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/SVGP_CIQ.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/SVGP_Multitask_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/SVGP_Multitask_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/SVGP_Regression_CUDA.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/SVGP_Regression_CUDA.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/VNNGP.ipynb` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/VNNGP.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/04_Variational_and_Approximate_GPs/index.rst` & `gpytorch-1.9.1/examples/04_Variational_and_Approximate_GPs/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/DGP_Multitask_Regression.ipynb` & `gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/DGP_Multitask_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/Deep_Gaussian_Processes.ipynb` & `gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/Deep_Gaussian_Processes.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999299719887955%*

 * *Differences: {"'cells'": "{9: {'source': {insert: [(0, 'num_hidden_dims = 2 if smoke_test else 10\\n'), (7, "*

 * *            "'            output_dims=num_hidden_dims,\\n')], delete: [7, 0]}}}"}*

```diff
@@ -218,22 +218,22 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "num_output_dims = 2 if smoke_test else 10\n",
+                "num_hidden_dims = 2 if smoke_test else 10\n",
                 "\n",
                 "\n",
                 "class DeepGP(DeepGP):\n",
                 "    def __init__(self, train_x_shape):\n",
                 "        hidden_layer = ToyDeepGPHiddenLayer(\n",
                 "            input_dims=train_x_shape[-1],\n",
-                "            output_dims=num_output_dims,\n",
+                "            output_dims=num_hidden_dims,\n",
                 "            mean_type='linear',\n",
                 "        )\n",
                 "        \n",
                 "        last_layer = ToyDeepGPHiddenLayer(\n",
                 "            input_dims=hidden_layer.output_dims,\n",
                 "            output_dims=None,\n",
                 "            mean_type='constant',\n",
```

### Comparing `gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/Deep_Sigma_Point_Processes.ipynb` & `gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/Deep_Sigma_Point_Processes.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/README.rst` & `gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/README.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/05_Deep_Gaussian_Processes/index.rst` & `gpytorch-1.9.1/examples/05_Deep_Gaussian_Processes/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/Deep_Kernel_Learning_DenseNet_CIFAR_Tutorial.ipynb` & `gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/Deep_Kernel_Learning_DenseNet_CIFAR_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/KISSGP_Deep_Kernel_Regression_CUDA.ipynb` & `gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/KISSGP_Deep_Kernel_Regression_CUDA.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/README.rst` & `gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/README.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/densenet.py` & `gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/densenet.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/06_PyTorch_NN_Integration_DKL/index.rst` & `gpytorch-1.9.1/examples/06_PyTorch_NN_Integration_DKL/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/07_Pyro_Integration/Clustered_Multitask_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/07_Pyro_Integration/Clustered_Multitask_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/07_Pyro_Integration/Cox_Process_Example.ipynb` & `gpytorch-1.9.1/examples/07_Pyro_Integration/Cox_Process_Example.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/07_Pyro_Integration/Pyro_GPyTorch_High_Level.ipynb` & `gpytorch-1.9.1/examples/07_Pyro_Integration/Pyro_GPyTorch_High_Level.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/07_Pyro_Integration/Pyro_GPyTorch_Low_Level.ipynb` & `gpytorch-1.9.1/examples/07_Pyro_Integration/Pyro_GPyTorch_Low_Level.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/07_Pyro_Integration/README.rst` & `gpytorch-1.9.1/examples/07_Pyro_Integration/README.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/07_Pyro_Integration/index.rst` & `gpytorch-1.9.1/examples/07_Pyro_Integration/index.rst`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/08_Advanced_Usage/README.rst` & `gpytorch-1.9.1/examples/08_Advanced_Usage/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   See the `Batch Mode Regression`_ example for more details.
 
 .. toctree::
    :glob:
    :maxdepth: 1
    :hidden:
 
+   ../03_Multitask_Exact_GPs/Batch_Independent_Multioutput_GP.ipynb
    Simple_Batch_Mode_GP_Regression.ipynb
 
 
 GPs with Derivatives
 ----------------------
 
 Derivative information can be used by GPs to accelerate Bayesian optimization.
@@ -43,30 +44,37 @@
    :maxdepth: 1
    :hidden:
 
    Simple_GP_Regression_Derivative_Information_1d.ipynb
    Simple_GP_Regression_Derivative_Information_2d.ipynb
 
 .. _Batch Independent Multioutput GP:
-  Batch_Independent_Multioutput_GP.ipynb
+  ../03_Multitask_Exact_GPs/Batch_Independent_Multioutput_GP.ipynb
 
 .. _Batch Mode Regression:
   Simple_Batch_Mode_GP_Regression.ipynb
 
 .. _1D derivatives GP example:
-  Batch_Independent_Multioutput_GP.ipynb
+  Simple_GP_Regression_Derivative_Information_1d.ipynb
 
 .. _2D derivatives GP example:
-  Simple_Batch_Mode_GP_Regression.ipynb:
+  Simple_GP_Regression_Derivative_Information_2d.ipynb
 
 
 Variational Fantasization
 ----------------------------------
 We also include an example of how to perform fantasy modelling (e.g. efficient, closed form updates) for variational
-Gaussian process models, enabling their usage for lookahead optimization.
+Gaussian process models, enabling their usage for lookahead optimization. See the `Variational fantasization`_ example.
+
+.. toctree::
+   :glob:
+   :maxdepth: 1
+   :hidden:
+
+   SVGP_Model_Updating.ipynb
 
 .. _Variational fantasization:
   SVGP_Model_Updating.ipynb
 
 Converting Models to TorchScript
 ----------------------------------
 
@@ -77,8 +85,7 @@
 .. toctree::
    :glob:
    :maxdepth: 1
    :hidden:
 
    TorchScript_Exact_Models.ipynb
    TorchScript_Variational_Models.ipynb
-   SVGP_Model_Updating.ipynb
```

### Comparing `gpytorch-1.9.0/examples/08_Advanced_Usage/SVGP_Model_Updating.ipynb` & `gpytorch-1.9.1/examples/08_Advanced_Usage/SVGP_Model_Updating.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/08_Advanced_Usage/Simple_Batch_Mode_GP_Regression.ipynb` & `gpytorch-1.9.1/examples/08_Advanced_Usage/Simple_Batch_Mode_GP_Regression.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/08_Advanced_Usage/Simple_GP_Regression_Derivative_Information_1d.ipynb` & `gpytorch-1.9.1/examples/08_Advanced_Usage/Simple_GP_Regression_Derivative_Information_1d.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/08_Advanced_Usage/TorchScript_Exact_Models.ipynb` & `gpytorch-1.9.1/examples/08_Advanced_Usage/TorchScript_Exact_Models.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/08_Advanced_Usage/TorchScript_Variational_Models.ipynb` & `gpytorch-1.9.1/examples/08_Advanced_Usage/TorchScript_Variational_Models.ipynb`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/08_Advanced_Usage/index.rst` & `gpytorch-1.9.1/examples/08_Advanced_Usage/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   See the `Batch Mode Regression`_ example for more details.
 
 .. toctree::
    :glob:
    :maxdepth: 1
    :hidden:
 
+   ../03_Multitask_Exact_GPs/Batch_Independent_Multioutput_GP.ipynb
    Simple_Batch_Mode_GP_Regression.ipynb
 
 
 GPs with Derivatives
 ----------------------
 
 Derivative information can be used by GPs to accelerate Bayesian optimization.
@@ -43,30 +44,37 @@
    :maxdepth: 1
    :hidden:
 
    Simple_GP_Regression_Derivative_Information_1d.ipynb
    Simple_GP_Regression_Derivative_Information_2d.ipynb
 
 .. _Batch Independent Multioutput GP:
-  Batch_Independent_Multioutput_GP.ipynb
+  ../03_Multitask_Exact_GPs/Batch_Independent_Multioutput_GP.ipynb
 
 .. _Batch Mode Regression:
   Simple_Batch_Mode_GP_Regression.ipynb
 
 .. _1D derivatives GP example:
-  Batch_Independent_Multioutput_GP.ipynb
+  Simple_GP_Regression_Derivative_Information_1d.ipynb
 
 .. _2D derivatives GP example:
-  Simple_Batch_Mode_GP_Regression.ipynb:
+  Simple_GP_Regression_Derivative_Information_2d.ipynb
 
 
 Variational Fantasization
 ----------------------------------
 We also include an example of how to perform fantasy modelling (e.g. efficient, closed form updates) for variational
-Gaussian process models, enabling their usage for lookahead optimization.
+Gaussian process models, enabling their usage for lookahead optimization. See the `Variational fantasization`_ example.
+
+.. toctree::
+   :glob:
+   :maxdepth: 1
+   :hidden:
+
+   SVGP_Model_Updating.ipynb
 
 .. _Variational fantasization:
   SVGP_Model_Updating.ipynb
 
 Converting Models to TorchScript
 ----------------------------------
 
@@ -77,8 +85,7 @@
 .. toctree::
    :glob:
    :maxdepth: 1
    :hidden:
 
    TorchScript_Exact_Models.ipynb
    TorchScript_Variational_Models.ipynb
-   SVGP_Model_Updating.ipynb
```

### Comparing `gpytorch-1.9.0/examples/08_Advanced_Usage/svgp_elevators.pt` & `gpytorch-1.9.1/examples/08_Advanced_Usage/svgp_elevators.pt`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/examples/LBFGS.py` & `gpytorch-1.9.1/examples/LBFGS.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/__init__.py` & `gpytorch-1.9.1/gpytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/beta_features.py` & `gpytorch-1.9.1/gpytorch/beta_features.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/constraints/constraints.py` & `gpytorch-1.9.1/gpytorch/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/distributions/__init__.py` & `gpytorch-1.9.1/gpytorch/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/distributions/delta.py` & `gpytorch-1.9.1/gpytorch/distributions/delta.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/distributions/distribution.py` & `gpytorch-1.9.1/gpytorch/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/distributions/multitask_multivariate_normal.py` & `gpytorch-1.9.1/gpytorch/distributions/multitask_multivariate_normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,32 +240,36 @@
         samples = super().rsample(sample_shape=sample_shape, base_samples=base_samples)
         if not self._interleaved:
             # flip shape of last two dimensions
             new_shape = sample_shape + self._output_shape[:-2] + self._output_shape[:-3:-1]
             return samples.view(new_shape).transpose(-1, -2).contiguous()
         return samples.view(sample_shape + self._output_shape)
 
-    def to_data_independent_dist(self):
+    def to_data_independent_dist(self, jitter_val=1e-4):
         """
         Convert a multitask MVN into a batched (non-multitask) MVNs
         The result retains the intertask covariances, but gets rid of the inter-data covariances.
         The resulting distribution will have ``len(mvns)`` tasks, and the tasks will be independent.
 
         :returns: the bached data-independent MVN
         :rtype: gpytorch.distributions.MultivariateNormal
         """
         # Create batch distribution where all data are independent, but the tasks are dependent
         full_covar = self.lazy_covariance_matrix
         num_data, num_tasks = self.mean.shape[-2:]
-        data_indices = torch.arange(0, num_data * num_tasks, num_tasks, device=full_covar.device).view(-1, 1, 1)
-        task_indices = torch.arange(num_tasks, device=full_covar.device)
+        if self._interleaved:
+            data_indices = torch.arange(0, num_data * num_tasks, num_tasks, device=full_covar.device).view(-1, 1, 1)
+            task_indices = torch.arange(num_tasks, device=full_covar.device)
+        else:
+            data_indices = torch.arange(num_data, device=full_covar.device).view(-1, 1, 1)
+            task_indices = torch.arange(0, num_data * num_tasks, num_data, device=full_covar.device)
         task_covars = full_covar[
             ..., data_indices + task_indices.unsqueeze(-2), data_indices + task_indices.unsqueeze(-1)
         ]
-        return MultivariateNormal(self.mean, to_linear_operator(task_covars).add_jitter())
+        return MultivariateNormal(self.mean, to_linear_operator(task_covars).add_jitter(jitter_val=jitter_val))
 
     @property
     def variance(self):
         var = super().variance
         if not self._interleaved:
             # flip shape of last two dimensions
             new_shape = self._output_shape[:-2] + self._output_shape[:-3:-1]
```

### Comparing `gpytorch-1.9.0/gpytorch/distributions/multivariate_normal.py` & `gpytorch-1.9.1/gpytorch/distributions/multivariate_normal.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 #!/usr/bin/env python3
 
+from __future__ import annotations
+
 import math
 import warnings
+from numbers import Number
+from typing import Optional, Tuple, Union
 
 import torch
 from linear_operator import to_dense, to_linear_operator
 from linear_operator.operators import DiagLinearOperator, LinearOperator, RootLinearOperator
+from torch import Tensor
 from torch.distributions import MultivariateNormal as TMultivariateNormal
 from torch.distributions.kl import register_kl
 from torch.distributions.utils import _standard_normal, lazy_property
 
 from .. import settings
 from ..utils.warnings import NumericalWarning
 from .distribution import Distribution
@@ -19,20 +24,29 @@
     """
     Constructs a multivariate normal random variable, based on mean and covariance.
     Can be multivariate, or a batch of multivariate normals
 
     Passing a vector mean corresponds to a multivariate normal.
     Passing a matrix mean corresponds to a batch of multivariate normals.
 
-    :param torch.tensor mean: Vector n or matrix b x n mean of mvn distribution.
-    :param ~linear_operator.operators.LinearOperator covar: ... x N X N covariance matrix of
-        mvn distribution.
+    :param mean: `... x N` mean of mvn distribution.
+    :param covariance_matrix: `... x N X N` covariance matrix of mvn distribution.
+    :param validate_args: If True, validate `mean` anad `covariance_matrix` arguments. (Default: False.)
+
+    :ivar torch.Size base_sample_shape: The shape of a base sample (without
+        batching) that is used to generate a single sample.
+    :ivar torch.Tensor covariance_matrix: The covariance matrix, represented as a dense :class:`torch.Tensor`
+    :ivar ~linear_operator.LinearOperator lazy_covariance_matrix: The covariance matrix, represented
+        as a :class:`~linear_operator.LinearOperator`.
+    :ivar torch.Tensor mean: The mean.
+    :ivar torch.Tensor stddev: The standard deviation.
+    :ivar torch.Tensor variance: The variance.
     """
 
-    def __init__(self, mean, covariance_matrix, validate_args=False):
+    def __init__(self, mean: Tensor, covariance_matrix: Union[Tensor, LinearOperator], validate_args: bool = False):
         self._islazy = isinstance(mean, LinearOperator) or isinstance(covariance_matrix, LinearOperator)
         if self._islazy:
             if validate_args:
                 ms = mean.size(-1)
                 cs1 = covariance_matrix.size(-1)
                 cs2 = covariance_matrix.size(-2)
                 if not (ms == cs1 and ms == cs2):
@@ -46,107 +60,117 @@
             event_shape = self.loc.shape[-1:]
 
             # TODO: Integrate argument validation for LinearOperators into torch.distribution validation logic
             super(TMultivariateNormal, self).__init__(batch_shape, event_shape, validate_args=False)
         else:
             super().__init__(loc=mean, covariance_matrix=covariance_matrix, validate_args=validate_args)
 
+    def _extended_shape(self, sample_shape: torch.Size = torch.Size()) -> torch.Size:
+        """
+        Returns the size of the sample returned by the distribution, given
+        a `sample_shape`. Note, that the batch and event shapes of a distribution
+        instance are fixed at the time of construction. If this is empty, the
+        returned shape is upcast to (1,).
+
+        :param sample_shape: the size of the sample to be drawn.
+        """
+        if not isinstance(sample_shape, torch.Size):
+            sample_shape = torch.Size(sample_shape)
+        return sample_shape + self._batch_shape + self.base_sample_shape
+
+    @staticmethod
+    def _repr_sizes(mean: Tensor, covariance_matrix: Union[Tensor, LinearOperator]) -> str:
+        return f"MultivariateNormal(loc: {mean.size()}, scale: {covariance_matrix.size()})"
+
     @property
-    def _unbroadcasted_scale_tril(self):
+    def _unbroadcasted_scale_tril(self) -> Tensor:
         if self.islazy and self.__unbroadcasted_scale_tril is None:
             # cache root decoposition
             ust = to_dense(self.lazy_covariance_matrix.cholesky())
             self.__unbroadcasted_scale_tril = ust
         return self.__unbroadcasted_scale_tril
 
     @_unbroadcasted_scale_tril.setter
-    def _unbroadcasted_scale_tril(self, ust):
+    def _unbroadcasted_scale_tril(self, ust: Tensor):
         if self.islazy:
             raise NotImplementedError("Cannot set _unbroadcasted_scale_tril for lazy MVN distributions")
         else:
             self.__unbroadcasted_scale_tril = ust
 
-    def add_jitter(self, noise=1e-4):
+    def add_jitter(self, noise: float = 1e-4) -> MultivariateNormal:
+        r"""
+        Adds a small constant diagonal to the MVN covariance matrix for numerical stability.
+
+        :param noise: The size of the constant diagonal.
+        """
         return self.__class__(self.mean, self.lazy_covariance_matrix.add_jitter(noise))
 
-    def expand(self, batch_size):
-        new_loc = self.loc.expand(torch.Size(batch_size) + self.loc.shape[-1:])
-        new_covar = self._covar.expand(torch.Size(batch_size) + self._covar.shape[-2:])
-        res = self.__class__(new_loc, new_covar)
-        return res
+    @property
+    def base_sample_shape(self) -> torch.Size:
+        base_sample_shape = self.event_shape
+        if isinstance(self.lazy_covariance_matrix, RootLinearOperator):
+            base_sample_shape = self.lazy_covariance_matrix.root.shape[-1:]
 
-    def _extended_shape(self, sample_shape=torch.Size()):
-        """
-        Returns the size of the sample returned by the distribution, given
-        a `sample_shape`. Note, that the batch and event shapes of a distribution
-        instance are fixed at the time of construction. If this is empty, the
-        returned shape is upcast to (1,).
+        return base_sample_shape
 
-        Args:
-            sample_shape (torch.Size): the size of the sample to be drawn.
-        """
-        if not isinstance(sample_shape, torch.Size):
-            sample_shape = torch.Size(sample_shape)
-        return sample_shape + self._batch_shape + self.base_sample_shape
+    @lazy_property
+    def covariance_matrix(self) -> Tensor:
+        if self.islazy:
+            return self._covar.to_dense()
+        else:
+            return super().covariance_matrix
 
-    def confidence_region(self):
+    def confidence_region(self) -> Tuple[Tensor, Tensor]:
         """
         Returns 2 standard deviations above and below the mean.
 
-        :rtype: (torch.Tensor, torch.Tensor)
-        :return: pair of tensors of size (b x d) or (d), where
-            b is the batch size and d is the dimensionality of the random
-            variable. The first (second) Tensor is the lower (upper) end of
-            the confidence region.
+        :return: Pair of tensors of size `... x N`, where N is the
+            dimensionality of the random variable. The first (second) Tensor is the
+            lower (upper) end of the confidence region.
         """
         std2 = self.stddev.mul_(2)
         mean = self.mean
         return mean.sub(std2), mean.add(std2)
 
-    @staticmethod
-    def _repr_sizes(mean, covariance_matrix):
-        return f"MultivariateNormal(loc: {mean.size()}, scale: {covariance_matrix.size()})"
+    def expand(self, batch_size: torch.Size) -> MultivariateNormal:
+        r"""
+        See :py:meth:`torch.distributions.Distribution.expand
+        <torch.distributions.distribution.Distribution.expand>`.
+        """
+        new_loc = self.loc.expand(torch.Size(batch_size) + self.loc.shape[-1:])
+        new_covar = self._covar.expand(torch.Size(batch_size) + self._covar.shape[-2:])
+        res = self.__class__(new_loc, new_covar)
+        return res
 
-    @lazy_property
-    def covariance_matrix(self):
-        if self.islazy:
-            return self._covar.to_dense()
-        else:
-            return super().covariance_matrix
+    def get_base_samples(self, sample_shape: torch.Size = torch.Size()) -> Tensor:
+        r"""
+        Returns i.i.d. standard Normal samples to be used with
+        :py:meth:`MultivariateNormal.rsample(base_samples=base_samples)
+        <gpytorch.distributions.MultivariateNormal.rsample>`.
 
-    def get_base_samples(self, sample_shape=torch.Size()):
-        """Get i.i.d. standard Normal samples (to be used with rsample(base_samples=base_samples))"""
+        :param sample_shape: The number of samples to generate. (Default: `torch.Size([])`.)
+        :return: A `*sample_shape x *batch_shape x N` tensor of i.i.d. standard Normal samples.
+        """
         with torch.no_grad():
             shape = self._extended_shape(sample_shape)
             base_samples = _standard_normal(shape, dtype=self.loc.dtype, device=self.loc.device)
         return base_samples
 
-    @property
-    def base_sample_shape(self):
-        """
-        Returns the shape of a base sample (without batching) that is used to
-        generate a single sample.
-        """
-        base_sample_shape = self.event_shape
-        if isinstance(self.lazy_covariance_matrix, RootLinearOperator):
-            base_sample_shape = self.lazy_covariance_matrix.root.shape[-1:]
-
-        return base_sample_shape
-
     @lazy_property
-    def lazy_covariance_matrix(self):
-        """
-        The covariance_matrix, represented as a LinearOperator
-        """
+    def lazy_covariance_matrix(self) -> LinearOperator:
         if self.islazy:
             return self._covar
         else:
             return to_linear_operator(super().covariance_matrix)
 
-    def log_prob(self, value):
+    def log_prob(self, value: Tensor) -> Tensor:
+        r"""
+        See :py:meth:`torch.distributions.Distribution.log_prob
+        <torch.distributions.distribution.Distribution.log_prob>`.
+        """
         if settings.fast_computations.log_prob.off():
             return super().log_prob(value)
 
         if self._validate_args:
             self._validate_sample(value)
 
         mean, covar = self.loc, self.lazy_covariance_matrix
@@ -167,15 +191,37 @@
         # Get log determininant and first part of quadratic form
         covar = covar.evaluate_kernel()
         inv_quad, logdet = covar.inv_quad_logdet(inv_quad_rhs=diff.unsqueeze(-1), logdet=True)
 
         res = -0.5 * sum([inv_quad, logdet, diff.size(-1) * math.log(2 * math.pi)])
         return res
 
-    def rsample(self, sample_shape=torch.Size(), base_samples=None):
+    def rsample(self, sample_shape: torch.Size = torch.Size(), base_samples: Optional[Tensor] = None) -> Tensor:
+        r"""
+        Generates a `sample_shape` shaped reparameterized sample or `sample_shape`
+        shaped batch of reparameterized samples if the distribution parameters
+        are batched.
+
+        For the MultivariateNormal distribution, this is accomplished through:
+
+        .. math::
+            \boldsymbol \mu + \mathbf L \boldsymbol \epsilon
+
+        where :math:`\boldsymbol \mu \in \mathcal R^N` is the MVN mean,
+        :math:`\mathbf L \in \mathcal R^{N \times N}` is a "root" of the
+        covariance matrix :math:`\mathbf K` (i.e. :math:`\mathbf L \mathbf
+        L^\top = \mathbf K`), and :math:`\boldsymbol \epsilon \in \mathcal R^N` is a
+        vector of (approximately) i.i.d. standard Normal random variables.
+
+        :param sample_shape: The number of samples to generate. (Default: `torch.Size([])`.)
+        :param base_samples: The `*sample_shape x *batch_shape x N` tensor of
+            i.i.d. (or approximately i.i.d.) standard Normal samples to
+            reparameterize. (Defualt: None.)
+        :return: A `*sample_shape x *batch_shape x N` tensor of i.i.d. reparameterized samples.
+        """
         covar = self.lazy_covariance_matrix
         if base_samples is None:
             # Create some samples
             num_samples = sample_shape.numel() or 1
 
             # Get samples
             res = covar.zero_mean_mvn_samples(num_samples) + self.loc.unsqueeze(0)
@@ -213,41 +259,55 @@
 
             # Permute and reshape new samples to be original size
             res = res.permute(-1, *range(self.loc.dim())).contiguous()
             res = res.view(sample_shape + self.loc.shape)
 
         return res
 
-    def sample(self, sample_shape=torch.Size(), base_samples=None):
+    def sample(self, sample_shape: torch.Size = torch.Size(), base_samples: Optional[Tensor] = None) -> Tensor:
+        r"""
+        Generates a `sample_shape` shaped sample or `sample_shape`
+        shaped batch of samples if the distribution parameters
+        are batched.
+
+        Note that these samples are not reparameterized and therefore cannot be backpropagated through.
+
+        :param sample_shape: The number of samples to generate. (Default: `torch.Size([])`.)
+        :param base_samples: The `*sample_shape x *batch_shape x N` tensor of
+            i.i.d. (or approximately i.i.d.) standard Normal samples to
+            reparameterize. (Defualt: None.)
+        :return: A `*sample_shape x *batch_shape x N` tensor of i.i.d. samples.
+        """
         with torch.no_grad():
             return self.rsample(sample_shape=sample_shape, base_samples=base_samples)
 
-    def to_data_independent_dist(self):
+    @property
+    def stddev(self) -> Tensor:
+        # self.variance is guaranteed to be positive, because we do clamping.
+        return self.variance.sqrt()
+
+    def to_data_independent_dist(self) -> torch.distributions.Normal:
         """
-        Convert a MVN into a batched Normal distribution
+        Convert a `... x N` MVN distribution into a batch of independent Normal distributions.
+        Essentially, this throws away all covariance information
+        and treats all dimensions as batch dimensions.
 
-        :returns: the bached data-independent Normal
-        :rtype: gpytorch.distributions.Normal
+        :returns: A (data-independent) Normal distribution with batch shape `*batch_shape x N`.
         """
         # Create batch distribution where all data are independent, but the tasks are dependent
         try:
             # If pyro is installed, use that set of base distributions
             import pyro.distributions as base_distributions
         except ImportError:
             # Otherwise, use PyTorch
             import torch.distributions as base_distributions
         return base_distributions.Normal(self.mean, self.stddev)
 
     @property
-    def stddev(self):
-        # self.variance is guaranteed to be positive, because we do clamping.
-        return self.variance.sqrt()
-
-    @property
-    def variance(self):
+    def variance(self) -> Tensor:
         if self.islazy:
             # overwrite this since torch MVN uses unbroadcasted_scale_tril for this
             diag = self.lazy_covariance_matrix.diagonal(dim1=-1, dim2=-2)
             diag = diag.view(diag.shape[:-1] + self._event_shape)
             variance = diag.expand(self._batch_shape + self._event_shape)
         else:
             variance = super().variance
@@ -261,41 +321,35 @@
                 "This is likely due to numerical instabilities. "
                 f"Rounding negative variances up to {min_variance}.",
                 NumericalWarning,
             )
             variance = variance.clamp_min(min_variance)
         return variance
 
-    def __add__(self, other):
+    def __add__(self, other: MultivariateNormal) -> MultivariateNormal:
         if isinstance(other, MultivariateNormal):
             return self.__class__(
                 mean=self.mean + other.mean,
                 covariance_matrix=(self.lazy_covariance_matrix + other.lazy_covariance_matrix),
             )
         elif isinstance(other, int) or isinstance(other, float):
             return self.__class__(self.mean + other, self.lazy_covariance_matrix)
         else:
             raise RuntimeError("Unsupported type {} for addition w/ MultivariateNormal".format(type(other)))
 
-    def __radd__(self, other):
-        if other == 0:
-            return self
-        return self.__add__(other)
+    def __getitem__(self, idx) -> MultivariateNormal:
+        r"""
+        Constructs a new MultivariateNormal that represents a random variable
+        modified by an indexing operation.
 
-    def __mul__(self, other):
-        if not (isinstance(other, int) or isinstance(other, float)):
-            raise RuntimeError("Can only multiply by scalars")
-        if other == 1:
-            return self
-        return self.__class__(mean=self.mean * other, covariance_matrix=self.lazy_covariance_matrix * (other**2))
+        The mean and covariance matrix arguments are indexed accordingly.
 
-    def __truediv__(self, other):
-        return self.__mul__(1.0 / other)
+        :param idx: Index to apply.
+        """
 
-    def __getitem__(self, idx):
         if not isinstance(idx, tuple):
             idx = (idx,)
         rest_idx = idx[:-1]
         last_idx = idx[-1]
         new_mean = self.mean[idx]
 
         if len(idx) <= self.mean.dim() - 1 and (Ellipsis not in rest_idx):
@@ -313,17 +367,32 @@
                 new_cov = self.lazy_covariance_matrix[(*rest_idx, last_idx, last_idx)]
             elif last_idx is (...):
                 new_cov = self.lazy_covariance_matrix[rest_idx]
             else:
                 new_cov = self.lazy_covariance_matrix[(*rest_idx, last_idx, slice(None, None, None))][..., last_idx]
         return self.__class__(mean=new_mean, covariance_matrix=new_cov)
 
+    def __mul__(self, other: Number) -> MultivariateNormal:
+        if not (isinstance(other, int) or isinstance(other, float)):
+            raise RuntimeError("Can only multiply by scalars")
+        if other == 1:
+            return self
+        return self.__class__(mean=self.mean * other, covariance_matrix=self.lazy_covariance_matrix * (other**2))
+
+    def __radd__(self, other: MultivariateNormal) -> MultivariateNormal:
+        if other == 0:
+            return self
+        return self.__add__(other)
+
+    def __truediv__(self, other: Number) -> MultivariateNormal:
+        return self.__mul__(1.0 / other)
+
 
 @register_kl(MultivariateNormal, MultivariateNormal)
-def kl_mvn_mvn(p_dist, q_dist):
+def kl_mvn_mvn(p_dist: MultivariateNormal, q_dist: MultivariateNormal) -> Tensor:
     output_shape = torch.broadcast_shapes(p_dist.batch_shape, q_dist.batch_shape)
     if output_shape != p_dist.batch_shape:
         p_dist = p_dist.expand(output_shape)
     if output_shape != q_dist.batch_shape:
         q_dist = q_dist.expand(output_shape)
 
     q_mean = q_dist.loc
```

### Comparing `gpytorch-1.9.0/gpytorch/functions/__init__.py` & `gpytorch-1.9.1/gpytorch/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/functions/_log_normal_cdf.py` & `gpytorch-1.9.1/gpytorch/functions/_log_normal_cdf.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/functions/matern_covariance.py` & `gpytorch-1.9.1/gpytorch/functions/matern_covariance.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/functions/rbf_covariance.py` & `gpytorch-1.9.1/gpytorch/functions/rbf_covariance.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/__init__.py` & `gpytorch-1.9.1/gpytorch/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/additive_structure_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/additive_structure_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/arc_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/arc_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/cosine_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/cosine_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/cylindrical_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/cylindrical_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/distributional_input_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/distributional_input_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/gaussian_symmetrized_kl_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/gaussian_symmetrized_kl_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/grid_interpolation_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/grid_interpolation_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/grid_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/grid_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/index_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/index_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/inducing_point_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/inducing_point_kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from linear_operator import to_dense
 from linear_operator.operators import (
     DiagLinearOperator,
     LowRankRootAddedDiagLinearOperator,
     LowRankRootLinearOperator,
     MatmulLinearOperator,
 )
+from linear_operator.utils.cholesky import psd_safe_cholesky
 from torch import Tensor
 
 from .. import settings
 from ..distributions import MultivariateNormal
 from ..likelihoods import Likelihood
 from ..mlls import InducingPointKernelAddedLossTerm
 from ..models import exact_prediction_strategies
-from ..utils.cholesky import psd_safe_cholesky
 from .kernel import Kernel
 
 
 class InducingPointKernel(Kernel):
     def __init__(
         self,
         base_kernel: Kernel,
```

### Comparing `gpytorch-1.9.0/gpytorch/kernels/keops/keops_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/keops/keops_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/keops/matern_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/keops/matern_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/keops/rbf_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/keops/rbf_kernel.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,21 +18,16 @@
         the same arguments. There are currently a few limitations, for example a lack of batch mode support. However,
         most other features like ARD will work.
         """
 
         has_lengthscale = True
 
         def _nonkeops_covar_func(self, x1, x2, diag=False):
-            return self.covar_dist(
-                x1,
-                x2,
-                square_dist=True,
-                diag=diag,
-                dist_postprocess_func=postprocess_rbf,
-                postprocess=True,
+            return postprocess_rbf(
+                self.covar_dist(x1, x2, square_dist=True, diag=diag)
             )
 
         def covar_func(self, x1, x2, diag=False):
             # We only should use KeOps on big kernel matrices
             # If we would otherwise be performing Cholesky inference, (or when just computing a kernel matrix diag)
             # then don't apply KeOps
             # enable gradients to ensure that test time caches on small predictions are still
```

### Comparing `gpytorch-1.9.0/gpytorch/kernels/kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/kernel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,102 @@
 #!/usr/bin/env python3
 
+from __future__ import annotations
+
 import warnings
 from abc import abstractmethod
 from copy import deepcopy
-from typing import Optional, Tuple
+from typing import Callable, Dict, Iterable, Optional, Tuple, Union
 
 import torch
 from linear_operator import to_dense, to_linear_operator
-from linear_operator.operators import ZeroLinearOperator
+from linear_operator.operators import LinearOperator, ZeroLinearOperator
+from torch import Tensor
 from torch.nn import ModuleList
 
 from .. import settings
 from ..constraints import Interval, Positive
+from ..distributions import MultivariateNormal
 from ..lazy import LazyEvaluatedKernelTensor
+from ..likelihoods import GaussianLikelihood
 from ..models import exact_prediction_strategies
 from ..module import Module
 from ..priors import Prior
 
 
-def default_postprocess_script(x):
-    return x
+def sq_dist(x1, x2, x1_eq_x2=False):
+    # TODO: use torch squared cdist once implemented: https://github.com/pytorch/pytorch/pull/25799
+    adjustment = x1.mean(-2, keepdim=True)
+    x1 = x1 - adjustment
+
+    # Compute squared distance matrix using quadratic expansion
+    x1_norm = x1.pow(2).sum(dim=-1, keepdim=True)
+    x1_pad = torch.ones_like(x1_norm)
+    if x1_eq_x2 and not x1.requires_grad and not x2.requires_grad:
+        x2, x2_norm, x2_pad = x1, x1_norm, x1_pad
+    else:
+        x2 = x2 - adjustment  # x1 and x2 should be identical in all dims except -2 at this point
+        x2_norm = x2.pow(2).sum(dim=-1, keepdim=True)
+        x2_pad = torch.ones_like(x2_norm)
+    x1_ = torch.cat([-2.0 * x1, x1_norm, x1_pad], dim=-1)
+    x2_ = torch.cat([x2, x2_pad, x2_norm], dim=-1)
+    res = x1_.matmul(x2_.transpose(-2, -1))
 
+    if x1_eq_x2 and not x1.requires_grad and not x2.requires_grad:
+        res.diagonal(dim1=-2, dim2=-1).fill_(0)
 
-class Distance(torch.nn.Module):
-    def __init__(self, postprocess_script=default_postprocess_script):
-        super().__init__()
-        self._postprocess = postprocess_script
+    # Zero out negative values
+    return res.clamp_min_(0)
 
-    def _sq_dist(self, x1, x2, postprocess, x1_eq_x2=False):
-        # TODO: use torch squared cdist once implemented: https://github.com/pytorch/pytorch/pull/25799
-        adjustment = x1.mean(-2, keepdim=True)
-        x1 = x1 - adjustment
-        x2 = x2 - adjustment  # x1 and x2 should be identical in all dims except -2 at this point
 
-        # Compute squared distance matrix using quadratic expansion
-        x1_norm = x1.pow(2).sum(dim=-1, keepdim=True)
-        x1_pad = torch.ones_like(x1_norm)
-        if x1_eq_x2 and not x1.requires_grad and not x2.requires_grad:
-            x2_norm, x2_pad = x1_norm, x1_pad
-        else:
-            x2_norm = x2.pow(2).sum(dim=-1, keepdim=True)
-            x2_pad = torch.ones_like(x2_norm)
-        x1_ = torch.cat([-2.0 * x1, x1_norm, x1_pad], dim=-1)
-        x2_ = torch.cat([x2, x2_pad, x2_norm], dim=-1)
-        res = x1_.matmul(x2_.transpose(-2, -1))
+def dist(x1, x2, x1_eq_x2=False):
+    # TODO: use torch cdist once implementation is improved: https://github.com/pytorch/pytorch/pull/25799
+    res = sq_dist(x1, x2, x1_eq_x2=x1_eq_x2)
+    return res.clamp_min_(1e-30).sqrt_()
 
-        if x1_eq_x2 and not x1.requires_grad and not x2.requires_grad:
-            res.diagonal(dim1=-2, dim2=-1).fill_(0)
 
-        # Zero out negative values
-        res.clamp_min_(0)
+# only necessary for legacy purposes
+class Distance(torch.nn.Module):
+    def __init__(self, postprocess: Optional[Callable] = None):
+        super().__init__()
+        if postprocess is not None:
+            warnings.warn(
+                "The `postprocess` argument is deprecated. "
+                "See https://github.com/cornellius-gp/gpytorch/pull/2205 for details.",
+                DeprecationWarning,
+            )
+        self._postprocess = postprocess
+
+    def _sq_dist(self, x1, x2, x1_eq_x2=False, postprocess=False):
+        res = sq_dist(x1, x2, x1_eq_x2=x1_eq_x2)
         return self._postprocess(res) if postprocess else res
 
-    def _dist(self, x1, x2, postprocess, x1_eq_x2=False):
-        # TODO: use torch cdist once implementation is improved: https://github.com/pytorch/pytorch/pull/25799
-        res = self._sq_dist(x1, x2, postprocess=False, x1_eq_x2=x1_eq_x2)
-        res = res.clamp_min_(1e-30).sqrt_()
+    def _dist(self, x1, x2, x1_eq_x2=False, postprocess=False):
+        res = dist(x1, x2, x1_eq_x2=x1_eq_x2)
         return self._postprocess(res) if postprocess else res
 
 
 class Kernel(Module):
     r"""
-    Kernels in GPyTorch are implemented as a :class:`gpytorch.Module` that, when called on two :obj:`torch.tensor`
-    objects `x1` and `x2` returns either a :obj:`torch.tensor` or a
+    Kernels in GPyTorch are implemented as a :class:`gpytorch.Module` that, when called on two :class:`torch.Tensor`
+    objects :math:`\mathbf x_1` and :math:`\mathbf x_2` returns either a :obj:`torch.Tensor` or a
     :obj:`~linear_operator.operators.LinearOperator` that represents the
-    covariance matrix between `x1` and `x2`.
+    covariance matrix between :math:`\mathbf x_1` and :math:`\mathbf x_2`.
 
-    In the typical use case, to extend this class means to implement the :func:`~gpytorch.kernels.Kernel.forward`
-    method.
+    In the typical use case, extend this class simply requires implementing a
+    :py:meth:`~gpytorch.kernels.Kernel.forward` method.
 
     .. note::
-        The :func:`~gpytorch.kernels.Kernel.__call__` does some additional internal work. In particular,
-        all kernels are lazily evaluated so that, in some cases, we can index in to the kernel matrix before actually
-        computing it. Furthermore, many built in kernel modules return LinearOperators that allow for more efficient
+        The :py:meth:`~gpytorch.kernels.Kernel.__call__` method does some additional internal work. In particular,
+        all kernels are lazily evaluated so that we can index in to the kernel matrix before actually
+        computing it. Furthermore, many built-in kernel modules return
+        :class:`~linear_operator.LinearOperators` that allow for more efficient
         inference than if we explicitly computed the kernel matrix itself.
 
-        As a result, if you want to use a :obj:`gpytorch.kernels.Kernel` object just to get an actual
+        As a result, if you want to get an actual
         :obj:`torch.tensor` representing the covariance matrix, you may need to call the
         :func:`~linear_operator.operators.LinearOperator.to_dense` method on the output.
 
     This base :class:`Kernel` class includes a lengthscale parameter
     :math:`\Theta`, which is used by many common kernel functions.
     There are a few options for the lengthscale:
 
@@ -89,38 +106,47 @@
       (i.e. :math:`\Theta` is a constant diagonal matrix).
       This is controlled by setting the attribute `has_lengthscale=True`.
 
     * ARD: Each input dimension gets its own separate lengthscale
       (i.e. :math:`\Theta` is a non-constant diagonal matrix).
       This is controlled by the `ard_num_dims` keyword argument (as well as `has_lengthscale=True`).
 
-    In batch-mode (i.e. when :math:`x_1` and :math:`x_2` are batches of input matrices), each
+    In batch mode (i.e. when :math:`\mathbf x_1` and :math:`\mathbf x_2` are batches of input matrices), each
     batch of data can have its own lengthscale parameter by setting the `batch_shape`
     keyword argument to the appropriate number of batches.
 
     .. note::
 
-        The lengthscale parameter is parameterized on a log scale to constrain it to be positive.
-        You can set a prior on this parameter using the lengthscale_prior argument.
+        You can set a prior on the lengthscale parameter using the lengthscale_prior argument.
 
     :param ard_num_dims: Set this if you want a separate lengthscale for each input
-        dimension. It should be `d` if x1 is a `n x d` matrix. (Default: `None`.)
+        dimension. It should be `D` if :math:`\mathbf x` is a `... x N x D` matrix. (Default: `None`.)
     :param batch_shape: Set this if you want a separate lengthscale for each batch of input
-        data. It should be :math:`B_1 \times \ldots \times B_k` if :math:`\mathbf x1` is
+        data. It should be :math:`B_1 \times \ldots \times B_k` if :math:`\mathbf x_1` is
         a :math:`B_1 \times \ldots \times B_k \times N \times D` tensor.
     :param active_dims: Set this if you want to compute the covariance of only
         a few input dimensions. The ints corresponds to the indices of the
         dimensions. (Default: `None`.)
     :param lengthscale_prior: Set this if you want to apply a prior to the
-        lengthscale parameter. (Default: `None`)
+        lengthscale parameter. (Default: `None`.)
     :param lengthscale_constraint: Set this if you want to apply a constraint
-        to the lengthscale parameter. (Default: `Positive`.)
-    :param eps: The minimum value that the lengthscale can take (prevents
-        divide by zero errors). (Default: `1e-6`.)
-
+        to the lengthscale parameter. (Default: :class:`~gpytorch.constraints.Positive`.)
+    :param eps: A small positive value added to the lengthscale to prevent
+        divide by zero errors. (Default: `1e-6`.)
+
+    :ivar torch.Size batch_shape:
+        The (minimum) number of batch dimensions supported by this kernel.
+        Typically, this captures the batch shape of the lengthscale and other parameters,
+        and is usually set by the `batch_shape` argument in the constructor.
+    :ivar torch.dtype dtype:
+        The dtype supported by this kernel.
+        Typically, this depends on the dtype of the lengthscale and other parameters.
+    :ivar bool is_stationary:
+        Set to True if the Kernel represents a stationary function
+        (one that depends only on :math:`\mathbf x_1 - \mathbf x_2`).
     :ivar torch.Tensor lengthscale:
         The lengthscale parameter. Size/shape of parameter depends on the
         `ard_num_dims` and `batch_shape` arguments.
 
     Example:
         >>> covar_module = gpytorch.kernels.LinearKernel()
         >>> x1 = torch.randn(50, 3)
@@ -129,23 +155,23 @@
     """
 
     has_lengthscale = False
 
     def __init__(
         self,
         ard_num_dims: Optional[int] = None,
-        batch_shape: Optional[torch.Size] = torch.Size([]),
+        batch_shape: Optional[torch.Size] = None,
         active_dims: Optional[Tuple[int, ...]] = None,
         lengthscale_prior: Optional[Prior] = None,
         lengthscale_constraint: Optional[Interval] = None,
-        eps: Optional[float] = 1e-6,
+        eps: float = 1e-6,
         **kwargs,
     ):
         super(Kernel, self).__init__()
-        self._batch_shape = batch_shape
+        self._batch_shape = torch.Size([]) if batch_shape is None else batch_shape
         if active_dims is not None and not torch.is_tensor(active_dims):
             active_dims = torch.tensor(active_dims, dtype=torch.long)
         self.register_buffer("active_dims", active_dims)
         self.ard_num_dims = ard_num_dims
 
         self.eps = eps
 
@@ -176,197 +202,287 @@
 
             self.register_constraint("raw_lengthscale", lengthscale_constraint)
 
         self.distance_module = None
         # TODO: Remove this on next official PyTorch release.
         self.__pdist_supports_batch = True
 
+    def _lengthscale_param(self, m: Kernel) -> Tensor:
+        # Used by the lengthscale_prior
+        return m.lengthscale
+
+    def _lengthscale_closure(self, m: Kernel, v: Tensor) -> Tensor:
+        # Used by the lengthscale_prior
+        return m._set_lengthscale(v)
+
+    def _set_lengthscale(self, value: Tensor):
+        # Used by the lengthscale_prior
+        if not self.has_lengthscale:
+            raise RuntimeError("Kernel has no lengthscale.")
+
+        if not torch.is_tensor(value):
+            value = torch.as_tensor(value).to(self.raw_lengthscale)
+
+        self.initialize(raw_lengthscale=self.raw_lengthscale_constraint.inverse_transform(value))
+
     @abstractmethod
-    def forward(self, x1, x2, diag=False, last_dim_is_batch=False, **params):
+    def forward(
+        self, x1: Tensor, x2: Tensor, diag: bool = False, last_dim_is_batch: bool = False, **params
+    ) -> Union[Tensor, LinearOperator]:
         r"""
-        Computes the covariance between x1 and x2.
+        Computes the covariance between :math:`\mathbf x_1` and :math:`\mathbf x_2`.
         This method should be imlemented by all Kernel subclasses.
 
-        Args:
-            x1 (Tensor `n x d` or `b x n x d`):
-                First set of data
-            x2 (Tensor `m x d` or `b x m x d`):
-                Second set of data
-            diag (bool):
-                Should the Kernel compute the whole kernel, or just the diag?
-            last_dim_is_batch (tuple, optional):
-                If this is true, it treats the last dimension of the data as another batch dimension.
-                (Useful for additive structure over the dimensions). Default: False
-
-        Returns:
-            :class:`Tensor` or :class:`~linear_operator.operators.LinearOperator`.
-                The exact size depends on the kernel's evaluation mode:
-
-                * `full_covar`: `n x m` or `b x n x m`
-                * `full_covar` with `last_dim_is_batch=True`: `k x n x m` or `b x k x n x m`
-                * `diag`: `n` or `b x n`
-                * `diag` with `last_dim_is_batch=True`: `k x n` or `b x k x n`
+        :param x1: First set of data (... x N x D).
+        :param x2: Second set of data (... x M x D).
+        :param diag: Should the Kernel compute the whole kernel, or just the diag?
+            If True, it must be the case that `x1 == x2`. (Default: False.)
+        :param last_dim_is_batch: If True, treat the last dimension
+            of `x1` and `x2` as another batch dimension.
+            (Useful for additive structure over the dimensions). (Default: False.)
+
+        :return: The kernel matrix or vector. The shape depends on the kernel's evaluation mode:
+
+            * `full_covar`: `... x N x M`
+            * `full_covar` with `last_dim_is_batch=True`: `... x K x N x M`
+            * `diag`: `... x N`
+            * `diag` with `last_dim_is_batch=True`: `... x K x N`
         """
         raise NotImplementedError()
 
     @property
-    def batch_shape(self):
+    def batch_shape(self) -> torch.Size:
         kernels = list(self.sub_kernels())
         if len(kernels):
             return torch.broadcast_shapes(self._batch_shape, *[k.batch_shape for k in kernels])
         else:
             return self._batch_shape
 
     @batch_shape.setter
-    def batch_shape(self, val):
+    def batch_shape(self, val: torch.Size):
         self._batch_shape = val
 
     @property
-    def dtype(self):
+    def device(self) -> Optional[torch.device]:
         if self.has_lengthscale:
-            return self.lengthscale.dtype
-        else:
-            for param in self.parameters():
-                return param.dtype
-            return torch.get_default_dtype()
+            return self.lengthscale.device
+        devices = {param.device for param in self.parameters()}
+        if len(devices) > 1:
+            raise RuntimeError(f"The kernel's parameters are on multiple devices: {devices}.")
+        elif devices:
+            return devices.pop()
+        return None
 
     @property
-    def is_stationary(self) -> bool:
-        """
-        Property to indicate whether kernel is stationary or not.
-        """
-        return self.has_lengthscale
-
-    def _lengthscale_param(self, m):
-        return m.lengthscale
-
-    def _lengthscale_closure(self, m, v):
-        return m._set_lengthscale(v)
+    def dtype(self) -> torch.dtype:
+        if self.has_lengthscale:
+            return self.lengthscale.dtype
+        dtypes = {param.dtype for param in self.parameters()}
+        if len(dtypes) > 1:
+            raise RuntimeError(f"The kernel's parameters have multiple dtypes: {dtypes}.")
+        elif dtypes:
+            return dtypes.pop()
+        return torch.get_default_dtype()
 
     @property
-    def lengthscale(self):
+    def lengthscale(self) -> Tensor:
         if self.has_lengthscale:
             return self.raw_lengthscale_constraint.transform(self.raw_lengthscale)
         else:
             return None
 
     @lengthscale.setter
-    def lengthscale(self, value):
+    def lengthscale(self, value: Tensor):
         self._set_lengthscale(value)
 
-    def _set_lengthscale(self, value):
-        if not self.has_lengthscale:
-            raise RuntimeError("Kernel has no lengthscale.")
-
-        if not torch.is_tensor(value):
-            value = torch.as_tensor(value).to(self.raw_lengthscale)
-
-        self.initialize(raw_lengthscale=self.raw_lengthscale_constraint.inverse_transform(value))
+    @property
+    def is_stationary(self) -> bool:
+        return self.has_lengthscale
 
-    def local_load_samples(self, samples_dict, memo, prefix):
+    def local_load_samples(self, samples_dict: Dict[str, Tensor], memo: set, prefix: str):
         num_samples = next(iter(samples_dict.values())).size(0)
         self.batch_shape = torch.Size([num_samples]) + self.batch_shape
         super().local_load_samples(samples_dict, memo, prefix)
 
     def covar_dist(
         self,
-        x1,
-        x2,
-        diag=False,
-        last_dim_is_batch=False,
-        square_dist=False,
-        dist_postprocess_func=default_postprocess_script,
-        postprocess=True,
+        x1: Tensor,
+        x2: Tensor,
+        diag: bool = False,
+        last_dim_is_batch: bool = False,
+        square_dist: bool = False,
         **params,
-    ):
+    ) -> Tensor:
         r"""
         This is a helper method for computing the Euclidean distance between
-        all pairs of points in x1 and x2.
+        all pairs of points in :math:`\mathbf x_1` and :math:`\mathbf x_2`.
 
-        Args:
-            x1 (Tensor `n x d` or `b1 x ... x bk x n x d`):
-                First set of data.
-            x2 (Tensor `m x d` or `b1 x ... x bk x m x d`):
-                Second set of data.
-            diag (bool):
-                Should we return the whole distance matrix, or just the diagonal? If True, we must have `x1 == x2`.
-            last_dim_is_batch (tuple, optional):
-                Is the last dimension of the data a batch dimension or not?
-            square_dist (bool):
-                Should we square the distance matrix before returning?
-
-        Returns:
-            (:class:`Tensor`, :class:`Tensor) corresponding to the distance matrix between `x1` and `x2`.
-            The shape depends on the kernel's mode
-            * `diag=False`
-            * `diag=False` and `last_dim_is_batch=True`: (`b x d x n x n`)
-            * `diag=True`
-            * `diag=True` and `last_dim_is_batch=True`: (`b x d x n`)
+        :param x1: First set of data (... x N x D).
+        :param x2: Second set of data (... x M x D).
+        :param diag: Should the Kernel compute the whole kernel, or just the diag?
+            If True, it must be the case that `x1 == x2`. (Default: False.)
+        :param last_dim_is_batch: If True, treat the last dimension
+            of `x1` and `x2` as another batch dimension.
+            (Useful for additive structure over the dimensions). (Default: False.)
+        :param square_dist:
+            If True, returns the squared distance rather than the standard distance. (Default: False.)
+        :return: The kernel matrix or vector. The shape depends on the kernel's evaluation mode:
+
+            * `full_covar`: `... x N x M`
+            * `full_covar` with `last_dim_is_batch=True`: `... x K x N x M`
+            * `diag`: `... x N`
+            * `diag` with `last_dim_is_batch=True`: `... x K x N`
         """
         if last_dim_is_batch:
             x1 = x1.transpose(-1, -2).unsqueeze(-1)
             x2 = x2.transpose(-1, -2).unsqueeze(-1)
 
         x1_eq_x2 = torch.equal(x1, x2)
-
-        # torch scripts expect tensors
-        postprocess = torch.tensor(postprocess)
-
         res = None
 
-        # Cache the Distance object or else JIT will recompile every time
-        if not self.distance_module or self.distance_module._postprocess != dist_postprocess_func:
-            self.distance_module = Distance(dist_postprocess_func)
-
         if diag:
             # Special case the diagonal because we can return all zeros most of the time.
             if x1_eq_x2:
-                res = torch.zeros(*x1.shape[:-2], x1.shape[-2], dtype=x1.dtype, device=x1.device)
-                if postprocess:
-                    res = dist_postprocess_func(res)
-                return res
+                return torch.zeros(*x1.shape[:-2], x1.shape[-2], dtype=x1.dtype, device=x1.device)
             else:
-                res = torch.norm(x1 - x2, p=2, dim=-1)
-                if square_dist:
-                    res = res.pow(2)
-            if postprocess:
-                res = dist_postprocess_func(res)
-            return res
+                res = torch.linalg.norm(x1 - x2, dim=-1)  # 2-norm by default
+                return res.pow(2) if square_dist else res
+        else:
+            dist_func = sq_dist if square_dist else dist
+            return dist_func(x1, x2, x1_eq_x2)
 
-        elif square_dist:
-            res = self.distance_module._sq_dist(x1, x2, postprocess, x1_eq_x2)
+    def expand_batch(self, *sizes: Union[torch.Size, Tuple[int, ...]]) -> Kernel:
+        r"""
+        Constructs a new kernel where the lengthscale (and other kernel parameters)
+        are expanded to match the batch dimension determined by `sizes`.
+
+        :param sizes: The batch shape of the new tensor
+        """
+        # Type checking
+        if len(sizes) == 1 and hasattr(sizes, "__iter__"):
+            new_batch_shape = torch.Size(sizes[0])
+        elif all(isinstance(size, int) for size in sizes):
+            new_batch_shape = torch.Size(sizes)
         else:
-            res = self.distance_module._dist(x1, x2, postprocess, x1_eq_x2)
+            raise RuntimeError("Invalid arguments {} to expand_batch.".format(sizes))
 
-        return res
+        # Check for easy case:
+        orig_batch_shape = self.batch_shape
+        if new_batch_shape == orig_batch_shape:
+            return self
+
+        # Ensure that the expansion size is compatible with the given batch shape
+        try:
+            torch.broadcast_shapes(new_batch_shape, orig_batch_shape)
+        except RuntimeError:
+            raise RuntimeError(
+                f"Cannot expand a kernel with batch shape {self.batch_shape} to new shape {new_batch_shape}"
+            )
+
+        # Create a new kernel with updated batch shape
+        new_kernel = deepcopy(self)
+        new_kernel._batch_shape = new_batch_shape
+
+        # Reshape the parameters of the kernel
+        for param_name, param in self.named_parameters(recurse=False):
+            # For a given parameter, get the number of dimensions that do not correspond to the batch shape
+            non_batch_shape = param.shape[len(orig_batch_shape) :]
+            new_param_shape = torch.Size([*new_batch_shape, *non_batch_shape])
+            new_kernel.__getattr__(param_name).data = param.expand(new_param_shape)
+
+        # Reshape the buffers of the kernel
+        for buffr_name, buffr in self.named_buffers(recurse=False):
+            # For a given buffer, get the number of dimensions that do not correspond to the batch shape
+            non_batch_shape = buffr.shape[len(orig_batch_shape) :]
+            new_buffer_shape = torch.Size([*new_batch_shape, *non_batch_shape])
+            new_kernel.__getattr__(buffr_name).data = buffr.expand(new_buffer_shape)
+
+        # Recurse, if necessary
+        for sub_module_name, sub_module in self.named_sub_kernels():
+            new_kernel.__setattr__(sub_module_name, sub_module.expand_batch(new_batch_shape))
 
-    def named_sub_kernels(self):
+        return new_kernel
+
+    def named_sub_kernels(self) -> Iterable[Tuple[str, Kernel]]:
+        """
+        For compositional Kernel classes (e.g. :class:`~gpytorch.kernels.AdditiveKernel`
+        or :class:`~gpytorch.kernels.ProductKernel`).
+
+        :return: An iterator over the component kernel objects,
+            along with the name of each component kernel.
+        """
         for name, module in self.named_modules():
             if module is not self and isinstance(module, Kernel):
                 yield name, module
 
-    def num_outputs_per_input(self, x1, x2):
+    def num_outputs_per_input(self, x1: Tensor, x2: Tensor) -> int:
         """
-        How many outputs are produced per input (default 1)
-        if x1 is size `n x d` and x2 is size `m x d`, then the size of the kernel
-        will be `(n * num_outputs_per_input) x (m * num_outputs_per_input)`
-        Default: 1
+        For most kernels, `num_outputs_per_input = 1`.
+
+        However, some kernels (e.g. multitask kernels or interdomain kernels) return a
+        `num_outputs_per_input x num_outputs_per_input` matrix of covariance values for
+        every pair of data points.
+
+        I.e. if `x1` is size `... x N x D` and `x2` is size `... x M x D`, then the size of the kernel
+        will be `... x (N * num_outputs_per_input) x (M * num_outputs_per_input)`.
+
+        :return: `num_outputs_per_input` (usually 1).
         """
         return 1
 
-    def prediction_strategy(self, train_inputs, train_prior_dist, train_labels, likelihood):
+    def prediction_strategy(
+        self,
+        train_inputs: Tensor,
+        train_prior_dist: MultivariateNormal,
+        train_labels: Tensor,
+        likelihood: GaussianLikelihood,
+    ) -> exact_prediction_strategies.PredictionStrategy:
         return exact_prediction_strategies.DefaultPredictionStrategy(
             train_inputs, train_prior_dist, train_labels, likelihood
         )
 
-    def sub_kernels(self):
+    def sub_kernels(self) -> Iterable[Kernel]:
+        """
+        For compositional Kernel classes (e.g. :class:`~gpytorch.kernels.AdditiveKernel`
+        or :class:`~gpytorch.kernels.ProductKernel`).
+
+        :return: An iterator over the component kernel objects.
+        """
         for _, kernel in self.named_sub_kernels():
             yield kernel
 
-    def __call__(self, x1, x2=None, diag=False, last_dim_is_batch=False, **params):
+    def __call__(
+        self, x1: Tensor, x2: Optional[Tensor] = None, diag: bool = False, last_dim_is_batch: bool = False, **params
+    ) -> Union[LazyEvaluatedKernelTensor, LinearOperator, Tensor]:
+        r"""
+        Computes the covariance between :math:`\mathbf x_1` and :math:`\mathbf x_2`.
+
+        .. note::
+            Following PyTorch convention, all :class:`~gpytorch.models.GP` objects should use `__call__`
+            rather than :py:meth:`~gpytorch.kernels.Kernel.forward`.
+            The `__call__` method applies additional pre- and post-processing to the `forward` method,
+            and additionally employs a lazy evaluation scheme to reduce memory and computational costs.
+
+        :param x1: First set of data (... x N x D).
+        :param x2: Second set of data (... x M x D).
+            (If `None`, then `x2` is set to `x1`.)
+        :param diag: Should the Kernel compute the whole kernel, or just the diag?
+            If True, it must be the case that `x1 == x2`. (Default: False.)
+        :param last_dim_is_batch: If True, treat the last dimension
+            of `x1` and `x2` as another batch dimension.
+            (Useful for additive structure over the dimensions). (Default: False.)
+
+        :return: An object that will lazily evaluate to the kernel matrix or vector.
+            The shape depends on the kernel's evaluation mode:
+
+            * `full_covar`: `... x N x M`
+            * `full_covar` with `last_dim_is_batch=True`: `... x K x N x M`
+            * `diag`: `... x N`
+            * `diag` with `last_dim_is_batch=True`: `... x K x N`
+        """
         x1_, x2_ = x1, x2
 
         # Select the active dimensions
         if self.active_dims is not None:
             x1_ = x1_.index_select(-1, self.active_dims)
             if x2_ is not None:
                 x2_ = x2_.index_select(-1, self.active_dims)
@@ -410,114 +526,128 @@
             return res
 
     def __getstate__(self):
         # JIT ScriptModules cannot be pickled
         self.distance_module = None
         return self.__dict__
 
-    def __add__(self, other):
+    def __add__(self, other: Kernel) -> Kernel:
         kernels = []
         kernels += self.kernels if isinstance(self, AdditiveKernel) else [self]
         kernels += other.kernels if isinstance(other, AdditiveKernel) else [other]
         return AdditiveKernel(*kernels)
 
-    def __mul__(self, other):
+    def __mul__(self, other: Kernel) -> Kernel:
         kernels = []
         kernels += self.kernels if isinstance(self, ProductKernel) else [self]
         kernels += other.kernels if isinstance(other, ProductKernel) else [other]
         return ProductKernel(*kernels)
 
     def __setstate__(self, d):
         self.__dict__ = d
 
-    def __getitem__(self, index):
+    def __getitem__(self, index) -> Kernel:
+        r"""
+        Constructs a new kernel where the lengthscale (and other kernel parameters)
+        are modified by an indexing operation.
+
+        :param index: Index to apply to all parameters.
+        """
+
         if len(self.batch_shape) == 0:
             return self
 
         new_kernel = deepcopy(self)
         # Process the index
         index = index if isinstance(index, tuple) else (index,)
 
-        for param_name, param in self._parameters.items():
-            new_kernel._parameters[param_name].data = param.__getitem__(index)
-            ndim_removed = len(param.shape) - len(new_kernel._parameters[param_name].shape)
+        for param_name, param in self.named_parameters(recurse=False):
+            new_param = new_kernel.__getattr__(param_name)
+            new_param.data = new_param.__getitem__(index)
+            ndim_removed = len(param.shape) - len(new_param.shape)
+            new_batch_shape_len = len(self.batch_shape) - ndim_removed
+            new_kernel.batch_shape = new_param.shape[:new_batch_shape_len]
+
+        for buffr_name, buffr in self.named_buffers(recurse=False):
+            # For a given buffer, get the number of dimensions that do not correspond to the batch shape
+            new_buffr = new_kernel.__getattr__(buffr_name)
+            new_buffr.data = new_buffr.__getitem__(index)
+            ndim_removed = len(buffr.shape) - len(new_buffr.shape)
             new_batch_shape_len = len(self.batch_shape) - ndim_removed
-            new_kernel.batch_shape = new_kernel._parameters[param_name].shape[:new_batch_shape_len]
+            new_kernel.batch_shape = new_buffr.shape[:new_batch_shape_len]
 
         for sub_module_name, sub_module in self.named_sub_kernels():
-            new_kernel._modules[sub_module_name] = sub_module.__getitem__(index)
+            new_kernel.__setattr__(sub_module_name, sub_module.__getitem__(index))
 
         return new_kernel
 
 
 class AdditiveKernel(Kernel):
     """
     A Kernel that supports summing over multiple component kernels.
 
     Example:
         >>> covar_module = RBFKernel(active_dims=torch.tensor([1])) + RBFKernel(active_dims=torch.tensor([2]))
         >>> x1 = torch.randn(50, 2)
         >>> additive_kernel_matrix = covar_module(x1)
+
+    :param kernels: Kernels to add together.
     """
 
     @property
     def is_stationary(self) -> bool:
-        """
-        Kernel is stationary if all components are stationary.
-        """
         return all(k.is_stationary for k in self.kernels)
 
-    def __init__(self, *kernels):
+    def __init__(self, *kernels: Iterable[Kernel]):
         super(AdditiveKernel, self).__init__()
         self.kernels = ModuleList(kernels)
 
-    def forward(self, x1, x2, diag=False, **params):
+    def forward(self, x1: Tensor, x2: Tensor, diag: bool = False, **params) -> Union[Tensor, LinearOperator]:
         res = ZeroLinearOperator() if not diag else 0
         for kern in self.kernels:
             next_term = kern(x1, x2, diag=diag, **params)
             if not diag:
                 res = res + to_linear_operator(next_term)
             else:
                 res = res + next_term
 
         return res
 
     def num_outputs_per_input(self, x1, x2):
         return self.kernels[0].num_outputs_per_input(x1, x2)
 
-    def __getitem__(self, index):
+    def __getitem__(self, index) -> Kernel:
         new_kernel = deepcopy(self)
         for i, kernel in enumerate(self.kernels):
-            new_kernel.kernels[i] = self.kernels[i].__getitem__(index)
+            new_kernel.kernels[i] = kernel.__getitem__(index)
 
         return new_kernel
 
 
 class ProductKernel(Kernel):
     """
     A Kernel that supports elementwise multiplying multiple component kernels together.
 
     Example:
         >>> covar_module = RBFKernel(active_dims=torch.tensor([1])) * RBFKernel(active_dims=torch.tensor([2]))
         >>> x1 = torch.randn(50, 2)
         >>> kernel_matrix = covar_module(x1) # The RBF Kernel already decomposes multiplicatively, so this is foolish!
+
+    :param kernels: Kernels to multiply together.
     """
 
     @property
     def is_stationary(self) -> bool:
-        """
-        Kernel is stationary if all components are stationary.
-        """
         return all(k.is_stationary for k in self.kernels)
 
-    def __init__(self, *kernels):
+    def __init__(self, *kernels: Iterable[Kernel]):
         super(ProductKernel, self).__init__()
         self.kernels = ModuleList(kernels)
 
-    def forward(self, x1, x2, diag=False, **params):
+    def forward(self, x1: Tensor, x2: Tensor, diag: bool = False, **params) -> Union[Tensor, LinearOperator]:
         x1_eq_x2 = torch.equal(x1, x2)
 
         if not x1_eq_x2:
             # If x1 != x2, then we can't make a MulLinearOperator because the kernel won't necessarily be
             # square/symmetric
             res = to_dense(self.kernels[0](x1, x2, diag=diag, **params))
         else:
@@ -535,16 +665,16 @@
                 if not diag:
                     res = res * to_linear_operator(next_term)
                 else:
                     res = res * next_term
 
         return res
 
-    def num_outputs_per_input(self, x1, x2):
+    def num_outputs_per_input(self, x1: Tensor, x2: Tensor) -> int:
         return self.kernels[0].num_outputs_per_input(x1, x2)
 
-    def __getitem__(self, index):
+    def __getitem__(self, index) -> Kernel:
         new_kernel = deepcopy(self)
         for i, kernel in enumerate(self.kernels):
-            new_kernel.kernels[i] = self.kernels[i].__getitem__(index)
+            new_kernel.kernels[i] = kernel.__getitem__(index)
 
         return new_kernel
```

### Comparing `gpytorch-1.9.0/gpytorch/kernels/lcm_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/lcm_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/linear_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/linear_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/matern_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/matern_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/multi_device_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/multi_device_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/multitask_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/multitask_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/newton_girard_additive_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/newton_girard_additive_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/periodic_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/periodic_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/piecewise_polynomial_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/piecewise_polynomial_kernel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,36 @@
+import math
 from typing import Optional
 
 import torch
+from torch import Tensor
 
 from .kernel import Kernel
 
 
+def _fmax(r: Tensor, j: int, q: int) -> Tensor:
+    return torch.max(torch.tensor(0.0, dtype=r.dtype, device=r.device), 1 - r).pow(j + q)
+
+
+def _get_cov(r: Tensor, j: int, q: int) -> Tensor:
+    if q == 0:
+        return 1
+    if q == 1:
+        return (j + 1) * r + 1
+    if q == 2:
+        return 1 + (j + 2) * r + ((j + 4 * j + 3) / 3.0) * (r**2)
+    if q == 3:
+        return (
+            1
+            + (j + 3) * r
+            + ((6 * j**2 + 36 * j + 45) / 15.0) * r.square()
+            + ((j**3 + 9 * j**2 + 23 * j + 15) / 15.0) * (r**3)
+        )
+
+
 class PiecewisePolynomialKernel(Kernel):
     r"""
     Computes a covariance matrix based on the Piecewise Polynomial kernel
     between inputs :math:`\mathbf{x_1}` and :math:`\mathbf{x_2}`:
 
     .. math::
 
@@ -75,43 +97,25 @@
 
     def __init__(self, q: Optional[int] = 2, **kwargs):
         super(PiecewisePolynomialKernel, self).__init__(**kwargs)
         if q not in {0, 1, 2, 3}:
             raise ValueError("q expected to be 0, 1, 2 or 3")
         self.q = q
 
-    def fmax(self, r, j, q):
-        return torch.max(torch.tensor(0.0), 1 - r).pow(j + q)
-
-    def get_cov(self, r, j, q):
-        if q == 0:
-            return 1
-        if q == 1:
-            return (j + 1) * r + 1
-        if q == 2:
-            return 1 + (j + 2) * r + ((j**2 + 4 * j + 3) / 3.0) * r**2
-        if q == 3:
-            return (
-                1
-                + (j + 3) * r
-                + ((6 * j**2 + 36 * j + 45) / 15.0) * r**2
-                + ((j**3 + 9 * j**2 + 23 * j + 15) / 15.0) * r**3
-            )
-
-    def forward(self, x1, x2, last_dim_is_batch=False, diag=False, **params):
+    def forward(self, x1: Tensor, x2: Tensor, last_dim_is_batch: bool = False, diag: bool = False, **params) -> Tensor:
         x1_ = x1.div(self.lengthscale)
         x2_ = x2.div(self.lengthscale)
         if last_dim_is_batch is True:
             D = x1.shape[1]
         else:
             D = x1.shape[-1]
-        j = torch.floor(torch.tensor(D / 2.0)) + self.q + 1
+        j = math.floor(D / 2.0) + self.q + 1
         if last_dim_is_batch and diag:
             r = self.covar_dist(x1_, x2_, last_dim_is_batch=True, diag=True)
         elif diag:
             r = self.covar_dist(x1_, x2_, diag=True)
         elif last_dim_is_batch:
             r = self.covar_dist(x1_, x2_, last_dim_is_batch=True)
         else:
             r = self.covar_dist(x1_, x2_)
-        cov_matrix = self.fmax(r, j, self.q) * self.get_cov(r, j, self.q)
+        cov_matrix = _fmax(r, j, self.q) * _get_cov(r, j, self.q)
         return cov_matrix
```

### Comparing `gpytorch-1.9.0/gpytorch/kernels/polynomial_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/polynomial_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/polynomial_kernel_grad.py` & `gpytorch-1.9.1/gpytorch/kernels/polynomial_kernel_grad.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/product_structure_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/product_structure_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/rbf_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/rbf_kernel.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,18 +72,14 @@
             or (self.ard_num_dims is not None and self.ard_num_dims > 1)
             or diag
             or params.get("last_dim_is_batch", False)
             or trace_mode.on()
         ):
             x1_ = x1.div(self.lengthscale)
             x2_ = x2.div(self.lengthscale)
-            return self.covar_dist(
-                x1_, x2_, square_dist=True, diag=diag, dist_postprocess_func=postprocess_rbf, postprocess=True, **params
-            )
+            return postprocess_rbf(self.covar_dist(x1_, x2_, square_dist=True, diag=diag, **params))
         return RBFCovariance.apply(
             x1,
             x2,
             self.lengthscale,
-            lambda x1, x2: self.covar_dist(
-                x1, x2, square_dist=True, diag=False, dist_postprocess_func=postprocess_rbf, postprocess=False, **params
-            ),
+            lambda x1, x2: self.covar_dist(x1, x2, square_dist=True, diag=False, **params),
         )
```

### Comparing `gpytorch-1.9.0/gpytorch/kernels/rbf_kernel_grad.py` & `gpytorch-1.9.1/gpytorch/kernels/rbf_kernel_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 
             # Form all possible rank-1 products for the gradient and Hessian blocks
             outer = x1_.view(*batch_shape, n1, 1, d) - x2_.view(*batch_shape, 1, n2, d)
             outer = outer / self.lengthscale.unsqueeze(-2)
             outer = torch.transpose(outer, -1, -2).contiguous()
 
             # 1) Kernel block
-            diff = self.covar_dist(x1_, x2_, square_dist=True, dist_postprocess_func=postprocess_rbf, **params)
-            K_11 = diff
+            diff = self.covar_dist(x1_, x2_, square_dist=True, **params)
+            K_11 = postprocess_rbf(diff)
             K[..., :n1, :n2] = K_11
 
             # 2) First gradient block
             outer1 = outer.view(*batch_shape, n1, n2 * d)
             K[..., :n1, n2:] = outer1 * K_11.repeat([*([1] * (n_batch_dims + 1)), d])
 
             # 3) Second gradient block
```

### Comparing `gpytorch-1.9.0/gpytorch/kernels/rff_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/rff_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/rq_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/rq_kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,24 +59,24 @@
         self.register_parameter(name="raw_alpha", parameter=torch.nn.Parameter(torch.zeros(*self.batch_shape, 1)))
         if alpha_constraint is None:
             alpha_constraint = Positive()
 
         self.register_constraint("raw_alpha", alpha_constraint)
 
     def forward(self, x1, x2, diag=False, **params):
-        def postprocess_rq(dist):
+        def postprocess_rq(dist_mat):
             alpha = self.alpha
-            for _ in range(1, len(dist.shape) - len(self.batch_shape)):
+            for _ in range(1, len(dist_mat.shape) - len(self.batch_shape)):
                 alpha = alpha.unsqueeze(-1)
-            return (1 + dist.div(2 * alpha)).pow(-alpha)
+            return (1 + dist_mat.div(2 * alpha)).pow(-alpha)
 
         x1_ = x1.div(self.lengthscale)
         x2_ = x2.div(self.lengthscale)
-        return self.covar_dist(
-            x1_, x2_, square_dist=True, diag=diag, dist_postprocess_func=postprocess_rq, postprocess=True, **params
+        return postprocess_rq(
+            self.covar_dist(x1_, x2_, square_dist=True, diag=diag, **params),
         )
 
     @property
     def alpha(self):
         return self.raw_alpha_constraint.transform(self.raw_alpha)
 
     @alpha.setter
```

### Comparing `gpytorch-1.9.0/gpytorch/kernels/scale_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/scale_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/spectral_delta_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/spectral_delta_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/kernels/spectral_mixture_kernel.py` & `gpytorch-1.9.1/gpytorch/kernels/spectral_mixture_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/lazy/__init__.py` & `gpytorch-1.9.1/gpytorch/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/lazy/lazy_evaluated_kernel_tensor.py` & `gpytorch-1.9.1/gpytorch/lazy/lazy_evaluated_kernel_tensor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,37 @@
 #!/usr/bin/env python3
 
+import functools
+from typing import Callable
+
 import torch
 from linear_operator import LinearOperator, to_linear_operator
 from linear_operator.utils.getitem import _noop_index
 
 from .. import beta_features, settings
 from ..utils import deprecation
 from ..utils.memoize import cached
 
 
+def recall_grad_state(method: Callable) -> Callable:
+    """Decorator for LazyEvaluatedKernelTensor's methods to put their execution
+    inside the same grad state as during the instantiation of the lazy object.
+    This makes the lazy tensor object behave in the same way as a regular tensor
+    with respect to the grad state.
+    """
+
+    @functools.wraps(method)
+    def wrapped(self, *args, **kwargs):
+        with torch.set_grad_enabled(self._is_grad_enabled):
+            output = method(self, *args, **kwargs)
+        return output
+
+    return wrapped
+
+
 class LazyEvaluatedKernelTensor(LinearOperator):
     _check_size = False
 
     def _check_args(self, x1, x2, kernel, last_dim_is_batch=False, **params):
         if not torch.is_tensor(x1):
             return "x1 must be a tensor. Got {}".format(x1.__class__.__name__)
         if not torch.is_tensor(x2):
@@ -23,14 +42,15 @@
             x1, x2, kernel=kernel, last_dim_is_batch=last_dim_is_batch, **params
         )
         self.kernel = kernel
         self.x1 = x1
         self.x2 = x2
         self.last_dim_is_batch = last_dim_is_batch
         self.params = params
+        self._is_grad_enabled = torch.is_grad_enabled()  # records grad state at instantiation
 
     @property
     def dtype(self):
         return self.kernel.dtype
 
     @property
     def device(self):
@@ -80,14 +100,15 @@
             sub_kernel_outputs = tuple(sub_kernel_matrix.representation())
             torch.autograd.backward(sub_kernel_outputs, sub_grad_outputs)
 
         x1.grad = torch.cat([sub_x1.grad.data for sub_x1 in sub_x1s], dim=-2)
         return x1.grad, x2.grad
 
     @cached(name="kernel_diag")
+    @recall_grad_state
     def _diagonal(self) -> torch.Tensor:
         # Getting the diagonal of a kernel can be handled more efficiently by
         # transposing the batch and data dimension before calling the kernel.
         # Implementing it this way allows us to compute predictions more efficiently
         # in cases where only the variances are required.
         from ..kernels import Kernel
 
@@ -107,27 +128,37 @@
                     "Got size {}".format(self.kernel.__class__.__name__, expected_shape, res.shape)
                 )
 
         if isinstance(res, LinearOperator):
             res = res.to_dense()
         return res.view(self.shape[:-1]).contiguous()
 
-    def _expand_batch(self, batch_shape):
-        return self.evaluate_kernel()._expand_batch(batch_shape)
-
+    @recall_grad_state
     def _getitem(self, row_index, col_index, *batch_indices):
         x1 = self.x1
         x2 = self.x2
         num_outs_per_in = self.kernel.num_outputs_per_input(x1, x2)
         if isinstance(num_outs_per_in, tuple):
             num_outs_per_in_rows, num_outs_per_in_cols = num_outs_per_in
         else:
             num_outs_per_in_rows = num_outs_per_in
             num_outs_per_in_cols = num_outs_per_in
 
+        # We will be running the __getitem__ command on x1, x2, and the kernel parameters
+        # Since kernels can broadcast, x1, x2, and the kernel parameters may not have all of the batch dimensions
+        # that are being indexed by the __getitem__ operation
+        # Therefore, we begin by figuring out the broadcasted shape, and expanding all of these objects to that shape
+        try:
+            batch_shape = torch.broadcast_shapes(x1.shape[:-2], x2.shape[:-2], self.kernel.batch_shape)
+        except RuntimeError:
+            raise RuntimeError(
+                f"The kernel inputs (sizes {x1.shape} and {x2.shape}) are incompatible with the kernel "
+                f"(batch size {self.kernel.batch_shape}). This is likely a bug in GPyTorch."
+            )
+
         # The row index and col index should exactly correspond to which entries of x1 and x2 we need
         # So we'll basically call x1[*batch_indices, row_index, :], x2[*batch_indices, col_index, :]
 
         # However - if we have multiple outputs per input, then the indices won't directly
         # correspond to the entries of row/col. We'll have to do a little pre-processing
         if num_outs_per_in_rows != 1 or num_outs_per_in_cols != 1:
             if not isinstance(x1, slice) or not isinstance(x2, slice):
@@ -170,46 +201,41 @@
             dim_index = _noop_index
 
         # Get the indices of x1 and x2 that matter for the kernel
         # Call x1[*batch_indices, row_index, :]
         try:
             x1 = x1[(*batch_indices, row_index, dim_index)]
         # We're going to handle multi-batch indexing with a try-catch loop
-        # This way - in the default case, we can avoid doing expansions of x1 which can be timely
+        # This way - in the default case, we can avoid doing expansions of x1 which can be
+        # costly in terms of time
         except IndexError:
-            if any(not isinstance(bi, slice) for bi in batch_indices):
-                raise RuntimeError(
-                    "Attempting to tensor index a non-batch matrix's batch dimensions. "
-                    f"Got batch index {batch_indices} but my shape was {self.shape}"
-                )
-            x1 = x1.expand(*([1] * (len(batch_indices) - self.x1.dim() + 2)), *self.x1.shape)
+            x1 = x1.expand(*batch_shape, *x1.shape[-2:])
             x1 = x1[(*batch_indices, row_index, dim_index)]
 
         # Call x2[*batch_indices, col_index, :]
         try:
             x2 = x2[(*batch_indices, col_index, dim_index)]
         # We're going to handle multi-batch indexing with a try-catch loop
-        # This way - in the default case, we can avoid doing expansions of x1 which can be timely
+        # This way - in the default case, we can avoid doing expansions of x2 which can be
+        # costly in terms of time
         except IndexError:
-            if any(not isinstance(bi, slice) for bi in batch_indices):
-                raise RuntimeError(
-                    "Attempting to tensor index a non-batch matrix's batch dimensions. "
-                    f"Got batch index {batch_indices} but my shape was {self.shape}"
-                )
-            x2 = x2.expand(*([1] * (len(batch_indices) - self.x2.dim() + 2)), *self.x2.shape)
+            x2 = x2.expand(*batch_shape, *x2.shape[-2:])
             x2 = x2[(*batch_indices, col_index, dim_index)]
 
         if len(batch_indices) == 0 or all(ind == slice(None, None, None) for ind in batch_indices):
             new_kernel = self.kernel  # Avoid unnecessary copying when we aren't explicitly indexing batch dims
         else:
-            # Deal with the fact that the batch shape could be different from the kernel's batch shape
-            # (e.g. this can happen due to broadcasting)
-            while len(batch_indices) > len(self.kernel._batch_shape) and batch_indices[0] == _noop_index:
-                batch_indices = batch_indices[1:]
-            new_kernel = self.kernel.__getitem__(batch_indices)
+            try:
+                new_kernel = self.kernel.__getitem__(batch_indices)
+            # We're going to handle multi-batch indexing with a try-catch loop
+            # This way - in the default case, we can avoid doing expansions of self.kernel which can be
+            # costly in terms of time
+            except IndexError:
+                expanded_kernel = self.kernel.expand_batch(batch_shape)
+                new_kernel = expanded_kernel.__getitem__(batch_indices)
 
         # Now construct a kernel with those indices
         return self.__class__(
             x1,
             x2,
             kernel=new_kernel,
             last_dim_is_batch=self.last_dim_is_batch,
@@ -287,38 +313,38 @@
                 )
 
         # Handle when the last dim is batch
         if self.last_dim_is_batch:
             expected_size = expected_size[:-2] + x1.shape[-1:] + expected_size[-2:]
         return expected_size
 
+    @recall_grad_state
     def _transpose_nonbatch(self):
         return self.__class__(
             self.x2,
             self.x1,
             kernel=self.kernel,
             last_dim_is_batch=self.last_dim_is_batch,
             **self.params,
         )
 
-    def add_jitter(self, jitter_val=1e-3):
-        return self.evaluate_kernel().add_jitter(jitter_val)
-
+    @recall_grad_state
     def _unsqueeze_batch(self, dim):
         x1 = self.x1.unsqueeze(dim)
         x2 = self.x2.unsqueeze(dim)
         return self.__class__(
             x1,
             x2,
             kernel=self.kernel,
             last_dim_is_batch=self.last_dim_is_batch,
             **self.params,
         )
 
     @cached(name="kernel_eval")
+    @recall_grad_state
     def evaluate_kernel(self):
         """
         NB: This is a meta LinearOperator, in the sense that evaluate can return
         a LinearOperator if the kernel being evaluated does so.
         """
         x1 = self.x1
         x2 = self.x2
@@ -341,14 +367,15 @@
                 raise RuntimeError(
                     f"The expected shape of the kernel was {self.shape}, but got {res.shape}. "
                     "This is likely a bug in GPyTorch."
                 )
 
         return to_linear_operator(res)
 
+    @recall_grad_state
     def repeat(self, *repeats):
         if len(repeats) == 1 and hasattr(repeats[0], "__iter__"):
             repeats = repeats[0]
         *batch_repeat, row_repeat, col_repeat = repeats
 
         x1 = self.x1.repeat(*batch_repeat, row_repeat, 1)
         x2 = self.x2.repeat(*batch_repeat, col_repeat, 1)
@@ -378,14 +405,15 @@
         else:
             return self.evaluate_kernel().representation_tree()
 
     @cached
     def to_dense(self):
         return self.evaluate_kernel().to_dense()
 
+    @recall_grad_state
     def __getitem__(self, index):
         """
         Supports subindexing of the matrix this LinearOperator represents. This may return either another
         :obj:`~linear_operator.operators.LinearOperator` or a :obj:`torch.tensor` depending on the exact implementation.
         """
         # Process the index
         index = index if isinstance(index, tuple) else (index,)
```

### Comparing `gpytorch-1.9.0/gpytorch/lazy/lazy_tensor.py` & `gpytorch-1.9.1/gpytorch/lazy/lazy_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,19 @@
             return self.eigvalsh(), None
 
     def __getattr__(self, name):
         if "lazy_tensor" in name:
             new_name = name.replace("lazy_tensor", "linear_op")
             if hasattr(self, new_name):
                 warnings.warn(
-                    f"The property {self.__class__.__name__}#{name} is depreated. Use "
+                    f"The property {self.__class__.__name__}#{name} is deprecated. Use "
                     f"{self.__class__.__name__}#{new_name} instead."
                 )
                 return getattr(self, new_name)
-        raise AttributeError("Unknown attribute {name} for {self.__name__.__class__}")
+        raise AttributeError(f"Unknown attribute {name} for {self.__class__.__name__}")
 
     _add_deprecated_method(_LinearOperatorClass, "_approx_diag", "_approx_diagonal")
     _add_deprecated_method(_LinearOperatorClass, "_quad_form_derivative", "_bilinear_derivative")
     _add_deprecated_method(_LinearOperatorClass, "add_diag", "add_diagonal")
     _add_deprecated_method(_LinearOperatorClass, "diag", "diagonal")
     _add_deprecated_method(_LinearOperatorClass, "evaluate", "to_dense")
     _add_deprecated_method(_LinearOperatorClass, "inv_matmul", "solve")
```

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/__init__.py` & `gpytorch-1.9.1/gpytorch/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/bernoulli_likelihood.py` & `gpytorch-1.9.1/gpytorch/likelihoods/bernoulli_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/beta_likelihood.py` & `gpytorch-1.9.1/gpytorch/likelihoods/beta_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/gaussian_likelihood.py` & `gpytorch-1.9.1/gpytorch/likelihoods/gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/laplace_likelihood.py` & `gpytorch-1.9.1/gpytorch/likelihoods/laplace_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/likelihood.py` & `gpytorch-1.9.1/gpytorch/likelihoods/likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/likelihood_list.py` & `gpytorch-1.9.1/gpytorch/likelihoods/likelihood_list.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/multitask_gaussian_likelihood.py` & `gpytorch-1.9.1/gpytorch/likelihoods/multitask_gaussian_likelihood.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,33 +88,34 @@
         :class:`gpytorch.likelihoods.GaussianLikelihood` that we extend.
 
         The final covariance matrix after this method is then
         :math:`\mathbf K + \mathbf D_{t} \otimes \mathbf I_{n} + \sigma^{2} \mathbf I_{nt}`.
 
         :param function_dist: Random variable whose covariance
             matrix is a :obj:`~linear_operator.operators.LinearOperator` we intend to augment.
-        Returns:
-            :obj:`gpytorch.distributions.MultitaskMultivariateNormal`:
+        :rtype: `gpytorch.distributions.MultitaskMultivariateNormal`:
         :return: A new random variable whose covariance matrix is a
             :obj:`~linear_operator.operators.LinearOperator` with
             :math:`\mathbf D_{t} \otimes \mathbf I_{n}` and :math:`\sigma^{2} \mathbf I_{nt}` added.
         """
         mean, covar = function_dist.mean, function_dist.lazy_covariance_matrix
 
         # ensure that sumKroneckerLT is actually called
         if isinstance(covar, LazyEvaluatedKernelTensor):
             covar = covar.evaluate_kernel()
 
-        covar_kron_lt = self._shaped_noise_covar(mean.shape, add_noise=self.has_global_noise)
+        covar_kron_lt = self._shaped_noise_covar(
+            mean.shape, add_noise=self.has_global_noise, interleaved=function_dist._interleaved
+        )
         covar = covar + covar_kron_lt
 
-        return function_dist.__class__(mean, covar)
+        return function_dist.__class__(mean, covar, interleaved=function_dist._interleaved)
 
     def _shaped_noise_covar(
-        self, shape: torch.Size, add_noise: Optional[bool] = True, *params, **kwargs
+        self, shape: torch.Size, add_noise: Optional[bool] = True, interleaved: bool = True, *params, **kwargs
     ) -> LinearOperator:
         if not self.has_task_noise:
             noise = ConstantDiagLinearOperator(self.noise, diag_shape=shape[-2] * self.num_tasks)
             return noise
 
         if self.rank == 0:
             task_noises = self.raw_task_noises_constraint.transform(self.raw_task_noises)
@@ -136,15 +137,18 @@
         # I \kron D_T + \sigma^2 I_{NT} = I \kron (D_T + \sigma^2 I)
         # which allows us to move the latent noise inside the task dependent noise
         # thereby allowing exploitation of Kronecker structure in this likelihood.
         if add_noise and self.has_global_noise:
             noise = ConstantDiagLinearOperator(self.noise, diag_shape=task_var_lt.shape[-1])
             task_var_lt = task_var_lt + noise
 
-        covar_kron_lt = ckl_init(eye_lt, task_var_lt)
+        if interleaved:
+            covar_kron_lt = ckl_init(eye_lt, task_var_lt)
+        else:
+            covar_kron_lt = ckl_init(task_var_lt, eye_lt)
 
         return covar_kron_lt
 
     def forward(self, function_samples: Tensor, *params: Any, **kwargs: Any) -> base_distributions.Normal:
         noise = self._shaped_noise_covar(function_samples.shape, *params, **kwargs).diagonal(dim1=-1, dim2=-2)
         noise = noise.reshape(*noise.shape[:-1], *function_samples.shape[-2:])
         return base_distributions.Independent(base_distributions.Normal(function_samples, noise.sqrt()), 1)
```

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/noise_models.py` & `gpytorch-1.9.1/gpytorch/likelihoods/noise_models.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/softmax_likelihood.py` & `gpytorch-1.9.1/gpytorch/likelihoods/softmax_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/likelihoods/student_t_likelihood.py` & `gpytorch-1.9.1/gpytorch/likelihoods/student_t_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/means/constant_mean.py` & `gpytorch-1.9.1/gpytorch/means/constant_mean.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/means/constant_mean_grad.py` & `gpytorch-1.9.1/gpytorch/means/constant_mean_grad.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/means/linear_mean.py` & `gpytorch-1.9.1/gpytorch/means/linear_mean.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/means/multitask_mean.py` & `gpytorch-1.9.1/gpytorch/means/multitask_mean.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/means/zero_mean.py` & `gpytorch-1.9.1/gpytorch/means/zero_mean.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/metrics/metrics.py` & `gpytorch-1.9.1/gpytorch/metrics/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     Gaussian Processes for Machine Learning,
     Carl Edward Rasmussen and Christopher K. I. Williams,
     The MIT Press, 2006. ISBN 0-262-18253-X
     """
     combine_dim = -2 if isinstance(pred_dist, MultitaskMultivariateNormal) else -1
     f_mean = pred_dist.mean
     f_var = pred_dist.variance
-    return 0.5 * (torch.log(2 * pi * f_var) + torch.square(test_y - f_mean) / (2 * f_var)).mean(dim=combine_dim)
+    return (0.5 * torch.log(2 * pi * f_var) + torch.square(test_y - f_mean) / (2 * f_var)).mean(dim=combine_dim)
 
 
 def quantile_coverage_error(
     pred_dist: MultivariateNormal,
     test_y: torch.Tensor,
     quantile: float = 95.0,
 ):
```

### Comparing `gpytorch-1.9.0/gpytorch/mlls/__init__.py` & `gpytorch-1.9.1/gpytorch/mlls/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/_approximate_mll.py` & `gpytorch-1.9.1/gpytorch/mlls/_approximate_mll.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/deep_approximate_mll.py` & `gpytorch-1.9.1/gpytorch/mlls/deep_approximate_mll.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/deep_predictive_log_likelihood.py` & `gpytorch-1.9.1/gpytorch/mlls/deep_predictive_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/exact_marginal_log_likelihood.py` & `gpytorch-1.9.1/gpytorch/mlls/exact_marginal_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/gamma_robust_variational_elbo.py` & `gpytorch-1.9.1/gpytorch/mlls/gamma_robust_variational_elbo.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/leave_one_out_pseudo_likelihood.py` & `gpytorch-1.9.1/gpytorch/mlls/leave_one_out_pseudo_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/marginal_log_likelihood.py` & `gpytorch-1.9.1/gpytorch/mlls/marginal_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/predictive_log_likelihood.py` & `gpytorch-1.9.1/gpytorch/mlls/predictive_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/sum_marginal_log_likelihood.py` & `gpytorch-1.9.1/gpytorch/mlls/sum_marginal_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/mlls/variational_elbo.py` & `gpytorch-1.9.1/gpytorch/mlls/variational_elbo.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/__init__.py` & `gpytorch-1.9.1/gpytorch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/approximate_gp.py` & `gpytorch-1.9.1/gpytorch/models/approximate_gp.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/deep_gps/__init__.py` & `gpytorch-1.9.1/gpytorch/models/deep_gps/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/deep_gps/deep_gp.py` & `gpytorch-1.9.1/gpytorch/models/deep_gps/deep_gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         # Repeat the input for all possible outputs
         if self.output_dims is not None:
             inputs = inputs.unsqueeze(-3)
             inputs = inputs.expand(*inputs.shape[:-3], self.output_dims, *inputs.shape[-2:])
 
         # Now run samples through the GP
-        output = ApproximateGP.__call__(self, inputs)
+        output = ApproximateGP.__call__(self, inputs, **kwargs)
         if self.output_dims is not None:
             mean = output.loc.transpose(-1, -2)
             covar = BlockDiagLinearOperator(output.lazy_covariance_matrix, block_dim=-3)
             output = MultitaskMultivariateNormal(mean, covar, interleaved=False)
 
         # Maybe expand inputs?
         if deterministic_inputs:
```

### Comparing `gpytorch-1.9.0/gpytorch/models/deep_gps/dspp.py` & `gpytorch-1.9.1/gpytorch/models/deep_gps/dspp.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/exact_gp.py` & `gpytorch-1.9.1/gpytorch/models/exact_gp.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/exact_prediction_strategies.py` & `gpytorch-1.9.1/gpytorch/models/exact_prediction_strategies.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     InterpolatedLinearOperator,
     LinearOperator,
     LowRankRootAddedDiagLinearOperator,
     MatmulLinearOperator,
     RootLinearOperator,
     ZeroLinearOperator,
 )
+from linear_operator.utils.cholesky import psd_safe_cholesky
 from linear_operator.utils.interpolation import left_interp, left_t_interp
 from torch import Tensor
 
 from .. import settings
 from ..lazy import LazyEvaluatedKernelTensor
-from ..utils.cholesky import psd_safe_cholesky
 from ..utils.memoize import add_to_cache, cached, clear_cache_hook, pop_from_cache
 
 
 def prediction_strategy(train_inputs, train_prior_dist, train_labels, likelihood):
     train_train_covar = train_prior_dist.lazy_covariance_matrix
     if isinstance(train_train_covar, LazyEvaluatedKernelTensor):
         cls = train_train_covar.kernel.prediction_strategy
```

### Comparing `gpytorch-1.9.0/gpytorch/models/gplvm/bayesian_gplvm.py` & `gpytorch-1.9.1/gpytorch/models/gplvm/bayesian_gplvm.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/gplvm/latent_variable.py` & `gpytorch-1.9.1/gpytorch/models/gplvm/latent_variable.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/model_list.py` & `gpytorch-1.9.1/gpytorch/models/model_list.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/pyro/__init__.py` & `gpytorch-1.9.1/gpytorch/models/pyro/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/pyro/_pyro_mixin.py` & `gpytorch-1.9.1/gpytorch/models/pyro/_pyro_mixin.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/models/pyro/pyro_gp.py` & `gpytorch-1.9.1/gpytorch/models/pyro/pyro_gp.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/module.py` & `gpytorch-1.9.1/gpytorch/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,25 +353,28 @@
             raise RuntimeError("Unknown prior name '{}'".format(prior_name))
         prior, _, setting_closure = self._priors[prior_name]
         if setting_closure is None:
             raise RuntimeError("Must provide inverse transform to be able to sample from prior.")
         setting_closure(self, prior.sample())
 
     def to_pyro_random_module(self):
-        pyro_random_module_cls = type("_Pyro" + self.__class__.__name__, (RandomModuleMixin, self.__class__), {})
-        if not isinstance(self, pyro_random_module_cls):
+        return self.to_random_module()
+
+    def to_random_module(self):
+        random_module_cls = type("_Random" + self.__class__.__name__, (RandomModuleMixin, self.__class__), {})
+        if not isinstance(self, random_module_cls):
             new_module = copy.deepcopy(self)
-            new_module.__class__ = pyro_random_module_cls  # hack
+            new_module.__class__ = random_module_cls  # hack
         else:
             # Unclear if this branch would ever get used in practice, but it semantically makes sense to have.
             new_module = copy.deepcopy(self)
 
         for mname, child in new_module.named_children():
             if isinstance(child, Module):
-                setattr(new_module, mname, child.to_pyro_random_module())
+                setattr(new_module, mname, child.to_random_module())
 
         return new_module
 
     def pyro_sample_from_prior(self):
         """
         For each parameter in this Module and submodule that have defined priors, sample a value for that parameter
         from its corresponding prior with a pyro.sample primitive and load the resulting value in to the parameter.
```

### Comparing `gpytorch-1.9.0/gpytorch/optim/ngd.py` & `gpytorch-1.9.1/gpytorch/optim/ngd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-from typing import Iterable, Union
+from typing import Callable, Iterable, Optional, Union
 
 import torch
 
 
 class NGD(torch.optim.Optimizer):
     r"""Implements a natural gradient descent step.
     It **can only** be used in conjunction with a :obj:`~gpytorch.variational._NaturalVariationalDistribution`.
@@ -24,16 +24,21 @@
     """
 
     def __init__(self, params: Iterable[Union[torch.nn.Parameter, dict]], num_data: int, lr: float = 0.1):
         self.num_data = num_data
         super().__init__(params, defaults=dict(lr=lr))
 
     @torch.no_grad()
-    def step(self) -> None:
-        """Performs a single optimization step."""
+    def step(self, closure: Optional[Callable] = None) -> None:
+        """
+        Performs a single optimization step.
+
+        (Note that the :attr:`closure` argument is not used by this optimizer; it is simply included to be
+        compatible with the PyTorch optimizer API.)
+        """
         for group in self.param_groups:
             for p in group["params"]:
                 if p.grad is None:
                     continue
                 p.add_(p.grad, alpha=(-group["lr"] * self.num_data))
 
         return None
```

### Comparing `gpytorch-1.9.0/gpytorch/priors/__init__.py` & `gpytorch-1.9.1/gpytorch/priors/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 from .horseshoe_prior import HorseshoePrior
 from .lkj_prior import LKJCholeskyFactorPrior, LKJCovariancePrior, LKJPrior
 from .prior import Prior
 from .smoothed_box_prior import SmoothedBoxPrior
 from .torch_priors import (
     GammaPrior,
     HalfCauchyPrior,
+    HalfNormalPrior,
     LogNormalPrior,
     MultivariateNormalPrior,
     NormalPrior,
     UniformPrior,
 )
 
 # from .wishart_prior import InverseWishartPrior, WishartPrior
 
 
 __all__ = [
     "Prior",
     "GammaPrior",
     "HalfCauchyPrior",
+    "HalfNormalPrior",
     "HorseshoePrior",
     "LKJPrior",
     "LKJCholeskyFactorPrior",
     "LKJCovariancePrior",
     "LogNormalPrior",
     "MultivariateNormalPrior",
     "NormalPrior",
```

### Comparing `gpytorch-1.9.0/gpytorch/priors/horseshoe_prior.py` & `gpytorch-1.9.1/gpytorch/priors/horseshoe_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/priors/lkj_prior.py` & `gpytorch-1.9.1/gpytorch/priors/lkj_prior.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import torch
+from linear_operator.utils.cholesky import psd_safe_cholesky
 from torch.distributions import LKJCholesky, constraints
 from torch.nn import Module as TModule
 
 from .. import settings
-from ..utils.cholesky import psd_safe_cholesky
 from .prior import Prior
 
 
 class LKJCholeskyFactorPrior(Prior, LKJCholesky):
     r"""LKJ prior over n x n (positive definite) Cholesky-decomposed
     correlation matrices
```

### Comparing `gpytorch-1.9.0/gpytorch/priors/prior.py` & `gpytorch-1.9.1/gpytorch/priors/prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/priors/smoothed_box_prior.py` & `gpytorch-1.9.1/gpytorch/priors/smoothed_box_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/priors/torch_priors.py` & `gpytorch-1.9.1/gpytorch/priors/torch_priors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 import torch
-from torch.distributions import Gamma, HalfCauchy, LogNormal, MultivariateNormal, Normal, Uniform
+from torch.distributions import Gamma, HalfCauchy, HalfNormal, LogNormal, MultivariateNormal, Normal, Uniform
 from torch.nn import Module as TModule
 
 from .prior import Prior
 from .utils import _bufferize_attributes, _del_attributes
 
 MVN_LAZY_PROPERTIES = ("covariance_matrix", "scale_tril", "precision_matrix")
 
@@ -26,14 +26,30 @@
         self._transform = transform
 
     def expand(self, batch_shape):
         batch_shape = torch.Size(batch_shape)
         return NormalPrior(self.loc.expand(batch_shape), self.scale.expand(batch_shape))
 
 
+class HalfNormalPrior(Prior, HalfNormal):
+    """
+    Half-Normal prior.
+    pdf(x) = 2 * (2 * pi * scale^2)^-0.5 * exp(-x^2 / (2 * scale^2)) for x >= 0; 0 for x < 0
+    where scale^2 is the variance.
+    """
+
+    def __init__(self, scale, validate_args=None, transform=None):
+        TModule.__init__(self)
+        HalfNormal.__init__(self, scale=scale, validate_args=validate_args)
+        self._transform = transform
+
+    def expand(self, batch_shape):
+        return HalfNormal(self.scale.expand(batch_shape))
+
+
 class LogNormalPrior(Prior, LogNormal):
     """
     Log Normal prior.
     """
 
     def __init__(self, loc, scale, validate_args=None, transform=None):
         TModule.__init__(self)
@@ -67,15 +83,15 @@
 
     def __init__(self, scale, validate_args=None, transform=None):
         TModule.__init__(self)
         HalfCauchy.__init__(self, scale=scale, validate_args=validate_args)
         self._transform = transform
 
     def expand(self, batch_shape):
-        return HalfCauchy(self.loc.expand(batch_shape), self.scale.expand(batch_shape))
+        return HalfCauchyPrior(self.scale.expand(batch_shape))
 
 
 class GammaPrior(Prior, Gamma):
     """Gamma Prior parameterized by concentration and rate
 
     pdf(x) = beta^alpha / Gamma(alpha) * x^(alpha - 1) * exp(-beta * x)
```

### Comparing `gpytorch-1.9.0/gpytorch/priors/utils.py` & `gpytorch-1.9.1/gpytorch/priors/utils.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/priors/wishart_prior.py` & `gpytorch-1.9.1/gpytorch/priors/wishart_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/settings.py` & `gpytorch-1.9.1/gpytorch/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -52,21 +52,21 @@
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
+        self._orig_float_value = self.__class__.value(torch.float)
+        self._instance_float_value = float_value if float_value is not None else self._orig_float_value
+        self._orig_double_value = self.__class__.value(torch.double)
+        self._instance_double_value = double_value if double_value is not None else self._orig_double_value
+        self._orig_half_value = self.__class__.value(torch.half)
+        self._instance_half_value = half_value if half_value is not None else self._orig_half_value
 
     def __enter__(
         self,
     ):
         self.__class__._set_value(
             self._instance_float_value,
             self._instance_double_value,
@@ -381,14 +381,30 @@
 
     (Default: False)
     """
 
     _default = False
 
 
+class variational_cholesky_jitter(_dtype_value_context):
+    """
+    The jitter value used for Cholesky factorizations in variational models.
+
+    - Default for `float`: 1e-4
+    - Default for `double`: 1e-6
+    """
+
+    _global_float_value = 1e-4
+    _global_double_value = 1e-6
+
+    @classmethod
+    def value(cls, dtype=None):
+        return super().value(dtype=dtype)
+
+
 __all__ = [
     "_linalg_dtype_symeig",
     "_linalg_dtype_cholesky",
     "cg_tolerance",
     "cholesky_jitter",
     "cholesky_max_tries",
     "ciq_samples",
@@ -420,9 +436,10 @@
     "sgpr_diagonal_correction",
     "skip_logdet_forward",
     "skip_posterior_variances",
     "terminate_cg_by_size",
     "trace_mode",
     "tridiagonal_jitter",
     "use_toeplitz",
+    "variational_cholesky_jitter",
     "verbose_linalg",
 ]
```

### Comparing `gpytorch-1.9.0/gpytorch/test/base_kernel_test_case.py` & `gpytorch-1.9.1/test/kernels/test_spectral_mixture_kernel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,167 +1,139 @@
 #!/usr/bin/env python3
 
-import pickle
-from abc import abstractmethod
+import unittest
 
 import torch
 
-from .base_test_case import BaseTestCase
+from gpytorch.kernels import SpectralMixtureKernel
 
 
-class BaseKernelTestCase(BaseTestCase):
-    @abstractmethod
-    def create_kernel_no_ard(self, **kwargs):
-        raise NotImplementedError()
-
-    def create_kernel_ard(self, num_dims, **kwargs):
-        raise NotImplementedError()
+class TestSpectralMixtureKernel(unittest.TestCase):
+    def create_kernel(self, num_dims, **kwargs):
+        return SpectralMixtureKernel(num_mixtures=5, ard_num_dims=num_dims, **kwargs)
 
     def create_data_no_batch(self):
         return torch.randn(50, 10)
 
     def create_data_single_batch(self):
-        return torch.randn(2, 3, 2)
+        return torch.randn(2, 50, 2)
 
     def create_data_double_batch(self):
         return torch.randn(3, 2, 50, 2)
 
     def test_active_dims_list(self):
-        kernel = self.create_kernel_no_ard(active_dims=[0, 2, 4, 6])
         x = self.create_data_no_batch()
+        kernel = self.create_kernel(num_dims=4, active_dims=[0, 2, 4, 6])
+        y = torch.randn_like(x[..., 0])
+        kernel.initialize_from_data(x, y)
+        kernel.initialize_from_data_empspect(x, y)
+
         covar_mat = kernel(x).evaluate_kernel().to_dense()
-        kernel_basic = self.create_kernel_no_ard()
+        kernel_basic = self.create_kernel(num_dims=4)
+        kernel_basic.raw_mixture_weights.data = kernel.raw_mixture_weights
+        kernel_basic.raw_mixture_means.data = kernel.raw_mixture_means
+        kernel_basic.raw_mixture_scales.data = kernel.raw_mixture_scales
         covar_mat_actual = kernel_basic(x[:, [0, 2, 4, 6]]).evaluate_kernel().to_dense()
 
-        self.assertAllClose(covar_mat, covar_mat_actual, rtol=1e-3, atol=1e-5)
+        self.assertLess(torch.norm(covar_mat - covar_mat_actual) / covar_mat_actual.norm(), 1e-4)
 
     def test_active_dims_range(self):
         active_dims = list(range(3, 9))
-        kernel = self.create_kernel_no_ard(active_dims=active_dims)
         x = self.create_data_no_batch()
+        kernel = self.create_kernel(num_dims=6, active_dims=active_dims)
+        y = torch.randn_like(x[..., 0])
+        kernel.initialize_from_data(x, y)
+        kernel.initialize_from_data_empspect(x, y)
+
         covar_mat = kernel(x).evaluate_kernel().to_dense()
-        kernel_basic = self.create_kernel_no_ard()
+        kernel_basic = self.create_kernel(num_dims=6)
+        kernel_basic.raw_mixture_weights.data = kernel.raw_mixture_weights
+        kernel_basic.raw_mixture_means.data = kernel.raw_mixture_means
+        kernel_basic.raw_mixture_scales.data = kernel.raw_mixture_scales
         covar_mat_actual = kernel_basic(x[:, active_dims]).evaluate_kernel().to_dense()
 
-        self.assertAllClose(covar_mat, covar_mat_actual, rtol=1e-3, atol=1e-5)
+        self.assertLess(torch.norm(covar_mat - covar_mat_actual) / covar_mat_actual.norm(), 1e-4)
 
-    def test_no_batch_kernel_single_batch_x_no_ard(self):
-        kernel = self.create_kernel_no_ard()
+    def test_no_batch_kernel_single_batch_x(self):
         x = self.create_data_single_batch()
+        kernel = self.create_kernel(num_dims=x.size(-1))
+        y = torch.randn_like(x[..., 0])
+        kernel.initialize_from_data(x, y)
+        kernel.initialize_from_data_empspect(x, y)
         batch_covar_mat = kernel(x).evaluate_kernel().to_dense()
 
         actual_mat_1 = kernel(x[0]).evaluate_kernel().to_dense()
         actual_mat_2 = kernel(x[1]).evaluate_kernel().to_dense()
         actual_covar_mat = torch.cat([actual_mat_1.unsqueeze(0), actual_mat_2.unsqueeze(0)])
 
-        self.assertAllClose(batch_covar_mat, actual_covar_mat, rtol=1e-3, atol=1e-5)
+        self.assertLess(torch.norm(batch_covar_mat - actual_covar_mat) / actual_covar_mat.norm(), 1e-4)
 
         # Test diagonal
         kernel_diag = kernel(x, diag=True)
         actual_diag = actual_covar_mat.diagonal(dim1=-1, dim2=-2)
-        self.assertAllClose(kernel_diag, actual_diag, rtol=1e-3, atol=1e-5)
+        self.assertLess(torch.norm(kernel_diag - actual_diag) / actual_diag.norm(), 1e-4)
 
-    def test_single_batch_kernel_single_batch_x_no_ard(self):
-        kernel = self.create_kernel_no_ard(batch_shape=torch.Size([]))
+    def test_single_batch_kernel_single_batch_x(self):
         x = self.create_data_single_batch()
+        kernel = self.create_kernel(num_dims=x.size(-1), batch_shape=torch.Size([]))
+        y = torch.randn_like(x[..., 0])
+        kernel.initialize_from_data(x, y)
+        kernel.initialize_from_data_empspect(x, y)
         batch_covar_mat = kernel(x).evaluate_kernel().to_dense()
 
         actual_mat_1 = kernel(x[0]).evaluate_kernel().to_dense()
         actual_mat_2 = kernel(x[1]).evaluate_kernel().to_dense()
         actual_covar_mat = torch.cat([actual_mat_1.unsqueeze(0), actual_mat_2.unsqueeze(0)])
 
-        self.assertAllClose(batch_covar_mat, actual_covar_mat, rtol=1e-3, atol=1e-5)
+        self.assertLess(torch.norm(batch_covar_mat - actual_covar_mat) / actual_covar_mat.norm(), 1e-4)
 
         # Test diagonal
         kernel_diag = kernel(x, diag=True)
         actual_diag = actual_covar_mat.diagonal(dim1=-1, dim2=-2)
-        self.assertAllClose(kernel_diag, actual_diag, rtol=1e-3, atol=1e-5)
+        self.assertLess(torch.norm(kernel_diag - actual_diag) / actual_diag.norm(), 1e-4)
 
-    def test_no_batch_kernel_double_batch_x_no_ard(self):
-        kernel = self.create_kernel_no_ard(batch_shape=torch.Size([]))
+    def test_smoke_double_batch_kernel_double_batch_x(self):
         x = self.create_data_double_batch()
-        batch_covar_mat = kernel(x).evaluate_kernel().to_dense()
-
-        ij_actual_covars = []
-        for i in range(x.size(0)):
-            i_actual_covars = []
-            for j in range(x.size(1)):
-                i_actual_covars.append(kernel(x[i, j]).evaluate_kernel().to_dense())
-            ij_actual_covars.append(torch.cat([ac.unsqueeze(0) for ac in i_actual_covars]))
+        kernel = self.create_kernel(num_dims=x.size(-1), batch_shape=torch.Size([3, 2]))
+        y = torch.randn_like(x[..., 0])
+        kernel.initialize_from_data(x, y)
+        kernel.initialize_from_data_empspect(x, y)
 
-        actual_covar_mat = torch.cat([ac.unsqueeze(0) for ac in ij_actual_covars])
-
-        self.assertAllClose(batch_covar_mat, actual_covar_mat, rtol=1e-3, atol=1e-5)
-
-        # Test diagonal
-        kernel_diag = kernel(x, diag=True)
-        actual_diag = actual_covar_mat.diagonal(dim1=-1, dim2=-2)
-        self.assertAllClose(kernel_diag, actual_diag, rtol=1e-3, atol=1e-5)
-
-    def test_no_batch_kernel_double_batch_x_ard(self):
-        try:
-            kernel = self.create_kernel_ard(num_dims=2, batch_shape=torch.Size([]))
-        except NotImplementedError:
-            return
-
-        x = self.create_data_double_batch()
         batch_covar_mat = kernel(x).evaluate_kernel().to_dense()
-
-        ij_actual_covars = []
-        for i in range(x.size(0)):
-            i_actual_covars = []
-            for j in range(x.size(1)):
-                i_actual_covars.append(kernel(x[i, j]).evaluate_kernel().to_dense())
-            ij_actual_covars.append(torch.cat([ac.unsqueeze(0) for ac in i_actual_covars]))
-
-        actual_covar_mat = torch.cat([ac.unsqueeze(0) for ac in ij_actual_covars])
-
-        self.assertAllClose(batch_covar_mat, actual_covar_mat, rtol=1e-3, atol=1e-5)
-
-        # Test diagonal
         kernel_diag = kernel(x, diag=True)
-        actual_diag = actual_covar_mat.diagonal(dim1=-1, dim2=-2)
-        self.assertAllClose(kernel_diag, actual_diag, rtol=1e-3, atol=1e-5)
-
-    def test_smoke_double_batch_kernel_double_batch_x_no_ard(self):
-        kernel = self.create_kernel_no_ard(batch_shape=torch.Size([3, 2]))
-        x = self.create_data_double_batch()
-        batch_covar_mat = kernel(x).evaluate_kernel().to_dense()
-        kernel(x, diag=True)
-        return batch_covar_mat
-
-    def test_smoke_double_batch_kernel_double_batch_x_ard(self):
-        try:
-            kernel = self.create_kernel_ard(num_dims=2, batch_shape=torch.Size([3, 2]))
-        except NotImplementedError:
-            return
-
-        x = self.create_data_double_batch()
-        batch_covar_mat = kernel(x).evaluate_kernel().to_dense()
-        kernel(x, diag=True)
-        return batch_covar_mat
+        return batch_covar_mat, kernel_diag
 
     def test_kernel_getitem_single_batch(self):
-        kernel = self.create_kernel_no_ard(batch_shape=torch.Size([2]))
         x = self.create_data_single_batch()
+        kernel = self.create_kernel(num_dims=x.size(-1), batch_shape=torch.Size([2]))
 
         res1 = kernel(x).to_dense()[0]  # Result of first kernel on first batch of data
 
         new_kernel = kernel[0]
         res2 = new_kernel(x[0]).to_dense()  # Should also be result of first kernel on first batch of data.
 
-        self.assertAllClose(res1, res2, rtol=1e-3, atol=1e-5)
+        self.assertLess(torch.norm(res1 - res2) / res1.norm(), 1e-4)
+
+        # Test diagonal
+        kernel_diag = kernel(x, diag=True)
+        actual_diag = res1.diagonal(dim1=-1, dim2=-2)
+        self.assertLess(torch.norm(kernel_diag - actual_diag) / actual_diag.norm(), 1e-4)
 
     def test_kernel_getitem_double_batch(self):
-        kernel = self.create_kernel_no_ard(batch_shape=torch.Size([3, 2]))
         x = self.create_data_double_batch()
+        kernel = self.create_kernel(num_dims=x.size(-1), batch_shape=torch.Size([3, 2]))
 
         res1 = kernel(x).to_dense()[0, 1]  # Result of first kernel on first batch of data
 
         new_kernel = kernel[0, 1]
         res2 = new_kernel(x[0, 1]).to_dense()  # Should also be result of first kernel on first batch of data.
 
-        self.assertAllClose(res1, res2, rtol=1e-3, atol=1e-5)
+        self.assertLess(torch.norm(res1 - res2) / res1.norm(), 1e-4)
+
+        # Test diagonal
+        kernel_diag = kernel(x, diag=True)
+        actual_diag = res1.diagonal(dim1=-1, dim2=-2)
+        self.assertLess(torch.norm(kernel_diag - actual_diag) / actual_diag.norm(), 1e-4)
+
 
-    def test_kernel_pickle_unpickle(self):
-        kernel = self.create_kernel_no_ard(batch_shape=torch.Size([]))
-        pickle.loads(pickle.dumps(kernel))  # Should be able to pickle and unpickle a kernel
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `gpytorch-1.9.0/gpytorch/test/base_likelihood_test_case.py` & `gpytorch-1.9.1/gpytorch/test/base_likelihood_test_case.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/test/base_mean_test_case.py` & `gpytorch-1.9.1/gpytorch/test/base_mean_test_case.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/test/base_test_case.py` & `gpytorch-1.9.1/gpytorch/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/test/model_test_case.py` & `gpytorch-1.9.1/gpytorch/test/model_test_case.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/test/utils.py` & `gpytorch-1.9.1/gpytorch/test/utils.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/test/variational_test_case.py` & `gpytorch-1.9.1/gpytorch/test/variational_test_case.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/__init__.py` & `gpytorch-1.9.1/gpytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/broadcasting.py` & `gpytorch-1.9.1/gpytorch/utils/broadcasting.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/cholesky.py` & `gpytorch-1.9.1/gpytorch/utils/cholesky.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/deprecation.py` & `gpytorch-1.9.1/gpytorch/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/errors.py` & `gpytorch-1.9.1/gpytorch/utils/errors.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/getitem.py` & `gpytorch-1.9.1/gpytorch/utils/getitem.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/grid.py` & `gpytorch-1.9.1/gpytorch/utils/grid.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/interpolation.py` & `gpytorch-1.9.1/gpytorch/utils/interpolation.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/lanczos.py` & `gpytorch-1.9.1/gpytorch/utils/lanczos.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/memoize.py` & `gpytorch-1.9.1/gpytorch/utils/memoize.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/nearest_neighbors.py` & `gpytorch-1.9.1/gpytorch/utils/nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/permutation.py` & `gpytorch-1.9.1/gpytorch/utils/permutation.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/quadrature.py` & `gpytorch-1.9.1/gpytorch/utils/quadrature.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/sparse.py` & `gpytorch-1.9.1/gpytorch/utils/sparse.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/toeplitz.py` & `gpytorch-1.9.1/gpytorch/utils/toeplitz.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/transforms.py` & `gpytorch-1.9.1/gpytorch/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/utils/warnings.py` & `gpytorch-1.9.1/gpytorch/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/__init__.py` & `gpytorch-1.9.1/gpytorch/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/_variational_distribution.py` & `gpytorch-1.9.1/gpytorch/variational/_variational_distribution.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/_variational_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,24 @@
 class _VariationalStrategy(Module, ABC):
     """
     Abstract base class for all Variational Strategies.
     """
 
     has_fantasy_strategy = False
 
-    def __init__(self, model, inducing_points, variational_distribution, learn_inducing_locations=True):
+    def __init__(
+        self, model, inducing_points, variational_distribution, learn_inducing_locations=True, jitter_val=None
+    ):
         super().__init__()
 
+        if jitter_val is None:
+            self.jitter_val = settings.variational_cholesky_jitter.value(inducing_points.dtype)
+        else:
+            self.jitter_val = jitter_val
+
         # Model
         object.__setattr__(self, "model", model)
 
         # Inducing points
         inducing_points = inducing_points.clone()
         if inducing_points.dim() == 1:
             inducing_points = inducing_points.unsqueeze(-1)
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/additive_grid_interpolation_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/additive_grid_interpolation_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/batch_decoupled_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/batch_decoupled_variational_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,21 @@
         >>>         self.covar_module = gpytorch.kernels.ScaleKernel(
         >>>             gpytorch.kernels.RBFKernel(batch_shape=torch.Size([3, 1])),
         >>>             batch_shape=torch.Size([3, 1]),
         >>>         )
     """
 
     def __init__(
-        self, model, inducing_points, variational_distribution, learn_inducing_locations=True, mean_var_batch_dim=None
+        self,
+        model,
+        inducing_points,
+        variational_distribution,
+        learn_inducing_locations=True,
+        mean_var_batch_dim=None,
+        jitter_val=None,
     ):
         if isinstance(variational_distribution, DeltaVariationalDistribution):
             raise NotImplementedError(
                 "BatchDecoupledVariationalStrategy does not work with DeltaVariationalDistribution"
             )
 
         if mean_var_batch_dim is not None and mean_var_batch_dim >= 0:
@@ -149,15 +155,17 @@
 
         # We're going to create two set of inducing points
         # One set for computing the mean, one set for computing the variance
         if self.mean_var_batch_dim is not None:
             inducing_points = torch.stack([inducing_points, inducing_points], dim=(self.mean_var_batch_dim - 2))
         else:
             inducing_points = torch.stack([inducing_points, inducing_points], dim=-3)
-        super().__init__(model, inducing_points, variational_distribution, learn_inducing_locations)
+        super().__init__(
+            model, inducing_points, variational_distribution, learn_inducing_locations, jitter_val=jitter_val
+        )
 
     def _expand_inputs(self, x, inducing_points):
         # If we haven't explicitly marked a dimension as batch, add the corresponding batch dimension to the input
         if self.mean_var_batch_dim is None:
             x = x.unsqueeze(-3)
         else:
             x = x.unsqueeze(self.mean_var_batch_dim - 2)
@@ -173,15 +181,15 @@
         full_inputs = torch.cat([inducing_points, x], dim=-2)
         full_output = self.model.forward(full_inputs, **kwargs)
         full_covar = full_output.lazy_covariance_matrix
 
         # Covariance terms
         num_induc = inducing_points.size(-2)
         test_mean = full_output.mean[..., num_induc:]
-        induc_induc_covar = full_covar[..., :num_induc, :num_induc].add_jitter()
+        induc_induc_covar = full_covar[..., :num_induc, :num_induc].add_jitter(self.jitter_val)
         induc_data_covar = full_covar[..., :num_induc, num_induc:].to_dense()
         data_data_covar = full_covar[..., num_induc:, num_induc:]
 
         # Compute interpolation terms
         # K_ZZ^{-1/2} K_ZX
         # K_ZZ^{-1/2} \mu_Z
         L = self._cholesky_factor(induc_induc_covar)
@@ -207,15 +215,15 @@
 
         # Compute the covariance of q(f)
         # K_XX + k_XZ K_ZZ^{-1/2} (S - I) K_ZZ^{-1/2} k_ZX
         middle_term = self.prior_distribution.lazy_covariance_matrix.mul(-1)
         if variational_inducing_covar is not None:
             middle_term = SumLinearOperator(variational_inducing_covar, middle_term)
         predictive_covar = SumLinearOperator(
-            data_data_covar.add_jitter(1e-4).to_dense().select(mean_var_batch_dim - 2, 1),
+            data_data_covar.add_jitter(self.jitter_val).to_dense().select(mean_var_batch_dim - 2, 1),
             MatmulLinearOperator(var_interp_term.transpose(-1, -2), middle_term @ var_interp_term),
         )
 
         return MultivariateNormal(predictive_mean, predictive_covar)
 
     def kl_divergence(self):
         variational_dist = self.variational_distribution
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/cholesky_variational_distribution.py` & `gpytorch-1.9.1/gpytorch/variational/cholesky_variational_distribution.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/ciq_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/ciq_variational_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,17 +198,17 @@
         full_inputs = torch.cat([inducing_points, x], dim=-2)
         full_output = self.model.forward(full_inputs)
         full_covar = full_output.lazy_covariance_matrix
 
         # Covariance terms
         num_induc = inducing_points.size(-2)
         test_mean = full_output.mean[..., num_induc:]
-        induc_induc_covar = full_covar[..., :num_induc, :num_induc].evaluate_kernel().add_jitter(1e-2)
+        induc_induc_covar = full_covar[..., :num_induc, :num_induc].evaluate_kernel().add_jitter(self.jitter_val)
         induc_data_covar = full_covar[..., :num_induc, num_induc:].to_dense()
-        data_data_covar = full_covar[..., num_induc:, num_induc:].add_jitter(1e-4)
+        data_data_covar = full_covar[..., num_induc:, num_induc:].add_jitter(self.jitter_val)
 
         # Compute interpolation terms
         # K_XZ K_ZZ^{-1} \mu_z
         # K_XZ K_ZZ^{-1/2} \mu_Z
         with settings.max_preconditioner_size(0):  # Turn off preconditioning for CIQ
             interp_term = to_linear_operator(induc_induc_covar).sqrt_inv_matmul(induc_data_covar)
 
@@ -238,15 +238,15 @@
             ).squeeze(-1)
 
             # Compute the covariance of q(f)
             middle_term = self.prior_distribution.lazy_covariance_matrix.mul(-1)
             if variational_inducing_covar is not None:
                 middle_term = SumLinearOperator(variational_inducing_covar, middle_term)
             predictive_covar = SumLinearOperator(
-                data_data_covar.add_jitter(1e-4),
+                data_data_covar.add_jitter(self.jitter_val),
                 MatmulLinearOperator(interp_term.transpose(-1, -2), middle_term @ interp_term),
             )
 
         # Compute the mean of q(f)
         # k_XZ K_ZZ^{-1/2} (m - K_ZZ^{-1/2} \mu_Z) + \mu_X
         predictive_mean = interp_mean + test_mean
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/delta_variational_distribution.py` & `gpytorch-1.9.1/gpytorch/variational/delta_variational_distribution.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/grid_interpolation_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/grid_interpolation_variational_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
             interp_values = interp_values.expand(*batch_shape, *interp_values.shape[-2:])
         return interp_indices, interp_values
 
     @property
     @cached(name="prior_distribution_memo")
     def prior_distribution(self):
         out = self.model.forward(self.inducing_points)
-        res = MultivariateNormal(out.mean, out.lazy_covariance_matrix.add_jitter())
+        # TODO: investigate why smaller than 1e-3 breaks some tests
+        res = MultivariateNormal(out.mean, out.lazy_covariance_matrix.add_jitter(1e-3))
         return res
 
     def forward(self, x, inducing_points, inducing_values, variational_inducing_covar=None):
         if variational_inducing_covar is None:
             raise RuntimeError(
                 "GridInterpolationVariationalStrategy is only compatible with Gaussian variational "
                 f"distributions. Got ({self.variational_distribution.__class__.__name__}."
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/independent_multitask_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/independent_multitask_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/lmc_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/lmc_variational_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,19 +74,19 @@
         >>>
         >>>         # The variational parameters have a batch_shape of [3] - for 3 latent functions
         >>>         variational_distribution = gpytorch.variational.MeanFieldVariationalDistribution(
         >>>             inducing_points.size(-1), batch_shape=torch.Size([3]),
         >>>         )
         >>>         variational_strategy = gpytorch.variational.LMCVariationalStrategy(
         >>>             gpytorch.variational.VariationalStrategy(
-        >>>                 inducing_points, variational_distribution, learn_inducing_locations=True,
+        >>>                 self, inducing_points, variational_distribution, learn_inducing_locations=True,
         >>>             ),
         >>>             num_tasks=5,
         >>>             num_latents=3,
-        >>>             latent_dim=0,
+        >>>             latent_dim=-1,
         >>>         )
         >>>
         >>>         # Each latent function has its own mean/kernel function
         >>>         super().__init__(variational_strategy)
         >>>         self.mean_module = gpytorch.means.ConstantMean(batch_shape=torch.Size([3]))
         >>>         self.covar_module = gpytorch.kernels.ScaleKernel(
         >>>             gpytorch.kernels.RBFKernel(batch_shape=torch.Size([3])),
@@ -104,14 +104,15 @@
 
     def __init__(
         self,
         base_variational_strategy,
         num_tasks,
         num_latents=1,
         latent_dim=-1,
+        jitter_val=None,
     ):
         Module.__init__(self)
         self.base_variational_strategy = base_variational_strategy
         self.num_tasks = num_tasks
         batch_shape = self.base_variational_strategy._variational_distribution.batch_shape
 
         # Check if no functions
@@ -130,14 +131,21 @@
         del self.batch_shape[self.latent_dim]
         self.batch_shape = torch.Size(self.batch_shape)
 
         # LCM coefficients
         lmc_coefficients = torch.randn(*batch_shape, self.num_tasks)
         self.register_parameter("lmc_coefficients", torch.nn.Parameter(lmc_coefficients))
 
+        if jitter_val is None:
+            self.jitter_val = settings.variational_cholesky_jitter.value(
+                self.base_variational_strategy.inducing_points.dtype
+            )
+        else:
+            self.jitter_val = jitter_val
+
     @property
     def prior_distribution(self):
         return self.base_variational_strategy.prior_distribution
 
     @property
     def variational_distribution(self):
         return self.base_variational_strategy.variational_distribution
@@ -202,15 +210,15 @@
             )
 
             # Covar: ... x (N x num_tasks) x (N x num_tasks)
             latent_covar = latent_dist.lazy_covariance_matrix
             lmc_factor = RootLinearOperator(lmc_coefficients.unsqueeze(-1))
             covar = KroneckerProductLinearOperator(latent_covar, lmc_factor).sum(latent_dim)
             # Add a bit of jitter to make the covar PD
-            covar = covar.add_jitter(settings.cholesky_jitter.value(dtype=mean.dtype))
+            covar = covar.add_jitter(self.jitter_val)
 
             # Done!
             function_dist = MultitaskMultivariateNormal(mean, covar)
 
         else:
             # Each data point will get a single output corresponding to a single task
             # Therefore, we will select the appropriate lmc coefficients for each task
@@ -220,13 +228,13 @@
             mean = (latent_dist.mean * lmc_coefficients).sum(latent_dim)
 
             # Covar: ... x N x N
             latent_covar = latent_dist.lazy_covariance_matrix
             lmc_factor = RootLinearOperator(lmc_coefficients.unsqueeze(-1))
             covar = (latent_covar * lmc_factor).sum(latent_dim)
             # Add a bit of jitter to make the covar PD
-            covar = covar.add_jitter(settings.cholesky_jitter.value(dtype=mean.dtype))
+            covar = covar.add_jitter(self.jitter_val)
 
             # Done!
             function_dist = MultivariateNormal(mean, covar)
 
         return function_dist
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/mean_field_variational_distribution.py` & `gpytorch-1.9.1/gpytorch/variational/mean_field_variational_distribution.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/natural_variational_distribution.py` & `gpytorch-1.9.1/gpytorch/variational/natural_variational_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 import abc
 
 import torch
 from linear_operator.operators import CholLinearOperator, TriangularLinearOperator
+from linear_operator.utils.cholesky import psd_safe_cholesky
 
 from ..distributions import MultivariateNormal
-from ..utils.cholesky import psd_safe_cholesky
 from ._variational_distribution import _VariationalDistribution
 
 
 class _NaturalVariationalDistribution(_VariationalDistribution, abc.ABC):
     r"""Any :obj:`~gpytorch.variational._VariationalDistribution` which calculates
     natural gradients with respect to its parameters.
     """
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/nearest_neighbor_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/nearest_neighbor_variational_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python3
 
 
 import torch
 from linear_operator import to_dense
 from linear_operator.operators import DiagLinearOperator, TriangularLinearOperator
+from linear_operator.utils.cholesky import psd_safe_cholesky
 
-from .. import settings
 from ..distributions import MultivariateNormal
-from ..utils.cholesky import psd_safe_cholesky
 from ..utils.errors import CachingError
 from ..utils.memoize import add_to_cache, cached, pop_from_cache
 from ..utils.nearest_neighbors import NNUtil
 from .mean_field_variational_distribution import MeanFieldVariationalDistribution
 from .unwhitened_variational_strategy import UnwhitenedVariationalStrategy
 
 
@@ -100,16 +99,15 @@
         self.training_batch_size = training_batch_size
         self._set_training_iterator()
 
     @property
     @cached(name="prior_distribution_memo")
     def prior_distribution(self):
         out = self.model.forward(self.inducing_points)
-        jitter_val = settings.cholesky_jitter.value(self.inducing_points.dtype)
-        res = MultivariateNormal(out.mean, out.lazy_covariance_matrix.add_jitter(jitter_val))
+        res = MultivariateNormal(out.mean, out.lazy_covariance_matrix.add_jitter(self.jitter_val))
         return res
 
     def _cholesky_factor(self, induc_induc_covar):
         # Uncached version
         L = psd_safe_cholesky(to_dense(induc_induc_covar))
         return TriangularLinearOperator(L)
 
@@ -232,30 +230,28 @@
     def _firstk_kl_helper(self):
         # Compute the KL divergence for first k inducing points
         train_x_firstk = self.inducing_points[..., : self.k, :]
         full_output = self.model.forward(train_x_firstk)
 
         induc_mean, induc_induc_covar = full_output.mean, full_output.lazy_covariance_matrix
 
-        jitter_val = settings.cholesky_jitter.value(self.inducing_points.dtype)
-        induc_induc_covar = induc_induc_covar.add_jitter(jitter_val)
+        induc_induc_covar = induc_induc_covar.add_jitter(self.jitter_val)
         prior_dist = MultivariateNormal(induc_mean, induc_induc_covar)
 
         inducing_values = self._variational_distribution.variational_mean[..., : self.k]
         variational_covar_fisrtk = self._variational_distribution._variational_stddev[..., : self.k] ** 2
         variational_inducing_covar = DiagLinearOperator(variational_covar_fisrtk)
 
         variational_distribution = MultivariateNormal(inducing_values, variational_inducing_covar)
         kl = torch.distributions.kl.kl_divergence(variational_distribution, prior_dist)  # model_batch_shape
         return kl
 
     def _stochastic_kl_helper(self, kl_indices):
         # Compute the KL divergence for a mini batch of the rest M-1 inducing points
         # See paper appendix for kl breakdown
-        jitter_val = settings.cholesky_jitter.value(self.inducing_points.dtype)
         kl_bs = len(kl_indices)
         variational_mean = self._variational_distribution.variational_mean
         variational_stddev = self._variational_distribution._variational_stddev
 
         # compute logdet_q
         inducing_point_log_variational_covar = (variational_stddev[..., kl_indices] ** 2).log()
         logdet_q = torch.sum(inducing_point_log_variational_covar, dim=-1)
@@ -271,22 +267,22 @@
         )
         nearest_neighbors = expanded_inducing_points_all.gather(-3, expanded_nearest_neighbor_indices)
 
         # compute interp_term
         cov = self.model.covar_module.forward(nearest_neighbors, nearest_neighbors)
         cross_cov = self.model.covar_module.forward(nearest_neighbors, inducing_points.unsqueeze(-2))
         interp_term = torch.linalg.solve(
-            cov + jitter_val * torch.eye(self.k, device=self.inducing_points.device), cross_cov
+            cov + self.jitter_val * torch.eye(self.k, device=self.inducing_points.device), cross_cov
         ).squeeze(-1)
 
         # compte logdet_p
         invquad_term_for_F = torch.sum(interp_term * cross_cov.squeeze(-1), dim=-1)
         cov_inducing_points = self.model.covar_module.forward(inducing_points, inducing_points, diag=True)
         F = cov_inducing_points - invquad_term_for_F
-        F = F + jitter_val
+        F = F + self.jitter_val
         logdet_p = F.log().sum(dim=-1)
 
         # compute trace_term
         expanded_variational_stddev = variational_stddev.unsqueeze(-1).expand(*self._batch_shape, self.M, self.k)
         expanded_variational_mean = variational_mean.unsqueeze(-1).expand(*self._batch_shape, self.M, self.k)
         expanded_nearest_neighbor_indices = nearest_neighbor_indices.expand(*self._batch_shape, kl_bs, self.k)
         nearest_neighbor_variational_covar = (
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/orthogonally_decoupled_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/orthogonally_decoupled_variational_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         )
         self.base_variational_strategy = covar_variational_strategy
 
     @property
     @cached(name="prior_distribution_memo")
     def prior_distribution(self):
         out = self.model(self.inducing_points)
-        res = MultivariateNormal(out.mean, out.lazy_covariance_matrix.add_jitter())
+        res = MultivariateNormal(out.mean, out.lazy_covariance_matrix.add_jitter(self.jitter_val))
         return res
 
     def forward(self, x, inducing_points, inducing_values, variational_inducing_covar=None, **kwargs):
         if variational_inducing_covar is not None:
             raise NotImplementedError(
                 "OrthogonallyDecoupledVariationalStrategy currently works with DeltaVariationalDistribution"
             )
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/tril_natural_variational_distribution.py` & `gpytorch-1.9.1/gpytorch/variational/tril_natural_variational_distribution.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/gpytorch/variational/unwhitened_variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/unwhitened_variational_strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     CholLinearOperator,
     DiagLinearOperator,
     PsdSumLinearOperator,
     RootLinearOperator,
     TriangularLinearOperator,
     ZeroLinearOperator,
 )
+from linear_operator.utils.cholesky import psd_safe_cholesky
+from linear_operator.utils.errors import NotPSDError
 
 from .. import settings
 from ..distributions import MultivariateNormal
-from ..utils.cholesky import psd_safe_cholesky
-from ..utils.errors import NotPSDError
 from ..utils.memoize import add_to_cache, cached
 from ._variational_strategy import _VariationalStrategy
 from .cholesky_variational_distribution import CholeskyVariationalDistribution
 
 
 class UnwhitenedVariationalStrategy(_VariationalStrategy):
     r"""
@@ -88,32 +88,32 @@
         # D_a = (S^{-1} - K^{-1})^{-1} = S + S R^{-1} S
         # note that in the whitened case R = I - S, unwhitened R = K - S
         # we compute (R R^{T})^{-1} R^T S for stability reasons as R is probably not PSD.
         eval_lhs = var_cov.to_dense()
         eval_rhs = cov_diff.transpose(-1, -2).matmul(eval_lhs)
         inner_term = cov_diff.matmul(cov_diff.transpose(-1, -2))
         # TODO: flag the jitter here
-        inner_solve = inner_term.add_jitter(1e-3).solve(eval_rhs, eval_lhs.transpose(-1, -2))
+        inner_solve = inner_term.add_jitter(self.jitter_val).solve(eval_rhs, eval_lhs.transpose(-1, -2))
         inducing_covar = var_cov + inner_solve
 
         # mean term: D_a S^{-1} m
         # unwhitened: (S - S R^{-1} S) S^{-1} m = (I - S R^{-1}) m
         rhs = cov_diff.transpose(-1, -2).matmul(var_mean)
-        inner_rhs_mean_solve = inner_term.add_jitter(1e-3).solve(rhs)
+        inner_rhs_mean_solve = inner_term.add_jitter(self.jitter_val).solve(rhs)
         pseudo_target_mean = var_mean + var_cov.matmul(inner_rhs_mean_solve)
 
         # ensure inducing covar is psd
         try:
-            pseudo_target_covar = CholLinearOperator(inducing_covar.add_jitter(1e-3).cholesky()).to_dense()
+            pseudo_target_covar = CholLinearOperator(inducing_covar.add_jitter(self.jitter_val).cholesky()).to_dense()
         except NotPSDError:
             from linear_operator.operators import DiagLinearOperator
 
             evals, evecs = torch.linalg.eigh(inducing_covar)
             pseudo_target_covar = (
-                evecs.matmul(DiagLinearOperator(evals + 1e-4)).matmul(evecs.transpose(-1, -2)).to_dense()
+                evecs.matmul(DiagLinearOperator(evals + self.jitter_val)).matmul(evecs.transpose(-1, -2)).to_dense()
             )
 
         return pseudo_target_covar, pseudo_target_mean
 
     def forward(self, x, inducing_points, inducing_values, variational_inducing_covar=None):
         # If our points equal the inducing points, we're done
         if torch.equal(x, inducing_points):
@@ -130,15 +130,15 @@
 
         # Mean terms
         test_mean = full_mean[..., num_induc:]
         induc_mean = full_mean[..., :num_induc]
         mean_diff = (inducing_values - induc_mean).unsqueeze(-1)
 
         # Covariance terms
-        induc_induc_covar = full_covar[..., :num_induc, :num_induc].add_jitter()
+        induc_induc_covar = full_covar[..., :num_induc, :num_induc].add_jitter(self.jitter_val)
         induc_data_covar = full_covar[..., :num_induc, num_induc:].to_dense()
         data_data_covar = full_covar[..., num_induc:, num_induc:]
 
         # Compute Cholesky factorization of inducing covariance matrix
         if settings.fast_computations.log_prob.off() or (num_induc <= settings.max_cholesky_size.value()):
             induc_induc_covar = CholLinearOperator(self._cholesky_factor(induc_induc_covar))
```

### Comparing `gpytorch-1.9.0/gpytorch/variational/variational_strategy.py` & `gpytorch-1.9.1/gpytorch/variational/variational_strategy.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,26 @@
     CholLinearOperator,
     DiagLinearOperator,
     MatmulLinearOperator,
     RootLinearOperator,
     SumLinearOperator,
     TriangularLinearOperator,
 )
+from linear_operator.utils.cholesky import psd_safe_cholesky
+from linear_operator.utils.errors import NotPSDError
 
 from gpytorch.variational._variational_strategy import _VariationalStrategy
 from gpytorch.variational.cholesky_variational_distribution import CholeskyVariationalDistribution
 
 from ..distributions import MultivariateNormal
 from ..settings import _linalg_dtype_cholesky, trace_mode
-from ..utils.cholesky import psd_safe_cholesky
-from ..utils.errors import CachingError, NotPSDError
+from ..utils.errors import CachingError
 from ..utils.memoize import cached, clear_cache_hook, pop_from_cache_ignore_args
 from ..utils.warnings import OldVersionWarning
 
-# from ._variational_strategy import _VariationalStrategy
-
 
 def _ensure_updated_strategy_flag_set(
     state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs
 ):
     device = state_dict[list(state_dict.keys())[0]].device
     if prefix + "updated_strategy" not in state_dict:
         state_dict[prefix + "updated_strategy"] = torch.tensor(False, device=device)
@@ -70,19 +69,22 @@
 
     .. _Hensman et al. (2015):
         http://proceedings.mlr.press/v38/hensman15.pdf
     .. _Matthews (2017):
         https://www.repository.cam.ac.uk/handle/1810/278022
     """
 
-    def __init__(self, model, inducing_points, variational_distribution, learn_inducing_locations=True):
-        super().__init__(model, inducing_points, variational_distribution, learn_inducing_locations)
+    def __init__(
+        self, model, inducing_points, variational_distribution, learn_inducing_locations=True, jitter_val=None
+    ):
+        super().__init__(
+            model, inducing_points, variational_distribution, learn_inducing_locations, jitter_val=jitter_val
+        )
         self.register_buffer("updated_strategy", torch.tensor(True))
         self._register_load_state_dict_pre_hook(_ensure_updated_strategy_flag_set)
-
         self.has_fantasy_strategy = True
 
     @cached(name="cholesky_factor", ignore_args=True)
     def _cholesky_factor(self, induc_induc_covar):
         L = psd_safe_cholesky(to_dense(induc_induc_covar).type(_linalg_dtype_cholesky.value()))
         return TriangularLinearOperator(L)
 
@@ -129,50 +131,50 @@
         # D_a = (S^{-1} - K^{-1})^{-1} = S + S R^{-1} S
         # note that in the whitened case R = I - S, unwhitened R = K - S
         # we compute (R R^{T})^{-1} R^T S for stability reasons as R is probably not PSD.
         eval_var_cov = var_cov.to_dense()
         eval_rhs = cov_diff.transpose(-1, -2).matmul(eval_var_cov)
         inner_term = cov_diff.matmul(cov_diff.transpose(-1, -2))
         # TODO: flag the jitter here
-        inner_solve = inner_term.add_jitter(1e-3).solve(eval_rhs, eval_var_cov.transpose(-1, -2))
+        inner_solve = inner_term.add_jitter(self.jitter_val).solve(eval_rhs, eval_var_cov.transpose(-1, -2))
         inducing_covar = var_cov + inner_solve
 
         inducing_covar = Kmm_root.matmul(inducing_covar).matmul(Kmm_root.transpose(-1, -2))
 
         # mean term: D_a S^{-1} m
         # unwhitened: (S - S R^{-1} S) S^{-1} m = (I - S R^{-1}) m
         rhs = cov_diff.transpose(-1, -2).matmul(var_mean)
         # TODO: this jitter too
-        inner_rhs_mean_solve = inner_term.add_jitter(1e-3).solve(rhs)
+        inner_rhs_mean_solve = inner_term.add_jitter(self.jitter_val).solve(rhs)
         pseudo_target_mean = Kmm_root.matmul(inner_rhs_mean_solve)
 
         # ensure inducing covar is psd
         # TODO: make this be an explicit root decomposition
         try:
-            pseudo_target_covar = CholLinearOperator(inducing_covar.add_jitter(1e-3).cholesky()).to_dense()
+            pseudo_target_covar = CholLinearOperator(inducing_covar.add_jitter(self.jitter_val).cholesky()).to_dense()
         except NotPSDError:
             from linear_operator.operators import DiagLinearOperator
 
             evals, evecs = torch.linalg.eigh(inducing_covar)
             pseudo_target_covar = (
-                evecs.matmul(DiagLinearOperator(evals + 1e-4)).matmul(evecs.transpose(-1, -2)).to_dense()
+                evecs.matmul(DiagLinearOperator(evals + self.jitter_val)).matmul(evecs.transpose(-1, -2)).to_dense()
             )
 
         return pseudo_target_covar, pseudo_target_mean
 
     def forward(self, x, inducing_points, inducing_values, variational_inducing_covar=None, **kwargs):
         # Compute full prior distribution
         full_inputs = torch.cat([inducing_points, x], dim=-2)
         full_output = self.model.forward(full_inputs, **kwargs)
         full_covar = full_output.lazy_covariance_matrix
 
         # Covariance terms
         num_induc = inducing_points.size(-2)
         test_mean = full_output.mean[..., num_induc:]
-        induc_induc_covar = full_covar[..., :num_induc, :num_induc].add_jitter()
+        induc_induc_covar = full_covar[..., :num_induc, :num_induc].add_jitter(self.jitter_val)
         induc_data_covar = full_covar[..., :num_induc, num_induc:].to_dense()
         data_data_covar = full_covar[..., num_induc:, num_induc:]
 
         # Compute interpolation terms
         # K_ZZ^{-1/2} K_ZX
         # K_ZZ^{-1/2} \mu_Z
         L = self._cholesky_factor(induc_induc_covar)
@@ -194,33 +196,33 @@
         # K_XX + k_XZ K_ZZ^{-1/2} (S - I) K_ZZ^{-1/2} k_ZX
         middle_term = self.prior_distribution.lazy_covariance_matrix.mul(-1)
         if variational_inducing_covar is not None:
             middle_term = SumLinearOperator(variational_inducing_covar, middle_term)
 
         if trace_mode.on():
             predictive_covar = (
-                data_data_covar.add_jitter(1e-4).to_dense()
+                data_data_covar.add_jitter(self.jitter_val).to_dense()
                 + interp_term.transpose(-1, -2) @ middle_term.to_dense() @ interp_term
             )
         else:
             predictive_covar = SumLinearOperator(
-                data_data_covar.add_jitter(1e-4),
+                data_data_covar.add_jitter(self.jitter_val),
                 MatmulLinearOperator(interp_term.transpose(-1, -2), middle_term @ interp_term),
             )
 
         # Return the distribution
         return MultivariateNormal(predictive_mean, predictive_covar)
 
     def __call__(self, x, prior=False, **kwargs):
         if not self.updated_strategy.item() and not prior:
             with torch.no_grad():
                 # Get unwhitened p(u)
                 prior_function_dist = self(self.inducing_points, prior=True)
                 prior_mean = prior_function_dist.loc
-                L = self._cholesky_factor(prior_function_dist.lazy_covariance_matrix.add_jitter())
+                L = self._cholesky_factor(prior_function_dist.lazy_covariance_matrix.add_jitter(self.jitter_val))
 
                 # Temporarily turn off noise that's added to the mean
                 orig_mean_init_std = self._variational_distribution.mean_init_std
                 self._variational_distribution.mean_init_std = 0.0
 
                 # Change the variational parameters to be whitened
                 variational_dist = self.variational_distribution
```

### Comparing `gpytorch-1.9.0/gpytorch.egg-info/PKG-INFO` & `gpytorch-1.9.1/gpytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpytorch
-Version: 1.9.0
+Version: 1.9.1
 Summary: An implementation of Gaussian Processes in Pytorch
 Home-page: https://gpytorch.ai
 Author: Jake Gardner, Geoff Pleiss
 Author-email: jrg365@cornell.edu, gpleiss@gmail.com
 License: MIT
 Project-URL: Documentation, https://gpytorch.readthedocs.io
 Project-URL: Source, https://github.com/cornellius-gp/gpytorch/
@@ -40,14 +40,15 @@
         (To use packages globally but install GPyTorch as a user-only package, use `pip install --user` above.)
         
         #### Latest (unstable) version
         
         To upgrade to the latest (unstable) version, run
         
         ```bash
+        pip install --upgrade git+https://github.com/cornellius-gp/linear_operator.git
         pip install --upgrade git+https://github.com/cornellius-gp/gpytorch.git
         ```
         
         #### ArchLinux Package
         Note: Experimental AUR package. For most users, we recommend installation by conda or pip.
         
         GPyTorch is also available on the [ArchLinux User Repository](https://wiki.archlinux.org/index.php/Arch_User_Repository) (AUR).
```

### Comparing `gpytorch-1.9.0/gpytorch.egg-info/SOURCES.txt` & `gpytorch-1.9.1/gpytorch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,15 @@
 test/examples/test_kissgp_gp_regression.py
 test/examples/test_kissgp_kronecker_product_classification.py
 test/examples/test_kissgp_kronecker_product_regression.py
 test/examples/test_kissgp_multiplicative_regression.py
 test/examples/test_kissgp_variational_regression.py
 test/examples/test_kissgp_white_noise_regression.py
 test/examples/test_kronecker_multitask_gp_regression.py
+test/examples/test_kronecker_multitask_sgpr_regression.py
 test/examples/test_kronecker_multitask_ski_gp_regression.py
 test/examples/test_lcm_kernel_regression.py
 test/examples/test_lmc_svgp_regression.py
 test/examples/test_model_list_gp_regression.py
 test/examples/test_pyro_integration.py
 test/examples/test_rff_gp_regression.py
 test/examples/test_sgpr_regression.py
@@ -372,24 +373,26 @@
 test/means/test_linear_mean.py
 test/means/test_multitask_mean.py
 test/means/test_zero_mean.py
 test/metrics/__init__.py
 test/metrics/test_metrics.py
 test/mlls/__init__.py
 test/mlls/test_exact_marginal_log_likelihood.py
+test/mlls/test_inducing_point_kernel_added_loss_term.py
 test/mlls/test_leave_one_out_pseudo_likelihood.py
 test/models/__init__.py
 test/models/test_exact_gp.py
 test/models/test_model_list.py
 test/models/test_variational_gp.py
 test/optim/__init__.py
 test/optim/test_ngd.py
 test/priors/__init__.py
 test/priors/test_gamma_prior.py
 test/priors/test_half_cauchy_prior.py
+test/priors/test_half_normal_prior.py
 test/priors/test_horseshoe_prior.py
 test/priors/test_lkj_prior.py
 test/priors/test_multivariate_normal_prior.py
 test/priors/test_normal_prior.py
 test/priors/test_smoothed_box_prior.py
 test/utils/__init__.py
 test/utils/test_grid.py
```

### Comparing `gpytorch-1.9.0/setup.py` & `gpytorch-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 readme = open("README.md").read()
 
 
 torch_min = "1.11"
 install_requires = [
     "scikit-learn",
-    "linear_operator>=0.1.1",
+    "linear_operator>=0.2.0",
 ]
 # if recent dev version of PyTorch is installed, no need to install stable
 try:
     import torch
 
     if torch.__version__ >= torch_min:
         install_requires = [">=".join(["torch", torch_min])] + install_requires
```

### Comparing `gpytorch-1.9.0/test/constraints/test_constraints.py` & `gpytorch-1.9.1/test/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/distributions/test_delta.py` & `gpytorch-1.9.1/test/distributions/test_delta.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/distributions/test_multitask_multivariate_normal.py` & `gpytorch-1.9.1/test/distributions/test_multitask_multivariate_normal.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import math
 import os
 import random
 import unittest
 
 import torch
-from linear_operator.operators import DiagLinearOperator
+from linear_operator.operators import DiagLinearOperator, KroneckerProductLinearOperator
 
 from gpytorch.distributions import MultitaskMultivariateNormal, MultivariateNormal
 from gpytorch.test.base_test_case import BaseTestCase
 from gpytorch.test.utils import least_used_cuda_device
 
 
 class TestMultiTaskMultivariateNormal(BaseTestCase, unittest.TestCase):
@@ -197,14 +197,36 @@
             self.assertLess((res - actual).div(res).abs().norm(), 1e-2)
 
     def test_log_prob_cuda(self):
         if torch.cuda.is_available():
             with least_used_cuda_device():
                 self.test_log_prob(cuda=True)
 
+    def test_to_data_independent_dist(self, dtype=torch.float, device="cpu", interleaved=True):
+        # Create a fake covariance
+        factor = torch.randn(4, 4, device=device, dtype=dtype)
+        data_covar = factor.mT @ factor
+        task_covar = torch.tensor([[1.0, 0.3, 0.1], [0.3, 1.0, 0.3], [0.1, 0.3, 1.0]], device=device, dtype=dtype)
+        if interleaved:
+            covar = KroneckerProductLinearOperator(data_covar, task_covar)
+        else:
+            covar = KroneckerProductLinearOperator(task_covar, data_covar)
+
+        mean = torch.randn(4, 3, device=device, dtype=dtype)
+        dist = MultitaskMultivariateNormal(mean, covar, interleaved=interleaved)
+
+        res = dist.to_data_independent_dist(jitter_val=1e-4)
+        self.assertEqual(res.mean, mean)
+        data_var = data_covar.diagonal(dim1=-1, dim2=-2)
+        jitter = torch.eye(3, dtype=dtype, device=device) * 1e-4
+        self.assertAllClose(res.covariance_matrix, data_var.view(-1, 1, 1) * task_covar + jitter)
+
+    def test_to_data_independent_dist_no_interleave(self, dtype=torch.float, device="cpu"):
+        return self.test_to_data_independent_dist(dtype=dtype, device=device, interleaved=False)
+
     def test_multitask_from_batch(self):
         mean = torch.randn(2, 3)
         variance = torch.randn(2, 3).clamp_min(1e-6)
         mvn = MultivariateNormal(mean, DiagLinearOperator(variance))
         mmvn = MultitaskMultivariateNormal.from_batch_mvn(mvn, task_dim=-1)
         self.assertTrue(isinstance(mmvn, MultitaskMultivariateNormal))
         self.assertEqual(mmvn.batch_shape, torch.Size([]))
```

### Comparing `gpytorch-1.9.0/test/distributions/test_multivariate_normal.py` & `gpytorch-1.9.1/test/distributions/test_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/old_variational_strategy_model.pth` & `gpytorch-1.9.1/test/examples/old_variational_strategy_model.pth`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_batch_decoupled_ppgpr_regression.py` & `gpytorch-1.9.1/test/examples/test_batch_decoupled_ppgpr_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_batch_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_batch_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_batch_multitask_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_batch_multitask_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_batch_svgp_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_batch_svgp_gp_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 
 class SVGPRegressionModel(ApproximateGP):
     def __init__(self, inducing_points):
         variational_distribution = CholeskyVariationalDistribution(
             inducing_points.size(-2), batch_shape=torch.Size([2])
         )
         variational_strategy = VariationalStrategy(
-            self, inducing_points, variational_distribution, learn_inducing_locations=True
+            self, inducing_points, variational_distribution,
+            learn_inducing_locations=True,
+            jitter_val=1e-3
         )
         super(SVGPRegressionModel, self).__init__(variational_strategy)
         self.mean_module = gpytorch.means.ConstantMean()
         self.covar_module = gpytorch.kernels.ScaleKernel(
             gpytorch.kernels.RBFKernel(lengthscale_prior=gpytorch.priors.SmoothedBoxPrior(0.001, 1.0, sigma=0.1))
         )
```

### Comparing `gpytorch-1.9.0/test/examples/test_decoupled_svgp_regression.py` & `gpytorch-1.9.1/test/examples/test_decoupled_svgp_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         variational_distribution = gpytorch.variational.DeltaVariationalDistribution(inducing_points.size(-1))
         variational_strategy = gpytorch.variational.OrthogonallyDecoupledVariationalStrategy(
             gpytorch.variational.VariationalStrategy(
                 self,
                 base_inducing_points,
                 base_variational_distribution,
                 learn_inducing_locations=True,
+                jitter_val=1e-4,
             ),
             inducing_points,
             variational_distribution,
         )
         super(SVGPRegressionModel, self).__init__(variational_strategy)
         self.mean_module = gpytorch.means.ConstantMean()
         self.covar_module = gpytorch.kernels.ScaleKernel(gpytorch.kernels.RBFKernel())
```

### Comparing `gpytorch-1.9.0/test/examples/test_dspp_regression.py` & `gpytorch-1.9.1/test/examples/test_dspp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_fixed_noise_fanatasy_updates.py` & `gpytorch-1.9.1/test/examples/test_fixed_noise_fanatasy_updates.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_grid_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_grid_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_hadamard_multitask_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_hadamard_multitask_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_independent_multitask_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_independent_multitask_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_additive_classification.py` & `gpytorch-1.9.1/test/examples/test_kissgp_additive_classification.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_additive_regression.py` & `gpytorch-1.9.1/test/examples/test_kissgp_additive_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_dkl_regression.py` & `gpytorch-1.9.1/test/examples/test_kissgp_dkl_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_gp_classification.py` & `gpytorch-1.9.1/test/examples/test_kissgp_gp_classification.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_kissgp_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_kronecker_product_classification.py` & `gpytorch-1.9.1/test/examples/test_kissgp_kronecker_product_classification.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_kronecker_product_regression.py` & `gpytorch-1.9.1/test/examples/test_kissgp_kronecker_product_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_multiplicative_regression.py` & `gpytorch-1.9.1/test/examples/test_kissgp_multiplicative_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_variational_regression.py` & `gpytorch-1.9.1/test/examples/test_kissgp_variational_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kissgp_white_noise_regression.py` & `gpytorch-1.9.1/test/examples/test_kissgp_white_noise_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kronecker_multitask_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_kronecker_multitask_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_kronecker_multitask_ski_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_kronecker_multitask_ski_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_lcm_kernel_regression.py` & `gpytorch-1.9.1/test/examples/test_lcm_kernel_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_lmc_svgp_regression.py` & `gpytorch-1.9.1/test/examples/test_lmc_svgp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_model_list_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_model_list_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_pyro_integration.py` & `gpytorch-1.9.1/test/examples/test_pyro_integration.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_rff_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_rff_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_sgpr_regression.py` & `gpytorch-1.9.1/test/examples/test_sgpr_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_simple_gp_classification.py` & `gpytorch-1.9.1/test/examples/test_simple_gp_classification.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_simple_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_simple_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_spectral_mixture_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_spectral_mixture_gp_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/examples/test_svgp_gp_classification.py` & `gpytorch-1.9.1/test/examples/test_svgp_gp_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         return train_x, train_y
 
 
 class SVGPClassificationModel(ApproximateGP):
     def __init__(self, inducing_points):
         variational_distribution = CholeskyVariationalDistribution(inducing_points.size(-1))
         variational_strategy = VariationalStrategy(
-            self, inducing_points, variational_distribution, learn_inducing_locations=True
+            self, inducing_points, variational_distribution, learn_inducing_locations=True, jitter_val=1e-4
         )
         super(SVGPClassificationModel, self).__init__(variational_strategy)
         self.mean_module = gpytorch.means.ConstantMean()
         self.covar_module = gpytorch.kernels.ScaleKernel(
             gpytorch.kernels.RBFKernel(lengthscale_prior=gpytorch.priors.SmoothedBoxPrior(0.001, 1.0, sigma=0.1))
         )
```

### Comparing `gpytorch-1.9.0/test/examples/test_svgp_gp_regression.py` & `gpytorch-1.9.1/test/examples/test_svgp_gp_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return train_x, train_y
 
 
 class SVGPRegressionModel(ApproximateGP):
     def __init__(self, inducing_points, distribution_cls):
         variational_distribution = distribution_cls(inducing_points.size(-1))
         variational_strategy = gpytorch.variational.VariationalStrategy(
-            self, inducing_points, variational_distribution, learn_inducing_locations=True
+            self, inducing_points, variational_distribution, learn_inducing_locations=True, jitter_val=1e-4
         )
         super(SVGPRegressionModel, self).__init__(variational_strategy)
         self.mean_module = gpytorch.means.ConstantMean()
         self.covar_module = gpytorch.kernels.ScaleKernel(gpytorch.kernels.RBFKernel())
 
     def forward(self, x):
         mean_x = self.mean_module(x)
```

### Comparing `gpytorch-1.9.0/test/examples/test_unwhitened_svgp_regression.py` & `gpytorch-1.9.1/test/examples/test_unwhitened_svgp_regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         return train_x, train_y
 
 
 class SVGPRegressionModel(ApproximateGP):
     def __init__(self, inducing_points, distribution_cls):
         variational_distribution = distribution_cls(inducing_points.size(-1))
         variational_strategy = gpytorch.variational.UnwhitenedVariationalStrategy(
-            self, inducing_points, variational_distribution, learn_inducing_locations=True
+            self, inducing_points, variational_distribution, learn_inducing_locations=True, jitter_val=1e-4
         )
         super(SVGPRegressionModel, self).__init__(variational_strategy)
         self.mean_module = gpytorch.means.ConstantMean()
         self.covar_module = gpytorch.kernels.ScaleKernel(gpytorch.kernels.RBFKernel())
 
     def forward(self, x):
         mean_x = self.mean_module(x)
```

### Comparing `gpytorch-1.9.0/test/examples/test_white_noise_regression.py` & `gpytorch-1.9.1/test/examples/test_white_noise_regression.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/functions/test_log_normal_cdf.py` & `gpytorch-1.9.1/test/functions/test_log_normal_cdf.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/functions/test_matern_covariance.py` & `gpytorch-1.9.1/test/functions/test_matern_covariance.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import torch
 
 import gpytorch
 
 
 def dist_func(x1, x2):
     dist_module = gpytorch.kernels.kernel.Distance()
-    return dist_module._dist(x1, x2, postprocess=torch.tensor(False))
+    return dist_module._dist(x1, x2)
 
 
 class TestMaternCovariance(unittest.TestCase):
     def test_1_2_forward(self):
         nu = 1 / 2
         batch_size = (3, 2, 4)
         x1 = torch.randn(*batch_size, 7, 9)
```

### Comparing `gpytorch-1.9.0/test/functions/test_rbf_covariance.py` & `gpytorch-1.9.1/test/functions/test_rbf_covariance.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import torch
 
 import gpytorch
 
 
 def sq_dist_func(x1, x2):
     dist_module = gpytorch.kernels.kernel.Distance()
-    return dist_module._sq_dist(x1, x2, postprocess=torch.tensor(False))
+    return dist_module._sq_dist(x1, x2)
 
 
 class TestRBFCovariance(unittest.TestCase):
     def test_forward(self):
         batch_size = (3, 2, 4)
         x1 = torch.randn(*batch_size, 7, 9)
         x2 = torch.randn(*batch_size, 6, 9)
```

### Comparing `gpytorch-1.9.0/test/kernels/keops/test_matern_kernel.py` & `gpytorch-1.9.1/test/kernels/keops/test_matern_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/keops/test_rbf_kernel.py` & `gpytorch-1.9.1/test/kernels/keops/test_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_additive_and_product_kernels.py` & `gpytorch-1.9.1/test/kernels/test_additive_and_product_kernels.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_arc_kernel.py` & `gpytorch-1.9.1/test/kernels/test_arc_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_cosine_kernel.py` & `gpytorch-1.9.1/test/kernels/test_cosine_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_cylindrical_kernel.py` & `gpytorch-1.9.1/test/kernels/test_cylindrical_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_gaussian_symmetrized_kl_kernel.py` & `gpytorch-1.9.1/test/kernels/test_gaussian_symmetrized_kl_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_grid_interpolation_kernel.py` & `gpytorch-1.9.1/test/kernels/test_grid_interpolation_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_grid_kernel.py` & `gpytorch-1.9.1/test/kernels/test_grid_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_index_kernel.py` & `gpytorch-1.9.1/test/kernels/test_index_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_inducing_point_kernel.py` & `gpytorch-1.9.1/test/kernels/test_inducing_point_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_linear_kernel.py` & `gpytorch-1.9.1/test/kernels/test_linear_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_matern_kernel.py` & `gpytorch-1.9.1/test/kernels/test_matern_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_newton_girard_additive_kernel.py` & `gpytorch-1.9.1/test/kernels/test_newton_girard_additive_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_periodic_kernel.py` & `gpytorch-1.9.1/test/kernels/test_periodic_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_piecewise_polynomial_kernel.py` & `gpytorch-1.9.1/test/kernels/test_piecewise_polynomial_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_polynomial_kernel.py` & `gpytorch-1.9.1/test/kernels/test_polynomial_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_rbf_kernel.py` & `gpytorch-1.9.1/test/kernels/test_rbf_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_rbf_kernel_grad.py` & `gpytorch-1.9.1/test/kernels/test_rbf_kernel_grad.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_rff_kernel.py` & `gpytorch-1.9.1/test/kernels/test_rff_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_rq_kernel.py` & `gpytorch-1.9.1/test/kernels/test_rq_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_scale_kernel.py` & `gpytorch-1.9.1/test/kernels/test_scale_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/kernels/test_spectral_delta_kernel.py` & `gpytorch-1.9.1/test/kernels/test_spectral_delta_kernel.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/lazy/test_lazy_evaluated_kernel_tensor.py` & `gpytorch-1.9.1/test/lazy/test_lazy_evaluated_kernel_tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,14 +155,24 @@
     def test_half(self):
         # many transform operations aren't supported in half so we overwrite
         # this test
         lazy_tensor = self.create_linear_op()
         lazy_tensor.kernel.raw_lengthscale_constraint.transform = lambda x: x + 0.1
         self._test_half(lazy_tensor)
 
+    def test_grad_state(self):
+        k = gpytorch.kernels.RBFKernel()
+        X = torch.randn(2, 3)
+        X.requires_grad = True
+        lazy_tensor = k(X)
+        self.assertTrue(lazy_tensor.to_dense().requires_grad)
+        with torch.no_grad():
+            lazy_tensor = k(X)
+        self.assertFalse(lazy_tensor.to_dense().requires_grad)
+
 
 class TestLazyEvaluatedKernelTensorMultitaskBatch(TestLazyEvaluatedKernelTensorBatch):
     seed = 0
     skip_slq_tests = True  # we skip these because of the kronecker structure
 
     def create_linear_op(self):
         kern = gpytorch.kernels.MultitaskKernel(gpytorch.kernels.RBFKernel(), num_tasks=3, rank=2)
```

### Comparing `gpytorch-1.9.0/test/lazy/test_lazy_tensor_deprecation.py` & `gpytorch-1.9.1/test/lazy/test_lazy_tensor_deprecation.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/likelihoods/test_bernoulli_likelihood.py` & `gpytorch-1.9.1/test/likelihoods/test_bernoulli_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/likelihoods/test_beta_likelihood.py` & `gpytorch-1.9.1/test/likelihoods/test_beta_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/likelihoods/test_gaussian_likelihood.py` & `gpytorch-1.9.1/test/likelihoods/test_gaussian_likelihood.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
         likelihood.MISSING_VALUE_FILL = 999.0
         like_init_plus = likelihood.log_marginal(samples, mvn).sum().data
 
         likelihood.MISSING_VALUE_FILL = -999.0
         like_init_minus = likelihood.log_marginal(samples, mvn).sum().data
 
-        torch.testing.assert_allclose(like_init_plus, like_init_minus)
+        torch.testing.assert_close(like_init_plus, like_init_minus)
 
         # check that the correct noise sd is recovered
 
         opt = torch.optim.Adam(likelihood.parameters(), lr=0.05)
 
         for _ in range(100):
             opt.zero_grad()
```

### Comparing `gpytorch-1.9.0/test/likelihoods/test_general_multitask_gaussian_likelihood.py` & `gpytorch-1.9.1/test/likelihoods/test_general_multitask_gaussian_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/likelihoods/test_laplace_likelihood.py` & `gpytorch-1.9.1/test/likelihoods/test_laplace_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/likelihoods/test_multitask_gaussian_likelihood.py` & `gpytorch-1.9.1/test/likelihoods/test_multitask_gaussian_likelihood.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,53 @@
 #!/usr/bin/env python3
 
 import unittest
 
 import torch
-from linear_operator.operators import KroneckerProductLinearOperator, RootLinearOperator
+from linear_operator.operators import KroneckerProductLinearOperator, RootLinearOperator, ToeplitzLinearOperator
 
 from gpytorch.distributions import MultitaskMultivariateNormal
 from gpytorch.likelihoods import MultitaskGaussianLikelihood
 from gpytorch.test.base_likelihood_test_case import BaseLikelihoodTestCase
 
 
 class TestMultitaskGaussianLikelihood(BaseLikelihoodTestCase, unittest.TestCase):
     seed = 2
 
     def _create_conditional_input(self, batch_shape=torch.Size([])):
         return torch.randn(*batch_shape, 5, 4)
 
     def _create_marginal_input(self, batch_shape=torch.Size([])):
-        mat = torch.randn(*batch_shape, 5, 5)
-        mat2 = torch.randn(*batch_shape, 4, 4)
-        covar = KroneckerProductLinearOperator(RootLinearOperator(mat), RootLinearOperator(mat2))
+        data_mat = ToeplitzLinearOperator(torch.tensor([1, 0.6, 0.4, 0.2, 0.1]))
+        task_mat = RootLinearOperator(torch.tensor([[1.0], [2.0], [3.0], [4.0]]))
+        covar = KroneckerProductLinearOperator(data_mat, task_mat)
         return MultitaskMultivariateNormal(torch.randn(*batch_shape, 5, 4), covar)
 
     def _create_targets(self, batch_shape=torch.Size([])):
         return torch.randn(*batch_shape, 5, 4)
 
     def create_likelihood(self):
         return MultitaskGaussianLikelihood(num_tasks=4, rank=2)
 
+    def test_marginal_variance(self):
+        likelihood = MultitaskGaussianLikelihood(num_tasks=4, rank=0, has_global_noise=False)
+        likelihood.task_noises = torch.tensor([[0.1], [0.2], [0.3], [0.4]])
+
+        input = self._create_marginal_input()
+        variance = likelihood(input).variance
+        self.assertAllClose(variance, torch.tensor([1.1, 4.2, 9.3, 16.4]).repeat(5, 1))
+
+        likelihood = MultitaskGaussianLikelihood(num_tasks=4, rank=1, has_global_noise=True)
+        likelihood.noise = torch.tensor(0.1)
+        likelihood.task_noise_covar_factor.data = torch.tensor([[1.0], [2.0], [3.0], [4.0]])
+
+        input = self._create_marginal_input()
+        variance = likelihood(input).variance
+        self.assertAllClose(variance, torch.tensor([2.1, 8.1, 18.1, 32.1]).repeat(5, 1))
+
     def test_setters(self):
         likelihood = MultitaskGaussianLikelihood(num_tasks=3, rank=0)
 
         a = torch.randn(3, 2)
         mat = a.matmul(a.transpose(-1, -2))
 
         # test rank 0 setters
@@ -55,14 +71,24 @@
         self.assertAllClose(mat, likelihood.task_noise_covar)
 
         with self.assertRaises(AttributeError) as context:
             likelihood.task_noises = torch.tensor([0.04, 0.04, 0.04])
         self.assertTrue("task noises" in str(context.exception))
 
 
+class TestMultitaskGaussianLikelihoodNonInterleaved(TestMultitaskGaussianLikelihood, unittest.TestCase):
+    seed = 2
+
+    def _create_marginal_input(self, batch_shape=torch.Size([])):
+        data_mat = ToeplitzLinearOperator(torch.tensor([1, 0.6, 0.4, 0.2, 0.1]))
+        task_mat = RootLinearOperator(torch.tensor([[1.0], [2.0], [3.0], [4.0]]))
+        covar = KroneckerProductLinearOperator(task_mat, data_mat)
+        return MultitaskMultivariateNormal(torch.randn(*batch_shape, 5, 4), covar, interleaved=False)
+
+
 class TestMultitaskGaussianLikelihoodBatch(TestMultitaskGaussianLikelihood):
     seed = 0
 
     def create_likelihood(self):
         return MultitaskGaussianLikelihood(num_tasks=4, rank=2, batch_shape=torch.Size([3]))
 
     def test_nonbatch(self):
```

### Comparing `gpytorch-1.9.0/test/likelihoods/test_softmax_likelihood.py` & `gpytorch-1.9.1/test/likelihoods/test_softmax_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/likelihoods/test_student_t_likelihood.py` & `gpytorch-1.9.1/test/likelihoods/test_student_t_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/means/test_constant_mean.py` & `gpytorch-1.9.1/test/means/test_constant_mean.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/means/test_constant_mean_grad.py` & `gpytorch-1.9.1/test/means/test_constant_mean_grad.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/means/test_linear_mean.py` & `gpytorch-1.9.1/test/means/test_linear_mean.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/means/test_multitask_mean.py` & `gpytorch-1.9.1/test/means/test_multitask_mean.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/metrics/test_metrics.py` & `gpytorch-1.9.1/test/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/mlls/test_exact_marginal_log_likelihood.py` & `gpytorch-1.9.1/test/mlls/test_exact_marginal_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/mlls/test_leave_one_out_pseudo_likelihood.py` & `gpytorch-1.9.1/test/mlls/test_leave_one_out_pseudo_likelihood.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/models/test_exact_gp.py` & `gpytorch-1.9.1/test/models/test_exact_gp.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/models/test_model_list.py` & `gpytorch-1.9.1/test/models/test_model_list.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/models/test_variational_gp.py` & `gpytorch-1.9.1/test/models/test_variational_gp.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/optim/test_ngd.py` & `gpytorch-1.9.1/test/optim/test_ngd.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/priors/test_gamma_prior.py` & `gpytorch-1.9.1/test/priors/test_gamma_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/priors/test_half_cauchy_prior.py` & `gpytorch-1.9.1/test/priors/test_half_cauchy_prior.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
             prior = HalfCauchy(1.0).cuda()
             self.assertEqual(prior.concentration.device.type, "cuda")
             self.assertEqual(prior.rate.device.type, "cuda")
 
     def test_half_cauchy_prior_validate_args(self):
         with self.assertRaises(ValueError):
             HalfCauchyPrior(-1, validate_args=True)
-        with self.assertRaises(ValueError):
-            HalfCauchyPrior(-1, validate_args=True)
 
     def test_half_cauchy_prior_log_prob(self, cuda=False):
         device = torch.device("cuda") if cuda else torch.device("cpu")
         prior = HalfCauchyPrior(0.1)
         dist = HalfCauchy(0.1)
 
         t = torch.tensor(1.0, device=device)
@@ -33,15 +31,15 @@
         self.assertTrue(torch.equal(prior.log_prob(t), dist.log_prob(t)))
         t = torch.tensor([[1.0, 0.5], [3.0, 0.25]], device=device)
         self.assertTrue(torch.equal(prior.log_prob(t), dist.log_prob(t)))
 
     def test_half_cauchy_prior_log_prob_cuda(self):
         if torch.cuda.is_available():
             with least_used_cuda_device():
-                return self.test_gamma_prior_log_prob(cuda=True)
+                return self.test_half_cauchy_prior_log_prob(cuda=True)
 
     def test_half_cauchy_prior_log_prob_log_transform(self, cuda=False):
         device = torch.device("cuda") if cuda else torch.device("cpu")
         prior = HalfCauchyPrior(0.1, transform=torch.exp)
         dist = HalfCauchy(0.1)
 
         t = torch.tensor(0.0, device=device)
```

### Comparing `gpytorch-1.9.0/test/priors/test_horseshoe_prior.py` & `gpytorch-1.9.1/test/priors/test_horseshoe_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/priors/test_lkj_prior.py` & `gpytorch-1.9.1/test/priors/test_lkj_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/priors/test_multivariate_normal_prior.py` & `gpytorch-1.9.1/test/priors/test_multivariate_normal_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/priors/test_normal_prior.py` & `gpytorch-1.9.1/test/priors/test_normal_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/priors/test_smoothed_box_prior.py` & `gpytorch-1.9.1/test/priors/test_smoothed_box_prior.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/test_module.py` & `gpytorch-1.9.1/test/test_module.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/utils/test_grid.py` & `gpytorch-1.9.1/test/utils/test_grid.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/utils/test_interpolation.py` & `gpytorch-1.9.1/test/utils/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/utils/test_nearest_neighbors.py` & `gpytorch-1.9.1/test/utils/test_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/utils/test_quadrature.py` & `gpytorch-1.9.1/test/utils/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_batch_decoupled_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_batch_decoupled_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_ciq_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_ciq_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_grid_interpolation_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_grid_interpolation_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_independent_multitask_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_independent_multitask_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_lmc_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_lmc_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_natural_variational_distribution.py` & `gpytorch-1.9.1/test/variational/test_natural_variational_distribution.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,28 +2,94 @@
 
 import unittest
 
 import torch
 from linear_operator.operators import CholLinearOperator, TriangularLinearOperator
 
 import gpytorch
+from gpytorch.constraints import GreaterThan
 from gpytorch.distributions import MultivariateNormal
 from gpytorch.variational import NaturalVariationalDistribution, TrilNaturalVariationalDistribution
 
 
 class Float64Test(unittest.TestCase):
     def setUp(self):
         self.prev_type = torch.get_default_dtype()
         torch.set_default_dtype(torch.float64)
 
     def tearDown(self):
         torch.set_default_dtype(self.prev_type)
 
 
 class TestNatVariational(Float64Test):
+    def test_one_step_optimal_high_precision(self):
+        X = torch.linspace(-3, 3, 10)
+        Y = torch.sin(X)
+
+        class ExactGP(gpytorch.models.ExactGP):
+            def __init__(self, train_x, train_y, kern, likelihood):
+                super().__init__(train_x, train_y, likelihood)
+                self.mean_module = gpytorch.means.ZeroMean()
+                self.covar_module = kern
+
+            def forward(self, x):
+                mean = self.mean_module(x)
+                covar = self.covar_module(x)
+                return gpytorch.distributions.MultivariateNormal(mean, covar)
+
+        likelihood = gpytorch.likelihoods.GaussianLikelihood(noise_constraint=GreaterThan(0, initial_value=0.1))
+
+        kern = gpytorch.kernels.ScaleKernel(gpytorch.kernels.RBFKernel())
+        kern.outputscale = 1
+
+        model_exact_gp = ExactGP(X, Y, kern, likelihood)
+        model_exact_gp.eval()
+        prediction_exact = model_exact_gp(X)
+
+        class NatGradsGP(gpytorch.models.ApproximateGP):
+            def __init__(self, kern, inducing_points):
+                variational_distribution = gpytorch.variational.NaturalVariationalDistribution(inducing_points.shape[0])
+                variational_strategy = gpytorch.variational.VariationalStrategy(
+                    self,
+                    inducing_points,
+                    variational_distribution,
+                    learn_inducing_locations=True,
+                    jitter_val=1e-24,
+                )
+                super().__init__(variational_strategy)
+                self.mean_module = gpytorch.means.ConstantMean()
+                self.covar_module = kern
+
+            def forward(self, x):
+                mean_x = self.mean_module(x)
+                covar_x = self.covar_module(x)
+                return gpytorch.distributions.MultivariateNormal(mean_x, covar_x)
+
+        model_ng = NatGradsGP(kern, X)
+
+        mll = gpytorch.mlls.VariationalELBO(likelihood, model_ng, num_data=X.shape[0])
+        from torch.utils.data import DataLoader, TensorDataset
+
+        data = DataLoader(TensorDataset(X, Y), batch_size=X.shape[0])
+
+        variational_ngd_optimizer = gpytorch.optim.NGD(model_ng.variational_parameters(), num_data=X.size(0), lr=1)
+        for _ in range(1):  # one step
+            for x, y in data:
+                variational_ngd_optimizer.zero_grad()
+
+                loss = -mll(model_ng(x), y)
+                # minibatch_iter.set_postfix(loss=loss.item())
+                loss.backward()
+                variational_ngd_optimizer.step()
+
+        prediction_ng = model_ng(X)
+
+        assert torch.allclose(prediction_exact.mean, prediction_ng.mean, rtol=1e-12, atol=1e-12)
+        assert torch.allclose(prediction_exact.variance, prediction_ng.variance, rtol=1e-12, atol=1e-12)
+
     def test_invertible_init(self, D=5):
         mu = torch.randn(D)
         cov = torch.randn(D, D).tril_()
         dist = MultivariateNormal(mu, CholLinearOperator(TriangularLinearOperator(cov)))
 
         v_dist = NaturalVariationalDistribution(D, mean_init_std=0.0)
         v_dist.initialize_variational_distribution(dist)
```

### Comparing `gpytorch-1.9.0/test/variational/test_nearest_neighbor_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_nearest_neighbor_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_orthogonally_decoupled_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_orthogonally_decoupled_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_unwhitened_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_unwhitened_variational_strategy.py`

 * *Files identical despite different names*

### Comparing `gpytorch-1.9.0/test/variational/test_variational_strategy.py` & `gpytorch-1.9.1/test/variational/test_variational_strategy.py`

 * *Files identical despite different names*

