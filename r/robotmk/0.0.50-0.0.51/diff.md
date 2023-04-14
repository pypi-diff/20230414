# Comparing `tmp/robotmk-0.0.50.tar.gz` & `tmp/robotmk-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.50.tar", last modified: Thu Apr 13 05:37:59 2023, max compression
+gzip compressed data, was "robotmk-0.0.51.tar", last modified: Fri Apr 14 10:36:47 2023, max compression
```

## Comparing `robotmk-0.0.50.tar` & `robotmk-0.0.51.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      110 2023-04-13 05:37:52.711274 robotmk-0.0.50/.bumpversion.cfg
--rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.50/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.50/README.md
--rw-r--r--   0        0        0      739 2023-04-12 16:12:36.358474 robotmk-0.0.50/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.50/src/_confitree/__init__.py
--rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.50/src/_confitree/confitree.py
--rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.50/src/_confitree/robotmk.yml
--rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.50/src/_robotmk/__init__.py
--rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.50/src/_robotmk/__main__.py
--rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.50/src/_robotmk/cli.py
--rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/agent/__init__.py
--rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/agent/agent.py
--rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/agent/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/output/__init__.py
--rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/output/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/robot/__init__.py
--rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/robot/cli.py
--rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/robotmk.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/specialagent/__init__.py
--rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.50/src/_robotmk/modes/specialagent/cli.py
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.50/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.50/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-13 05:37:52.711274 robotmk-0.0.50/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.50/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.50/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.50/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    15053 2023-04-13 05:21:28.444796 robotmk-0.0.50/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.50/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.50/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2293 2023-03-30 15:57:46.648634 robotmk-0.0.50/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0      644 2023-03-29 10:27:39.457231 robotmk-0.0.50/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.50/src/robotmk/context/local/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-04 10:17:17.443557 robotmk-0.0.50/src/robotmk/context/local/cli.py
--rw-r--r--   0        0        0     2091 2023-03-29 11:50:24.791476 robotmk-0.0.50/src/robotmk/context/local/local.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.50/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.50/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.50/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.50/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.50/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.50/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.50/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3728 2023-04-04 10:54:27.529704 robotmk-0.0.50/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.50/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     6576 2023-04-13 05:28:33.289623 robotmk-0.0.50/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     4293 2023-04-04 11:45:02.256091 robotmk-0.0.50/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.50/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     4608 2023-04-13 05:35:37.852792 robotmk-0.0.50/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.50/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5559 2023-04-09 16:52:38.817097 robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6448 2023-04-09 16:54:03.952360 robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4662 2023-04-09 17:05:22.342438 robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     2768 2023-04-13 05:33:55.966022 robotmk-0.0.50/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.50/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.50/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     2013 2023-03-20 12:52:41.400361 robotmk-0.0.50/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.50/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.50/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.50/src/robotmk/logger.py
--rw-r--r--   0        0        0     3463 2023-04-03 08:53:57.612055 robotmk-0.0.50/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.50/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.50/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.50/tests/config/robotmk.yml
--rw-r--r--   0        0        0     9958 2023-04-12 15:08:57.203733 robotmk-0.0.50/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.50/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.50/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.50/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.50/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.50/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.50/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.50/tests/context/test_cli.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.50/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 robotmk-0.0.50/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-14 10:36:34.281720 robotmk-0.0.51/.bumpversion.cfg
+-rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.51/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.51/README.md
+-rw-r--r--   0        0        0      739 2023-04-12 16:12:36.358474 robotmk-0.0.51/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.51/src/_confitree/__init__.py
+-rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.51/src/_confitree/confitree.py
+-rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.51/src/_confitree/robotmk.yml
+-rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.51/src/_robotmk/__init__.py
+-rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.51/src/_robotmk/__main__.py
+-rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.51/src/_robotmk/cli.py
+-rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/agent/__init__.py
+-rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/agent/agent.py
+-rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/agent/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/output/__init__.py
+-rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/output/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/robot/__init__.py
+-rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/robot/cli.py
+-rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/robotmk.py
+-rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/specialagent/__init__.py
+-rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.51/src/_robotmk/modes/specialagent/cli.py
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.51/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.51/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-14 10:36:34.281720 robotmk-0.0.51/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.51/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.51/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.51/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    17518 2023-04-14 10:20:54.767048 robotmk-0.0.51/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.51/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.51/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.51/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0      681 2023-04-13 13:22:33.639789 robotmk-0.0.51/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.51/src/robotmk/context/local/__init__.py
+-rw-r--r--   0        0        0     1491 2023-04-13 11:46:06.562610 robotmk-0.0.51/src/robotmk/context/local/cli.py
+-rw-r--r--   0        0        0     2052 2023-04-13 11:47:44.173586 robotmk-0.0.51/src/robotmk/context/local/local.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.51/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.51/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.51/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.51/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.51/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.51/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.51/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3825 2023-04-13 11:46:27.306392 robotmk-0.0.51/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.51/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     6576 2023-04-13 05:28:33.289623 robotmk-0.0.51/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     4506 2023-04-14 10:30:06.489439 robotmk-0.0.51/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.51/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     4728 2023-04-14 08:45:52.961802 robotmk-0.0.51/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.51/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5559 2023-04-09 16:52:38.817097 robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6448 2023-04-09 16:54:03.952360 robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4662 2023-04-09 17:05:22.342438 robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     2762 2023-04-13 05:44:33.655252 robotmk-0.0.51/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.51/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.51/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     3404 2023-04-14 10:11:36.108721 robotmk-0.0.51/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.51/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.51/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.51/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3643 2023-04-14 10:22:44.709931 robotmk-0.0.51/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.51/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.51/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.51/tests/config/robotmk.yml
+-rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.51/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.51/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.51/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.51/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.51/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.51/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.51/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.51/tests/context/test_cli.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.51/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 robotmk-0.0.51/PKG-INFO
```

### Comparing `robotmk-0.0.50/pyproject.toml` & `robotmk-0.0.51/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/_confitree/confitree.py` & `robotmk-0.0.51/src/_confitree/confitree.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/_confitree/robotmk.yml` & `robotmk-0.0.51/src/_confitree/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/_robotmk/__init__.py` & `robotmk-0.0.51/src/_robotmk/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/_robotmk/__main__.py` & `robotmk-0.0.51/src/_robotmk/__main__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/_robotmk/cli.py` & `robotmk-0.0.51/src/_robotmk/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/_robotmk/modes/__init__.py` & `robotmk-0.0.51/src/_robotmk/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/_robotmk/modes/agent/agent.py` & `robotmk-0.0.51/src/_robotmk/modes/agent/agent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/_robotmk/modes/agent/cli.py` & `robotmk-0.0.51/src/_robotmk/modes/agent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/categories.json` & `robotmk-0.0.51/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/click_tutorial.py` & `robotmk-0.0.51/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/cli/cli.py` & `robotmk-0.0.51/src/robotmk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.51/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/config/config.py` & `robotmk-0.0.51/src/robotmk/config/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 import os
 import re
 import yaml
 from mergedeep import merge, Strategy
 from typing import Union
 from collections import defaultdict
