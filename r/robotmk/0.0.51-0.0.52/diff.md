# Comparing `tmp/robotmk-0.0.51.tar.gz` & `tmp/robotmk-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.51.tar", last modified: Fri Apr 14 10:36:47 2023, max compression
+gzip compressed data, was "robotmk-0.0.52.tar", last modified: Fri Apr 14 11:57:43 2023, max compression
```

## Comparing `robotmk-0.0.51.tar` & `robotmk-0.0.52.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      110 2023-04-14 10:36:34.281720 robotmk-0.0.51/.bumpversion.cfg
--rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.51/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.51/README.md
--rw-r--r--   0        0        0      739 2023-04-12 16:12:36.358474 robotmk-0.0.51/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.51/src/_confitree/__init__.py
--rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.51/src/_confitree/confitree.py
--rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.51/src/_confitree/robotmk.yml
--rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.51/src/_robotmk/__init__.py
--rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.51/src/_robotmk/__main__.py
--rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.51/src/_robotmk/cli.py
--rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/agent/__init__.py
--rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/agent/agent.py
--rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/agent/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/output/__init__.py
--rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/output/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/robot/__init__.py
--rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/robot/cli.py
--rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/robotmk.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/specialagent/__init__.py
--rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/specialagent/cli.py
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.51/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.51/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-14 10:36:34.281720 robotmk-0.0.51/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.51/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.51/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.51/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    17518 2023-04-14 10:20:54.767048 robotmk-0.0.51/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.51/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.51/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.51/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0      681 2023-04-13 13:22:33.639789 robotmk-0.0.51/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.51/src/robotmk/context/local/__init__.py
--rw-r--r--   0        0        0     1491 2023-04-13 11:46:06.562610 robotmk-0.0.51/src/robotmk/context/local/cli.py
--rw-r--r--   0        0        0     2052 2023-04-13 11:47:44.173586 robotmk-0.0.51/src/robotmk/context/local/local.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.51/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.51/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.51/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.51/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.51/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.51/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.51/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3825 2023-04-13 11:46:27.306392 robotmk-0.0.51/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.51/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     6576 2023-04-13 05:28:33.289623 robotmk-0.0.51/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     4506 2023-04-14 10:30:06.489439 robotmk-0.0.51/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.51/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     4728 2023-04-14 08:45:52.961802 robotmk-0.0.51/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.51/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-09 16:52:38.817097 robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6448 2023-04-09 16:54:03.952360 robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4662 2023-04-09 17:05:22.342438 robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     2762 2023-04-13 05:44:33.655252 robotmk-0.0.51/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.51/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.51/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     3404 2023-04-14 10:11:36.108721 robotmk-0.0.51/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.51/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.51/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.51/src/robotmk/logger.py
--rw-r--r--   0        0        0     3643 2023-04-14 10:22:44.709931 robotmk-0.0.51/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.51/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.51/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.51/tests/config/robotmk.yml
--rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.51/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.51/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.51/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.51/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.51/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.51/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.51/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.51/tests/context/test_cli.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.51/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 robotmk-0.0.51/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-14 11:57:35.028413 robotmk-0.0.52/.bumpversion.cfg
+-rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.52/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.52/README.md
+-rw-r--r--   0        0        0      739 2023-04-12 16:12:36.358474 robotmk-0.0.52/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.52/src/_confitree/__init__.py
+-rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.52/src/_confitree/confitree.py
+-rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.52/src/_confitree/robotmk.yml
+-rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.52/src/_robotmk/__init__.py
+-rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.52/src/_robotmk/__main__.py
+-rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.52/src/_robotmk/cli.py
+-rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/agent/__init__.py
+-rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/agent/agent.py
+-rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/agent/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/output/__init__.py
+-rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/output/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/robot/__init__.py
+-rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/robot/cli.py
+-rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/robotmk.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/specialagent/__init__.py
+-rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.52/src/_robotmk/modes/specialagent/cli.py
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.52/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.52/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-14 11:57:35.028413 robotmk-0.0.52/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.52/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.52/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.52/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    17797 2023-04-14 11:06:00.625074 robotmk-0.0.52/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.52/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.52/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.52/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0      681 2023-04-13 13:22:33.639789 robotmk-0.0.52/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.52/src/robotmk/context/local/__init__.py
+-rw-r--r--   0        0        0     1491 2023-04-13 11:46:06.562610 robotmk-0.0.52/src/robotmk/context/local/cli.py
+-rw-r--r--   0        0        0     2052 2023-04-13 11:47:44.173586 robotmk-0.0.52/src/robotmk/context/local/local.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.52/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.52/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.52/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.52/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.52/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.52/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.52/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3825 2023-04-13 11:46:27.306392 robotmk-0.0.52/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.52/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     6662 2023-04-14 11:19:23.461781 robotmk-0.0.52/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     4506 2023-04-14 10:30:06.489439 robotmk-0.0.52/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.52/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     4732 2023-04-14 11:14:59.168198 robotmk-0.0.52/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.52/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.52/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5623 2023-04-14 11:35:03.948826 robotmk-0.0.52/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6474 2023-04-14 11:50:43.784189 robotmk-0.0.52/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4818 2023-04-14 11:43:33.303934 robotmk-0.0.52/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     2793 2023-04-14 11:13:48.468830 robotmk-0.0.52/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.52/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.52/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     3363 2023-04-14 11:56:36.876954 robotmk-0.0.52/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.52/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.52/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.52/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3643 2023-04-14 10:22:44.709931 robotmk-0.0.52/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.52/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.52/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.52/tests/config/robotmk.yml
+-rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.52/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.52/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.52/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.52/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.52/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.52/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.52/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.52/tests/context/test_cli.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.52/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 robotmk-0.0.52/PKG-INFO
```

### Comparing `robotmk-0.0.51/pyproject.toml` & `robotmk-0.0.52/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/_confitree/confitree.py` & `robotmk-0.0.52/src/_confitree/confitree.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/_confitree/robotmk.yml` & `robotmk-0.0.52/src/_confitree/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/_robotmk/__init__.py` & `robotmk-0.0.52/src/_robotmk/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/_robotmk/__main__.py` & `robotmk-0.0.52/src/_robotmk/__main__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/_robotmk/cli.py` & `robotmk-0.0.52/src/_robotmk/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/_robotmk/modes/__init__.py` & `robotmk-0.0.52/src/_robotmk/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/_robotmk/modes/agent/agent.py` & `robotmk-0.0.52/src/_robotmk/modes/agent/agent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/_robotmk/modes/agent/cli.py` & `robotmk-0.0.52/src/_robotmk/modes/agent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/categories.json` & `robotmk-0.0.52/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/click_tutorial.py` & `robotmk-0.0.52/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/cli/cli.py` & `robotmk-0.0.52/src/robotmk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.52/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/config/config.py` & `robotmk-0.0.52/src/robotmk/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,22 +77,29 @@
             suitename = self.configdict["common"]["suiteuname"]
             keys[:1] = ["suites", suitename]
         return keys
 
     def get(self, name: str, default=None) -> str:
         """Get a value from the object with dot notation.
 
-        Shorthand 'suitecfg' can be used for 'suites.<suiteuname>'.
+        Shorthands:
+        - 'suitecfg' can be used for 'suites.<suiteuname>'.
+        - 'basic_cfg' can be used for the basic config dict.
 
         Examples:
             cfg.get("common.cfgdir")
             cfg.get("suitecfg.run.rcc")
+            cfg.get("basic_cfg.common.cfgdir") -> returns cfgdir value from the configuration
         """
         keys = self.__translate_keys(name)
