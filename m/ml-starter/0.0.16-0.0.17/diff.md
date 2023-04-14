# Comparing `tmp/ml-starter-0.0.16.tar.gz` & `tmp/ml-starter-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.16.tar", last modified: Thu Apr 13 03:26:31 2023, max compression
+gzip compressed data, was "ml-starter-0.0.17.tar", last modified: Fri Apr 14 01:50:32 2023, max compression
```

## Comparing `ml-starter-0.0.16.tar` & `ml-starter-0.0.17.tar`

### file list

```diff
@@ -1,148 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.114343 ml-starter-0.0.16/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-13 03:26:20.000000 ml-starter-0.0.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-13 03:26:31.114343 ml-starter-0.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-13 03:26:20.000000 ml-starter-0.0.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/__version__.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.098342 ml-starter-0.0.16/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.102342 ml-starter-0.0.16/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.102342 ml-starter-0.0.16/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.102342 ml-starter-0.0.16/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/mp_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.102342 ml-starter-0.0.16/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17584 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.106342 ml-starter-0.0.16/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17834 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/ddp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.110342 ml-starter-0.0.16/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/cpu_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.110342 ml-starter-0.0.16/ml/trainers/mixins/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.114343 ml-starter-0.0.16/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-13 03:26:20.000000 ml-starter-0.0.16/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 03:26:31.114343 ml-starter-0.0.16/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-13 03:26:31.000000 ml-starter-0.0.16/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-13 03:26:20.000000 ml-starter-0.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 03:26:20.000000 ml-starter-0.0.16/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-13 03:26:20.000000 ml-starter-0.0.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 03:26:31.114343 ml-starter-0.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 03:26:20.000000 ml-starter-0.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.267999 ml-starter-0.0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 01:50:19.000000 ml-starter-0.0.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-14 01:50:32.267999 ml-starter-0.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 01:50:19.000000 ml-starter-0.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.219998 ml-starter-0.0.17/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/__version__.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.219998 ml-starter-0.0.17/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21504 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.223998 ml-starter-0.0.17/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.227998 ml-starter-0.0.17/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.227998 ml-starter-0.0.17/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.231998 ml-starter-0.0.17/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.231998 ml-starter-0.0.17/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.235998 ml-starter-0.0.17/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/mp_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.235998 ml-starter-0.0.17/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17564 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.243998 ml-starter-0.0.17/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.247999 ml-starter-0.0.17/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.247999 ml-starter-0.0.17/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.247999 ml-starter-0.0.17/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17640 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.247999 ml-starter-0.0.17/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.251999 ml-starter-0.0.17/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19149 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/ddp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.255998 ml-starter-0.0.17/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.263999 ml-starter-0.0.17/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.267999 ml-starter-0.0.17/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7805 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14152 2023-04-14 01:50:19.000000 ml-starter-0.0.17/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:50:32.267999 ml-starter-0.0.17/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-14 01:50:32.000000 ml-starter-0.0.17/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-14 01:50:19.000000 ml-starter-0.0.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 01:50:19.000000 ml-starter-0.0.17/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 01:50:19.000000 ml-starter-0.0.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 01:50:32.271999 ml-starter-0.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-14 01:50:19.000000 ml-starter-0.0.17/setup.py
```

### Comparing `ml-starter-0.0.16/PKG-INFO` & `ml-starter-0.0.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.16
+Version: 0.0.17
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.16/README.md` & `ml-starter-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/api.py` & `ml-starter-0.0.17/ml/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     "get_type_from_string",
     "get_worker_info",
     "get_world_size_optional",
     "get_world_size",
     "init_",
     "init_empty_weights",
     "InitializationType",
+    "instantiate_config",
     "is_debugging",
     "is_distributed",
     "is_master",
     "LearnedPositionalEmbeddings",
     "load_model_and_task",
     "Loss",
     "meta_to_empty_func",
@@ -198,16 +199,14 @@
     WorkerPool,
 )
 from ml.tasks.losses.reduce import cast_reduce_type, reduce
 from ml.tasks.rl.base import ReinforcementLearningTask, ReinforcementLearningTaskConfig
 from ml.tasks.sl.base import SupervisedLearningTask, SupervisedLearningTaskConfig
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig
 from ml.trainers.ddp import DDPTrainer
