# Comparing `tmp/stable_baselines3-2.0.0a4.tar.gz` & `tmp/stable_baselines3-2.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable_baselines3-2.0.0a4.tar", last modified: Thu Apr 13 14:50:21 2023, max compression
+gzip compressed data, was "stable_baselines3-2.0.0a5.tar", last modified: Fri Apr 14 11:50:42 2023, max compression
```

## Comparing `stable_baselines3-2.0.0a4.tar` & `stable_baselines3-2.0.0a5.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.010671 stable_baselines3-2.0.0a4/
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.0.0a4/LICENSE
--rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a4/NOTICE
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-13 14:50:21.010671 stable_baselines3-2.0.0a4/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14112 2023-03-29 22:22:11.000000 stable_baselines3-2.0.0a4/README.md
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2893 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/pyproject.toml
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-13 14:50:21.010671 stable_baselines3-2.0.0a4/setup.cfg
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5706 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/setup.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:20.998671 stable_baselines3-2.0.0a4/stable_baselines3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/__init__.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:20.998671 stable_baselines3-2.0.0a4/stable_baselines3/a2c/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/a2c/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8679 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/a2c/a2c.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a4/stable_baselines3/a2c/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/common/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11195 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/atari_wrappers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    37082 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/base_class.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    33755 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26487 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    27242 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20619 2023-04-13 10:43:35.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7539 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/env_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8099 2023-04-13 13:46:46.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/bit_flipping_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-04-13 13:46:46.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/identity_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6449 2023-04-13 13:46:46.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/envs/multi_input_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/evaluation.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    23428 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9068 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5545 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/noise.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26104 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/off_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12001 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/on_policy_algorithm.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    40200 2023-04-13 14:18:35.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8732 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/results_plotter.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/running_mean_std.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20664 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/save_util.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/common/sb2_compat/
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/sb2_compat/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5631 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/torch_layers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3117 2023-04-13 13:46:31.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/type_aliases.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20971 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/utils.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3113 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15814 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/base_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7073 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/dummy_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3519 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/patch_gym.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8298 2023-04-13 10:53:06.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/stacked_observations.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10631 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/subproc_vec_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2986 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/util.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-04-12 13:21:02.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2062 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_frame_stack.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3807 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12739 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4229 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_transpose.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3873 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_video_recorder.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/ddpg/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/ddpg/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5732 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a4/stable_baselines3/ddpg/ddpg.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/ddpg/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.002671 stable_baselines3-2.0.0a4/stable_baselines3/dqn/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/dqn/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    12908 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/dqn/dqn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    10673 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/dqn/policies.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.006671 stable_baselines3-2.0.0a4/stable_baselines3/her/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/her/__init__.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.0.0a4/stable_baselines3/her/goal_selection_strategy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17793 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/stable_baselines3/her/her_replay_buffer.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.006671 stable_baselines3-2.0.0a4/stable_baselines3/ppo/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/ppo/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a4/stable_baselines3/ppo/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14928 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/ppo/ppo.py
--rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a4/stable_baselines3/py.typed
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.006671 stable_baselines3-2.0.0a4/stable_baselines3/sac/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/sac/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20669 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/sac/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    15920 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/sac/sac.py
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.006671 stable_baselines3-2.0.0a4/stable_baselines3/td3/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/stable_baselines3/td3/__init__.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14471 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/td3/policies.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11193 2023-04-13 13:42:20.000000 stable_baselines3-2.0.0a4/stable_baselines3/td3/td3.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-13 13:45:04.000000 stable_baselines3-2.0.0a4/stable_baselines3/version.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:20.998671 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/PKG-INFO
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/SOURCES.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/dependency_links.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)      744 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/requires.txt
--rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2023-04-13 14:50:20.000000 stable_baselines3-2.0.0a4/stable_baselines3.egg-info/top_level.txt
-drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-13 14:50:21.010671 stable_baselines3-2.0.0a4/tests/
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5687 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_buffers.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     8324 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_callbacks.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_cnn.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/tests/test_custom_policy.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a4/tests/test_deterministic.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_dict_env.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_distributions.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3739 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_env_checker.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     9887 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_gae.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    11297 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_her.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_identity.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14793 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_logger.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     3756 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_predict.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_preprocessing.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_run.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    26907 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_save_load.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2781 2022-10-13 10:32:57.000000 stable_baselines3-2.0.0a4/tests/test_sde.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     4338 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_spaces.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a4/tests/test_tensorboard.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_train_eval_mode.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    22809 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_utils.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     1389 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_check_nan.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    20064 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_envs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     2231 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_extract_dict_obs.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_monitor.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    17089 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_normalize.py
--rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-12 14:32:39.000000 stable_baselines3-2.0.0a4/tests/test_vec_stacked_obs.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.672670 stable_baselines3-2.0.0a5/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1075 2020-03-18 13:32:59.000000 stable_baselines3-2.0.0a5/LICENSE
+-rw-r--r--   0 antonin   (1000) antonin   (1000)     1338 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a5/NOTICE
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-14 11:50:42.672670 stable_baselines3-2.0.0a5/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14112 2023-03-29 22:22:11.000000 stable_baselines3-2.0.0a5/README.md
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2893 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/pyproject.toml
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       38 2023-04-14 11:50:42.672670 stable_baselines3-2.0.0a5/setup.cfg
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5706 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/setup.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.656670 stable_baselines3-2.0.0a5/stable_baselines3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      939 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/__init__.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.656670 stable_baselines3-2.0.0a5/stable_baselines3/a2c/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/a2c/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8679 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/a2c/a2c.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a5/stable_baselines3/a2c/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.660670 stable_baselines3-2.0.0a5/stable_baselines3/common/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-10-07 09:00:57.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11195 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/atari_wrappers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    37082 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/base_class.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    33755 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26487 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    27242 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20619 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7539 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/env_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.660670 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      533 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8099 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/bit_flipping_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6029 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/identity_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6449 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/envs/multi_input_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6451 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/evaluation.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    23428 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9068 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5545 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/noise.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26104 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/off_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12001 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/on_policy_algorithm.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    40165 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8732 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4326 2023-03-12 17:58:51.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/results_plotter.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2012 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/running_mean_std.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20664 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/save_util.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.660670 stable_baselines3-2.0.0a5/stable_baselines3/common/sb2_compat/
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-08-06 19:36:01.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/sb2_compat/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5631 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13722 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/torch_layers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3117 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/type_aliases.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    21221 2023-04-14 11:50:27.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/utils.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3113 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15814 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/base_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7073 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/dummy_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3519 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/patch_gym.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8298 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/stacked_observations.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10631 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/subproc_vec_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2986 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/util.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4239 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      917 2023-04-12 13:21:02.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2062 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_frame_stack.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3807 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12739 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4229 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_transpose.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3873 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_video_recorder.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/ddpg/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      194 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/ddpg/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5732 2023-02-06 21:42:23.000000 stable_baselines3-2.0.0a5/stable_baselines3/ddpg/ddpg.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      139 2022-03-31 10:10:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/ddpg/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/dqn/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/dqn/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    12908 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/dqn/dqn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    10673 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/dqn/policies.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/her/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      204 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/her/__init__.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)      649 2020-10-24 10:56:51.000000 stable_baselines3-2.0.0a5/stable_baselines3/her/goal_selection_strategy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17793 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/her/her_replay_buffer.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/ppo/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/ppo/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      301 2022-08-17 12:52:47.000000 stable_baselines3-2.0.0a5/stable_baselines3/ppo/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14928 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/ppo/ppo.py
+-rw-r--r--   0 antonin   (1000) antonin   (1000)        0 2020-07-16 10:57:35.000000 stable_baselines3-2.0.0a5/stable_baselines3/py.typed
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.664670 stable_baselines3-2.0.0a5/stable_baselines3/sac/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/sac/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20669 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/sac/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    15920 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/sac/sac.py
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.668670 stable_baselines3-2.0.0a5/stable_baselines3/td3/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      189 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/stable_baselines3/td3/__init__.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14471 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/td3/policies.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11193 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/stable_baselines3/td3/td3.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        8 2023-04-14 11:50:27.000000 stable_baselines3-2.0.0a5/stable_baselines3/version.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.656670 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3277 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/PKG-INFO
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3614 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)        1 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)      744 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/requires.txt
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)       18 2023-04-14 11:50:42.000000 stable_baselines3-2.0.0a5/stable_baselines3.egg-info/top_level.txt
+drwxrwxr-x   0 antonin   (1000) antonin   (1000)        0 2023-04-14 11:50:42.672670 stable_baselines3-2.0.0a5/tests/
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5687 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_buffers.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     8324 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_callbacks.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13692 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_cnn.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2360 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/tests/test_custom_policy.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1362 2023-02-11 16:20:42.000000 stable_baselines3-2.0.0a5/tests/test_deterministic.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11765 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_dict_env.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9900 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_distributions.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3739 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_env_checker.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     9887 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     6776 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_gae.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    11297 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_her.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1989 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_identity.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14793 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_logger.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3957 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     3756 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_predict.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2429 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_preprocessing.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     7403 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_run.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    26907 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_save_load.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2781 2022-10-13 10:32:57.000000 stable_baselines3-2.0.0a5/tests/test_sde.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     4338 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_spaces.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2978 2023-01-25 14:44:15.000000 stable_baselines3-2.0.0a5/tests/test_tensorboard.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    13175 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_train_eval_mode.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    22809 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_utils.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     1389 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_check_nan.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    20064 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_envs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     2231 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_extract_dict_obs.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)     5276 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_monitor.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    17089 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_normalize.py
+-rw-rw-r--   0 antonin   (1000) antonin   (1000)    14821 2023-04-14 11:14:22.000000 stable_baselines3-2.0.0a5/tests/test_vec_stacked_obs.py
```

### Comparing `stable_baselines3-2.0.0a4/LICENSE` & `stable_baselines3-2.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/NOTICE` & `stable_baselines3-2.0.0a5/NOTICE`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/PKG-INFO` & `stable_baselines3-2.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable_baselines3
-Version: 2.0.0a4
+Version: 2.0.0a5
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
```