-        m = self.configdict
+        if keys[0] == "basic_cfg":
+            m = self.basic_cfg
+            keys = keys[1:]
+        else:
+            m = self.configdict
         # prev = self.configdict
         try:
             for key in keys:
                 # prev = m
                 # prev_k = key
                 m = m.get(key, {})
             if type(m) is dict:
```

### Comparing `robotmk-0.0.51/src/robotmk/config/yml.py` & `robotmk-0.0.52/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/abstract.py` & `robotmk-0.0.52/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/context.py` & `robotmk-0.0.52/src/robotmk/context/context.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/local/cli.py` & `robotmk-0.0.52/src/robotmk/context/local/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/local/local.py` & `robotmk-0.0.52/src/robotmk/context/local/local.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.52/src/robotmk/context/specialagent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.52/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/suite/cli.py` & `robotmk-0.0.52/src/robotmk/context/suite/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.52/src/robotmk/context/suite/strategies/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     def prepare(self, *args, **kwargs) -> int:
         # nothing to do
         return 0
 
     def execute(self, *args, **kwargs) -> int:
         # DEBUG: " ".join(self.target.command)
+        # DEBUG: [f"{k}={v}" for (k,v) in environment.items()  if k.startswith("RO")]
         if kwargs.get("env"):
             environment = kwargs["env"]
         else:
             environment = os.environ
         result = subprocess.run(
             self.target.command, capture_output=True, env=environment
         )
