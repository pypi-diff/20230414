# Comparing `tmp/onefuzz-7.0.0.tar.gz` & `tmp/onefuzz-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\onefuzz-7.0.0.tar", last modified: Tue Mar 21 20:49:48 2023, max compression
+gzip compressed data, was "dist\onefuzz-8.0.0.tar", last modified: Wed Apr 12 01:46:38 2023, max compression
```

## Comparing `onefuzz-7.0.0.tar` & `onefuzz-8.0.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/
--rw-rw-rw-   0        0        0     1162 2023-03-21 20:48:33.000000 onefuzz-7.0.0/LICENSE
--rw-rw-rw-   0        0        0      162 2023-03-21 20:48:33.000000 onefuzz-7.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2335 2023-03-21 20:49:48.000000 onefuzz-7.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-03-21 20:48:33.000000 onefuzz-7.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/examples/
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/examples/azure-functions-example/
--rw-rw-rw-   0        0        0      297 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/azure-functions-example/README.md
--rw-rw-rw-   0        0        0      141 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/azure-functions-example/host.json
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/examples/azure-functions-example/info/
--rw-rw-rw-   0        0        0      512 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/azure-functions-example/info/__init__.py
--rw-rw-rw-   0        0        0      319 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/azure-functions-example/info/function.json
--rw-rw-rw-   0        0        0       64 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/azure-functions-example/requirements.txt
--rw-rw-rw-   0        0        0     7557 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/domato.py
--rw-rw-rw-   0        0        0      773 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/get-running.py
--rw-rw-rw-   0        0        0     4649 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/honggfuzz.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/examples/llvm-source-coverage/
--rw-rw-rw-   0        0        0       41 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/llvm-source-coverage/.gitignore
--rw-rw-rw-   0        0        0     7347 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/llvm-source-coverage/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/examples/llvm-source-coverage/inputs/
--rw-rw-rw-   0        0        0        4 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/llvm-source-coverage/inputs/input.txt
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/examples/llvm-source-coverage/setup/
--rw-rw-rw-   0        0        0      398 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/llvm-source-coverage/setup/Makefile
--rw-rw-rw-   0        0        0     1556 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/llvm-source-coverage/setup/simple.c
--rw-rw-rw-   0        0        0     3277 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
--rw-rw-rw-   0        0        0     2963 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/llvm-source-coverage/source-coverage.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/examples/llvm-source-coverage/tools/
--rw-rw-rw-   0        0        0     1177 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/llvm-source-coverage/tools/source-coverage.sh
--rw-rw-rw-   0        0        0     2800 2023-03-21 20:48:33.000000 onefuzz-7.0.0/examples/oss-fuzz-target.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/extra/
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/extra/pyinstaller/
--rw-rw-rw-   0        0        0      200 2023-03-21 20:48:33.000000 onefuzz-7.0.0/extra/pyinstaller/hook-onefuzz.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz/
--rw-rw-rw-   0        0        0      129 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/__init__.py
--rw-rw-rw-   0        0        0      431 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/__main__.py
--rw-rw-rw-   0        0        0      126 2023-03-21 20:48:34.000000 onefuzz-7.0.0/onefuzz/__version__.py
--rw-rw-rw-   0        0        0    67833 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/api.py
--rw-rw-rw-   0        0        0     1059 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/azcopy.py
--rw-rw-rw-   0        0        0     2982 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/azure_identity_credential_adapter.py
--rw-rw-rw-   0        0        0    22224 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/backend.py
--rw-rw-rw-   0        0        0    20501 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/cli.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz/data/
--rw-rw-rw-   0        0        0     1222 2023-03-21 20:49:47.000000 onefuzz-7.0.0/onefuzz/data/licenses.json
--rw-rw-rw-   0        0        0     1004 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/data/privacy.txt
--rw-rw-rw-   0        0        0    29481 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/debug.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz/job_templates/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/job_templates/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/job_templates/builder.py
--rw-rw-rw-   0        0        0     1723 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/job_templates/cache.py
--rw-rw-rw-   0        0        0     6161 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/job_templates/handlers.py
--rw-rw-rw-   0        0        0     3596 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/job_templates/job_monitor.py
--rw-rw-rw-   0        0        0     3159 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/job_templates/main.py
--rw-rw-rw-   0        0        0     1851 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/job_templates/manage.py
--rw-rw-rw-   0        0        0     1682 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/rdp.py
--rw-rw-rw-   0        0        0     3522 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/ssh.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz/status/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/status/__init__.py
--rw-rw-rw-   0        0        0    13902 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/status/cache.py
--rw-rw-rw-   0        0        0     5152 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/status/cmd.py
--rw-rw-rw-   0        0        0      905 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/status/raw.py
--rw-rw-rw-   0        0        0     1856 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/status/signalr.py
--rw-rw-rw-   0        0        0     3009 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/status/top.py
--rw-rw-rw-   0        0        0     6255 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/status/top_view.py
--rw-rw-rw-   0        0        0     2882 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/template.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz/templates/
--rw-rw-rw-   0        0        0    10491 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/templates/__init__.py
--rw-rw-rw-   0        0        0     6837 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/templates/afl.py
--rw-rw-rw-   0        0        0    39810 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/templates/libfuzzer.py
--rw-rw-rw-   0        0        0     8788 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/templates/ossfuzz.py
--rw-rw-rw-   0        0        0     9530 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/templates/radamsa.py
--rw-rw-rw-   0        0        0    10649 2023-03-21 20:48:33.000000 onefuzz-7.0.0/onefuzz/templates/regression.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1981 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      341 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-21 20:49:48.000000 onefuzz-7.0.0/onefuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2023-03-21 20:48:33.000000 onefuzz-7.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      101 2023-03-21 20:48:33.000000 onefuzz-7.0.0/requirements-lint.txt
--rw-rw-rw-   0        0        0      455 2023-03-21 20:48:35.000000 onefuzz-7.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-21 20:49:48.000000 onefuzz-7.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-03-21 20:48:33.000000 onefuzz-7.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 20:49:48.000000 onefuzz-7.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-21 20:48:33.000000 onefuzz-7.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-03-21 20:48:33.000000 onefuzz-7.0.0/tests/test_template_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/
+-rw-rw-rw-   0        0        0     1162 2023-04-12 01:46:00.000000 onefuzz-8.0.0/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-04-12 01:46:00.000000 onefuzz-8.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2335 2023-04-12 01:46:38.000000 onefuzz-8.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1742 2023-04-12 01:46:00.000000 onefuzz-8.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/azure-functions-example/
+-rw-rw-rw-   0        0        0      297 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/README.md
+-rw-rw-rw-   0        0        0      141 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/host.json
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/azure-functions-example/info/
+-rw-rw-rw-   0        0        0      391 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/info/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/info/function.json
+-rw-rw-rw-   0        0        0       57 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/requirements.txt
+-rw-rw-rw-   0        0        0     7557 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/domato.py
+-rw-rw-rw-   0        0        0      773 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/get-running.py
+-rw-rw-rw-   0        0        0     4649 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/honggfuzz.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/llvm-source-coverage/
+-rw-rw-rw-   0        0        0       41 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/.gitignore
+-rw-rw-rw-   0        0        0     7347 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/README.md
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/llvm-source-coverage/inputs/
+-rw-rw-rw-   0        0        0        4 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/inputs/input.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/llvm-source-coverage/setup/
+-rw-rw-rw-   0        0        0      398 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/setup/Makefile
+-rw-rw-rw-   0        0        0     1556 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/setup/simple.c
+-rw-rw-rw-   0        0        0     3277 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
+-rw-rw-rw-   0        0        0     2963 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/source-coverage.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/llvm-source-coverage/tools/
+-rw-rw-rw-   0        0        0     1177 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/tools/source-coverage.sh
+-rw-rw-rw-   0        0        0     2800 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/oss-fuzz-target.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/extra/
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/extra/pyinstaller/
+-rw-rw-rw-   0        0        0      200 2023-04-12 01:46:00.000000 onefuzz-8.0.0/extra/pyinstaller/hook-onefuzz.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/
+-rw-rw-rw-   0        0        0      129 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/__main__.py
+-rw-rw-rw-   0        0        0      126 2023-04-12 01:46:01.000000 onefuzz-8.0.0/onefuzz/__version__.py
+-rw-rw-rw-   0        0        0    67292 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/api.py
+-rw-rw-rw-   0        0        0     1059 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/azcopy.py
+-rw-rw-rw-   0        0        0     2982 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/azure_identity_credential_adapter.py
+-rw-rw-rw-   0        0        0    22112 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/backend.py
+-rw-rw-rw-   0        0        0    20501 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/cli.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/data/
+-rw-rw-rw-   0        0        0     1223 2023-04-12 01:46:37.000000 onefuzz-8.0.0/onefuzz/data/licenses.json
+-rw-rw-rw-   0        0        0     1004 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/data/privacy.txt
+-rw-rw-rw-   0        0        0    29481 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/debug.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/job_templates/
+-rw-rw-rw-   0        0        0        0 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/__init__.py
+-rw-rw-rw-   0        0        0     4095 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/builder.py
+-rw-rw-rw-   0        0        0     1723 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/cache.py
+-rw-rw-rw-   0        0        0     6161 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/handlers.py
+-rw-rw-rw-   0        0        0     3596 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/job_monitor.py
+-rw-rw-rw-   0        0        0     3159 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/main.py
+-rw-rw-rw-   0        0        0     1851 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/manage.py
+-rw-rw-rw-   0        0        0     1682 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/rdp.py
+-rw-rw-rw-   0        0        0     3522 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/ssh.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/status/
+-rw-rw-rw-   0        0        0        0 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/cache.py
+-rw-rw-rw-   0        0        0     5152 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/cmd.py
+-rw-rw-rw-   0        0        0      905 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/raw.py
+-rw-rw-rw-   0        0        0     1856 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/signalr.py
+-rw-rw-rw-   0        0        0     3009 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/top.py
+-rw-rw-rw-   0        0        0     6255 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/top_view.py
+-rw-rw-rw-   0        0        0     2882 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/template.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/templates/
+-rw-rw-rw-   0        0        0    10491 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/__init__.py
+-rw-rw-rw-   0        0        0     6837 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/afl.py
+-rw-rw-rw-   0        0        0    40759 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/libfuzzer.py
+-rw-rw-rw-   0        0        0     8788 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/ossfuzz.py
+-rw-rw-rw-   0        0        0     9530 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/radamsa.py
+-rw-rw-rw-   0        0        0    10649 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/regression.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1981 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      344 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2023-04-12 01:46:00.000000 onefuzz-8.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      101 2023-04-12 01:46:00.000000 onefuzz-8.0.0/requirements-lint.txt
+-rw-rw-rw-   0        0        0      458 2023-04-12 01:46:01.000000 onefuzz-8.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 01:46:38.000000 onefuzz-8.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-04-12 01:46:00.000000 onefuzz-8.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-12 01:46:00.000000 onefuzz-8.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-12 01:46:00.000000 onefuzz-8.0.0/tests/test_template_helper.py
```

### Comparing `onefuzz-7.0.0/LICENSE` & `onefuzz-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/PKG-INFO` & `onefuzz-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 7.0.0
+Version: 8.0.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-7.0.0/README.md` & `onefuzz-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/domato.py` & `onefuzz-8.0.0/examples/domato.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/get-running.py` & `onefuzz-8.0.0/examples/get-running.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/honggfuzz.py` & `onefuzz-8.0.0/examples/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/llvm-source-coverage/README.md` & `onefuzz-8.0.0/examples/llvm-source-coverage/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/llvm-source-coverage/setup/simple.c` & `onefuzz-8.0.0/examples/llvm-source-coverage/setup/simple.c`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py` & `onefuzz-8.0.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/llvm-source-coverage/source-coverage.py` & `onefuzz-8.0.0/examples/llvm-source-coverage/source-coverage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/llvm-source-coverage/tools/source-coverage.sh` & `onefuzz-8.0.0/examples/llvm-source-coverage/tools/source-coverage.sh`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/examples/oss-fuzz-target.py` & `onefuzz-8.0.0/examples/oss-fuzz-target.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/api.py` & `onefuzz-8.0.0/onefuzz/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,15 @@
 from .__version__ import __version__
 from .azcopy import azcopy_sync
 from .backend import Backend, BackendConfig, ContainerWrapper, wait
 from .ssh import build_ssh_command, ssh_connect, temp_file
 
 UUID_EXPANSION = TypeVar("UUID_EXPANSION", UUID, str)
 