+import json
+import hashlib
 
 # from collections import namedtuple
 from pathlib import Path
 from .yml import RobotmkConfigSchema
 
 # TODO: add config validation
 # ["%s:%s" % (v, os.environ[v]) for v in os.environ if v.startswith("ROBO")]
@@ -47,26 +49,31 @@
 # yaml.add_constructor(
 #     "tag:yaml.org,2002:python/object/apply:collections.defaultdict",
 #     default_dict_constructor,
 # )
 
 
 class Config:
-    def __init__(self, envvar_prefix: str = "ROBOTMK", initdict: dict = None):
+    def __init__(self, envvar_prefix: str = "ROBOTMK", initdict: dict = {}):
         self.envvar_prefix = envvar_prefix
         if initdict:
             self.default_cfg = initdict
         else:
             self.default_cfg = {}
         self.yml_config = {}
         self.env_config = {}
         # this is a dict of all config values that were added by the user.
         # they are applied last and can overwrite any other config values.
         self.added_config = {}
 
+    def __iter__(self):
+        # TODO: iterator added afterwards - where is it useful?
+        for key in self.configdict:
+            yield key, self.get(key)
+
     def __translate_keys(self, name: str) -> list:
         """Translate a key name to a list of keys and respect shorthand 'suitecfg'."""
         keys = name.split(".")
         if keys[0] == "suitecfg":
             suitename = self.configdict["common"]["suiteuname"]
             keys[:1] = ["suites", suitename]
         return keys
@@ -131,34 +138,75 @@
 
     #     cur_dict[keys[-1]] = value
 
     def asdict(self):
         """Returns the config as a dict."""
         return self.configdict
 
+    def suite_cfghash(self, suiteuname) -> str:
+        """Returns a hash of the common + suite config (passed as arg) to identify a possible change.
+
+        Used in the scheduler and sequencer."""
+        common_cfg = {"common": self.get("common").asdict()}
+        suite_cfg = {"suites": self.get("suites.%s" % suiteuname).asdict()}
+        cfg = merge({}, common_cfg, suite_cfg)
+        return hashlib.sha256(json.dumps(cfg).encode("utf-8")).hexdigest()
+
     @property
     def configdict(self):
-        """This property merges the three config sources in the right order."""
+        """This property represents all config dicts merged.
+
+        It consist of the following dicts:
+        - basic_cfg = predefiend from start
+            - default_cfg
+            - yml_config
+            - env_config
+        - added_config = added at runtime
+
+        """
 
+        # https://mergedeep.readthedocs.io/en/latest/#merge-strategies
+        # Collection values are merged additively. Others get replaced.
+        # The last/rightmost dictionary has the highest priority.
         return merge(
-            self.default_cfg, self.yml_config, self.env_config, self.added_config
+            {},
+            self.basic_cfg,  # Config set by OS default values, YML file, environment variables and/or variables file
+            self.added_config,  # Config changed/added at runtime (config.set() method)
+            strategy=Strategy.ADDITIVE,
+        )
+
+    @configdict.setter
+    def configdict(self, cfg: dict):
+        """This setter allows to write a whole new config dict. It is used e.g. when the scheduler creates
+        job object for each suite."""
+        self.default_cfg = cfg
+
+    @property
+    def basic_cfg(self):
+        """Returns the basic config dict."""
+        return merge(
+            {},
+            self.default_cfg,  # Config set by OS default values
+            self.yml_config,  # Config loaded from YML file
+            self.env_config,  # Config loaded from environment variables and/or variables file
+            strategy=Strategy.ADDITIVE,
         )
 
     # 1. Defaults (common/OS specific)
     def set_defaults(self, os_defaults: dict = None) -> None:
         """Sets the defaults for the current OS."""
         self.default_cfg["common"] = {}
         if os_defaults:
             self.default_cfg["common"].update(os_defaults["common"])
         if os.name in os_defaults:
             self.default_cfg["common"].update(os_defaults[os.name])
 
     # 2. YML
     def read_yml_cfg(self, path=None, must_exist=True):
-        """Reads a YML config"""
+        """Reads a YML config, either default or custom."""
         if path is None:
             # Linux default: /etc/check_mk/robotmk.yml
             # Windows default: C:\Program Data\check_mk\agent\config\robotmk.yml
             ymlfile = (
                 Path(self.configdict["common"]["cfgdir"])
                 / self.configdict["common"]["robotmk_yml"]
             )
