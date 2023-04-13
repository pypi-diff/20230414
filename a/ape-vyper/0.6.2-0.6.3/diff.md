# Comparing `tmp/ape-vyper-0.6.2.tar.gz` & `tmp/ape-vyper-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-vyper-0.6.2.tar", last modified: Thu Mar  2 17:41:25 2023, max compression
+gzip compressed data, was "ape-vyper-0.6.3.tar", last modified: Thu Apr 13 22:01:54 2023, max compression
```

## Comparing `ape-vyper-0.6.2.tar` & `ape-vyper-0.6.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.734545 ape-vyper-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.734545 ape-vyper-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.734545 ape-vyper-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/ape_vyper/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/ape_vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/ape_vyper/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/ape_vyper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-02 17:41:25.000000 ape-vyper-0.6.2/ape_vyper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/ape_vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-03-02 17:41:25.000000 ape-vyper-0.6.2/ape_vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-02 17:41:25.000000 ape-vyper-0.6.2/ape_vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 17:41:25.000000 ape-vyper-0.6.2/ape_vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 17:41:25.000000 ape-vyper-0.6.2/ape_vyper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-02 17:41:25.000000 ape-vyper-0.6.2/ape_vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-02 17:41:25.000000 ape-vyper-0.6.2/ape_vyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.734545 ape-vyper-0.6.2/tests/ExampleDependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/tests/ExampleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/ExampleDependency/contracts/Dependency.vy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.734545 ape-vyper-0.6.2/tests/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/tests/contracts/failing_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/failing_contracts/contract_undeclared_variable.vy
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/failing_contracts/contract_unknown_pragma.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/tests/contracts/passing_contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/contract_no_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/contract_with_dev_messages.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:41:25.738545 ape-vyper-0.6.2/tests/contracts/passing_contracts/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/interfaces/IFace.vy
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/interfaces/IFace2.vy
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/older_version.vy
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/use_iface.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/contracts/passing_contracts/use_iface2.vy
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-03-02 17:40:33.000000 ape-vyper-0.6.2/tests/test_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.122390 ape-vyper-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.122390 ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/ape_vyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/ape_vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19803 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/ape_vyper/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/ape_vyper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 22:01:53.000000 ape-vyper-0.6.3/ape_vyper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/ape_vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 22:01:54.000000 ape-vyper-0.6.3/ape_vyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.122390 ape-vyper-0.6.3/tests/ExampleDependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/ExampleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/ExampleDependency/contracts/Dependency.vy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.122390 ape-vyper-0.6.3/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/contracts/failing_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/failing_contracts/contract_undeclared_variable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/failing_contracts/contract_unknown_pragma.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/contracts/passing_contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/contract_no_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/contract_with_dev_messages.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:01:54.126391 ape-vyper-0.6.3/tests/contracts/passing_contracts/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/interfaces/IFace.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/interfaces/IFace2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/older_version.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/use_iface.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/contracts/passing_contracts/use_iface2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-04-13 22:01:09.000000 ape-vyper-0.6.3/tests/test_compiler.py
```

### Comparing `ape-vyper-0.6.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-vyper-0.6.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.github/release-drafter.yml` & `ape-vyper-0.6.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.github/workflows/commitlint.yaml` & `ape-vyper-0.6.3/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.github/workflows/prtitle.yaml` & `ape-vyper-0.6.3/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.github/workflows/publish.yaml` & `ape-vyper-0.6.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.github/workflows/test.yaml` & `ape-vyper-0.6.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.gitignore` & `ape-vyper-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/.pre-commit-config.yaml` & `ape-vyper-0.6.3/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
     -   id: mypy