### Comparing `stable_baselines3-2.0.0a4/README.md` & `stable_baselines3-2.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/pyproject.toml` & `stable_baselines3-2.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/setup.py` & `stable_baselines3-2.0.0a5/setup.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/__init__.py` & `stable_baselines3-2.0.0a5/stable_baselines3/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/a2c/a2c.py` & `stable_baselines3-2.0.0a5/stable_baselines3/a2c/a2c.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/atari_wrappers.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/base_class.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/base_class.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/buffers.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/buffers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/callbacks.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/distributions.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/env_checker.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/env_checker.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/env_util.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/env_util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/envs/__init__.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/envs/bit_flipping_env.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/envs/bit_flipping_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/envs/identity_env.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/envs/identity_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/envs/multi_input_envs.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/envs/multi_input_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/evaluation.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/evaluation.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/logger.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/logger.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/monitor.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/noise.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/noise.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/off_policy_algorithm.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/off_policy_algorithm.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/on_policy_algorithm.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/on_policy_algorithm.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/policies.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,22 +894,20 @@
     :param normalize_images: Whether to normalize images or not,
          dividing by 255.0 (True by default)
     :param n_critics: Number of critic networks to create.
     :param share_features_extractor: Whether the features extractor is shared or not
         between the actor and the critic (this saves computation time)
     """
 
-    features_extractor: BaseFeaturesExtractor
-
     def __init__(
         self,
         observation_space: spaces.Space,
         action_space: spaces.Box,
         net_arch: List[int],
-        features_extractor: nn.Module,
+        features_extractor: BaseFeaturesExtractor,
         features_dim: int,
         activation_fn: Type[nn.Module] = nn.ReLU,
         normalize_images: bool = True,
         n_critics: int = 2,
         share_features_extractor: bool = True,
     ):
         super().__init__(
```

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/preprocessing.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/results_plotter.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/results_plotter.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/running_mean_std.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/running_mean_std.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/save_util.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/save_util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/sb2_compat/rmsprop_tf_like.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/torch_layers.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/torch_layers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/type_aliases.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/type_aliases.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/utils.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import random
 import re
 from collections import deque
 from inspect import signature
 from itertools import zip_longest
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 
+import cloudpickle
 import gymnasium as gym
 import numpy as np
 import torch as th
 from gymnasium import spaces
 
 import stable_baselines3 as sb3
 
@@ -528,16 +529,24 @@
         # wrongly linking to another issue on GitHub. Example: turn "#42" to "# 42".
         "OS": re.sub(r"#(\d)", r"# \1", f"{platform.platform()} {platform.version()}"),
         "Python": platform.python_version(),
         "Stable-Baselines3": sb3.__version__,
         "PyTorch": th.__version__,
         "GPU Enabled": str(th.cuda.is_available()),
         "Numpy": np.__version__,
-        "Gym": gym.__version__,
+        "Cloudpickle": cloudpickle.__version__,
+        "Gymnasium": gym.__version__,
     }
+    try:
+        import gym as openai_gym  # pytype: disable=import-error
+
+        env_info.update({"OpenAI Gym": openai_gym.__version__})
+    except ImportError:
+        pass
+
     env_info_str = ""
     for key, value in env_info.items():
         env_info_str += f"- {key}: {value}\n"
     if print_info:
         print(env_info_str)
     return env_info, env_info_str
```

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/__init__.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/__init__.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/base_vec_env.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/base_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/dummy_vec_env.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/dummy_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/patch_gym.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/patch_gym.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/stacked_observations.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/stacked_observations.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/subproc_vec_env.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/subproc_vec_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/util.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/util.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_check_nan.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_extract_dict_obs.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_extract_dict_obs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_frame_stack.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_frame_stack.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_monitor.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_normalize.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_transpose.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_transpose.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/common/vec_env/vec_video_recorder.py` & `stable_baselines3-2.0.0a5/stable_baselines3/common/vec_env/vec_video_recorder.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/ddpg/ddpg.py` & `stable_baselines3-2.0.0a5/stable_baselines3/ddpg/ddpg.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/dqn/dqn.py` & `stable_baselines3-2.0.0a5/stable_baselines3/dqn/dqn.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/dqn/policies.py` & `stable_baselines3-2.0.0a5/stable_baselines3/dqn/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/her/goal_selection_strategy.py` & `stable_baselines3-2.0.0a5/stable_baselines3/her/goal_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/her/her_replay_buffer.py` & `stable_baselines3-2.0.0a5/stable_baselines3/her/her_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/ppo/ppo.py` & `stable_baselines3-2.0.0a5/stable_baselines3/ppo/ppo.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/sac/policies.py` & `stable_baselines3-2.0.0a5/stable_baselines3/sac/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/sac/sac.py` & `stable_baselines3-2.0.0a5/stable_baselines3/sac/sac.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/td3/policies.py` & `stable_baselines3-2.0.0a5/stable_baselines3/td3/policies.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3/td3/td3.py` & `stable_baselines3-2.0.0a5/stable_baselines3/td3/td3.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3.egg-info/PKG-INFO` & `stable_baselines3-2.0.0a5/stable_baselines3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-baselines3
-Version: 2.0.0a4
+Version: 2.0.0a5
 Summary: Pytorch version of Stable Baselines, implementations of reinforcement learning algorithms.
 Home-page: https://github.com/DLR-RM/stable-baselines3
 Author: Antonin Raffin
 Author-email: antonin.raffin@dlr.de
 License: MIT
 Project-URL: Code, https://github.com/DLR-RM/stable-baselines3
 Project-URL: Documentation, https://stable-baselines3.readthedocs.io/
```

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3.egg-info/SOURCES.txt` & `stable_baselines3-2.0.0a5/stable_baselines3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/stable_baselines3.egg-info/requires.txt` & `stable_baselines3-2.0.0a5/stable_baselines3.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_buffers.py` & `stable_baselines3-2.0.0a5/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_callbacks.py` & `stable_baselines3-2.0.0a5/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_cnn.py` & `stable_baselines3-2.0.0a5/tests/test_cnn.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_custom_policy.py` & `stable_baselines3-2.0.0a5/tests/test_custom_policy.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_deterministic.py` & `stable_baselines3-2.0.0a5/tests/test_deterministic.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_dict_env.py` & `stable_baselines3-2.0.0a5/tests/test_dict_env.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_distributions.py` & `stable_baselines3-2.0.0a5/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_env_checker.py` & `stable_baselines3-2.0.0a5/tests/test_env_checker.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_envs.py` & `stable_baselines3-2.0.0a5/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_gae.py` & `stable_baselines3-2.0.0a5/tests/test_gae.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_her.py` & `stable_baselines3-2.0.0a5/tests/test_her.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_identity.py` & `stable_baselines3-2.0.0a5/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_logger.py` & `stable_baselines3-2.0.0a5/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_monitor.py` & `stable_baselines3-2.0.0a5/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_predict.py` & `stable_baselines3-2.0.0a5/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_preprocessing.py` & `stable_baselines3-2.0.0a5/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_run.py` & `stable_baselines3-2.0.0a5/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_save_load.py` & `stable_baselines3-2.0.0a5/tests/test_save_load.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_sde.py` & `stable_baselines3-2.0.0a5/tests/test_sde.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_spaces.py` & `stable_baselines3-2.0.0a5/tests/test_spaces.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_tensorboard.py` & `stable_baselines3-2.0.0a5/tests/test_tensorboard.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_train_eval_mode.py` & `stable_baselines3-2.0.0a5/tests/test_train_eval_mode.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_utils.py` & `stable_baselines3-2.0.0a5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_vec_check_nan.py` & `stable_baselines3-2.0.0a5/tests/test_vec_check_nan.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_vec_envs.py` & `stable_baselines3-2.0.0a5/tests/test_vec_envs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_vec_extract_dict_obs.py` & `stable_baselines3-2.0.0a5/tests/test_vec_extract_dict_obs.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_vec_monitor.py` & `stable_baselines3-2.0.0a5/tests/test_vec_monitor.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_vec_normalize.py` & `stable_baselines3-2.0.0a5/tests/test_vec_normalize.py`

 * *Files identical despite different names*

### Comparing `stable_baselines3-2.0.0a4/tests/test_vec_stacked_obs.py` & `stable_baselines3-2.0.0a5/tests/test_vec_stacked_obs.py`

 * *Files identical despite different names*