@@ -190,15 +238,15 @@
         # a dict with still flat var names
         vars = merge(filevars, envvars)
         # convert flat vars to nested dicts
         vdict = defaultdict(dict)
         for k, v in vars.items():
             # iterate over each variable and convert it to a nested data structure
             vdict = self._var2cfg(k, v, vdict)
-        self.env_config = merge(self.env_config, vdict)
+        self.env_config = merge({}, self.env_config, vdict, strategy=Strategy.ADDITIVE)
 
     def _envvar2dict(self) -> dict:
         """Returns all environment variables starting with the ROBOTMK prefix.
 
         Example:
         {"ROBOTMK_foo_bar": "baz",
          "ROBOTMK_foo_baz": "bar"}
@@ -237,146 +285,167 @@
     def validate(self, schema: RobotmkConfigSchema):
         """Validates the whole config according to the given context schema."""
 
         schema = RobotmkConfigSchema(self.configdict)
         if not schema.validate():
             raise ValueError(f"Config is invalid: {schema.error}")
 
+    @staticmethod
+    def partition_at_digit(s):
+        """Divides the string at the first digit and returns a list of the
+        left part, the digit and the right part.
+
+        The digit indicates the index in the list."""
+        m = re.search("_\d+", s)
+        if m:
+            return s[: m.start()], int(s[m.start() + 1 : m.end()]), s[m.end() + 1 :]
+        else:
+            return [s, None, None]
+
+    @staticmethod
+    def split_varstring(s):
+        """Helper function to reconstruct the nested key path of a dict from
+        a varname. The keys are separated by "_", a double underscore protects the string from splitting.
+        """
+        keys = []
+        starti = 0
+        i = 0
+        while i < len(s):
+            poschar = s[i]
+            if poschar == "_" or i == len(s) - 1:
+                if len(s) > i + 1 and s[i + 1] == "_":
+                    # not at and and double underscore in front of us!
+                    # skip next underscore and continue until next SINGLE underscore
+                    i += 2
+                    continue
+                else:
+                    # Single underscore in front or last piece; add current piece to list
+                    # (replace __ by _) and start a new one
+                    if len(s) > i + 1:
+                        # last piece
+                        last_single_usc_index = i
+                    else:
+                        # not last piece
+                        last_single_usc_index = i + 1
+                    piece = s[starti:last_single_usc_index].replace("__", "_")
+                    keys.append(piece)
+                    starti = i + 1
+            else:
+                # Add the current character to the current piece
+                pass
+            i += 1
+        return keys
+
+    def uscore_str2dict(string, value, vdict=None):
+        """Converts a variable string to a nested dict.
+
+        Digit inside the string indicate the index in the list."""
+        # curdict is a moving reference to the current dict
+        cur_dict = vdict
+
+        (s_left, s_list_index, s_right) = Config.partition_at_digit(string)
+        # list of keys "left" of the list index (if any)
+        left_keys = Config.split_varstring(s_left)
+        for ki, key in enumerate(left_keys):
+            # descend now key by key until we reach the leaf key. cur_dict gets always
+            # moved forward to have a reference on the key we want to change.
+            if ki < len(left_keys) - 1:
+                if not key in cur_dict:
+                    cur_dict[key] = defaultdict(dict)
+                cur_dict = cur_dict[key]
+            else:
+                # we have reached the leaf key of left side, just before the index.
+                if not s_list_index is None:  # list index
+                    if (
+                        not key in cur_dict
+                    ):  # key not present, create all (empty) list items
+                        cur_dict[key] = [defaultdict(dict)] * (s_list_index + 1)
+                    else:
+                        if (
+                            len(cur_dict[key]) < s_list_index + 1
+                        ):  # key present, but not enough list items
+                            cur_dict[key] = cur_dict[key] + [defaultdict(dict)] * (
+                                s_list_index + 1 - len(cur_dict[key])
+                            )
+                    if not s_right:  # list entry without subkeys
+                        cur_dict[key][s_list_index] = value
+                    else:
+                        # dict inside the list!
+                        # call the function recursively to descend into the dict. We also
+                        # pass the current list item as cur_dict, so that the function can
+                        # modify it.
+                        subdict = Config.uscore_str2dict(
+                            s_right, value, cur_dict[key][s_list_index]
+                        )
+                        # assign the modified subdict to the list item
+                        cur_dict[key][s_list_index] = subdict
+                else:
+                    # simple value assignment. Make sure that values of numbers are not stored as strings.
+                    if isinstance(value, str) and value.isdigit():
+                        value = int(value)
+                    cur_dict[key] = value
+
+        return vdict
+
     def _var2cfg(self, o_varname, value, vdict) -> dict:
         """Helper function to convert a variable to a dict/list/value entry and assigns the value.
 
         Example:
             - ROBOTMK_foo_bar_0_baz = "bar"
                 will be converted to:
                 {"foo": {"bar": [{"baz": "bar"}]}}
             - ROBOTMK_foo__bar_0_baz = "bar
                 will be converted to:
                 {"foo_bar": [{"baz": "bar"}]}
         """
 
-        def _partition_at_digit(s):
-            """Divides the string at the first digit and returns a list of the
-            left part, the digit and the right part.
-
-            The digit indicates the index in the list."""
-            m = re.search("_\d+", s)
-            if m:
-                return s[: m.start()], int(s[m.start() + 1 : m.end()]), s[m.end() + 1 :]
-            else:
-                return [s, None, None]
-
-        def _split_varstring(s):
-            """Helper function to reconstruct the nested key path of a dict from
-            a varname. The keys are separated by "_", a double underscore protects the string from splitting.
-            """
-            keys = []
-            starti = 0
-            i = 0
-            while i < len(s):
-                poschar = s[i]
-                if poschar == "_" or i == len(s) - 1:
-                    if len(s) > i + 1 and s[i + 1] == "_":
-                        # not at and and double underscore in front of us!
-                        # skip next underscore and continue until next SINGLE underscore
-                        i += 2
-                        continue
-                    else:
-                        # Single underscore in front or last piece; add current piece to list
-                        # (replace __ by _) and start a new one
-                        if len(s) > i + 1:
-                            # last piece
-                            last_single_usc_index = i
-                        else:
-                            # not last piece
-                            last_single_usc_index = i + 1
-                        piece = s[starti:last_single_usc_index].replace("__", "_")
-                        keys.append(piece)
-                        starti = i + 1
-                else:
-                    # Add the current character to the current piece
-                    pass
-                i += 1
-            return keys
-
-        def _str2dict(string, value, vdict=None):
-            # curdict is a moving reference to the current dict
-            cur_dict = vdict
-
-            (s_left, s_list_index, s_right) = _partition_at_digit(string)
-            # list of keys "left" of the list index (if any)
-            left_keys = _split_varstring(s_left)
-            for ki, key in enumerate(left_keys):
-                # descend now key by key until we reach the leaf key. cur_dict gets always
-                # moved forward to have a reference on the key we want to change.
-                if ki < len(left_keys) - 1:
-                    if not key in cur_dict:
-                        cur_dict[key] = defaultdict(dict)
-                    cur_dict = cur_dict[key]
-                else:
-                    # we have reached the leaf key of left side, just before the index.
-                    if not s_list_index is None:  # list index
-                        if (
-                            not key in cur_dict
-                        ):  # key not present, create all (empty) list items
-                            cur_dict[key] = [defaultdict(dict)] * (s_list_index + 1)
-                        else:
-                            if (
-                                len(cur_dict[key]) < s_list_index + 1
-                            ):  # key present, but not enough list items
-                                cur_dict[key] = cur_dict[key] + [defaultdict(dict)] * (
-                                    s_list_index + 1 - len(cur_dict[key])
-                                )
-                        if not s_right:  # list entry without subkeys
-                            cur_dict[key][s_list_index] = value
-                        else:
-                            # dict inside the list!
-                            # call the function recursively to descend into the dict. We also
-                            # pass the current list item as cur_dict, so that the function can
-                            # modify it.
-                            subdict = _str2dict(
-                                s_right, value, cur_dict[key][s_list_index]
-                            )
-                            # assign the modified subdict to the list item
-                            cur_dict[key][s_list_index] = subdict
-                    else:
-                        # simple value assignment. Make sure that values of numbers are not stored as strings.
-                        if isinstance(value, str) and value.isdigit():
-                            value = int(value)
-                        cur_dict[key] = value
-
-            return vdict
-
         # Remove the ROBOTMK_ prefix
         varname = o_varname.replace(self.envvar_prefix + "_", "")
-        _str2dict(varname, value, vdict)
+        Config.uscore_str2dict(varname, value, vdict)
         return vdict
 
-    def to_environment(self, d=None, prefix="", environ=None):
-        """Converts a given dict/value or self.configdict to environment variables.
+    def dotcfg_to_env(self, dotstrings: dict, environ: dict):
+        """Converts a dict of dotconfigs to an environment variable and assign it to environ.
+
+        This does not affect the current config at all; it just uses a temporary config object.
+        Example:
+            {"common.logdir": "foo",
+             "common.loglevel": "debug"}
+        """
+
+        tmp_cfg = Config()
+        # As we are using a temp config object, the suiteuname must be set manually to access the
+        # correct section with the shorthand "suitecfg"
+        tmp_cfg.set("common.suiteuname", self.get("common.suiteuname"))
+        for k, v in dotstrings.items():
+            tmp_cfg.set(k, v)
+        self.cfg_to_environment(tmp_cfg.configdict, environ=environ)
+
+    def cfg_to_environment(self, d, prefix="", environ=None):
+        """Converts a given dict to environment variables.
 
         If environ is given, the environment variables are added to the given dict.
         Otherwise the environment variables are added to the current environment.
 
         The conversion rules are:
         - there is no case conversion
         - underscores within key names are replaced by double underscores
         - the prefix is added to the environment variable name
         - dicts are converted to nested environment variables
         - lists get a number appended to their key name"""