-DEFAULT = BackendConfig(
-    authority="",
-    client_id="",
-    tenant_domain="",
-)
+DEFAULT = BackendConfig(endpoint="")
 
 # This was generated randomly and should be preserved moving forwards
 ONEFUZZ_GUID_NAMESPACE = uuid.UUID("27f25e3f-6544-4b69-b309-9b096c5a9cbc")
 
 ONE_HOUR_IN_SECONDS = 3600
 
 REPRO_SSH_FORWARD = "1337:127.0.0.1:1337"
@@ -1306,15 +1302,15 @@
 
         pool = self.get(pool_name)
 
         if pool.config is None:
             raise Exception("Missing AgentConfig in response")
 
         config = pool.config
-        if not pool.managed:
+        if not pool.managed and self.onefuzz._backend.config.authority:
             config.client_credentials = models.ClientCredentials(  # nosec
                 client_id=uuid.UUID(int=0),
                 client_secret="<client_secret>",
                 resource=self.onefuzz._backend.config.endpoint,
                 tenant=urlparse(self.onefuzz._backend.config.authority).path.strip("/"),
                 multi_tenant_domain=self.onefuzz._backend.config.get_multi_tenant_domain(),
             )
@@ -1890,27 +1886,22 @@
         self.info.get()
 
         return "succeeded"
 
     def config(
         self,
         endpoint: Optional[str] = None,
-        override_authority: Optional[str] = None,
-        client_id: Optional[str] = None,
-        override_tenant_domain: Optional[str] = None,
         enable_feature: Optional[PreviewFeature] = None,
         reset: Optional[bool] = None,
     ) -> BackendConfig:
         """Configure onefuzz CLI"""
         self.logger.debug("set config")
 
         if reset:
-            self._backend.config = BackendConfig(
-                authority="", client_id="", tenant_domain=""
-            )
+            self._backend.config = BackendConfig(endpoint="")
 
         if endpoint is not None:
             # The normal path for calling the API always uses the oauth2 workflow,
             # which the devicelogin can take upwards of 15 minutes to fail in
             # error cases.
             #
             # This check only happens on setting the configuration, as checking the
@@ -1918,25 +1909,20 @@
             verify = self._backend.session.request("GET", endpoint)
             if verify.status_code != 401:
                 self.logger.warning(
                     "This could be an invalid OneFuzz API endpoint: "
                     "Missing HTTP Authentication"
                 )
             self._backend.config.endpoint = endpoint
-        if client_id is not None:
-            self._backend.config.client_id = client_id
-        if override_authority is not None:
-            self._backend.config.authority = override_authority
+
         if enable_feature:
             self._backend.enable_feature(enable_feature.name)
-        if override_tenant_domain is not None:
-            self._backend.config.tenant_domain = override_tenant_domain
+
         self._backend.app = None
         self._backend.save_config()
-
         data = self._backend.config.copy(deep=True)
 
         if not data.endpoint:
             self.logger.warning("endpoint not configured yet")
 
         return data
```

### Comparing `onefuzz-7.0.0/onefuzz/azcopy.py` & `onefuzz-8.0.0/onefuzz/azcopy.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/azure_identity_credential_adapter.py` & `onefuzz-8.0.0/onefuzz/azure_identity_credential_adapter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/backend.py` & `onefuzz-8.0.0/onefuzz/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import json
 import logging
 import os
 import sys
 import tempfile
 import time
 from dataclasses import asdict, is_dataclass