-from ml.trainers.mixins.device.auto import AutoDevice
-from ml.trainers.mixins.device.base import BaseDevice
 from ml.trainers.rl import (
     ReinforcementLearningDDPTrainer,
     ReinforcementLearningSlurmTrainer,
     ReinforcementLearningSlurmTrainerConfig,
     ReinforcementLearningTrainerConfig,
     ReinforcementLearningVanillaTrainer,
 )
@@ -224,26 +223,28 @@
 from ml.utils.atomic import atomic_save, open_atomic
 from ml.utils.augmentation import get_image_mask
 from ml.utils.caching import cached_object
 from ml.utils.checks import assert_no_nans
 from ml.utils.colors import colorize
 from ml.utils.data import get_dataset_split_for_phase, get_dataset_splits, get_worker_info
 from ml.utils.datetime import format_timedelta
+from ml.utils.device.auto import AutoDevice
+from ml.utils.device.base import BaseDevice
 from ml.utils.distributed import (
     get_master_addr,
     get_master_port,
     get_random_port,
     get_rank,
     get_rank_optional,
     get_world_size,
     get_world_size_optional,
     is_distributed,
     is_master,
 )
-from ml.utils.io import load_model_and_task
+from ml.utils.io import instantiate_config, load_model_and_task
 from ml.utils.large_models import init_empty_weights, meta_to_empty_func
 from ml.utils.logging import configure_logging
 from ml.utils.numpy import as_cpu_tensor, as_numpy_array
 from ml.utils.random import set_random_seed
 from ml.utils.staging import stage_environment
 from ml.utils.timer import Timer, timeout
 from ml.utils.video import READERS as VIDEO_READERS, WRITERS as VIDEO_WRITERS
```

### Comparing `ml-starter-0.0.16/ml/core/config.py` & `ml-starter-0.0.17/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/core/env.py` & `ml-starter-0.0.17/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/core/registry.py` & `ml-starter-0.0.17/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/core/state.py` & `ml-starter-0.0.17/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/loggers/base.py` & `ml-starter-0.0.17/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/loggers/meter.py` & `ml-starter-0.0.17/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/loggers/multi.py` & `ml-starter-0.0.17/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/loggers/stdout.py` & `ml-starter-0.0.17/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/loggers/tensorboard.py` & `ml-starter-0.0.17/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/lr_schedulers/base.py` & `ml-starter-0.0.17/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.17/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.17/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/lr_schedulers/linear.py` & `ml-starter-0.0.17/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.17/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.17/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/models/activations.py` & `ml-starter-0.0.17/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/models/base.py` & `ml-starter-0.0.17/ml/models/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import torch
 from torch import Tensor, nn
 
 from ml.core.config import BaseConfig, BaseObject
 from ml.loggers.multi import MultiLogger
 from ml.utils.colors import colorize
+from ml.utils.device.base import allow_nonblocking
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
 class BaseModelConfig(BaseConfig):
     """Defines the base config for all modules."""
@@ -36,16 +37,16 @@
 
     def init(self, device: torch.device, dtype: torch.dtype | None = None) -> None:
         # Moves all non-meta tensors to the first device.
         def move_to_device(t: Tensor) -> Tensor:
             if t.is_meta:
                 return t
             if t.is_floating_point():