```

### Comparing `robotmk-0.0.51/src/robotmk/context/suite/suite.py` & `robotmk-0.0.52/src/robotmk/context/suite/suite.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/context/suite/target/rcc.py` & `robotmk-0.0.52/src/robotmk/context/suite/target/rcc.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,16 +46,16 @@
         This function first exports the current config to the environment and
         then adds the special settings on top.
         """
         env = os.environ.copy()
         added_settings = {
             "suitecfg.run.rcc": False,
             "suitecfg.uuid": self.uuid,
-            "common.logdir": "%s/%s"
-            % (self.config.basic_cfg["common"]["logdir"], "robotframework"),
+            # "common.logdir": "%s/%s"
+            # % (self.config.basic_cfg["common"]["logdir"], "robotframework"),
         }
         self.config.cfg_to_environment(self.config.configdict, environ=env)
         self.config.dotcfg_to_env(added_settings, environ=env)
         return env
 
     def run(self):
         # Before we blow up the whole thing, we should check if the suite is RCC compatible and allowed to run
```

### Comparing `robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.52/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,30 +97,32 @@
         # for f in filenames:
         #     self.suite._runner.logdebug(" - %s" % f)
 
         # rebot wants to print out the generated file names on stdout; write to devnull
         devnull = open(os.devnull, "w")
         rebot(
             *outputfiles,
-            outputdir=self.target.logdir,
+            outputdir=self.target.robot_params["outputdir"],
             output=self.target.output_xml,
             log=self.target.log_html,
             report=None,
             merge=True,
             stdout=devnull,
         )
         # self.suite._runner.loginfo("Merged results of all reexecutions into:")
         # self.suite._runner.loginfo(" - %s" % self.suite.output)
         # self.suite._runner.loginfo(" - %s" % self.suite.log)
 
     def _glob_target_outputfiles(self):
         """Returns the list of XML output files of the target execution attempts 1..n"""
         glob_pattern = "%s-*.xml" % self.target.output_filename.rsplit("-", 1)[0]
         outputfiles = sorted(
-            glob.glob(str(Path(self.target.logdir).joinpath(glob_pattern)))
+            glob.glob(
+                str(Path(self.target.robot_params["outputdir"]).joinpath(glob_pattern))
+            )
         )
         return outputfiles
 
 
 class CompleteRetry(RetryStrategy):
     """Execution strategy for suites with complete re-execution"""
 
@@ -143,12 +145,12 @@
     def _reparametrize(self):
         """Reparametrize the suite for the next attempt.
 
         The next attempt needs the XML file of the last attempt as input.
         From there it will read failed tests and re-execute them only."""
         # Chance for next try. Attempt gets increased, output files get bumped
         failed_xml = Path(self.target.logdir).joinpath(self.target.output_xml)
-        self.target.robotmk_params.update({"rerunfailed": str(failed_xml)})
+        self.target.robot_params.update({"rerunfailed": str(failed_xml)})
         rerun_selection = self.target.config.get(
             "suitecfg.retry_failed.rerun_selection", {}
         ).asdict()
-        self.target.robotmk_params.update(rerun_selection)
+        self.target.robot_params.update(rerun_selection)
```

### Comparing `robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.52/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,36 +35,36 @@
 
         self.shortuuid = self.uuid[:8]
         # this timestamp is used to keep all result files in order; it is used
         # for all target executions
         self._timestamp = self.get_now_as_epoch()
         self._state = RFState(self)
         # params for RF: global ones & re-execution
-        # self.robotmk_params = {"console": "NONE", "report": "NONE"}
-        self.robotmk_params = {"report": "NONE"}
+        # self.robot_params = {"console": "NONE", "report": "NONE"}
+        self.robot_params = {"report": "NONE"}
 
     def __str__(self) -> str:
         return "robotframework"
 
     @property
     def command(self):
         """The command will be used by the Run strategy (self.target.command).
 
         In RF target, the complete commandline must be built to execute the RF suite.
         (See https://robot-framework.readthedocs.io/en/latest/autodoc/robot.html#robot.run.run_cli)
         TODO: Logging"""
-        self.robotmk_params.update(
+        self.robot_params.update(
             {
                 "log": self.log_html,
                 "output": self.output_xml,
             }
         )
 
         suite_params = mergedeep.merge(
-            self.config.get("suitecfg.params").asdict(), self.robotmk_params
+            {}, self.config.get("suitecfg.params").asdict(), self.robot_params
         )
         arglist = ["robot"]
         for k, v in suite_params.items():
             arg = f"--{k}"
             # create something we can iterate over
             if isinstance(v, str):
                 # key:value    => convert to 1 el list
@@ -99,15 +99,17 @@
         if self.is_disabled_by_flagfile:
             # TODO: Log skipped
             # reason = self.get_disabled_reason()
             return
         else:
             # Tell Robot Framework to write its "output" files into the log dir.
             # The "outputdir" is where RMK produces files later for the agent.
-            self.robotmk_params.update({"outputdir": self.logdir})
+            self.robot_params.update(
+                {"outputdir": str(Path(self.logdir).joinpath("robotframework"))}
+            )
             self._state.timer_start()
             self.rc = self.retry_strategy.run()
             self._state.timer_stop()
             self._state.write()
             pass
 
     def get_now_as_dt(self):
@@ -162,33 +164,31 @@
             )
         return suite_filename
 
     @property
     def statefile_fullpath(self):
         return str(Path(self.outdir).joinpath(self.suiteuname + ".json"))
 
-    @property
-    def output_xml_fullpath(self):
-        return self.logdir.joinpath(self.output_xml)
-
+    # XML ---
     @property
     def output_xml(self):
         return self.output_filename + ".xml"
 
     @property
     def output_xml_fullpath(self):
-        return str(Path(self.logdir).joinpath(self.output_xml))
+        return str(Path(self.robot_params["outputdir"]).joinpath(self.output_xml))
 
+    # HTML ---
     @property
     def log_html(self):
         return self.output_filename + ".html"
 
     @property
     def log_html_fullpath(self):
-        return str(Path(self.logdir).joinpath(self.log_html))
+        return str(Path(self.robot_params["outputdir"]).joinpath(self.log_html))
 
     # Suite timestamp for filenames
     @property
     def timestamp(self):
         return self._timestamp
 
     @timestamp.setter
```

### Comparing `robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.52/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,23 +45,27 @@
         self._runtime = self._end_time - self._start_time
 
     def write_console_log(self) -> None:
         for k, result in self.target.console_results.items():
             # HEREIWAS:
             data = json.dumps(result, indent=4)
             filename = (
-                Path(self.target.logdir) / f"{self.target.output_filename}-{int(k)}.txt"
+                Path(self.target.robot_params["outputdir"])
+                / f"{self.target.output_filename}-{int(k)}.txt"
             )
             self.write_data2file(data, filename)
             pass
 
     def write_result_json(self) -> None:
         """ """
 
         try:
+            Path(self.target.statefile_fullpath).parent.mkdir(
+                parents=True, exist_ok=True
+            )
             with open(self.target.statefile_fullpath, "w", encoding="utf-8") as outfile:
                 json.dump(self.statedata, outfile, indent=2, sort_keys=False)
         except IOError as e:
             # Error gets logged, will come to light by staleness check
             pass
 
     def write_data2file(self, data: str, filename: str):
```

### Comparing `robotmk-0.0.51/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.52/src/robotmk/context/suite/target/target.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,17 +52,18 @@
         config: dict,
         logger: RobotmkLogger,
     ):
         super().__init__(suiteuname, config, logger)
 
         # Store RCC and RF logs in separate folders
         # TODO: relly needed?
-        self.config.set(
-            "common.logdir", "%s/%s" % (self.config.get("common.logdir"), str(self))
-        )
+        # self.config.set(
+        #     "common.logdir",
+        #     "%s/%s" % (self.config.get("basic_cfg.common.logdir"), str(self)),
+        # )
 
         self.path = Path(self.config.get("common.robotdir")).joinpath(
             self.config.get("suitecfg.path")
         )
         self.run_strategy = RunStrategyFactory(self).create()
         # list of subprocess' results and console output
         self.console_results = {}
```

### Comparing `robotmk-0.0.51/src/robotmk/executor/scheduler.py` & `robotmk-0.0.52/src/robotmk/executor/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,16 +73,15 @@
                     # args=[v],
                     max_instances=1,
                 )
                 self.suitecfg_hashes[suiteuname] = hash
 
     def run(self):
         """Start the scheduler and update the jobs every 5 seconds"""
-        # self.scheduler.add_listener(log)
 
         self.schedule_jobs()
         # self.scheduler.add_listener(self.log)
         self.scheduler.start()
         while True:
             # update the jobs every 5 seconds
             time.sleep(5)
-            print("Running tasks: " + str(self.scheduler.print_jobs()))
+            # print("Running tasks: " + str(self.scheduler.print_jobs()))
```

### Comparing `robotmk-0.0.51/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.52/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/logger.py` & `robotmk-0.0.52/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/src/robotmk/main.py` & `robotmk-0.0.52/src/robotmk/main.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/tests/config/robotmk.yml` & `robotmk-0.0.52/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/tests/config/test_config.py` & `robotmk-0.0.52/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/tests/context/local/test_local_cli.py` & `robotmk-0.0.52/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.52/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/tests/context/suite/robotmk.yml` & `robotmk-0.0.52/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.52/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/tests/context/test_cli.py` & `robotmk-0.0.52/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/tests/yml/robotmk.yml` & `robotmk-0.0.52/tests/yml/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.51/PKG-INFO` & `robotmk-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotmk
-Version: 0.0.51
+Version: 0.0.52
 Summary: Robot Framework test execution and result parsing for Check_MK
 Keywords: robotmk,checkmk,robotframework,automation,monitoring
 Author-email: Simon Meggle <simon.meggle@elabit.de>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: click
 Requires-Dist: psutil
```

