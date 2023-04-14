# Comparing `tmp/robotmk-0.0.53.tar.gz` & `tmp/robotmk-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.53.tar", last modified: Fri Apr 14 12:23:15 2023, max compression
+gzip compressed data, was "robotmk-0.0.54.tar", last modified: Fri Apr 14 12:44:34 2023, max compression
```

## Comparing `robotmk-0.0.53.tar` & `robotmk-0.0.54.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      110 2023-04-14 12:23:10.373344 robotmk-0.0.53/.bumpversion.cfg
--rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.53/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.53/README.md
--rw-r--r--   0        0        0      755 2023-04-14 12:23:02.253430 robotmk-0.0.53/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.53/src/_confitree/__init__.py
--rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.53/src/_confitree/confitree.py
--rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.53/src/_confitree/robotmk.yml
--rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.53/src/_robotmk/__init__.py
--rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.53/src/_robotmk/__main__.py
--rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.53/src/_robotmk/cli.py
--rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/agent/__init__.py
--rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/agent/agent.py
--rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/agent/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/output/__init__.py
--rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/output/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/robot/__init__.py
--rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/robot/cli.py
--rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/robotmk.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/specialagent/__init__.py
--rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.53/src/_robotmk/modes/specialagent/cli.py
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.53/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.53/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-14 12:23:10.373344 robotmk-0.0.53/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.53/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.53/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.53/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    17797 2023-04-14 11:06:00.625074 robotmk-0.0.53/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.53/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.53/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.53/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0      681 2023-04-13 13:22:33.639789 robotmk-0.0.53/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.53/src/robotmk/context/local/__init__.py
--rw-r--r--   0        0        0     1491 2023-04-13 11:46:06.562610 robotmk-0.0.53/src/robotmk/context/local/cli.py
--rw-r--r--   0        0        0     2052 2023-04-13 11:47:44.173586 robotmk-0.0.53/src/robotmk/context/local/local.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.53/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.53/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.53/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.53/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.53/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.53/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.53/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3825 2023-04-13 11:46:27.306392 robotmk-0.0.53/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.53/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     6662 2023-04-14 11:19:23.461781 robotmk-0.0.53/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     4506 2023-04-14 10:30:06.489439 robotmk-0.0.53/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.53/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     4732 2023-04-14 11:14:59.168198 robotmk-0.0.53/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.53/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.53/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5623 2023-04-14 11:35:03.948826 robotmk-0.0.53/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6474 2023-04-14 11:50:43.784189 robotmk-0.0.53/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4818 2023-04-14 11:43:33.303934 robotmk-0.0.53/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     2793 2023-04-14 11:13:48.468830 robotmk-0.0.53/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.53/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.53/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.53/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.53/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.53/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.53/src/robotmk/logger.py
--rw-r--r--   0        0        0     3643 2023-04-14 10:22:44.709931 robotmk-0.0.53/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.53/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.53/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.53/tests/config/robotmk.yml
--rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.53/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.53/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.53/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.53/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.53/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.53/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.53/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.53/tests/context/test_cli.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.53/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.53/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-14 12:44:31.988345 robotmk-0.0.54/.bumpversion.cfg
+-rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.54/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.54/README.md
+-rw-r--r--   0        0        0      755 2023-04-14 12:23:02.253430 robotmk-0.0.54/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.54/src/_confitree/__init__.py
+-rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.54/src/_confitree/confitree.py
+-rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.54/src/_confitree/robotmk.yml
+-rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.54/src/_robotmk/__init__.py
+-rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.54/src/_robotmk/__main__.py
+-rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.54/src/_robotmk/cli.py
+-rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/agent/__init__.py
+-rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/agent/agent.py
+-rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/agent/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/output/__init__.py
+-rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/output/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/robot/__init__.py
+-rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/robot/cli.py
+-rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/robotmk.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/specialagent/__init__.py
+-rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/specialagent/cli.py
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.54/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.54/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-14 12:44:31.988345 robotmk-0.0.54/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.54/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.54/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.54/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    17973 2023-04-14 12:38:42.931817 robotmk-0.0.54/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.54/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.54/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.54/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0      681 2023-04-13 13:22:33.639789 robotmk-0.0.54/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.54/src/robotmk/context/local/__init__.py
+-rw-r--r--   0        0        0     1491 2023-04-13 11:46:06.562610 robotmk-0.0.54/src/robotmk/context/local/cli.py
+-rw-r--r--   0        0        0     2052 2023-04-13 11:47:44.173586 robotmk-0.0.54/src/robotmk/context/local/local.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.54/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.54/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.54/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.54/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.54/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.54/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.54/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3825 2023-04-13 11:46:27.306392 robotmk-0.0.54/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.54/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     6793 2023-04-14 12:43:34.356917 robotmk-0.0.54/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     4506 2023-04-14 10:30:06.489439 robotmk-0.0.54/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.54/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     4732 2023-04-14 11:14:59.168198 robotmk-0.0.54/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.54/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5635 2023-04-14 12:31:44.104026 robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6474 2023-04-14 11:50:43.784189 robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4818 2023-04-14 11:43:33.303934 robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     2793 2023-04-14 11:13:48.468830 robotmk-0.0.54/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.54/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.54/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.54/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.54/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.54/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.54/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3643 2023-04-14 10:22:44.709931 robotmk-0.0.54/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.54/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.54/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.54/tests/config/robotmk.yml
+-rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.54/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.54/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.54/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.54/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.54/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.54/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.54/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.54/tests/context/test_cli.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.54/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.54/PKG-INFO
```

### Comparing `robotmk-0.0.53/pyproject.toml` & `robotmk-0.0.54/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/_confitree/confitree.py` & `robotmk-0.0.54/src/_confitree/confitree.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/_confitree/robotmk.yml` & `robotmk-0.0.54/src/_confitree/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/_robotmk/__init__.py` & `robotmk-0.0.54/src/_robotmk/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/_robotmk/__main__.py` & `robotmk-0.0.54/src/_robotmk/__main__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/_robotmk/cli.py` & `robotmk-0.0.54/src/_robotmk/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/_robotmk/modes/__init__.py` & `robotmk-0.0.54/src/_robotmk/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/_robotmk/modes/agent/agent.py` & `robotmk-0.0.54/src/_robotmk/modes/agent/agent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/_robotmk/modes/agent/cli.py` & `robotmk-0.0.54/src/_robotmk/modes/agent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/categories.json` & `robotmk-0.0.54/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/click_tutorial.py` & `robotmk-0.0.54/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/cli/cli.py` & `robotmk-0.0.54/src/robotmk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.54/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/config/config.py` & `robotmk-0.0.54/src/robotmk/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         """Translate a key name to a list of keys and respect shorthand 'suitecfg'."""
         keys = name.split(".")
         if keys[0] == "suitecfg":
             suitename = self.configdict["common"]["suiteuname"]
             keys[:1] = ["suites", suitename]
         return keys
 