-                return t.to(device=device, dtype=dtype, non_blocking=True)
-            return t.to(device=device, non_blocking=True)
+                return t.to(device=device, dtype=dtype, non_blocking=allow_nonblocking(device, t.device))
+            return t.to(device=device, non_blocking=allow_nonblocking(device, t.device))
 
         self._apply(move_to_device)
 
         bad_params = {(name, p.device) for name, p in self.named_parameters() if p.device != device}
         if bad_params:
             bad_param_names = sorted(list(bad_params))[:5]
             logger.warning(
@@ -75,9 +76,9 @@
     def get_dtype(self) -> torch.dtype:
         return next(p for p in self.parameters() if p.is_floating_point()).dtype
 
     @torch.jit.ignore
     def tensor_to(self, tensor: Tensor, non_blocking: bool = False) -> Tensor:
         device, dtype = self.get_device(), self.get_dtype()
         if tensor.is_floating_point() or tensor.is_complex():
-            return tensor.to(device, dtype, non_blocking=non_blocking)
-        return tensor.to(device, non_blocking=non_blocking)
+            return tensor.to(device, dtype, non_blocking=non_blocking and allow_nonblocking(device, tensor.device))
+        return tensor.to(device, non_blocking=non_blocking and allow_nonblocking(device, tensor.device))
```

### Comparing `ml-starter-0.0.16/ml/models/embeddings.py` & `ml-starter-0.0.17/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/models/init.py` & `ml-starter-0.0.17/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/models/norms.py` & `ml-starter-0.0.17/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/optimizers/adam.py` & `ml-starter-0.0.17/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/optimizers/adamw.py` & `ml-starter-0.0.17/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/optimizers/adan.py` & `ml-starter-0.0.17/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/optimizers/base.py` & `ml-starter-0.0.17/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/optimizers/sgd.py` & `ml-starter-0.0.17/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/optimizers/shampoo.py` & `ml-starter-0.0.17/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/scripts/cli.py` & `ml-starter-0.0.17/ml/scripts/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,24 +57,24 @@
     if len(args) == 0:
         show_help()
     option, args = args[0], args[1:]
 
     # Adds a global tag with the currently-selected option.
     add_global_tag(option)
 
-    # Parses the command-line arguments to a single DictConfig object.
-    config = parse_cli(args)
-    Objects.resolve_config(config)
-
     if option in without_objects_scripts:
         # Special handling for multi-processing; don't initialize anything since
         # everything will be initialized inside the child processes.
+        config = parse_cli(args)
+        Objects.resolve_config(config)
         without_objects_scripts[option](config)
     elif option in with_objects_scripts:
         # Converts the raw config to the objects they are pointing at.
+        config = parse_cli(args)
+        Objects.resolve_config(config)
         objs = Objects.parse_raw_config(config)
         with_objects_scripts[option](objs)
     else:
         print(f"Invalid option: {colorize(option, 'red')}\n", file=sys.stderr)
         show_help()
```

### Comparing `ml-starter-0.0.16/ml/scripts/compiler.py` & `ml-starter-0.0.17/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/scripts/stage.py` & `ml-starter-0.0.17/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/scripts/train.py` & `ml-starter-0.0.17/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/base.py` & `ml-starter-0.0.17/ml/tasks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 from ml.models.base import BaseModel
 from ml.tasks.datasets.collate import CollateMode, collate
 from ml.tasks.datasets.error_handling import (
     ErrorHandlingConfig,
     get_error_handling_dataset,
 )
 from ml.tasks.losses.reduce import cast_reduce_type, reduce
-from ml.trainers.mixins.device.auto import AutoDevice
-from ml.trainers.mixins.device.base import BaseDevice
+from ml.utils.device.auto import AutoDevice
+from ml.utils.device.base import BaseDevice
 from ml.utils.random import set_random_seed
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class CumulativeTimer:
     """Defines a simple timer to track an average value."""
```

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.17/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.17/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/collate.py` & `ml-starter-0.0.17/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.17/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.17/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.17/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.17/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.17/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/utils.py` & `ml-starter-0.0.17/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.17/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/environments/base.py` & `ml-starter-0.0.17/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/environments/utils.py` & `ml-starter-0.0.17/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/environments/worker.py` & `ml-starter-0.0.17/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/losses/reduce.py` & `ml-starter-0.0.17/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/rl/base.py` & `ml-starter-0.0.17/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/rl/replay.py` & `ml-starter-0.0.17/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/tasks/sl/base.py` & `ml-starter-0.0.17/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/trainers/base.py` & `ml-starter-0.0.17/ml/trainers/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import enum
 import functools
 import logging
 import os
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from pathlib import Path
+from pickle import UnpicklingError
 from typing import Any, Generic, Literal, TypeVar, cast, get_args
 
 import torch
 from omegaconf import II, MISSING, DictConfig, ListConfig, OmegaConf
 from torch import Tensor
 from torch.optim.optimizer import Optimizer
 
@@ -17,17 +18,17 @@
 from ml.core.state import State
 from ml.loggers.base import BaseLogger
 from ml.loggers.multi import MultiLogger
 from ml.lr_schedulers.base import BaseLRScheduler, SchedulerAdapter
 from ml.models.base import BaseModel
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.base import BaseTask
-from ml.trainers.mixins.device.auto import AutoDevice
-from ml.trainers.mixins.device.base import BaseDevice
 from ml.utils.colors import colorize
+from ml.utils.device.auto import AutoDevice
+from ml.utils.device.base import BaseDevice
 from ml.utils.distributed import is_master
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
@@ -308,22 +309,50 @@
         if self.checkpoint_config.save_every_n_steps is not None:
             if state.num_steps % self.checkpoint_config.save_every_n_steps == 0:
                 return True
         return False
 
     def load_checkpoint(
         self,
-        ckpt_path: Path,
+        ckpt: str | Path | dict,
         task: TaskT,
         model: ModelT,
         optim: Optimizer | None = None,
         lr_sched: SchedulerAdapter | None = None,
+        *,
+        weights_only: bool = True,
     ) -> State:
+        """Loads a given checkpoint, from a path or dictionary.
+
+        Args:
+            ckpt: The checkpoint to load.
+            task: The task to load the checkpoint into.
+            model: The model to load the checkpoint into.
+            optim: The optimizer to load the checkpoint into.
+            lr_sched: The learning rate scheduler to load the checkpoint into.
+            weights_only: If set, only load the model weights.
+
+        Returns:
+            The state loaded from the checkpoint.
+
+        Raises:
+            UnpicklingError: If there is some issue unpickling the checkpoint.
+        """
+
         with Timer("loading checkpoint"):
-            ckpt = torch.load(ckpt_path)
+            if isinstance(ckpt, (str, Path)):
+                try:
+                    ckpt = cast(dict, torch.load(ckpt, weights_only=weights_only))
+                except UnpicklingError:
+                    if weights_only:
+                        logger.warning("Failed to load checkpoint using `weights_only` flag, retrying without it")
+                        ckpt = cast(dict, torch.load(cast(str | Path, ckpt), weights_only=False))
+                    else:
+                        raise
+
             task.on_after_load_checkpoint(ckpt)
             if "model" in ckpt:
                 model.load_state_dict(ckpt["model"])
             else:
                 logger.warning("Checkpoint does not contain a model state dict")
             if "task" in ckpt:
                 task.load_state_dict(ckpt["task"])
@@ -336,15 +365,15 @@
                     logger.warning("Checkpoint does not contain an optimizer state dict")
             if lr_sched is not None:
                 if "lr_sched" in ckpt:
                     lr_sched.load_state_dict(ckpt["lr_sched"])
                 else:
                     logger.warning("Checkpoint does not contain a learning rate scheduler state dict")
             self.load_state_dict(ckpt)
-            state = ckpt["state"]
+            state = State(**ckpt["state"])
         return state
 
     def save_checkpoint(
         self,
         state: State,
         task: TaskT,
         model: ModelT,
@@ -353,21 +382,23 @@
     ) -> None:
         if is_master():
             with Timer("saving checkpoint"):
                 ckpt_path = self.get_ckpt_path(state)
                 logger.info("Saving checkpoint to %s", ckpt_path)
                 last_ckpt_path = self.get_ckpt_path()
                 ckpt_path.parent.mkdir(exist_ok=True, parents=True)
-                state_dict = {
+                state_dict: dict[str, Any] = {
                     "model": model.state_dict(),
                     "task": task.state_dict(),
                     "optim": None if optim is None else optim.state_dict(),
                     "lr_sched": None if lr_sched is None else lr_sched.state_dict(),
-                    "state": state,
+                    "state": asdict(state),
                 }
+                if self._raw_config is not None:
+                    state_dict["config"] = OmegaConf.to_container(self._raw_config)
                 self.update_state_dict(state_dict)
                 if last_ckpt_path.exists():
                     if self.checkpoint_config.only_save_most_recent:
                         base_ckpt = last_ckpt_path.resolve()
                         if base_ckpt.is_file():
                             base_ckpt.unlink()
                     last_ckpt_path.unlink()
```

### Comparing `ml-starter-0.0.16/ml/trainers/ddp.py` & `ml-starter-0.0.17/ml/trainers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/device/auto.py` & `ml-starter-0.0.17/ml/utils/device/auto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import logging
 from typing import Type
 
-from ml.trainers.mixins.device.base import BaseDevice
-from ml.trainers.mixins.device.cpu import CPUDevice
-from ml.trainers.mixins.device.gpu import GPUDevice
-from ml.trainers.mixins.device.metal import MetalDevice
+from ml.utils.device.base import BaseDevice
+from ml.utils.device.cpu import CPUDevice
+from ml.utils.device.gpu import GPUDevice
+from ml.utils.device.metal import MetalDevice
 from ml.utils.logging import INFOALL
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 # These devices are ordered by priority, so an earlier device in the list
 # is preferred to a later device in the list.
 ALL_DEVICES: list[Type[BaseDevice]] = [
```

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/device/base.py` & `ml-starter-0.0.17/ml/utils/device/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     _MultiProcessingDataLoaderIter,
 )
 
 from ml.core.common_types import Batch
 from ml.utils.timer import Timer
 
 
+def allow_nonblocking(device_a: torch.device, device_b: torch.device) -> bool:
+    return device_a.type in ("cpu", "cuda") and device_b.type in ("cpu", "cuda")
+
+
 def get_tasks_outstanding(dataloader_iter: _BaseDataLoaderIter) -> int:
     if isinstance(dataloader_iter, _MultiProcessingDataLoaderIter):
         try:
             return dataloader_iter._worker_result_queue.qsize()
         except NotImplementedError:
             return -2
     return -1
@@ -65,24 +69,26 @@
 
         self.to_device_func = to_device_func
         self.dataloader = dataloader
         self.raise_stop_iter = raise_stop_iter
         self.dataloader_iter = iter(self.dataloader)
         self.next_sample = None
         self.get_batch_time = 0.0
+        self.to_device_time = 0.0
         self.num_queued_samples = -1
 
-    def get_next_sample(self) -> Any:
-        sample = self.to_device_func(next(self.dataloader_iter))
-        self.num_queued_samples = get_tasks_outstanding(self.dataloader_iter)
-        return sample
-
     def prefetch(self) -> None:
         try:
-            self.next_sample = self.get_next_sample()
+            with Timer("getting sample from dataloader") as timer:
+                next_sample = next(self.dataloader_iter)
+            self.get_batch_time = timer.elapsed_time
+            with Timer("moving sample to device") as timer:
+                self.next_sample = self.to_device_func(next_sample)
+            self.to_device_time = timer.elapsed_time
+            self.num_queued_samples = get_tasks_outstanding(self.dataloader_iter)
         except StopIteration:
             self.next_sample = None
 
     def recursive_chunk(self, item: Any, chunks: int) -> list[Any]:
         """Applies a function recursively to tensors in an item.
 
         Args:
@@ -119,18 +125,16 @@
     def __iter__(self) -> Iterator[Batch]:
         self.prefetch()
 
         try:
             while True:
                 if self.next_sample is None:
                     raise StopIteration
-                with Timer("getting batch") as timer:
-                    sample = self.next_sample
-                    self.prefetch()
-                self.get_batch_time = timer.elapsed_time
+                sample = self.next_sample
+                self.prefetch()
                 yield sample
 
         except StopIteration:
             # Resets the dataloader if the iteration has completed.
             self.dataloader_iter = iter(self.dataloader)
             if self.raise_stop_iter:
                 raise
@@ -190,15 +194,15 @@
         device = cls.get_device()
         dtype_fp = cls.get_floating_point_type()
         return Prefetcher.recursive_apply(
             sample,
             lambda t: t.to(
                 device,
                 dtype_fp if t.is_floating_point() else t.dtype,
-                non_blocking=True,
+                non_blocking=allow_nonblocking(t.device, device),
             ),
         )
 
     @classmethod
     def get_prefetcher(cls, dataloader: DataLoader) -> Prefetcher:
         return Prefetcher(functools.partial(cls.sample_to_device), dataloader)
```

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/device/cpu.py` & `ml-starter-0.0.17/ml/utils/device/cpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Callable
 
 import torch
 
-from ml.trainers.mixins.device.base import BaseDevice
+from ml.utils.device.base import BaseDevice
 
 
 class CPUDevice(BaseDevice):
     """Mixin to support CPU training."""
 
     @classmethod
     def has_device(cls) -> bool:
```

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/device/gpu.py` & `ml-starter-0.0.17/ml/utils/device/gpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import os
 from typing import Callable
 
 import torch
 
 from ml.core.env import is_gpu_disabled
-from ml.trainers.mixins.device.base import BaseDevice
+from ml.utils.device.base import BaseDevice
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def get_env_bool(key: str) -> bool:
     val = int(os.environ.get(key, 0))
     assert val in (0, 1), f"Invalid value for {key}: {val}"
```

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/device/metal.py` & `ml-starter-0.0.17/ml/utils/device/metal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Callable
 
 import torch
 
 from ml.core.env import is_metal_disabled
-from ml.trainers.mixins.device.base import BaseDevice
+from ml.utils.device.base import BaseDevice
 
 
 class MetalDevice(BaseDevice):
     """Mixin to support Metal training."""
 
     @classmethod
     def has_device(cls) -> bool:
```

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.17/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.17/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.17/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.17/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/trainers/rl.py` & `ml-starter-0.0.17/ml/trainers/rl.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,16 +129,15 @@
 
                     with self.step_context("build_rl_dataset"):
                         train_ds = task.build_rl_dataset(samples)
                         train_dl = task.get_dataloader(train_ds, "train")
                         train_pf = self._device.get_prefetcher(train_dl)
 
                     for train_batch in train_pf:
-                        self.logger.log_scalar("num_queued_samples", train_pf.num_queued_samples, namespace="trainer")
-                        self.logger.log_scalar("dt/get_batch", train_pf.get_batch_time, namespace="timers")
+                        self._log_prefetcher_stats(train_pf, "train")
 
                         if task.is_training_over(state):
                             on_finish_training()
 
                         with self.step_context("on_step_start"):
                             self.on_step_start(state, train_batch, task, model, optim, lr_sched)
 
@@ -166,15 +165,20 @@
 
                     with self.step_context("on_epoch_end"):
                         self.on_epoch_end(state, task, model, optim, lr_sched)
 
                     state.num_epochs += 1
 
         except TrainingFinishedException:
-            logger.info("Finished training for %s", self.exp_dir / "config.yaml")
+            logger.info(
+                "Finished training after %d epochs, %d steps, %d samples",
+                state.num_epochs,
+                state.num_steps,
+                state.num_samples,
+            )
 
         except Exception:
             logger.exception("Caught exception during training loop")
 
         finally:
             self.remove_lock_file("running", missing_ok=True)
             logger.info("Exiting training job for %s", self.exp_dir / "config.yaml")
```

### Comparing `ml-starter-0.0.16/ml/trainers/sl.py` & `ml-starter-0.0.17/ml/trainers/sl.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from ml.core.config import conf_field
 from ml.core.registry import register_trainer
 from ml.lr_schedulers.base import BaseLRScheduler
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.sl.base import SupervisedLearningTask
 from ml.trainers.base import ModelT
 from ml.trainers.ddp import DDPTrainer
-from ml.trainers.mixins.device.base import InfinitePrefetcher
 from ml.trainers.slurm import SlurmTrainer, SlurmTrainerConfig
 from ml.trainers.vanilla import TrainingFinishedException, VanillaTrainer, VanillaTrainerConfig
+from ml.utils.device.base import InfinitePrefetcher
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ValidationConfig:
@@ -129,16 +129,15 @@
                     with self.step_context("on_epoch_start"):
                         self.on_epoch_start(state, task, model, optim, lr_sched)
 
                     state.num_epoch_steps = 0
                     state.num_epoch_samples = 0
 
                     for train_batch in train_pf:
-                        self.logger.log_scalar("num_queued_samples", train_pf.num_queued_samples, namespace="trainer")
-                        self.logger.log_scalar("dt/get_batch", train_pf.get_batch_time, namespace="timers")
+                        self._log_prefetcher_stats(train_pf, "train")
 
                         if task.is_training_over(state):
                             on_finish_training()
 
                         with self.step_context("on_step_start"):
                             self.on_step_start(state, train_batch, task, model, optim, lr_sched)
 
@@ -150,14 +149,16 @@
                             model=model,
                             optim=optim,
                             lr_sched=lr_sched,
                         )
 
                         valid_every_n_steps = self.config.validation.valid_every_n_steps
                         if valid_every_n_steps is not None and state.num_steps % valid_every_n_steps == 0:
+                            self._log_prefetcher_stats(valid_pf, "valid")
+
                             self.val_step(
                                 task_model=task_model,
                                 batch=next(valid_pf_iter),
                                 state=state,
                                 task=task,
                                 model=model,
                             )
@@ -173,15 +174,20 @@
 
                     with self.step_context("on_epoch_end"):
                         self.on_epoch_end(state, task, model, optim, lr_sched)
 
                     state.num_epochs += 1
 
         except TrainingFinishedException:
-            logger.info("Finished training for %s", self.exp_dir / "config.yaml")
+            logger.info(
+                "Finished training after %d epochs, %d steps, %d samples",
+                state.num_epochs,
+                state.num_steps,
+                state.num_samples,
+            )
 
         except Exception:
             logger.exception("Caught exception during training loop")
 
         finally:
             self.remove_lock_file("running", missing_ok=True)
             logger.info("Exiting training job for %s", self.exp_dir / "config.yaml")
```

### Comparing `ml-starter-0.0.16/ml/trainers/slurm.py` & `ml-starter-0.0.17/ml/trainers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/trainers/vanilla.py` & `ml-starter-0.0.17/ml/trainers/vanilla.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 import torch
 from omegaconf import II
 from torch import Tensor, nn
 from torch.optim import Optimizer
 
 from ml.core.common_types import Batch, Loss
 from ml.core.config import conf_field
-from ml.core.state import State, set_phase
+from ml.core.state import Phase, State, set_phase
 from ml.lr_schedulers.base import BaseLRScheduler, SchedulerAdapter
 from ml.optimizers.base import BaseOptimizer
 from ml.trainers.base import BaseTrainer, BaseTrainerConfig, ModelT, TaskT
 from ml.trainers.mixins.cpu_stats import CPUStatsConfig, CPUStatsMixin
 from ml.trainers.mixins.gpu_stats import GPUStatsConfig, GPUStatsMixin
 from ml.trainers.mixins.grad_clipping import (
     GradientClippingConfig,
     GradientClippingTrainerMixin,
 )
 from ml.trainers.mixins.mixed_precision import (
     MixedPrecisionTrainerConfig,
     MixedPrecisionTrainerMixin,
 )
 from ml.trainers.mixins.profiler import ProfilerTrainerConfig, ProfilerTrainerMixin
+from ml.utils.device.base import Prefetcher
 from ml.utils.distributed import is_master
 from ml.utils.timer import Timer
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class TrainingFinishedException(Exception):
@@ -104,15 +105,15 @@
     CPUStatsMixin[VanillaTrainerConfigT, ModelT, TaskT],
     BaseTrainer[VanillaTrainerConfigT, ModelT, TaskT],
     Generic[VanillaTrainerConfigT, ModelT, TaskT],
 ):
     def get_task_model_impl(self, task: TaskT, model: ModelT) -> nn.Module:
         device, dtype = self._device.get_device(), self._weight_precision
         model.init(device, dtype)