-        if d is None:
-            d = self.configdict
+
         if isinstance(d, dict):  # DICT conversion
             for key, value in d.items():
                 safe_key = key.replace("_", "__")
                 new_prefix = f"{prefix}_{safe_key}"
-                self.to_environment(value, prefix=new_prefix, environ=environ)
+                self.cfg_to_environment(value, prefix=new_prefix, environ=environ)
         elif isinstance(d, list):  # LIST conversion
             for i, item in enumerate(d):
                 new_prefix = f"{prefix}_{i}"
-                self.to_environment(item, prefix=new_prefix, environ=environ)
+                self.cfg_to_environment(item, prefix=new_prefix, environ=environ)
         else:  # VALUE conversion
             varname = f"{self.envvar_prefix}{prefix}"
             print(f"{varname} = {d}")
             if environ is None:
                 os.environ[varname] = str(d)
             else:
                 environ[varname] = str(d)
```

### Comparing `robotmk-0.0.50/src/robotmk/config/yml.py` & `robotmk-0.0.51/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/context/abstract.py` & `robotmk-0.0.51/src/robotmk/context/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     encapsulate the different contexts in which robotmk can be run (local, specialagent, suite).
     """
 
     def __init__(self):
         # self._config_factory = Config()
         self._logger = None
         self.init_logger()
+        self.config = Config()
 
     @property
     def logger(self):
         # self.__init_logger()
         return self._logger
 
     def init_logger(self):
@@ -29,15 +30,15 @@
             self.debug = self._logger.debug
             self.info = self._logger.info
             self.warning = self._logger.warning
             self.error = self._logger.error
             self.critical = self._logger.critical
 
     @abstractmethod
-    def load_config(self, defaults, ymlfile: str, varfile: str) -> None:
+    def load_config(self, defaults, **kwargs) -> None:
         """Depening on the context strategy, the config object loads cfg from different sources."""
         raise NotImplementedError("Subclass must implement abstract method")
 
     @abstractmethod
     def refresh_config(self):
         """Load the config again, e.g. after a change in the config file."""
         raise NotImplementedError("Subclass must implement abstract method")
```

### Comparing `robotmk-0.0.50/src/robotmk/context/context.py` & `robotmk-0.0.51/src/robotmk/context/context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from .local.local import LocalContext
-from .specialagent.specialagent import SpecialAgentContext
-from .suite.suite import SuiteContext
-
-
 class ContextFactory:
     def __init__(self, contextname: str, log_level: str) -> None:
         self.contextname = contextname
         self._log_level = log_level
 
     def get_context(self) -> None:
         if self.contextname == "local":
+            from .local.local import LocalContext
+
             return LocalContext()
         elif self.contextname == "specialagent":
+            from .specialagent.specialagent import SpecialAgentContext
+
             return SpecialAgentContext()
         elif self.contextname == "suite":
+            from .suite.suite import SuiteContext
+
             return SuiteContext()
         else:
             # TODO: catch this error
             pass
```

### Comparing `robotmk-0.0.50/src/robotmk/context/local/cli.py` & `robotmk-0.0.51/src/robotmk/context/specialagent/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-"""CLI commands for the local context. 
+"""CLI commands for the specialagent context.
 
-Executes Robotmk in local context (Windows & Linux)"""
+Executes Robotmk in specialagent context. This CLI is rather used to debug the 
+specialagent than to run it in production."""
 import sys
 import click
 from robotmk.main import Robotmk, DEFAULTS
 
 
 # use module docstring as help text
 @click.group(help=__doc__, invoke_without_command=True)
 @click.pass_context
-@click.option("--yml", "-y", help="Read config from custom YML file")
+@click.option("--vars", "-v", help="Read vars from .env file (ignores environment)")
+def specialagent(ctx, vars):
+    click.echo("Executing specialagent....")
+    ctx.obj = Robotmk("specialagent", vars=vars)
+    ctx.obj.config.set("common.context", "specialagent")
 
-# @click.option("--vars", "-v", help="Read vars from .env file (ignores environment)")
-def local(ctx, yml):
-    ctx.obj = Robotmk("local", yml=yml)
-    ctx.obj.config.set("common.context", "local")
-    if ctx.invoked_subcommand is None:
-        click.secho("No subcommand given. Use --help for help.", fg="red")
-        sys.exit(1)
+    pass
 
 
-@local.command()
+@specialagent.command()
 @click.pass_context
-def scheduler(ctx):
-    click.secho("scheduler", fg="green")
+def sequencer(ctx):
+    click.secho("sequencer", fg="green")
     ctx.obj.execute()
-    pass
 
 
-@local.command()
+@specialagent.command()
 @click.pass_context
 def output(ctx):
     click.secho("output", fg="green")
     ctx.obj.output()
     pass
 
 
-@local.command(help="Dump the config as YML to STDOUT or FILE")
+@specialagent.command(help="Dump the config as YML to STDOUT or FILE")
 # add file arg
 @click.argument("file", required=False, type=click.Path(exists=False))
 @click.pass_context
 def ymldump(ctx, file):
     click.secho(ctx.obj.config.to_yml(file), fg="bright_white")
     sys.exit(0)
```

### Comparing `robotmk-0.0.50/src/robotmk/context/local/local.py` & `robotmk-0.0.51/src/robotmk/context/local/local.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
-
 from ..abstract import AbstractContext
 
-from robotmk.config.yml import RobotmkConfigSchema
+from robotmk.config import Config, RobotmkConfigSchema
+
 from robotmk.executor.scheduler import Scheduler
 
 
 class LocalContext(AbstractContext):
     def __init__(self):
         super().__init__()
         self.ymlschema = RobotmkConfigSchema
@@ -16,24 +16,25 @@
         if not self._logger:
             self._logger = RobotmkLogger(
                 Path(self.config.common.logdir).joinpath("robotmk.log"),
                 self.config.common.log_level,
             )
         return self._logger
 
-    def load_config(self, defaults, ymlfile: str, varfile: str) -> None:
+    def load_config(self, defaults, **kwargs) -> None:
         """Load the config for local context.
 
         Local context can merge the config from
         - OS defaults
         - + YML file (default/custom = --yml)
         - + environment variables
         """
+        # self.config = Config()
         self.config.set_defaults(defaults)
-        self.config.read_yml_cfg(must_exist=True, path=ymlfile)
+        self.config.read_yml_cfg(path=kwargs["ymlfile"], must_exist=True)
         self.config.read_cfg_vars(path=None)
         # TODO: validate later so that config can be dumped
         # self.config.validate(self.ymlschema)
 
     def refresh_config(self) -> bool:
         """Re-loads the config and returns True if it changed"""
         config_copy = copy.deepcopy(self.configdict)
@@ -45,16 +46,15 @@
     def run_default(self):
         """Implements the default action for local context."""
         # TODO: how do I call the coutputter here?
         print("Local context default action = output")
         pass
 
     def execute(self, *args, **kwargs):
-        """Implements the run action for local context ()."""
-        print("Local context run action")
+        """Starts the scheduler."""
         self.executor = Scheduler(self.config)
         self.executor.run()
         pass
 
     def output(self):
         """Implements the agent output for local context."""
         print("Local context agent output")
```

### Comparing `robotmk-0.0.50/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.51/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/context/suite/cli.py` & `robotmk-0.0.51/src/robotmk/context/suite/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 """CLI commands for execution of a single suite."""
 
 import sys
 import click
 from robotmk.cli.defaultgroup import DefaultGroup
 from robotmk.main import Robotmk, DEFAULTS
 
+# TODO: Refine the defaultgroup usage
+
+#             _ _
+#            (_) |
+#   ___ _   _ _| |_ ___
+#  / __| | | | | __/ _ \
+#  \__ \ |_| | | ||  __/
+#  |___/\__,_|_|\__\___|
+
 
 # use module docstring as help text
 @click.group(
     cls=DefaultGroup, default_if_no_args=True, help=__doc__, invoke_without_command=True
 )
 @click.pass_context
 @click.option("--yml", "-y", help="Read config from custom YML file")
 @click.option("--vars", "-v", help="Read vars from .env file (ignores environment)")
 def suite(ctx, yml, vars):
     if vars and yml:
         raise click.BadParameter("Cannot use --yml and --vars at the same time")
-    # click.echo("suite")
     ctx_loglevel = ctx.parent.params.get("loglevel", DEFAULTS["common"]["log_level"])
-    ctx.obj = Robotmk(contextname="suite", log_level=ctx_loglevel, yml=yml, vars=vars)
-    ctx.obj.config.set("common.context", "suite")
+    ctx.obj = Robotmk(
+        contextname="suite", log_level=ctx_loglevel, ymlfile=yml, varfile=vars
+    )
 
 
 @suite.command(default=True)
 @click.argument("suite", required=False)
 @click.pass_context
 def run(ctx, suite):
     """Trigger the start of a Robot Framework SUITE.
 
     SUITE must be a configuration subkey of the "suites" section.
     (can also be set by env:ROBOTMK_common_suiteuname.)
     """
-    # click.secho("run suite %s" % suite, fg="green")
     if suite:
         ctx.obj.config.set("common.suiteuname", suite)
     if ctx.obj.config.get("common.suiteuname", None):
         ctx.obj.execute()
     else:
         click.secho("Suite '%s' not found in configuration" % suite, fg="red")
 
@@ -47,14 +55,15 @@
     """Print the CMK agent output of SUITE on STDOUT.
 
     SUITEID is eiher equal to the suite dir or a combination of suite dir and its unique tag as set in the configuration.
     Examples are: suite1, suite2_tagfoo, suite3_tagbaz
     (can also be set by env:ROBOTMK_common_suiteuname.)
     """
     click.secho("output of suite %s" % suite, fg="green")
+    # TODO: to be implemented
     ctx.obj.output()
     pass
 
 
 @suite.command()
 @click.argument("suite", required=True)
 @click.option(
```

### Comparing `robotmk-0.0.50/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.51/src/robotmk/context/suite/strategies/run.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/context/suite/suite.py` & `robotmk-0.0.51/src/robotmk/context/suite/suite.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from pathlib import Path
 from ..abstract import AbstractContext
 
 from robotmk.config import Config, RobotmkConfigSchema
 
 from .target import Target, RobotFrameworkTarget, RCCTarget, RemoteTarget
+import time, os
 
 
 class SuiteContext(AbstractContext):
     def __init__(self):
         super().__init__()
         self._target = None
         self._ymlschema = RobotmkConfigSchema
@@ -64,31 +65,32 @@
                 self.error("Unknown target type for suite %s!" % self.suiteuname)
         return self._target
 
     @property
     def target(self) -> Target:
         return self._target
 
-    def load_config(self, defaults, ymlfile: str, varfile: str) -> None:
+    def load_config(self, defaults, **kwargs) -> None:
         """Load the config for suite context.
 
         Suite context can merge the config from
         - OS defaults
         - + YML file (default/custom = --yml)
         - + var file (= --vars)
         - + environment variables
         """
-        self.config = Config()
-        self.config.set_defaults(defaults)
-        self.config.read_yml_cfg(path=ymlfile, must_exist=False)
-        self.config.read_cfg_vars(path=varfile)
-        # self._config_factory.set_defaults(defaults)
-        # self._config_factory.read_yml_cfg(path=ymlfile, must_exist=False)
-        # self._config_factory.read_cfg_vars(path=varfile)
-        # self.config = self._config_factory.create_config()
+        if kwargs.get("default_cfg", {}):
+            # Suite was started by scheduler, config was passed
+            self.config.configdict = kwargs["default_cfg"]
+
+        else:
+            # Suite was started by CLI, load config from individual sources
+            self.config.set_defaults(defaults)
+            self.config.read_yml_cfg(path=kwargs["ymlfile"], must_exist=False)
+            self.config.read_cfg_vars(path=kwargs["varfile"])
         # TODO: validate later so that config can be dumped
         # self.config.validate(self._ymlschema)
 
     def refresh_config(self) -> bool:
         """Re-loads the config and returns True if it changed"""
         # TODO: implement this
         pass
@@ -97,14 +99,19 @@
         """Implements the default action for suite context."""
         # TODO: execute one single suite
         print("Suite context default action = execute single suite ")
         pass
 
     def execute(self):
         """Runs a single suite, either locally or remotely (via API call)."""
+        # TODO: is it better to pass the suitename to get_target()?
+        # pid = os.getpid()
+        # print(f"Suite start (PID: {pid})")
+        # time.sleep(1)
+        # print(f"Suite end (PID: {pid})")
         self.get_target().run()
 
     def output(self):
         # TODO: make this possible in CLI
         """Implements the agent output for local context."""
         print("Local context agent output")
         self.outputter = SuiteOutput(self.config)
```

### Comparing `robotmk-0.0.50/src/robotmk/context/suite/target/rcc.py` & `robotmk-0.0.51/src/robotmk/context/suite/target/rcc.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,43 +19,46 @@
 
     @property
     def command(self):
         """The command will be used by the Run strategy (self.target.command).
 
         In RCC target, the commandline gets buuilt to execute a RCC task (=Robotmk inside of RCC)
         """
-        arglist = [
+        return [
             "rcc",
             "task",
             "run",
             "--controller",
             "robotmk",
             "--space",
             self.suiteuname,
             "-t",
             "robotmk",
             "-r",
             str(self.path.joinpath("robot.yaml")),
         ]
 
-        return arglist
-
     def prepare_environment(self) -> dict:
+        """Sets up the environment for a subsequent run.
+
+        If Robotmk calls itself in a RCC task, the inner call of Robotmk needs
+        some special settings, e.g. NOT to use RCC again, to log into the default
+        logdir, etc.
+        This function first exports the current config to the environment and
+        then adds the special settings on top.
+        """
         env = os.environ.copy()
-        # When running Robotmk inside of a RCC, it must be told not
-        # to use RCC again. (Otherwise, it would run RCC inside of RCC.)
-        self.config.set("suitecfg.run.rcc", False)
-        # The wrapping RCC process gives his uuid to the inner Robotmk process
-        self.config.set("suitecfg.uuid", self.uuid)
-        # TODO: rethink the idea to separate the logs of rcc and robotframework
-        # self.config.set(
-        #     "common.logdir",
-        #     "%s/%s" % (self.config.get("common.logdir"), "robotframework"),
-        # )
-        self.config.to_environment(environ=env)
+        added_settings = {
+            "suitecfg.run.rcc": False,
+            "suitecfg.uuid": self.uuid,
+            "common.logdir": "%s/%s"
+            % (self.config.basic_cfg["common"]["logdir"], "robotframework"),
+        }
+        self.config.cfg_to_environment(self.config.configdict, environ=env)
+        self.config.dotcfg_to_env(added_settings, environ=env)
         return env
 
     def run(self):
         # Before we blow up the whole thing, we should check if the suite is RCC compatible and allowed to run
         if self.is_disabled_by_flagfile:
             # TODO: Log skipped
             # reason = self.get_disabled_reason()
```

### Comparing `robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.51/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.51/src/robotmk/context/suite/target/target.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,17 @@
         config: dict,
         logger: RobotmkLogger,
     ):
         super().__init__(suiteuname, config, logger)
 
         # Store RCC and RF logs in separate folders
         # TODO: relly needed?
-        # self.config.set(
-        #     "common.logdir", "%s/%s" % (self.config.get("common.logdir"), str(self))
-        # )
+        self.config.set(
+            "common.logdir", "%s/%s" % (self.config.get("common.logdir"), str(self))
+        )
 
         self.path = Path(self.config.get("common.robotdir")).joinpath(
             self.config.get("suitecfg.path")
         )
         self.run_strategy = RunStrategyFactory(self).create()
         # list of subprocess' results and console output
         self.console_results = {}
```

### Comparing `robotmk-0.0.50/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.51/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/logger.py` & `robotmk-0.0.51/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/src/robotmk/main.py` & `robotmk-0.0.51/src/robotmk/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,33 +45,37 @@
         "tmpdir": "/tmp/robotmk",
     },
 }
 
 
 class Robotmk:
     """This is the main class of the robotmk package. It is used to create a