-    def get(self, name: str, default=None) -> str:
+    def get(self, name: str, default=None, asdict=False) -> str:
         """Get a value from the object with dot notation.
 
         Shorthands:
         - 'suitecfg' can be used for 'suites.<suiteuname>'.
         - 'basic_cfg' can be used for the basic config dict.
 
         Examples:
@@ -98,21 +98,25 @@
             m = self.configdict
         # prev = self.configdict
         try:
             for key in keys:
                 # prev = m
                 # prev_k = key
                 m = m.get(key, {})
-            if type(m) is dict:
-                if m:
-                    return Config(initdict=m)
+            if m:  # non-empty value
+                if type(m) is dict:
+                    if asdict:  # TODO: usefule somewhere else??
+                        return m
+                    else:
+                        return Config(initdict=m)
                 else:
-                    return default
-            else:
-                return m
+                    return m
+            else:  # empty dict
+                return default
+
         except:
             return default
 
     def set(self, name: str, value: any) -> None:
         """Set a value in the object with dot notation.
 
         Shorthand 'suitecfg' can be used for 'suites.<suiteuname>'.
```

### Comparing `robotmk-0.0.53/src/robotmk/config/yml.py` & `robotmk-0.0.54/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/abstract.py` & `robotmk-0.0.54/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/context.py` & `robotmk-0.0.54/src/robotmk/context/context.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/local/cli.py` & `robotmk-0.0.54/src/robotmk/context/local/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/local/local.py` & `robotmk-0.0.54/src/robotmk/context/local/local.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.54/src/robotmk/context/specialagent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.54/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/suite/cli.py` & `robotmk-0.0.54/src/robotmk/context/suite/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.54/src/robotmk/context/suite/strategies/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
         result_dict = {
             "args": result.args,
             "returncode": result.returncode,
             "stdout": stdout_str,
             "stderr": stderr_str,
         }
         # TODO: log console output? Save it anyway because a a fatal RF error must be tracable.
+        # RCC does not re.execute...
+        if getattr(self.target, "attempt", None) is None:
+            self.target.attempt = 1
         self.target.console_results[self.target.attempt] = result_dict
         return result.returncode
 
     def cleanup(self, *args, **kwargs) -> int:
         # nothing to do
         return 0
```

### Comparing `robotmk-0.0.53/src/robotmk/context/suite/suite.py` & `robotmk-0.0.54/src/robotmk/context/suite/suite.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/suite/target/rcc.py` & `robotmk-0.0.54/src/robotmk/context/suite/target/rcc.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,10 +147,10 @@
 
         The next attempt needs the XML file of the last attempt as input.
         From there it will read failed tests and re-execute them only."""
         # Chance for next try. Attempt gets increased, output files get bumped
         failed_xml = Path(self.target.logdir).joinpath(self.target.output_xml)
         self.target.robot_params.update({"rerunfailed": str(failed_xml)})
         rerun_selection = self.target.config.get(
-            "suitecfg.retry_failed.rerun_selection", {}
-        ).asdict()
+            "suitecfg.retry_failed.rerun_selection", asdict=True, default={}
+        )
         self.target.robot_params.update(rerun_selection)
```

### Comparing `robotmk-0.0.53/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.54/src/robotmk/context/suite/target/target.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/executor/scheduler.py` & `robotmk-0.0.54/src/robotmk/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.54/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/logger.py` & `robotmk-0.0.54/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/src/robotmk/main.py` & `robotmk-0.0.54/src/robotmk/main.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/tests/config/robotmk.yml` & `robotmk-0.0.54/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/tests/config/test_config.py` & `robotmk-0.0.54/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/tests/context/local/test_local_cli.py` & `robotmk-0.0.54/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.54/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/tests/context/suite/robotmk.yml` & `robotmk-0.0.54/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.54/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/tests/context/test_cli.py` & `robotmk-0.0.54/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/tests/yml/robotmk.yml` & `robotmk-0.0.54/tests/yml/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.53/PKG-INFO` & `robotmk-0.0.54/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotmk
-Version: 0.0.53
+Version: 0.0.54
 Summary: Robot Framework test execution and result parsing for Check_MK
 Keywords: robotmk,checkmk,robotframework,automation,monitoring
 Author-email: Simon Meggle <simon.meggle@elabit.de>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: click
 Requires-Dist: psutil
```