-        task.to(device, dtype, non_blocking=True)
+        task.to(device, dtype)
         task_model: nn.Module = TaskModel(task=task, model=model)
         return task_model
 
     def get_task_model(self, task: TaskT, model: ModelT) -> nn.Module:
         return self.get_task_model_impl(task, model)
 
     def train_step(
@@ -284,9 +285,14 @@
         optim: Optimizer,
         lr_sched: SchedulerAdapter,
     ) -> State:
         if (ckpt_path := self.get_ckpt_path()).exists():
             return self.load_checkpoint(ckpt_path, task, model, optim, lr_sched)
         return State.init_state()
 
+    def _log_prefetcher_stats(self, pf: Prefetcher, phase: Phase) -> None:
+        self.logger.log_scalar(f"num_queued_{phase}_samples", pf.num_queued_samples, namespace="trainer")
+        self.logger.log_scalar(f"dt/get_{phase}_batch", pf.get_batch_time, namespace="timers")
+        self.logger.log_scalar(f"dt/get_{phase}_batch", pf.to_device_time, namespace="timers")
+
     def launch(self) -> None:
         raise NotImplementedError(f"{self.__class__.__name__} doesn't support multiprocess training")
```

### Comparing `ml-starter-0.0.16/ml/utils/argparse.py` & `ml-starter-0.0.17/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/atomic.py` & `ml-starter-0.0.17/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/augmentation.py` & `ml-starter-0.0.17/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/caching.py` & `ml-starter-0.0.17/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/call_train.py` & `ml-starter-0.0.17/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/cli.py` & `ml-starter-0.0.17/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/colors.py` & `ml-starter-0.0.17/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/compiler.py` & `ml-starter-0.0.17/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/data.py` & `ml-starter-0.0.17/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/datetime.py` & `ml-starter-0.0.17/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/distributed.py` & `ml-starter-0.0.17/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/large_models.py` & `ml-starter-0.0.17/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/logging.py` & `ml-starter-0.0.17/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/meter.py` & `ml-starter-0.0.17/ml/utils/meter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 from typing import Any, cast
 
 import torch
 import torch.distributed as dist
 from torch import Tensor
 
