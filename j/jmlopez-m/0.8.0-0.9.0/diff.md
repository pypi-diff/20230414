# Comparing `tmp/jmlopez-m-0.8.0.tar.gz` & `tmp/jmlopez-m-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmlopez-m-0.8.0.tar", last modified: Tue Mar 15 22:32:02 2022, max compression
+gzip compressed data, was "jmlopez-m-0.9.0.tar", last modified: Wed Jun 22 01:16:57 2022, max compression
```

## Comparing `jmlopez-m-0.8.0.tar` & `jmlopez-m-0.9.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.982573 jmlopez-m-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-03-15 22:32:02.982573 jmlopez-m-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.970573 jmlopez-m-0.8.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1276 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/bin/endRelease
--rwxr-xr-x   0 runner    (1001) docker     (121)      388 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/bin/m
--rwxr-xr-x   0 runner    (1001) docker     (121)     3500 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/bin/reviewRelease
--rwxr-xr-x   0 runner    (1001) docker     (121)      963 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/bin/startHotfix
--rwxr-xr-x   0 runner    (1001) docker     (121)      969 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/bin/startRelease
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-15 22:32:02.982573 jmlopez-m-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.966572 jmlopez-m-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.970573 jmlopez-m-0.8.0/src/jmlopez_m.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-03-15 22:32:02.000000 jmlopez-m-0.8.0/src/jmlopez_m.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-03-15 22:32:02.000000 jmlopez-m-0.8.0/src/jmlopez_m.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 22:32:02.000000 jmlopez-m-0.8.0/src/jmlopez_m.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-15 22:32:02.000000 jmlopez-m-0.8.0/src/jmlopez_m.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-03-15 22:32:02.000000 jmlopez-m-0.8.0/src/jmlopez_m.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.970573 jmlopez-m-0.8.0/src/m/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.974573 jmlopez-m-0.8.0/src/m/ci/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/assert_branch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.974573 jmlopez-m-0.8.0/src/m/ci/celt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.978572 jmlopez-m-0.8.0/src/m/ci/celt/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5328 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/core/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     8434 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/core/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/core/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      956 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/post_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.978572 jmlopez-m-0.8.0/src/m/ci/celt/post_processors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/post_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/post_processors/eslint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/post_processors/pycodestyle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/celt/post_processors/pylint.py
--rw-r--r--   0 runner    (1001) docker     (121)     4102 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     7386 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/git_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/init.py
--rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/m_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/release_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     3852 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/release_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/ci/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.978572 jmlopez-m-0.8.0/src/m/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.978572 jmlopez-m-0.8.0/src/m/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.978572 jmlopez-m-0.8.0/src/m/cli/commands/ci/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/ci/assert_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/ci/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4405 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/ci/celt.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/ci/env.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/ci/init.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/ci/npm_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/ci/release_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.978572 jmlopez-m-0.8.0/src/m/cli/commands/git/
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/git/branch.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/git/current_sha.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/git/first_sha.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/git/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.982573 jmlopez-m-0.8.0/src/m/cli/commands/github/
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/build_sha.py
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/create_pr.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/latest_release.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/merge_pr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/pr.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/release.py
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/github/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/jsonq.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.982573 jmlopez-m-0.8.0/src/m/cli/commands/message/
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/message/close.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/message/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/message/open.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/message/sibling_block.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/commands/message/warn.py
--rw-r--r--   0 runner    (1001) docker     (121)     9128 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/cli/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.982573 jmlopez-m-0.8.0/src/m/core/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/core/fp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/core/http.py
--rw-r--r--   0 runner    (1001) docker     (121)    12728 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/core/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/core/issue.py
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/core/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/core/one_of.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/core/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/git.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 22:32:02.982573 jmlopez-m-0.8.0/src/m/github/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/github/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     6075 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/github/ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/github/ci_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/github/ci_graph_queries.py
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/github/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-03-15 22:31:56.000000 jmlopez-m-0.8.0/src/m/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.744259 jmlopez-m-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-06-22 01:16:57.744259 jmlopez-m-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.732259 jmlopez-m-0.9.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1276 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/bin/endRelease
+-rwxr-xr-x   0 runner    (1001) docker     (121)      388 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/bin/m
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3500 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/bin/reviewRelease
+-rwxr-xr-x   0 runner    (1001) docker     (121)      963 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/bin/startHotfix
+-rwxr-xr-x   0 runner    (1001) docker     (121)      969 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/bin/startRelease
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-22 01:16:57.744259 jmlopez-m-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.728259 jmlopez-m-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.732259 jmlopez-m-0.9.0/src/jmlopez_m.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-06-22 01:16:57.000000 jmlopez-m-0.9.0/src/jmlopez_m.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-06-22 01:16:57.000000 jmlopez-m-0.9.0/src/jmlopez_m.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 01:16:57.000000 jmlopez-m-0.9.0/src/jmlopez_m.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-22 01:16:57.000000 jmlopez-m-0.9.0/src/jmlopez_m.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        2 2022-06-22 01:16:57.000000 jmlopez-m-0.9.0/src/jmlopez_m.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.732259 jmlopez-m-0.9.0/src/m/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.732259 jmlopez-m-0.9.0/src/m/ci/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/assert_branch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.732259 jmlopez-m-0.9.0/src/m/ci/celt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.736259 jmlopez-m-0.9.0/src/m/ci/celt/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5328 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/core/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8497 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/core/process.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2312 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      956 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/post_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.736259 jmlopez-m-0.9.0/src/m/ci/celt/post_processors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/post_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/post_processors/eslint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/post_processors/pycodestyle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/celt/post_processors/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8031 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/git_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/init.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2542 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/m_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3654 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/release_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3852 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/release_setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3047 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/ci/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.736259 jmlopez-m-0.9.0/src/m/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.736259 jmlopez-m-0.9.0/src/m/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.736259 jmlopez-m-0.9.0/src/m/cli/commands/ci/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/ci/assert_branch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/ci/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4405 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/ci/celt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      507 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/ci/env.py
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/ci/init.py
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/ci/npm_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/ci/release_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.740259 jmlopez-m-0.9.0/src/m/cli/commands/git/
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/git/branch.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/git/current_sha.py
+-rw-r--r--   0 runner    (1001) docker     (121)      559 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/git/first_sha.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/git/status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.740259 jmlopez-m-0.9.0/src/m/cli/commands/github/
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/build_sha.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/ci.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1788 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/create_pr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/latest_release.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/merge_pr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/pr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/release.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/github/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/jsonq.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.740259 jmlopez-m-0.9.0/src/m/cli/commands/message/
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/message/close.py
+-rw-r--r--   0 runner    (1001) docker     (121)      913 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/message/error.py
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/message/open.py
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/message/sibling_block.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/commands/message/warn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9092 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2701 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/cli/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.740259 jmlopez-m-0.9.0/src/m/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3124 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/core/fp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/core/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12716 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/core/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/core/issue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/core/json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/core/one_of.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/core/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/git.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:57.744259 jmlopez-m-0.9.0/src/m/github/
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3700 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/github/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6075 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/github/ci.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/github/ci_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/github/ci_graph_queries.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-22 01:16:49.000000 jmlopez-m-0.9.0/src/m/version.py
```

### Comparing `jmlopez-m-0.8.0/LICENSE` & `jmlopez-m-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/PKG-INFO` & `jmlopez-m-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: jmlopez-m
-Version: 0.8.0
+Version: 0.9.0
 Summary: m
 Home-page: https://github.com/jmlopez-rod/m
 Author: Manuel Lopez
 Author-email: jmlopez.rod@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jmlopez-rod/m/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -43,9 +41,7 @@
 ```
 @jmlopez-rod:registry=https://npm.pkg.github.com/
 //npm.pkg.github.com/:_authToken=${GITHUB_TOKEN}
 ```
 
 Make sure to have `GITHUB_TOKEN` defined in your environment variables with
 a valid token obtained from <https://github.com/settings/tokens>.