-    Robotmk instance with a specific context."""
+    Robotmk instance with a specific context.
+
+    Configuration loading (yml, var, env) depends on the context and is only
+    done when not config object is passed to the init method."""
 
     def __init__(
         self,
         log_level=None,
         contextname=None,
-        yml: str = None,
-        vars: str = None,
+        ymlfile: str = None,
+        varfile: str = None,
+        default_cfg: dict = {},
     ) -> None:
         """context is the strategy to use and in fact a set of factory methods.
         If called from the CLI without context argument, the default context
         will be read from environment variable ROBOTMK_common_context."""
 
         self.__set_context(contextname, log_level)
-        # self.load_config = self._context.load_config
-        self._context.load_config(DEFAULTS, yml, vars)
+        self._context.load_config(
+            DEFAULTS, ymlfile=ymlfile, varfile=varfile, default_cfg=default_cfg
+        )
+        self.config.set("common.context", contextname)
 
-        # TODO: needed?
-        # self.config = self._context.config
         self.run_default = self._context.run_default
         # execute and output are the two main functions of each context:
         self.execute = self._context.execute
         self.output = self._context.output
 
     @property
     def config(self):
```

### Comparing `robotmk-0.0.50/tests/config/robotmk.yml` & `robotmk-0.0.51/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/tests/config/test_config.py` & `robotmk-0.0.51/tests/config/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,55 +13,14 @@
     cfg = Config()
     cfg.set("common.suiteuname", "foosuite")
     cfg.set("suitecfg.foo.bar", "baz")
     assert cfg.configdict["suites"]["foosuite"]["foo"]["bar"] == "baz"
     assert cfg.get("suitecfg.foo.bar") == "baz"
 
 