-from datetime import datetime, timedelta
 from enum import Enum
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     List,
@@ -29,15 +28,15 @@
 from urllib.parse import urlparse, urlunparse
 from uuid import UUID
 
 import msal
 import requests
 from azure.storage.blob import ContainerClient
 from onefuzztypes import responses
-from pydantic import BaseModel, Field
+from pydantic import BaseModel
 from requests import Response
 from tenacity import RetryCallState, retry
 from tenacity.retry import retry_if_exception_type
 from tenacity.stop import stop_after_attempt
 from tenacity.wait import wait_random
 
 from .azcopy import azcopy_copy, azcopy_sync
@@ -89,28 +88,34 @@
                     f"request failed: application error (401: {as_json['title']}): {as_json['detail']}"
                 )
         except json.decoder.JSONDecodeError:
             pass
 
 
 class BackendConfig(BaseModel):
-    authority: str
-    client_id: str
-    endpoint: Optional[str]
-    features: Set[str] = Field(default_factory=set)
-    tenant_domain: str
-    expires_on: datetime = datetime.utcnow() + timedelta(hours=24)
+    authority: Optional[str]
+    client_id: Optional[str]
+    endpoint: str
+    features: Optional[Set[str]]
+    tenant_domain: Optional[str]
 
     def get_multi_tenant_domain(self) -> Optional[str]:
-        if "https://login.microsoftonline.com/common" in self.authority:
+        if (
+            self.authority
+            and "https://login.microsoftonline.com/common" in self.authority
+        ):
             return self.tenant_domain
         else:
             return None
 
 
+class CacheConfig(BaseModel):
+    endpoint: Optional[str]
+
+
 class Backend:
     def __init__(
         self,
         config: BackendConfig,
         config_path: Optional[str] = None,
         token_path: Optional[str] = None,
         client_secret: Optional[str] = None,
@@ -125,29 +130,34 @@
         self.token_expires = 0
         self.load_config()
         self.session = requests.Session()
 
         atexit.register(self.save_cache)
 
     def enable_feature(self, name: str) -> None:
+        if not self.config.features:
+            self.config.features = Set[str]()
         self.config.features.add(name)
 
     def is_feature_enabled(self, name: str) -> bool:
-        return name in self.config.features
+        if self.config.features:
+            return name in self.config.features
+        return False
 
     def load_config(self) -> None:
         if os.path.exists(self.config_path):
             with open(self.config_path, "r") as handle:
                 data = json.load(handle)
             self.config = BackendConfig.parse_obj(data)
 
     def save_config(self) -> None:
         os.makedirs(os.path.dirname(self.config_path), exist_ok=True)
         with open(self.config_path, "w") as handle:
-            handle.write(self.config.json(indent=4, exclude_none=True))
+            endpoint_cache = {"endpoint": f"{self.config.endpoint}"}
+            handle.write(json.dumps(endpoint_cache, indent=4, sort_keys=True))
 
     def init_cache(self) -> None:
         # Ensure the token_path directory exists
         try:
             dir_name = os.path.dirname(self.token_path)
             with _temporary_umask(_ACCESSTOKENCACHE_UMASK):
                 os.makedirs(dir_name)
@@ -327,47 +337,37 @@
         endpoint = self.config.endpoint
 
         response = self.session.request("GET", endpoint + "/api/config")
 
         endpoint_params = responses.Config.parse_obj(response.json())
 
         # Will override values in storage w/ provided values for SP use
-        if self.config.client_id == "":
+        if not self.config.client_id:
             self.config.client_id = endpoint_params.client_id
-        if self.config.authority == "":
+        if not self.config.authority:
             self.config.authority = endpoint_params.authority
-        if self.config.tenant_domain == "":
+        if not self.config.tenant_domain:
             self.config.tenant_domain = endpoint_params.tenant_domain
 
-        self.save_config()
-
     def request(
         self,
         method: str,
         path: str,
         json_data: Optional[Any] = None,
         params: Optional[Any] = None,
         _retry_on_auth_failure: bool = True,
     ) -> Response:
         endpoint = self.config.endpoint
 
         if not endpoint:
             raise Exception("endpoint not configured")
 
-        # If file expires, remove and force user to reset
-        if datetime.utcnow() > self.config.expires_on:
-            os.remove(self.config_path)
-            self.config = BackendConfig(
-                endpoint=endpoint, authority="", client_id="", tenant_domain=""
-            )
-
         url = endpoint + "/api/" + path
-
-        if self.config.client_id == "" or (
-            self.config.authority == "" and self.config.tenant_domain == ""
+        if not self.config.client_id or (
+            not self.config.authority and not self.config.tenant_domain
         ):
             self.config_params()
         headers = self.headers()
         json_data = serialize(json_data)
 
         # 401 errors with IDX10501: Signature validation failed occur
         # on rolling new oauth2 client secrets
```

### Comparing `onefuzz-7.0.0/onefuzz/cli.py` & `onefuzz-8.0.0/onefuzz/cli.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/data/licenses.json` & `onefuzz-8.0.0/onefuzz/data/licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.953125%*

 * *Differences: {'1': "{'Version': '6.3.0'}", '3': "{'Version': '5.10.0'}", '4': "{'Version': '2023.2'}"}*

```diff
@@ -5,33 +5,33 @@
         "URL": "https://altgraph.readthedocs.io",
         "Version": "0.17.3"
     },
     {
         "License": "Apache Software License",
         "Name": "importlib-metadata",
         "URL": "https://github.com/python/importlib_metadata",
-        "Version": "6.1.0"
+        "Version": "6.3.0"
     },
     {
         "License": "MIT",
         "Name": "pefile",
         "URL": "https://github.com/erocarrera/pefile",
         "Version": "2023.2.7"
     },
     {
         "License": "GNU General Public License v2 (GPLv2)",
         "Name": "pyinstaller",
         "URL": "https://www.pyinstaller.org/",
-        "Version": "5.9.0"
+        "Version": "5.10.0"
     },
     {
         "License": "UNKNOWN",
         "Name": "pyinstaller-hooks-contrib",
         "URL": "https://github.com/pyinstaller/pyinstaller-hooks-contrib",
-        "Version": "2023.1"
+        "Version": "2023.2"
     },
     {
         "License": "BSD",
         "Name": "pywin32-ctypes",
         "URL": "https://github.com/enthought/pywin32-ctypes",
         "Version": "0.2.0"
     },
```

### Comparing `onefuzz-7.0.0/onefuzz/data/privacy.txt` & `onefuzz-8.0.0/onefuzz/data/privacy.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/debug.py` & `onefuzz-8.0.0/onefuzz/debug.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/job_templates/builder.py` & `onefuzz-8.0.0/onefuzz/job_templates/builder.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/job_templates/cache.py` & `onefuzz-8.0.0/onefuzz/job_templates/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/job_templates/handlers.py` & `onefuzz-8.0.0/onefuzz/job_templates/handlers.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/job_templates/job_monitor.py` & `onefuzz-8.0.0/onefuzz/job_templates/job_monitor.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/job_templates/main.py` & `onefuzz-8.0.0/onefuzz/job_templates/main.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/job_templates/manage.py` & `onefuzz-8.0.0/onefuzz/job_templates/manage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/rdp.py` & `onefuzz-8.0.0/onefuzz/rdp.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/ssh.py` & `onefuzz-8.0.0/onefuzz/ssh.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/status/cache.py` & `onefuzz-8.0.0/onefuzz/status/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/status/cmd.py` & `onefuzz-8.0.0/onefuzz/status/cmd.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/status/raw.py` & `onefuzz-8.0.0/onefuzz/status/raw.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/status/signalr.py` & `onefuzz-8.0.0/onefuzz/status/signalr.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/status/top.py` & `onefuzz-8.0.0/onefuzz/status/top.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/status/top_view.py` & `onefuzz-8.0.0/onefuzz/status/top_view.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/template.py` & `onefuzz-8.0.0/onefuzz/template.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/templates/__init__.py` & `onefuzz-8.0.0/onefuzz/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/templates/afl.py` & `onefuzz-8.0.0/onefuzz/templates/afl.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/templates/libfuzzer.py` & `onefuzz-8.0.0/onefuzz/templates/libfuzzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,14 +324,15 @@
         *,
         target_exe: File = File("fuzz.exe"),
         setup_dir: Optional[Directory] = None,
         vm_count: int = 2,
         inputs: Optional[Directory] = None,
         reboot_after_setup: bool = False,
         duration: int = 24,
+        task_duration: Optional[int] = None,
         target_workers: Optional[int] = None,
         target_options: Optional[List[str]] = None,
         fuzzing_target_options: Optional[List[str]] = None,
         target_env: Optional[Dict[str, str]] = None,
         target_timeout: Optional[int] = None,
         check_retry_count: Optional[int] = None,
         crash_report_timeout: Optional[int] = None,
@@ -353,14 +354,15 @@
         module_allowlist: Optional[File] = None,
         source_allowlist: Optional[File] = None,
         analyzer_exe: Optional[str] = None,
         analyzer_options: Optional[List[str]] = None,
         analyzer_env: Optional[Dict[str, str]] = None,
         tools: Optional[Container] = None,
         extra_container: Optional[Container] = None,
+        crashes: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         Basic libfuzzer job
 
         :param bool ensemble_sync_delay: Specify duration between
             syncing inputs during ensemble fuzzing (0 to disable).
         """
@@ -368,14 +370,17 @@
         # verify containers exist
         if existing_inputs:
             self.onefuzz.containers.get(existing_inputs)
 
         if readonly_inputs:
             self.onefuzz.containers.get(readonly_inputs)
 
+        if crashes:
+            self.onefuzz.containers.get(crashes)
+
         if dryrun:
             return None
 
         self.logger.info("creating libfuzzer from template")
 
         self._check_is_libfuzzer(target_exe)
 
@@ -408,14 +413,17 @@
             helper.containers[ContainerType.inputs] = existing_inputs
         else:
             helper.define_containers(ContainerType.inputs)
 
         if readonly_inputs:
             helper.containers[ContainerType.readonly_inputs] = readonly_inputs
 
+        if crashes:
+            helper.containers[ContainerType.crashes] = crashes
+
         if analyzer_exe is not None:
             helper.define_containers(ContainerType.analysis)
 
         helper.create_containers()
         helper.setup_notifications(notification_config)
 
         helper.upload_setup(setup_dir, target_exe, extra_files)
@@ -447,15 +455,15 @@
         self._create_tasks(
             job=helper.job,
             containers=containers,
             pool_name=pool_name,
             target_exe=target_exe_blob_name,
             vm_count=vm_count,
             reboot_after_setup=reboot_after_setup,
-            duration=duration,
+            duration=task_duration if task_duration else duration,
             target_workers=target_workers,
             target_options=target_options,
             fuzzing_target_options=fuzzing_target_options,
             target_env=target_env,
             tags=helper.tags,
             crash_report_timeout=crash_report_timeout,
             check_retry_count=check_retry_count,
@@ -614,14 +622,15 @@
         target_dll: File,
         target_class: str,
         target_method: str,
         vm_count: int = 1,
         inputs: Optional[Directory] = None,
         reboot_after_setup: bool = False,
         duration: int = 24,
+        task_duration: Optional[int] = None,
         target_workers: Optional[int] = None,
         fuzzing_target_options: Optional[List[str]] = None,
         target_env: Optional[Dict[str, str]] = None,
         target_timeout: Optional[int] = None,
         check_retry_count: Optional[int] = None,
         tags: Optional[Dict[str, str]] = None,
         wait_for_running: bool = False,
@@ -631,24 +640,28 @@
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         colocate_secondary_tasks: bool = True,
         expect_crash_on_failure: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         extra_container: Optional[Container] = None,
+        crashes: Optional[Container] = None,
     ) -> Optional[Job]:
         pool = self.onefuzz.pools.get(pool_name)
 
         # verify containers exist
         if existing_inputs:
             self.onefuzz.containers.get(existing_inputs)
 
         if readonly_inputs:
             self.onefuzz.containers.get(readonly_inputs)
 
+        if crashes:
+            self.onefuzz.containers.get(crashes)
+
         # We _must_ proactively specify the OS based on pool.
         #
         # This is because managed DLLs are always (Windows-native) PE files, so the job
         # helper's platform guess (based on the file type of `target_exe`) will always
         # evaluate to `OS.windows`. In the case of true Linux `libfuzzer dotnet_dll` jobs,
         # this leads to a client- side validation error when the helper checks the nominal
         # target OS against the pool OS.
@@ -694,14 +707,17 @@
             helper.containers[ContainerType.inputs] = existing_inputs
         else:
             helper.define_containers(ContainerType.inputs)
 
         if readonly_inputs:
             helper.containers[ContainerType.readonly_inputs] = readonly_inputs
 
+        if crashes:
+            helper.containers[ContainerType.crashes] = crashes
+
         # Assumes that `libfuzzer-dotnet` and supporting tools were uploaded upon deployment.
         fuzzer_tools_container = Container(
             "dotnet-fuzzing-linux" if platform == OS.linux else "dotnet-fuzzing-windows"
         )
 
         fuzzer_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
@@ -726,15 +742,15 @@
         fuzzer_task = self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.libfuzzer_dotnet_fuzz,
             target_dll_blob_name,  # Not used
             fuzzer_containers,
             pool_name=pool_name,
             reboot_after_setup=reboot_after_setup,
-            duration=duration,
+            duration=task_duration if task_duration else duration,
             vm_count=vm_count,
             target_options=fuzzing_target_options,
             target_env=target_env,
             target_assembly=target_dll_blob_name,
             target_class=target_class,
             target_method=target_method,
             target_workers=target_workers,
@@ -774,15 +790,15 @@
         self.logger.info("creating `dotnet_coverage` task")
         self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.dotnet_coverage,
             libfuzzer_dotnet_loader_dll,
             coverage_containers,
             pool_name=pool_name,
-            duration=duration,
+            duration=task_duration if task_duration else duration,
             vm_count=1,
             reboot_after_setup=reboot_after_setup,
             target_options=sharpfuzz_harness_target_options,
             target_env=target_env,
             target_timeout=target_timeout,
             tags=tags,
             prereq_tasks=prereq_tasks,
@@ -805,15 +821,15 @@
         self.logger.info("creating `dotnet_crash_report` task")
         self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.dotnet_crash_report,
             libfuzzer_dotnet_loader_dll,
             report_containers,
             pool_name=pool_name,
-            duration=duration,
+            duration=task_duration if task_duration else duration,
             vm_count=1,
             reboot_after_setup=reboot_after_setup,
             target_options=sharpfuzz_harness_target_options,
             target_env=target_env,
             tags=tags,
             prereq_tasks=prereq_tasks,
             target_timeout=target_timeout,
@@ -836,14 +852,15 @@
         arch: QemuArch = QemuArch.aarch64,
         target_exe: File = File("fuzz.exe"),
         sysroot: Optional[File] = None,
         vm_count: int = 1,
         inputs: Optional[Directory] = None,
         reboot_after_setup: bool = False,
         duration: int = 24,
+        task_duration: Optional[int] = None,
         target_workers: Optional[int] = 1,
         target_options: Optional[List[str]] = None,
         fuzzing_target_options: Optional[List[str]] = None,
         target_env: Optional[Dict[str, str]] = None,
         tags: Optional[Dict[str, str]] = None,
         wait_for_running: bool = False,
         wait_for_files: Optional[List[ContainerType]] = None,
@@ -851,14 +868,15 @@
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         crash_report_timeout: Optional[int] = 1,
         check_retry_count: Optional[int] = 300,
         check_fuzzer_help: bool = True,
         extra_container: Optional[Container] = None,
+        crashes: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         libfuzzer tasks, wrapped via qemu-user (PREVIEW FEATURE)
         """
 
         self.logger.warning(
             "qemu_user jobs are a preview feature and may change in the future"
@@ -903,14 +921,18 @@
 
         if existing_inputs:
             self.onefuzz.containers.get(existing_inputs)
             helper.containers[ContainerType.inputs] = existing_inputs
         else:
             helper.define_containers(ContainerType.inputs)
 
+        if crashes:
+            self.onefuzz.containers.get(crashes)
+            helper.containers[ContainerType.crashes] = crashes
+
         fuzzer_containers = [
             (ContainerType.setup, helper.containers[ContainerType.setup]),
             (ContainerType.crashes, helper.containers[ContainerType.crashes]),
             (ContainerType.inputs, helper.containers[ContainerType.inputs]),
         ]
 
         if extra_container is not None:
@@ -982,15 +1004,15 @@
         fuzzer_task = self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.libfuzzer_fuzz,
             wrapper_name,
             fuzzer_containers,
             pool_name=pool_name,
             reboot_after_setup=reboot_after_setup,
-            duration=duration,
+            duration=task_duration if task_duration else duration,
             vm_count=vm_count,
             target_options=libfuzzer_fuzz_target_options,
             target_env=target_env,
             target_workers=target_workers,
             tags=tags,
             debug=debug,
             ensemble_sync_delay=ensemble_sync_delay,
@@ -1015,15 +1037,15 @@
         self.logger.info("creating libfuzzer_crash_report task")
         self.onefuzz.tasks.create(
             helper.job.job_id,
             TaskType.libfuzzer_crash_report,
             wrapper_name,
             report_containers,
             pool_name=pool_name,
-            duration=duration,
+            duration=task_duration if task_duration else duration,
             vm_count=1,
             reboot_after_setup=reboot_after_setup,
             target_options=target_options,
             target_env=target_env,
             tags=tags,
             prereq_tasks=[fuzzer_task.task_id],
             target_timeout=crash_report_timeout,
```

### Comparing `onefuzz-7.0.0/onefuzz/templates/ossfuzz.py` & `onefuzz-8.0.0/onefuzz/templates/ossfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/templates/radamsa.py` & `onefuzz-8.0.0/onefuzz/templates/radamsa.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz/templates/regression.py` & `onefuzz-8.0.0/onefuzz/templates/regression.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/onefuzz.egg-info/PKG-INFO` & `onefuzz-8.0.0/onefuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 7.0.0
+Version: 8.0.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-7.0.0/onefuzz.egg-info/SOURCES.txt` & `onefuzz-8.0.0/onefuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/setup.py` & `onefuzz-8.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzz-7.0.0/tests/test_template_helper.py` & `onefuzz-8.0.0/tests/test_template_helper.py`

 * *Files identical despite different names*