-
-
```

### Comparing `jmlopez-m-0.8.0/bin/endRelease` & `jmlopez-m-0.9.0/bin/endRelease`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/bin/reviewRelease` & `jmlopez-m-0.9.0/bin/reviewRelease`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/bin/startHotfix` & `jmlopez-m-0.9.0/bin/startHotfix`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/bin/startRelease` & `jmlopez-m-0.9.0/bin/startRelease`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/setup.py` & `jmlopez-m-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='jmlopez-m',
-    version='0.8.0',
+    version='0.9.0',
     author='Manuel Lopez',
     author_email='jmlopez.rod@gmail.com',
     description='m',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/jmlopez-rod/m',
     project_urls={
```

### Comparing `jmlopez-m-0.8.0/src/jmlopez_m.egg-info/PKG-INFO` & `jmlopez-m-0.9.0/src/jmlopez_m.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: jmlopez-m
-Version: 0.8.0
+Version: 0.9.0
 Summary: m
 Home-page: https://github.com/jmlopez-rod/m
 Author: Manuel Lopez
 Author-email: jmlopez.rod@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jmlopez-rod/m/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -43,9 +41,7 @@
 ```
 @jmlopez-rod:registry=https://npm.pkg.github.com/
 //npm.pkg.github.com/:_authToken=${GITHUB_TOKEN}
 ```
 
 Make sure to have `GITHUB_TOKEN` defined in your environment variables with
 a valid token obtained from <https://github.com/settings/tokens>.
-
-
```

### Comparing `jmlopez-m-0.8.0/src/jmlopez_m.egg-info/SOURCES.txt` & `jmlopez-m-0.9.0/src/jmlopez_m.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/assert_branch.py` & `jmlopez-m-0.9.0/src/m/ci/assert_branch.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/celt/core/io.py` & `jmlopez-m-0.9.0/src/m/ci/celt/core/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,19 +119,19 @@
     buffer.extend([
         f'  {file_name}: found {total}'
         for file_name, violations in by_file
         for total in (len(violations), )
     ])
     buffer.append('')
 
-    c1_w = max([len(x) for x in keys])
+    c1_w = max((len(x) for x in keys))
     c1_w = max([c1_w, len('rules')])
-    c2_w = max([len(str(s.found)) for s in rules])
+    c2_w = max((len(str(s.found)) for s in rules))
     c2_w = max([c2_w, len('found')])
-    c3_w = max([len(str(s.allowed)) for s in rules])
+    c3_w = max((len(str(s.allowed)) for s in rules))
     c3_w = max([c3_w, len('allowed')])
     widths = [c1_w, c2_w, c3_w]
 
     key_rule = sorted(
         project.rules.items(),
         key=cmp_to_key(_compare_rule_items),
     )
```

### Comparing `jmlopez-m-0.8.0/src/m/ci/celt/core/process.py` & `jmlopez-m-0.9.0/src/m/ci/celt/core/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,16 @@
     try:
         old, prefix = file_prefix.split(':')
     except ValueError as ex:
         return issue('file_prefix param missing `:`', cause=ex)
     return Good(re.sub(
         fr'({old})(.*?)\.([a-z]+)',
         lambda x: [
-            f'{prefix}{filename}.{ext}'
+            # Not sure how fix this mypy issue
+            f'{prefix}{filename}.{ext}'  # type: ignore
             for _, filename, ext in (x.groups(),)
         ][0],
         payload,
     ))
 
 
 def filter_reports(
```

### Comparing `jmlopez-m-0.8.0/src/m/ci/celt/core/types.py` & `jmlopez-m-0.9.0/src/m/ci/celt/core/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,24 +54,24 @@
     total_found: int = field(init=False)
     total_allowed: int = field(init=False)
     error_msg: str = field(init=False)
 
     def __post_init__(self):
         """Compute the rest of non initialized variables."""
         rules = self.rules.values()
-        total_found = sum([s.found for s in rules if not s.ignored])
-        total_allowed = sum([s.allowed for s in rules if not s.ignored])
+        total_found = sum((s.found for s in rules if not s.ignored))
+        total_allowed = sum((s.allowed for s in rules if not s.ignored))
         error_msg = ''
         if self.status == ExitCode.error:
-            diff = sum([
+            diff = sum((
                 d
                 for s in rules
                 for d in (s.found - s.allowed,)
                 if d > 0 and not s.ignored
-            ])
+            ))
             error_msg = f'{diff} extra errors were introduced'
         elif self.status == ExitCode.needs_readjustment:
             diff = total_allowed - total_found
             error_msg = f'{diff} errors were removed - lower error allowance'
 
         self.total_found = total_found  # noqa: WPS601
         self.total_allowed = total_allowed  # noqa: WPS601
```

### Comparing `jmlopez-m-0.8.0/src/m/ci/celt/post_processor.py` & `jmlopez-m-0.9.0/src/m/ci/celt/post_processor.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/celt/post_processors/eslint.py` & `jmlopez-m-0.9.0/src/m/ci/celt/post_processors/eslint.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/celt/post_processors/pycodestyle.py` & `jmlopez-m-0.9.0/src/m/ci/celt/post_processors/pycodestyle.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/celt/post_processors/pylint.py` & `jmlopez-m-0.9.0/src/m/ci/celt/post_processors/pylint.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/config.py` & `jmlopez-m-0.9.0/src/m/ci/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,23 @@
     return ''
 
 
 @dataclass
 class Config(JsonStr):
     """Object to store the m project configuration."""
 
+    # pylint: disable=too-many-instance-attributes
     owner: str
     repo: str
     version: str
     m_dir: str
     workflow: Workflow
     git_flow: GitFlowConfig
     m_flow: MFlowConfig
+    build_tag_with_version: bool = False
 
     def uses_git_flow(self):
         """Check if configuration is using the git flow.
 
         Returns:
             True if workflow is the git flow.
         """
@@ -119,15 +121,25 @@
     Args:
         m_dir: Directory containing `m.json`.
 
     Returns:
         A `OneOf` containing the `m` configuration or an `Issue`.
     """
     return one_of(lambda: [
-        Config(owner, repo, version, m_dir, workflow, git_flow, m_flow)
+        Config(
+            owner,
+            repo,
+            version,
+            m_dir,
+            workflow,
+            git_flow,
+            m_flow,
+            build_tag_with_version=with_version,
+        )
         for m_cfg in json.read_json(f'{m_dir}/m.json')
         for owner, repo in json.multi_get(m_cfg, 'owner', 'repo')
         for version in (m_cfg.get('version', '0.0.0'),)
         for workflow in read_workflow(m_cfg.get('workflow', 'free-flow'))
         for git_flow in read_git_flow(m_cfg.get('gitFlow', {}))
         for m_flow in read_m_flow(m_cfg.get('mFlow', {}))
+        for with_version in (m_cfg.get('build_tag_with_version', False),)
     ]).flat_map_bad(lambda x: issue('read_config failure', cause=x))
```

### Comparing `jmlopez-m-0.8.0/src/m/ci/git_env.py` & `jmlopez-m-0.9.0/src/m/ci/git_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,20 @@
 
     def is_hotfix_pr(self, config: Config) -> bool:
         """Determine if the the current pr is a hotfix pr.
 
         It is a release pr as far as the pull request should see it but
         from the context of the git environment we need to label it as a
         hotfix pr.
+
+        Args:
+            config: The m configuration object.
+
+        Returns:
+            True if the we are dealing with hotfix pr.
         """
         if not self.pull_request:
             return False
         hotfix_prefix = get_hotfix_prefix(config)
         return self.pull_request.is_release_pr(hotfix_prefix)
 
     def get_build_tag(self, config: Config, run_id: str) -> OneOf[Issue, str]:
@@ -141,15 +147,15 @@
         is_release = self.is_release(config)
         is_release_pr = self.is_release_pr(config)
         is_hotfix_pr = self.is_hotfix_pr(config)
         is_dev_branch = self.target_branch == config.git_flow.develop_branch
         if config.uses_git_flow() and is_dev_branch:
             if is_release or is_release_pr or is_hotfix_pr:
                 return Good('SKIP')
-        prefix = '' if config.uses_free_flow() else '0.0.0-'
+        prefix = '' if config.uses_free_flow() else _build_tag_prefix(config)
         if not run_id:
             return Good(f'{prefix}local.{self.sha}')
         if is_release:
             return Good(config.version)
         if self.pull_request:
             pr_number = self.pull_request.pr_number
             nprefix = ''
@@ -159,28 +165,49 @@
                 nprefix = 'hotfix'
             if nprefix:
                 return Good(f'{config.version}-{nprefix}{pr_number}.b{run_id}')
             return Good(f'{prefix}pr{pr_number}.b{run_id}')
         return Good(f'{prefix}{self.target_branch}.b{run_id}')
 
 
+def _build_tag_prefix(config: Config) -> str:
+    if config.build_tag_with_version:
+        return f'{config.version}-'
+    return '0.0.0-'
+
+
 def get_pr_number(branch: str) -> Optional[int]:
-    """Retrieve the pull request number from the branch name."""
+    """Retrieve the pull request number from the branch name.
+
+    Args:
+        branch: The branch name from where the pr number is extracted.py
+
+    Returns:
+        The pr number if the branch is a pull request otherwise `None`.
+    """
     if 'pull/' in branch:
         parts = branch.split('/')
         return int(parts[parts.index('pull') + 1])
     return None
 
 
-def _remove_strings(content: str, words: List[str]) -> str:
-    return re.sub('|'.join(words), '', content)
+def _remove_strings(str_content: str, words: List[str]) -> str:
+    return re.sub('|'.join(words), '', str_content)
 
 
 def get_git_env(config: Config, env_vars: EnvVars) -> OneOf[Issue, GitEnv]:
-    """Obtain the git environment by asking Github's API."""
+    """Obtain the git environment by asking Github's API.
+
+    Args:
+        config: The m configuration object.
+        env_vars: The environment variables.
+
+    Returns:
+        The git environment object or an issue.
+    """
     branch = _remove_strings(env_vars.git_branch, ['refs/heads/', 'heads/'])
     sha = env_vars.git_sha
     git_env = GitEnv(sha, branch, branch)
 
     # quick exit for local environment
     if not env_vars.ci_env:
         return Good(git_env)
```

### Comparing `jmlopez-m-0.8.0/src/m/ci/init.py` & `jmlopez-m-0.9.0/src/m/ci/init.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/m_env.py` & `jmlopez-m-0.9.0/src/m/ci/m_env.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/release_env.py` & `jmlopez-m-0.9.0/src/m/ci/release_env.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/release_setup.py` & `jmlopez-m-0.9.0/src/m/ci/release_setup.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/ci/types.py` & `jmlopez-m-0.9.0/src/m/ci/types.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/argparse.py` & `jmlopez-m-0.9.0/src/m/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/ci/assert_branch.py` & `jmlopez-m-0.9.0/src/m/cli/commands/ci/assert_branch.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/ci/bump_version.py` & `jmlopez-m-0.9.0/src/m/cli/commands/ci/bump_version.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/ci/celt.py` & `jmlopez-m-0.9.0/src/m/cli/commands/ci/celt.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/ci/npm_tag.py` & `jmlopez-m-0.9.0/src/m/cli/commands/ci/npm_tag.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/ci/release_setup.py` & `jmlopez-m-0.9.0/src/m/cli/commands/ci/release_setup.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/git/current_sha.py` & `jmlopez-m-0.9.0/src/m/cli/commands/git/current_sha.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/git/first_sha.py` & `jmlopez-m-0.9.0/src/m/cli/commands/git/first_sha.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/git/status.py` & `jmlopez-m-0.9.0/src/m/cli/commands/git/status.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/github/build_sha.py` & `jmlopez-m-0.9.0/src/m/cli/commands/github/build_sha.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/github/ci.py` & `jmlopez-m-0.9.0/src/m/cli/commands/github/ci.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/github/create_pr.py` & `jmlopez-m-0.9.0/src/m/cli/commands/github/create_pr.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/github/latest_release.py` & `jmlopez-m-0.9.0/src/m/cli/commands/github/latest_release.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/github/merge_pr.py` & `jmlopez-m-0.9.0/src/m/cli/commands/github/merge_pr.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/github/pr.py` & `jmlopez-m-0.9.0/src/m/cli/commands/github/pr.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/github/release.py` & `jmlopez-m-0.9.0/src/m/cli/commands/github/release.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/github/status.py` & `jmlopez-m-0.9.0/src/m/cli/commands/github/status.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/json.py` & `jmlopez-m-0.9.0/src/m/cli/commands/json.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/jsonq.py` & `jmlopez-m-0.9.0/src/m/cli/commands/jsonq.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/message/close.py` & `jmlopez-m-0.9.0/src/m/cli/commands/message/close.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/message/error.py` & `jmlopez-m-0.9.0/src/m/cli/commands/message/error.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/message/open.py` & `jmlopez-m-0.9.0/src/m/cli/commands/message/open.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/message/sibling_block.py` & `jmlopez-m-0.9.0/src/m/cli/commands/message/sibling_block.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/commands/message/warn.py` & `jmlopez-m-0.9.0/src/m/cli/commands/message/warn.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/cli/utils.py` & `jmlopez-m-0.9.0/src/m/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,32 +21,29 @@
     @staticmethod
     def add_arguments(_parser: argparse.ArgumentParser) -> None:
         """Define options that may apply to the subparsers.
 
         Should be defined if we want to manipulate the argument parser
         object.
         """
-        ...
 
     @staticmethod
     def add_parser(
         _subparser: argparse._SubParsersAction,  # noqa pylint: disable=protected-access
         _raw: Type[argparse.RawTextHelpFormatter],
     ) -> None:
         """Define cli arguments for a command."""
-        ...
 
     @staticmethod
     def run(_arg: argparse.Namespace) -> int:
         """Entry point for the cli.
 
         Call a library function and return 0 if successful or non-zero if there
         is a failure.
         """
-        ...
 
 
 def import_mod(name: str) -> CmdModule:
     """Import a module by string."""
     module = __import__(name)
     for part in name.split('.')[1:]:
         module = getattr(module, part)
```

### Comparing `jmlopez-m-0.8.0/src/m/cli/validators.py` & `jmlopez-m-0.9.0/src/m/cli/validators.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/core/fp.py` & `jmlopez-m-0.9.0/src/m/core/fp.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/core/http.py` & `jmlopez-m-0.9.0/src/m/core/http.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/core/io.py` & `jmlopez-m-0.9.0/src/m/core/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,14 @@
     def open_block(name: str, description: str) -> None:
         """Define how a block is opened."""
         print(f'{name}: {description}')
 
     @staticmethod
     def close_block(_name: str) -> None:
         """Define how a block is closed."""
-        ...
 
     @staticmethod
     def error(
         description: str,
         file: Optional[str] = None,
         line: Optional[str] = None,
         col: Optional[str] = None,
```

### Comparing `jmlopez-m-0.8.0/src/m/core/issue.py` & `jmlopez-m-0.9.0/src/m/core/issue.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/core/json.py` & `jmlopez-m-0.9.0/src/m/core/json.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/core/one_of.py` & `jmlopez-m-0.9.0/src/m/core/one_of.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/core/subprocess.py` & `jmlopez-m-0.9.0/src/m/core/subprocess.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/git.py` & `jmlopez-m-0.9.0/src/m/git.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/github/api.py` & `jmlopez-m-0.9.0/src/m/github/api.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/github/ci.py` & `jmlopez-m-0.9.0/src/m/github/ci.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/github/ci_dataclasses.py` & `jmlopez-m-0.9.0/src/m/github/ci_dataclasses.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/github/ci_graph_queries.py` & `jmlopez-m-0.9.0/src/m/github/ci_graph_queries.py`

 * *Files identical despite different names*

### Comparing `jmlopez-m-0.8.0/src/m/github/cli.py` & `jmlopez-m-0.9.0/src/m/github/cli.py`

 * *Files identical despite different names*