-from ml.trainers.mixins.device.auto import AutoDevice
+from ml.utils.device.auto import AutoDevice
 
 
 @functools.lru_cache
 def get_device() -> torch.device:
     return AutoDevice.detect_device().get_device()
```

### Comparing `ml-starter-0.0.16/ml/utils/staging.py` & `ml-starter-0.0.17/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/timer.py` & `ml-starter-0.0.17/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml/utils/video.py` & `ml-starter-0.0.17/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.17/ml_starter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.16
+Version: 0.0.17
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.16/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.17/ml_starter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -83,22 +83,17 @@
 ml/trainers/slurm.py
 ml/trainers/vanilla.py
 ml/trainers/mixins/__init__.py
 ml/trainers/mixins/cpu_stats.py
 ml/trainers/mixins/gpu_stats.py
 ml/trainers/mixins/grad_clipping.py
 ml/trainers/mixins/mixed_precision.py
+ml/trainers/mixins/monitor_process.py
 ml/trainers/mixins/profiler.py
 ml/trainers/mixins/step_wrapper.py
-ml/trainers/mixins/device/__init__.py
-ml/trainers/mixins/device/auto.py
-ml/trainers/mixins/device/base.py
-ml/trainers/mixins/device/cpu.py
-ml/trainers/mixins/device/gpu.py
-ml/trainers/mixins/device/metal.py
 ml/utils/__init__.py
 ml/utils/argparse.py
 ml/utils/atomic.py
 ml/utils/augmentation.py
 ml/utils/caching.py
 ml/utils/call_train.py
 ml/utils/checks.py
@@ -115,13 +110,19 @@
 ml/utils/networking.py
 ml/utils/numpy.py
 ml/utils/paths.py
 ml/utils/random.py
 ml/utils/staging.py
 ml/utils/timer.py
 ml/utils/video.py
+ml/utils/device/__init__.py
+ml/utils/device/auto.py
+ml/utils/device/base.py
+ml/utils/device/cpu.py
+ml/utils/device/gpu.py
+ml/utils/device/metal.py
 ml_starter.egg-info/PKG-INFO
 ml_starter.egg-info/SOURCES.txt
 ml_starter.egg-info/dependency_links.txt
 ml_starter.egg-info/entry_points.txt
 ml_starter.egg-info/requires.txt
 ml_starter.egg-info/top_level.txt
```

### Comparing `ml-starter-0.0.16/pyproject.toml` & `ml-starter-0.0.17/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.16/setup.py` & `ml-starter-0.0.17/setup.py`

 * *Files identical despite different names*