-def test_cfg2env():
-    """Tests the conversion of a config dictionary to environment variables."""
-    cfg = Config()
-    cfg.set("common.log_level", "INFO")
-    cfg.set("common.suiteuname", "foo_suite")
-    cfg.set("suitecfg.my_value", "qux")
-    cfg.set("suitecfg.my_list", ["one", "two", "three"])
-    cfg.set("suitecfg.my_dict", {"foo": "one", "bar": "two", "baz": "three"})
-    cfg.set(
-        "suitecfg.my_list_of_dict",
-        [
-            {"foo": "one", "bar": "two", "baz": "three"},
-            {"foo": "one", "bar": "two", "baz": "three"},
-            {"foo": "one", "bar": "two", "baz": "three"},
-        ],
-    )
-    cfg.to_environment()
-    # simple values
-    assert os.environ["ROBOTMK_common_log__level"] == "INFO"
-    assert os.environ["ROBOTMK_common_suiteuname"] == "foo_suite"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__value"] == "qux"
-    # lists
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list_0"] == "one"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list_1"] == "two"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list_2"] == "three"
-    # dicts
-    assert os.environ["ROBOTMK_suites_foo__suite_my__dict_foo"] == "one"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__dict_bar"] == "two"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__dict_baz"] == "three"
-    # list of dicts
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_0_foo"] == "one"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_0_bar"] == "two"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_0_baz"] == "three"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_1_foo"] == "one"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_1_bar"] == "two"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_1_baz"] == "three"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_2_foo"] == "one"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_2_bar"] == "two"
-    assert os.environ["ROBOTMK_suites_foo__suite_my__list__of__dict_2_baz"] == "three"
-
-
 def test_env2cfg_values():
     """Tests the conversion of environment variables to a config dictionary."""
     # simple values
     os.environ["ROBOTMK_suites_foo1"] = "qux"
     os.environ["ROBOTMK_common_log__level"] = "INFO"
     os.environ["ROBOTMK_common_suiteuname"] = "foo_suite"
     os.environ["ROBOTMK_suites_foo__suite_my__value"] = "qux"