```

### Comparing `ape-vyper-0.6.2/CONTRIBUTING.md` & `ape-vyper-0.6.3/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 It's a good idea to make pull requests early on.
 A pull request represents the start of a discussion, and doesn't necessarily need to be the final, finished submission.
 
 If you are opening a work-in-progress pull request to verify that it passes CI tests, please consider
 [marking it as a draft](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests#draft-pull-requests).
 
-Join the Ethereum Python [Discord](https://discord.gg/PcEJ54yX) if you have any questions.
+Join the ApeWorX [Discord](https://discord.gg/apeworx) if you have any questions.
 
 ## Testing
 
 By default, the test suite will use a new, temporary path for the Vyper compiler installations.
 This ensures that the tests always run from a clean slate without any relying on existing installations.
 
 If you wish to use your existing `~/.vvm` installations instead, you must set the environment variable `APE_VYPER_USE_SYSTEM_VYPER=1`.
```

### Comparing `ape-vyper-0.6.2/LICENSE` & `ape-vyper-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/PKG-INFO` & `ape-vyper-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.2
+Version: 0.6.3
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-vyper-0.6.2/README.md` & `ape-vyper-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/ape_vyper/compiler.py` & `ape-vyper-0.6.3/ape_vyper/compiler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import os
 import re
 import shutil
 from pathlib import Path
-from typing import Dict, List, Optional, Set, Union, cast
+from typing import Any, Dict, List, Optional, Set, Tuple, Union, cast
 
 import vvm  # type: ignore
 from ape.api import PluginConfig
 from ape.api.compiler import CompilerAPI
+from ape.exceptions import ContractLogicError
 from ape.types import ContractType
 from ape.utils import cached_property, get_relative_path
 from eth_utils import is_0x_prefixed
-from ethpm_types import ASTNode, PackageManifest
+from ethpm_types import ASTNode, PackageManifest, PCMap
 from ethpm_types.contract_type import SourceMap
 from semantic_version import NpmSpec, Version  # type: ignore
 from vvm.exceptions import VyperError  # type: ignore
 
-from .exceptions import VyperCompileError, VyperInstallError
+from ape_vyper.exceptions import (
+    RUNTIME_ERROR_MAP,
+    RuntimeErrorType,
+    VyperCompileError,
+    VyperInstallError,
+)
 
 DEV_MSG_PATTERN = re.compile(r"#\s*(dev:.+)")
 
 
 class VyperConfig(PluginConfig):
     evm_version: Optional[str] = None
 
@@ -131,21 +137,21 @@
         return versions
 
     @cached_property
     def package_version(self) -> Optional[Version]:
         try:
             import vyper  # type: ignore
 
-            # Strip off parts from source-installation
-            version = Version.coerce(vyper.__version__)
-            return Version(major=version.major, minor=version.minor, patch=version.patch)
-
         except ImportError:
             return None
 
+        # Strip off parts from source-installation
+        version = Version.coerce(vyper.__version__)
+        return Version(major=version.major, minor=version.minor, patch=version.patch)
+
     @cached_property
     def available_versions(self) -> List[Version]:
         # NOTE: Package version should already be included in available versions
         return vvm.get_installable_vyper_versions()
 
     @property
     def installed_versions(self) -> List[Version]:
@@ -241,47 +247,104 @@
                     # De-compress source map to get PC POS map.
                     ast = ASTNode.parse_obj(result["sources"][source_id]["ast"])
                     bytecode = output["evm"]["deployedBytecode"]
                     opcodes = bytecode["opcodes"].split(" ")
                     compressed_src_map = SourceMap(__root__=bytecode["sourceMap"])
                     src_map = list(compressed_src_map.parse())[1:]
                     pc = 0
-                    pc_map = {}
-                    content = (base_path / source_id).read_text()
+                    pc_map_list: List[Tuple[int, Dict[str, Optional[Any]]]] = []
+                    content = {
+                        i + 1: ln
+                        for i, ln in enumerate((base_path / source_id).read_text().splitlines())
+                    }
+                    last_value = None
+                    revert_pc = -1
+                    if _is_nonpayable_check(opcodes):
+                        # Starting in vyper 0.2.14, reverts without a reason string are optimized
+                        # with a jump to the "end" of the bytecode.
+                        revert_pc = (
+                            len(opcodes)
+                            + sum(int(i[4:]) - 1 for i in opcodes if i.startswith("PUSH"))
+                            - 18
+                        )
 
+                    processed_opcodes = []
                     while src_map and opcodes:
                         src = src_map.pop(0)
                         op = opcodes.pop(0)
-
+                        processed_opcodes.append(op)
+                        start_pc = pc
+                        pc += 1
                         if opcodes and is_0x_prefixed(opcodes[0]):
-                            opcodes.pop(0)  # Value
+                            last_value = int(opcodes.pop(0), 16)
                             pc += int(op[4:])
 
-                        pc += 1
+                        # Check for special Payable case.
+                        if src.start is None:
+                            if (
+                                op == "REVERT"
+                                and len(processed_opcodes) > 6
+                                and processed_opcodes[-7] == "CALLVALUE"
+                            ) or _is_revert_jump(op, last_value, revert_pc, processed_opcodes):
+                                pc_map_item = {
+                                    "location": None,
+                                    "dev": f"dev: {RuntimeErrorType.NONPAYABLE_CHECK.value}",
+                                }
+                                pc_map_list.append(
+                                    (pc if op == "REVERT" else start_pc, pc_map_item)
+                                )
+
+                            continue
+
+                        # Add content PC item.
+                        # Also check for compiler runtime error handling.
+                        # Runtime error locations are marked in the PCMap for further analysis.
                         if src.start is not None and src.length is not None:
                             stmt = ast.get_node(src)
                             if stmt:
-                                pc_map[pc] = list(stmt.line_numbers)
+                                item: Dict = {"location": list(stmt.line_numbers)}
+                                is_revert_jump = _is_revert_jump(
+                                    op, last_value, revert_pc, processed_opcodes
+                                )
+                                if op == "REVERT" or is_revert_jump:
+                                    dev = None
+                                    if stmt.ast_type in ("AugAssign", "BinOp"):
+                                        # SafeMath
+                                        for node in stmt.children:
+                                            dev = RuntimeErrorType.from_operator(node.ast_type)
+                                            if dev:
+                                                break
+
+                                    elif stmt.ast_type == "Subscript":
+                                        dev = RuntimeErrorType.INDEX_OUT_OF_RANGE
+
+                                    if dev:
+                                        val = f"dev: {dev.value}"
+                                        if is_revert_jump:
+                                            pc_map_list[-1][1]["dev"] = val
+                                        else:
+                                            item["dev"] = val
+
+                                pc_map_list.append((pc, item))
 
-                    # Find dev messages.
+                    # Find content-specified dev messages.
                     dev_messages = {}
-                    if pc_map:
-                        for line_index, line in enumerate(content.splitlines()):
-                            if match := re.search(DEV_MSG_PATTERN, line):
-                                dev_messages[line_index + 1] = match.group(1).strip()
+                    for line_no, line in content.items():
+                        if match := re.search(DEV_MSG_PATTERN, line):
+                            dev_messages[line_no] = match.group(1).strip()
 
                     contract_type = ContractType(
                         ast=ast,
                         contractName=name,
                         sourceId=source_id,
                         deploymentBytecode={"bytecode": output["evm"]["bytecode"]["object"]},
                         runtimeBytecode={"bytecode": bytecode["object"]},
                         abi=output["abi"],
                         sourcemap=compressed_src_map,
-                        pcmap=pc_map,
+                        pcmap=PCMap.parse_obj(dict(pc_map_list)),
                         userdoc=output["userdoc"],
                         devdoc=output["devdoc"],
                         dev_messages=dev_messages,
                     )
                     contract_types.append(contract_type)
 
         return contract_types
@@ -378,15 +441,51 @@
             }
 
         return arguments_map
 
     def _get_vyper_bin(self, vyper_version: Version):
         return shutil.which("vyper") if vyper_version is self.package_version else None
 
+    def enrich_error(self, err: ContractLogicError) -> ContractLogicError:
+        try:
+            dev_message = err.dev_message
+        except ValueError:
+            # Not available.
+            return err
+
+        if not dev_message:
+            return err
+
+        err_str = dev_message.replace("dev: ", "")
+
+        if err_str in [m.value for m in RuntimeErrorType]:
+            # Is a builtin compiler error.
+            runtime_error_type = RuntimeErrorType(err_str)
+            runtime_error_cls = RUNTIME_ERROR_MAP[runtime_error_type]
+            return runtime_error_cls(
+                txn=err.txn, trace=err.trace, contract_address=err.contract_address
+            )
+
+        else:
+            # Not a builtin compiler error; cannot enrich.
+            return err
+
 
 def _safe_append(data: Dict, version: Union[Version, NpmSpec], paths: Union[Path, Set]):
     if isinstance(paths, Path):
         paths = {paths}
     if version in data:
         data[version] = data[version].union(paths)
     else:
         data[version] = paths
+
+
+def _is_revert_jump(
+    op: str, value: Optional[int], revert_pc: int, processed_opcodes: List[str]
+) -> bool:
+    return op == "JUMPI" and value is not None and value == revert_pc and len(processed_opcodes) > 2
+
+
+def _is_nonpayable_check(opcodes: List[str]) -> bool:
+    return (len(opcodes) > 12 and opcodes[-13] == "JUMPDEST" and opcodes[-9] == "REVERT") or (
+        len(opcodes) > 4 and opcodes[-5] == "JUMPDEST" and opcodes[-1] == "REVERT"
+    )
```

### Comparing `ape-vyper-0.6.2/ape_vyper.egg-info/PKG-INFO` & `ape-vyper-0.6.3/ape_vyper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.2
+Version: 0.6.3
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Description: # Quick Start
```

### Comparing `ape-vyper-0.6.2/ape_vyper.egg-info/SOURCES.txt` & `ape-vyper-0.6.3/ape_vyper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/pyproject.toml` & `ape-vyper-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/setup.py` & `ape-vyper-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=22.12.0",  # auto-formatter and linter
-        "mypy>=0.991",  # Static type analyzer
+        "black>=23.3.0,<24",  # Auto-formatter and linter
+        "mypy>=0.991,<1",  # Static type analyzer
         "types-setuptools",  # Needed due to mypy typeshed
-        "flake8>=5.0.4",  # Style linter
+        "flake8>=6.0.0,<7",  # Style linter
         "isort>=5.10.1",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
@@ -53,16 +53,16 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-vyper",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.4,<0.7",
-        "ethpm-types",  # Use same version as eth-ape
+        "eth-ape>=0.6.8,<0.7",
+        "ethpm-types>=0.4.3",  # Use same version as eth-ape
         "tqdm",  # Use same version as eth-ape
         "vvm>=0.1.0,<0.2",
     ],
     python_requires=">=3.8,<3.11",
     extras_require=extras_require,
     py_modules=["ape_vyper"],
     license="Apache-2.0",
```

### Comparing `ape-vyper-0.6.2/tests/conftest.py` & `ape-vyper-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.2/tests/test_compiler.py` & `ape-vyper-0.6.3/tests/test_compiler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from pathlib import Path
 from typing import List
 
 import pytest
+from ape.exceptions import ContractLogicError
 from semantic_version import Version  # type: ignore
 from vvm import compile_source  # type: ignore
 from vvm.exceptions import VyperError  # type: ignore
 
-from ape_vyper.exceptions import VyperCompileError, VyperInstallError
+from ape_vyper.compiler import RuntimeErrorType
+from ape_vyper.exceptions import NonPayableError, VyperCompileError, VyperInstallError
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "contracts"
 PASSING_BASE = BASE_CONTRACTS_PATH / "passing_contracts"
 FAILING_BASE = BASE_CONTRACTS_PATH / "failing_contracts"
 
 # Currently, this is the only version specified from a pragma spec
 OLDER_VERSION_FROM_PRAGMA = Version("0.2.8")
@@ -18,14 +20,24 @@
 
 
 @pytest.fixture
 def dev_revert_source():
     return PASSING_BASE / "contract_with_dev_messages.vy"
 
 
+@pytest.fixture
+def contract_logic_error():
+    err = ContractLogicError()
+
+    # Inject cached PC message so no need to have tracing provider.
+    err.__dict__["dev_message"] = f"dev: {RuntimeErrorType.NONPAYABLE_CHECK.value}"
+
+    return err
+
+
 def contract_test_cases(passing: bool) -> List[str]:
     """
     Returns test-case names for outputting nicely with pytest.
     """
     suffix = "passing_contracts" if passing else "failing_contracts"
     return [p.name for p in (BASE_CONTRACTS_PATH / suffix).glob("*.vy") if p.is_file()]
 
@@ -165,9 +177,31 @@
     """
 
     path = PASSING_BASE / "contract.vy"
     result = compiler.compile([path], base_path=PASSING_BASE)[0]
     actual = result.pcmap.__root__
     code = path.read_text()
     src_map = compile_source(code)["<stdin>"]["source_map"]
-    expected = src_map["pc_pos_map"]
+
+    def item(dev: RuntimeErrorType, location=None):
+        return {"dev": f"dev: {dev.value}", "location": location}
+
+    expected = {pc: {"location": ln} for pc, ln in src_map["pc_pos_map"].items()}
+    expected["23"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
+    expected["52"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
+    expected["73"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
+    expected["94"] = item(RuntimeErrorType.INTEGER_OVERFLOW, [14, 12, 14, 20])
+    expected["151"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
+    expected["188"] = item(RuntimeErrorType.INTEGER_UNDERFLOW, [19, 11, 19, 25])
+    expected["229"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
+    expected["249"] = item(RuntimeErrorType.DIVISION_BY_ZERO, [24, 11, 24, 16])
+    expected["288"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
+    expected["308"] = item(RuntimeErrorType.MODULO_BY_ZERO, [29, 11, 29, 16])
+    expected["351"] = item(RuntimeErrorType.INDEX_OUT_OF_RANGE, [34, 11, 34, 24])
+    expected["392"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
+    expected["405"] = item(RuntimeErrorType.NONPAYABLE_CHECK)
     assert actual == expected
+
+
+def test_enrich_error(contract_logic_error, compiler):
+    actual = compiler.enrich_error(contract_logic_error)
+    assert isinstance(actual, NonPayableError)
```