@@ -249,9 +208,67 @@
     assert str(cfg.configdict["foo"]["bar1"]) == "1"
     assert str(cfg.configdict["foo"]["bar2"]) == "2"
     assert str(cfg.configdict["foo"]["bar3"]) == "3"
     # assert not
     assert not "bar4" in cfg.configdict["foo"]
 
 
+def test_dotcfg2env():
+    """Tests if the setenv() function works"""
+    environ = {}
+    dotstrings = {
+        "common.logdir": "/another/path",
+        "suitecfg.uuid": "1234",
+        "suitecfg.run.rcc": False,
+    }
+    cfg = Config()
+    cfg.set("common.suiteuname", "foo_suite")
+    cfg.dotcfg_to_env(dotstrings, environ=environ)
+    assert environ["ROBOTMK_common_logdir"] == "/another/path"
+    assert environ["ROBOTMK_suites_foo__suite_uuid"] == "1234"
+    assert environ["ROBOTMK_suites_foo__suite_run_rcc"] == "False"
+
+
+def test_cfg2env():
+    """Tests the conversion of a config dictionary to environment variables."""
+    environ = {}
+    cfg = Config()
+    cfg.set("common.log_level", "INFO")
+    cfg.set("common.suiteuname", "foo_suite")
+    cfg.set("suitecfg.my_value", "qux")
+    cfg.set("suitecfg.my_list", ["one", "two", "three"])
+    cfg.set("suitecfg.my_dict", {"foo": "one", "bar": "two", "baz": "three"})
+    cfg.set(
+        "suitecfg.my_list_of_dict",
+        [
+            {"foo": "one", "bar": "two", "baz": "three"},
+            {"foo": "one", "bar": "two", "baz": "three"},
+            {"foo": "one", "bar": "two", "baz": "three"},
+        ],
+    )
+    cfg.cfg_to_environment(cfg.configdict, environ=environ)
+    # simple values
+    assert environ["ROBOTMK_common_log__level"] == "INFO"
+    assert environ["ROBOTMK_common_suiteuname"] == "foo_suite"
+    assert environ["ROBOTMK_suites_foo__suite_my__value"] == "qux"
+    # lists
+    assert environ["ROBOTMK_suites_foo__suite_my__list_0"] == "one"
+    assert environ["ROBOTMK_suites_foo__suite_my__list_1"] == "two"
+    assert environ["ROBOTMK_suites_foo__suite_my__list_2"] == "three"
+    # dicts
+    assert environ["ROBOTMK_suites_foo__suite_my__dict_foo"] == "one"
+    assert environ["ROBOTMK_suites_foo__suite_my__dict_bar"] == "two"
+    assert environ["ROBOTMK_suites_foo__suite_my__dict_baz"] == "three"
+    # list of dicts
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_0_foo"] == "one"
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_0_bar"] == "two"
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_0_baz"] == "three"
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_1_foo"] == "one"
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_1_bar"] == "two"
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_1_baz"] == "three"
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_2_foo"] == "one"
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_2_bar"] == "two"
+    assert environ["ROBOTMK_suites_foo__suite_my__list__of__dict_2_baz"] == "three"
+
+
 # TODO: split_varstring
 # TODO: config validation
```

### Comparing `robotmk-0.0.50/tests/context/local/test_local_cli.py` & `robotmk-0.0.51/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.51/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/tests/context/suite/robotmk.yml` & `robotmk-0.0.51/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.51/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/tests/context/test_cli.py` & `robotmk-0.0.51/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/tests/yml/robotmk.yml` & `robotmk-0.0.51/tests/yml/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.50/PKG-INFO` & `robotmk-0.0.51/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotmk
-Version: 0.0.50
+Version: 0.0.51
 Summary: Robot Framework test execution and result parsing for Check_MK
 Keywords: robotmk,checkmk,robotframework,automation,monitoring
 Author-email: Simon Meggle <simon.meggle@elabit.de>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: click
 Requires-Dist: psutil
```

