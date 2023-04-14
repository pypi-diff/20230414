# Comparing `tmp/rubicon-objc-0.4.5rc1.tar.gz` & `tmp/rubicon-objc-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubicon-objc-0.4.5rc1.tar", last modified: Tue Jan 24 23:46:08 2023, max compression
+gzip compressed data, was "rubicon-objc-0.4.6.tar", last modified: Fri Apr 14 00:53:23 2023, max compression
```

## Comparing `rubicon-objc-0.4.5rc1.tar` & `rubicon-objc-0.4.6.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.848666 rubicon-objc-0.4.5rc1/
--rw-r--r--   0 runner     (501) staff       (20)       71 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.796531 rubicon-objc-0.4.5rc1/.github/
--rw-r--r--   0 runner     (501) staff       (20)      377 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.798735 rubicon-objc-0.4.5rc1/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     2991 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.github/workflows/ci.yml
--rw-r--r--   0 runner     (501) staff       (20)      230 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.github/workflows/dependabot-changenote.yml
--rw-r--r--   0 runner     (501) staff       (20)      513 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.github/workflows/publish.yml
--rw-r--r--   0 runner     (501) staff       (20)     1789 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.github/workflows/release.yml
--rw-r--r--   0 runner     (501) staff       (20)      151 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)     1156 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner     (501) staff       (20)      607 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.readthedocs.yml
--rw-r--r--   0 runner     (501) staff       (20)      842 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/.travis.yml
--rw-r--r--   0 runner     (501) staff       (20)      140 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/CHANGELOG.rst
--rw-r--r--   0 runner     (501) staff       (20)      181 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/CONTRIBUTING.md
--rw-r--r--   0 runner     (501) staff       (20)     3278 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      656 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     4682 2023-01-24 23:46:08.848918 rubicon-objc-0.4.5rc1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3397 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/README.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.799856 rubicon-objc-0.4.5rc1/changes/
--rw-r--r--   0 runner     (501) staff       (20)       12 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/changes/.gitignore
--rw-r--r--   0 runner     (501) staff       (20)      792 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/changes/template.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.802464 rubicon-objc-0.4.5rc1/docs/
--rw-r--r--   0 runner     (501) staff       (20)      728 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/Makefile
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.782984 rubicon-objc-0.4.5rc1/docs/_mocked_modules/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.803412 rubicon-objc-0.4.5rc1/docs/_mocked_modules/ctypes/
--rw-r--r--   0 runner     (501) staff       (20)    10469 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/_mocked_modules/ctypes/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      127 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/_mocked_modules/ctypes/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.783880 rubicon-objc-0.4.5rc1/docs/_static/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.804783 rubicon-objc-0.4.5rc1/docs/_static/images/
--rw-r--r--   0 runner     (501) staff       (20)    22360 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/_static/images/rubicon.png
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.808462 rubicon-objc-0.4.5rc1/docs/background/
--rw-r--r--   0 runner     (501) staff       (20)     1078 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/background/community.rst
--rw-r--r--   0 runner     (501) staff       (20)      826 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/background/faq.rst
--rw-r--r--   0 runner     (501) staff       (20)      245 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/background/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    25792 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/background/releases.rst
--rw-r--r--   0 runner     (501) staff       (20)       32 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/background/roadmap.rst
--rw-r--r--   0 runner     (501) staff       (20)      247 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/background/success.rst
--rw-r--r--   0 runner     (501) staff       (20)     8824 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/conf.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.814508 rubicon-objc-0.4.5rc1/docs/how-to/
--rw-r--r--   0 runner     (501) staff       (20)     3764 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/async.rst
--rw-r--r--   0 runner     (501) staff       (20)    20905 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/c-functions.rst
--rw-r--r--   0 runner     (501) staff       (20)     4908 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/contribute-code.rst
--rw-r--r--   0 runner     (501) staff       (20)     1001 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/contribute-docs.rst
--rw-r--r--   0 runner     (501) staff       (20)      487 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/get-started.rst
--rw-r--r--   0 runner     (501) staff       (20)      490 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/index.rst
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.816166 rubicon-objc-0.4.5rc1/docs/how-to/internal/
--rw-r--r--   0 runner     (501) staff       (20)      229 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/internal/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     4026 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/internal/release.rst
--rw-r--r--   0 runner     (501) staff       (20)     4691 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/memory-management.rst
--rw-r--r--   0 runner     (501) staff       (20)     3778 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/protocols.rst
--rw-r--r--   0 runner     (501) staff       (20)    14993 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/how-to/type-mapping.rst
--rw-r--r--   0 runner     (501) staff       (20)     1490 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/index.rst
--rw-r--r--   0 runner     (501) staff       (20)      932 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/make.bat
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.820250 rubicon-objc-0.4.5rc1/docs/reference/
--rw-r--r--   0 runner     (501) staff       (20)      448 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/reference/index.rst
--rw-r--r--   0 runner     (501) staff       (20)    19419 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc-api.rst
--rw-r--r--   0 runner     (501) staff       (20)      787 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc-eventloop.rst
--rw-r--r--   0 runner     (501) staff       (20)     5613 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc-runtime.rst
--rw-r--r--   0 runner     (501) staff       (20)    14527 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc-types.rst
--rw-r--r--   0 runner     (501) staff       (20)     3418 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc.rst
--rw-r--r--   0 runner     (501) staff       (20)      169 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/spelling_wordlist
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.822015 rubicon-objc-0.4.5rc1/docs/tutorial/
--rw-r--r--   0 runner     (501) staff       (20)      506 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/tutorial/index.rst
--rw-r--r--   0 runner     (501) staff       (20)     4379 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/tutorial/tutorial-1.rst
--rw-r--r--   0 runner     (501) staff       (20)     4790 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/docs/tutorial/tutorial-2.rst
--rw-r--r--   0 runner     (501) staff       (20)      494 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)     1696 2023-01-24 23:46:08.850085 rubicon-objc-0.4.5rc1/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.786335 rubicon-objc-0.4.5rc1/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.822592 rubicon-objc-0.4.5rc1/src/rubicon/
--rw-r--r--   0 runner     (501) staff       (20)      256 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/src/rubicon/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.827533 rubicon-objc-0.4.5rc1/src/rubicon/objc/
--rw-r--r--   0 runner     (501) staff       (20)     3490 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/src/rubicon/objc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    94582 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/src/rubicon/objc/api.py
--rw-r--r--   0 runner     (501) staff       (20)    13947 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/src/rubicon/objc/collections.py
--rw-r--r--   0 runner     (501) staff       (20)    10057 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/src/rubicon/objc/ctypes_patch.py
--rw-r--r--   0 runner     (501) staff       (20)    24603 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/src/rubicon/objc/eventloop.py
--rw-r--r--   0 runner     (501) staff       (20)    41952 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/src/rubicon/objc/runtime.py
--rw-r--r--   0 runner     (501) staff       (20)    29639 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/src/rubicon/objc/types.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.830647 rubicon-objc-0.4.5rc1/src/rubicon_objc.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     4682 2023-01-24 23:46:08.000000 rubicon-objc-0.4.5rc1/src/rubicon_objc.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2293 2023-01-24 23:46:08.000000 rubicon-objc-0.4.5rc1/src/rubicon_objc.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-01-24 23:46:08.000000 rubicon-objc-0.4.5rc1/src/rubicon_objc.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      281 2023-01-24 23:46:08.000000 rubicon-objc-0.4.5rc1/src/rubicon_objc.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2023-01-24 23:46:08.000000 rubicon-objc-0.4.5rc1/src/rubicon_objc.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.835550 rubicon-objc-0.4.5rc1/tests/
--rw-r--r--   0 runner     (501) staff       (20)      492 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-24 23:46:08.848210 rubicon-objc-0.4.5rc1/tests/objc/
--rw-r--r--   0 runner     (501) staff       (20)      567 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/BaseExample.h
--rw-r--r--   0 runner     (501) staff       (20)     1331 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/BaseExample.m
--rw-r--r--   0 runner     (501) staff       (20)      929 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Blocks.h
--rw-r--r--   0 runner     (501) staff       (20)     1239 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Blocks.m
--rw-r--r--   0 runner     (501) staff       (20)      264 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Callback.h
--rw-r--r--   0 runner     (501) staff       (20)      392 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/DescriptionTester.h
--rw-r--r--   0 runner     (501) staff       (20)      641 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/DescriptionTester.m
--rw-r--r--   0 runner     (501) staff       (20)     2531 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Example.h
--rw-r--r--   0 runner     (501) staff       (20)     4498 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Example.m
--rw-r--r--   0 runner     (501) staff       (20)      593 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Makefile
--rw-r--r--   0 runner     (501) staff       (20)      197 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Protocols.h
--rw-r--r--   0 runner     (501) staff       (20)      104 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/SpecificExample.h
--rw-r--r--   0 runner     (501) staff       (20)      394 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/SpecificExample.m
--rw-r--r--   0 runner     (501) staff       (20)      328 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Thing.h
--rw-r--r--   0 runner     (501) staff       (20)      711 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/objc/Thing.m
--rw-r--r--   0 runner     (501) staff       (20)    11896 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/test_NSArray.py
--rw-r--r--   0 runner     (501) staff       (20)    13232 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/test_NSDictionary.py
--rw-r--r--   0 runner     (501) staff       (20)    16384 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/test_NSString.py
--rw-r--r--   0 runner     (501) staff       (20)     5835 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/test_async.py
--rw-r--r--   0 runner     (501) staff       (20)     6330 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/test_blocks.py
--rw-r--r--   0 runner     (501) staff       (20)    64568 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/test_core.py
--rw-r--r--   0 runner     (501) staff       (20)     4333 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tests/test_ctypes_patch.py
--rw-r--r--   0 runner     (501) staff       (20)     1020 2023-01-24 23:45:10.000000 rubicon-objc-0.4.5rc1/tox.ini
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.655818 rubicon-objc-0.4.6/
+-rw-r--r--   0 runner     (501) staff       (20)       71 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.git-blame-ignore-revs
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.611498 rubicon-objc-0.4.6/.github/
+-rw-r--r--   0 runner     (501) staff       (20)      377 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.github/dependabot.yml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.613944 rubicon-objc-0.4.6/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     2030 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner     (501) staff       (20)      230 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.github/workflows/dependabot-changenote.yml
+-rw-r--r--   0 runner     (501) staff       (20)      257 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.github/workflows/pre-commit-update.yml
+-rw-r--r--   0 runner     (501) staff       (20)      704 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner     (501) staff       (20)     1863 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.github/workflows/release.yml
+-rw-r--r--   0 runner     (501) staff       (20)      158 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      685 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner     (501) staff       (20)      707 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.readthedocs.yml
+-rw-r--r--   0 runner     (501) staff       (20)      842 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/.travis.yml
+-rw-r--r--   0 runner     (501) staff       (20)      140 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/CHANGELOG.rst
+-rw-r--r--   0 runner     (501) staff       (20)      181 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/CONTRIBUTING.md
+-rw-r--r--   0 runner     (501) staff       (20)     3278 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      656 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     4679 2023-04-14 00:53:23.656062 rubicon-objc-0.4.6/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3397 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.614972 rubicon-objc-0.4.6/changes/
+-rw-r--r--   0 runner     (501) staff       (20)       12 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/changes/.gitignore
+-rw-r--r--   0 runner     (501) staff       (20)      792 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/changes/template.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.617354 rubicon-objc-0.4.6/docs/
+-rw-r--r--   0 runner     (501) staff       (20)      728 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/Makefile
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.601875 rubicon-objc-0.4.6/docs/_mocked_modules/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.618313 rubicon-objc-0.4.6/docs/_mocked_modules/ctypes/
+-rw-r--r--   0 runner     (501) staff       (20)    10469 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/_mocked_modules/ctypes/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      127 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/_mocked_modules/ctypes/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.602264 rubicon-objc-0.4.6/docs/_static/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.618863 rubicon-objc-0.4.6/docs/_static/images/
+-rw-r--r--   0 runner     (501) staff       (20)    22360 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/_static/images/rubicon.png
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.622015 rubicon-objc-0.4.6/docs/background/
+-rw-r--r--   0 runner     (501) staff       (20)     1045 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/background/community.rst
+-rw-r--r--   0 runner     (501) staff       (20)      826 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/background/faq.rst
+-rw-r--r--   0 runner     (501) staff       (20)      245 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/background/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)    25951 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/background/releases.rst
+-rw-r--r--   0 runner     (501) staff       (20)       18 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/background/roadmap.rst
+-rw-r--r--   0 runner     (501) staff       (20)      245 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/background/success.rst
+-rw-r--r--   0 runner     (501) staff       (20)     9621 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/conf.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.626502 rubicon-objc-0.4.6/docs/how-to/
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/async.rst
+-rw-r--r--   0 runner     (501) staff       (20)    20913 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/c-functions.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4898 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/contribute-code.rst
+-rw-r--r--   0 runner     (501) staff       (20)     2643 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/contribute-docs.rst
+-rw-r--r--   0 runner     (501) staff       (20)      487 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/get-started.rst
+-rw-r--r--   0 runner     (501) staff       (20)      490 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/index.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.627492 rubicon-objc-0.4.6/docs/how-to/internal/
+-rw-r--r--   0 runner     (501) staff       (20)      229 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/internal/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4097 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/internal/release.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4699 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/memory-management.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3778 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/protocols.rst
+-rw-r--r--   0 runner     (501) staff       (20)    15016 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/how-to/type-mapping.rst
+-rw-r--r--   0 runner     (501) staff       (20)     1490 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)      932 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/make.bat
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.630891 rubicon-objc-0.4.6/docs/reference/
+-rw-r--r--   0 runner     (501) staff       (20)      448 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/reference/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)    19449 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/reference/rubicon-objc-api.rst
+-rw-r--r--   0 runner     (501) staff       (20)      787 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/reference/rubicon-objc-eventloop.rst
+-rw-r--r--   0 runner     (501) staff       (20)     5613 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/reference/rubicon-objc-runtime.rst
+-rw-r--r--   0 runner     (501) staff       (20)    15157 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/reference/rubicon-objc-types.rst
+-rw-r--r--   0 runner     (501) staff       (20)     3418 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/reference/rubicon-objc.rst
+-rw-r--r--   0 runner     (501) staff       (20)      476 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/spelling_wordlist
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.632633 rubicon-objc-0.4.6/docs/tutorial/
+-rw-r--r--   0 runner     (501) staff       (20)      506 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/tutorial/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4383 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/tutorial/tutorial-1.rst
+-rw-r--r--   0 runner     (501) staff       (20)     4791 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/docs/tutorial/tutorial-2.rst
+-rw-r--r--   0 runner     (501) staff       (20)      494 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)     1794 2023-04-14 00:53:23.657286 rubicon-objc-0.4.6/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.604357 rubicon-objc-0.4.6/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.604107 rubicon-objc-0.4.6/src/rubicon/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.637136 rubicon-objc-0.4.6/src/rubicon/objc/
+-rw-r--r--   0 runner     (501) staff       (20)     3490 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/src/rubicon/objc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    94901 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/src/rubicon/objc/api.py
+-rw-r--r--   0 runner     (501) staff       (20)    13945 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/src/rubicon/objc/collections.py
+-rw-r--r--   0 runner     (501) staff       (20)    10057 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/src/rubicon/objc/ctypes_patch.py
+-rw-r--r--   0 runner     (501) staff       (20)    24338 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/src/rubicon/objc/eventloop.py
+-rw-r--r--   0 runner     (501) staff       (20)    42293 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/src/rubicon/objc/runtime.py
+-rw-r--r--   0 runner     (501) staff       (20)    29721 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/src/rubicon/objc/types.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.639937 rubicon-objc-0.4.6/src/rubicon_objc.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     4679 2023-04-14 00:53:23.000000 rubicon-objc-0.4.6/src/rubicon_objc.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2367 2023-04-14 00:53:23.000000 rubicon-objc-0.4.6/src/rubicon_objc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-14 00:53:23.000000 rubicon-objc-0.4.6/src/rubicon_objc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      361 2023-04-14 00:53:23.000000 rubicon-objc-0.4.6/src/rubicon_objc.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2023-04-14 00:53:23.000000 rubicon-objc-0.4.6/src/rubicon_objc.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.644840 rubicon-objc-0.4.6/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      492 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-14 00:53:23.655273 rubicon-objc-0.4.6/tests/objc/
+-rw-r--r--   0 runner     (501) staff       (20)      104 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Altered_Example.h
+-rw-r--r--   0 runner     (501) staff       (20)       85 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Altered_Example.m
+-rw-r--r--   0 runner     (501) staff       (20)      567 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/BaseExample.h
+-rw-r--r--   0 runner     (501) staff       (20)     1331 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/BaseExample.m
+-rw-r--r--   0 runner     (501) staff       (20)      929 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Blocks.h
+-rw-r--r--   0 runner     (501) staff       (20)     1239 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Blocks.m
+-rw-r--r--   0 runner     (501) staff       (20)      264 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Callback.h
+-rw-r--r--   0 runner     (501) staff       (20)      392 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/DescriptionTester.h
+-rw-r--r--   0 runner     (501) staff       (20)      641 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/DescriptionTester.m
+-rw-r--r--   0 runner     (501) staff       (20)     2558 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Example.h
+-rw-r--r--   0 runner     (501) staff       (20)     4767 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Example.m
+-rw-r--r--   0 runner     (501) staff       (20)      593 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)      197 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Protocols.h
+-rw-r--r--   0 runner     (501) staff       (20)      104 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/SpecificExample.h
+-rw-r--r--   0 runner     (501) staff       (20)      394 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/SpecificExample.m
+-rw-r--r--   0 runner     (501) staff       (20)      328 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Thing.h
+-rw-r--r--   0 runner     (501) staff       (20)      711 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/objc/Thing.m
+-rw-r--r--   0 runner     (501) staff       (20)    11896 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/test_NSArray.py
+-rw-r--r--   0 runner     (501) staff       (20)    13232 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/test_NSDictionary.py
+-rw-r--r--   0 runner     (501) staff       (20)    16384 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/test_NSString.py
+-rw-r--r--   0 runner     (501) staff       (20)     5835 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/test_async.py
+-rw-r--r--   0 runner     (501) staff       (20)     6330 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/test_blocks.py
+-rw-r--r--   0 runner     (501) staff       (20)    66335 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/test_core.py
+-rw-r--r--   0 runner     (501) staff       (20)     4333 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tests/test_ctypes_patch.py
+-rw-r--r--   0 runner     (501) staff       (20)     1999 2023-04-14 00:52:25.000000 rubicon-objc-0.4.6/tox.ini
```

### Comparing `rubicon-objc-0.4.5rc1/.github/workflows/ci.yml` & `rubicon-objc-0.4.6/.github/workflows/ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,75 @@
 name: CI
 on:
   pull_request:
   push:
     branches:
       - main
   workflow_call:
+    outputs:
+      artifact-name:
+        description: "Name of the uploaded artifact; use for artifact retrieval."
+        value: ${{ jobs.package.outputs.artifact-name }}
+
+# Cancel active CI runs for a PR before starting another run
+concurrency:
+  group: ${{ github.ref }}
+  cancel-in-progress: true
 
 jobs:
   pre-commit:
-    name: Pre-commit code style checks
-    runs-on: macos-latest
-    timeout-minutes: 10
-    steps:
-      - uses: actions/checkout@v3.3.0
-      - name: Set up Python
-        uses: actions/setup-python@v4.5.0
-        with:
-          python-version: "3.X"
-      - name: Lint with Pre-commit
-        uses: pre-commit/action@v3.0.0
+    name: Pre-commit checks
+    uses: beeware/.github/.github/workflows/pre-commit-run.yml@main
+    with:
+      runner-os: "macos-latest"
 
   towncrier:
-    runs-on: macos-latest
-    steps:
-    # Fetch main branch for comparison, then check out current branch.
-    - name: Check out main branch
-      uses: actions/checkout@v3.3.0
-      with:
-        fetch-depth: 0
-        ref: main
-    - name: Check out branch
-      uses: actions/checkout@v3.3.0
-      with:
-        fetch-depth: 0
-    - name: Set up Python
-      uses: actions/setup-python@v4.5.0
-      with:
-        python-version: "3.X"
-    - name: Install dev dependencies
-      run: |
-        # We don't actually want to install rubicon;
-        # we just want the dev etras so we have a known version of tox
-        python -m pip install -e .[dev]
-    - name: Run pre-test check
-      run: |
-        tox -e towncrier-check
+    name: Check towncrier
+    uses: beeware/.github/.github/workflows/towncrier-run.yml@main
+    with:
+      runner-os: "macos-latest"
 
   package:
-    runs-on: macos-latest
-    steps:
-    # Fetch all refs so setuptools_scm can generate the correct version number.
-    - uses: actions/checkout@v3.3.0
-      with:
-        fetch-depth: 0
-    - uses: actions/setup-python@v4.5.0
-      with:
-        python-version: "3.X"
-    - name: Install dev dependencies
-      run: |
-        # We don't actually want to install rubicon;
-        # we just want the dev extras so we have a known version of tox
-        python -m pip install -e .[dev]
-    - name: Build wheels
-      run: tox -e package
-    - uses: actions/upload-artifact@v3
-      with:
-        name: packages
-        path: dist
-        if-no-files-found: error
+    name: Python Package
+    uses: beeware/.github/.github/workflows/python-package-create.yml@main
+    with:
+      runner-os: "macos-latest"
 
   unit-tests:
     name: Unit tests
     needs: [pre-commit, towncrier, package]
+    runs-on: ${{ matrix.platform }}
+    continue-on-error: ${{ matrix.experimental }}
     strategy:
       matrix:
-        platform: ["macOS-11", "macOS-12"]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
+        platform: [ "macOS-11", "macOS-12" ]
+        python-version: [ "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev" ]
         include:
           - experimental: false
           - python-version: "3.12-dev"
             experimental: true
-    runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.experimental }}
     steps:
-    - name: Check out code
-      uses: actions/checkout@v3.3.0
+    - name: Checkout
+      uses: actions/checkout@v3.5.0
       with:
         fetch-depth: 0
+
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4.5.0
       with:
         python-version: ${{ matrix.python-version }}
+
     - name: Get packages
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v3.0.2
       with:
-        name: packages
+        name: ${{ needs.package.outputs.artifact-name }}
         path: dist
+
     - name: Install dev dependencies
       run: |
         # We don't actually want to install rubicon;
         # we just want the dev extras so we have a known version of tox.
         python -m pip install $(ls dist/rubicon_objc-*.whl)[dev]
+
     - name: Test
       run: |
         tox -e py --installpkg dist/rubicon_objc-*.whl
```

### Comparing `rubicon-objc-0.4.5rc1/.github/workflows/release.yml` & `rubicon-objc-0.4.6/.github/workflows/release.yml`

 * *Files 26% similar despite different names*

```diff
@@ -7,58 +7,64 @@
 
 jobs:
   ci:
     uses: ./.github/workflows/ci.yml
 
   release:
     name: Create Release
-    needs: [ci]
+    needs: ci
     # This has to be run on macOS, because rubicon tries to load the Foundation library
     runs-on: macOS-latest
     permissions:
       contents: write
     steps:
       - name: Set build variables
         run: |
           echo "VERSION=${GITHUB_REF_NAME#v}" >> $GITHUB_ENV
+
       - name: Set up Python
         uses: actions/setup-python@v4.5.0
         with:
-          python-version: '3.X'
+          python-version: "3.X"
+
       - name: Get packages
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v3.0.2
         with:
-          name: packages
+          name: ${{ needs.ci.outputs.artifact-name }}
           path: dist
+
       - name: Install packages
         run: pip install dist/rubicon_objc-*.whl
+
       - name: Check version number
         # Check that the setuptools_scm-generated version number is still the same when
         # installed from a wheel with setuptools_scm not present.
         run: |
           set -x
           test $(python -c "from rubicon.objc import __version__; print(__version__)") = $VERSION
+
       - name: Create Release
         uses: ncipollo/release-action@v1.12.0
         with:
           name: ${{ env.VERSION }}
           draft: true
           artifacts: dist/*
           artifactErrorsFailBuild: true
 
   test-publish:
     name: Publish test package
-    needs: [release]
+    needs: [ci, release]
     runs-on: ubuntu-latest
     permissions:
       contents: write
     steps:
       - name: Get packages
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v3.0.2
         with:
-          name: packages
+          name: ${{ needs.ci.outputs.artifact-name }}
           path: dist
+
       - name: Publish release to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           repository_url: https://test.pypi.org/legacy/
           password: ${{ secrets.TEST_PYPI_PASSWORD }}
```

### Comparing `rubicon-objc-0.4.5rc1/.travis.yml` & `rubicon-objc-0.4.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/LICENSE` & `rubicon-objc-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/MANIFEST.in` & `rubicon-objc-0.4.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/PKG-INFO` & `rubicon-objc-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-objc
-Version: 0.4.5rc1
+Version: 0.4.6
 Summary: A bridge between an Objective C runtime environment and Python.
 Home-page: https://beeware.org/rubicon
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
 License: New BSD
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://rubicon-objc.readthedocs.io/en/latest/
```

### Comparing `rubicon-objc-0.4.5rc1/README.rst` & `rubicon-objc-0.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/changes/template.rst` & `rubicon-objc-0.4.6/changes/template.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/Makefile` & `rubicon-objc-0.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/_mocked_modules/ctypes/__init__.py` & `rubicon-objc-0.4.6/docs/_mocked_modules/ctypes/__init__.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/_static/images/rubicon.png` & `rubicon-objc-0.4.6/docs/_static/images/rubicon.png`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/background/community.rst` & `rubicon-objc-0.4.6/docs/background/community.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 The Rubicon Objective-C Developer and User community
 ====================================================
 
 Rubicon Objective-C is part of the `BeeWare suite <https://beeware.org>`__. You
 can talk to the community through:
 
-* `@pybeeware on Twitter <https://twitter.com/pybeeware>`__
+* `@beeware@fosstodon.org <https://fosstodon.org/@beeware>`__
 
-* The `beeware/general <https://gitter.im/beeware/general>`__ channel on Gitter.
+* `Discord <https://beeware.org/bee/chat/>`__
 
 Code of Conduct
 ---------------
 
 The BeeWare community has a strict `Code of Conduct
 <https://beeware.org/contributing/index.html>`__. All users and developers are
 expected to adhere to this code.
```

### Comparing `rubicon-objc-0.4.5rc1/docs/background/faq.rst` & `rubicon-objc-0.4.6/docs/background/faq.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/background/releases.rst` & `rubicon-objc-0.4.6/docs/background/releases.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,50 @@
 Release History
 ===============
 
 .. towncrier release notes start
 
+0.4.6 (2023-04-14)
+==================
+
+Bugfixes
+--------
+
+* The error message returned when a selector has the wrong type has been improved. (`#271 <https://github.com/beeware/rubicon-objc/issues/271>`__)
+* Rubicon now uses an implicit namespace package, instead of relying on the deprecated ``pkg_resources`` API. (`#292 <https://github.com/beeware/rubicon-objc/issues/292>`__)
+
+
+Misc
+----
+
+* #267, #268, #269, #270, #273, #274, #275, #276, #277, #278, #279, #280, #281, #282, #283, #284, #285, #286, #287, #288, #289, #290, #291, #294
+
+
+0.4.5 (2023-02-03)
+==================
+
+Bugfixes
+--------
+
+* Classes that undergo a class name change between ``alloc()`` and ``init()`` (e.g., ``NSWindow`` becomes ``NSKVONotifying_Window``) no longer trigger instance cache eviction logic. (`#258 <https://github.com/beeware/rubicon-objc/pull/258>`__)
+
+
+Misc
+----
+
+* #259, #260, #262, #263, #264, #265, #266
+
+
 0.4.5rc1 (2023-01-25)
 =====================
 
 Features
 --------
 
-* Support for Python 3.6 was dropped. (#371)
+* Support for Python 3.6 was dropped. (`#255 <https://github.com/beeware/rubicon-objc/pull/255>`__)
 
 Misc
 ----
 
 * #254
 
 
@@ -24,24 +55,24 @@
 0.3.0dev39, which was the published Toga release at the time.
 
 Bugfixes
 --------
 
 * Background threads will no longer lock up on iOS when an asyncio event loop is
   in use. (`#228 <https://github.com/beeware/rubicon-objc/issues/228>`__)
-* The ObjCInstance cache no longer returns a stale wrapper objects if a memory
+* The ``ObjCInstance`` cache no longer returns a stale wrapper objects if a memory
   address is re-used by the Objective C runtime. (`#249
   <https://github.com/beeware/rubicon-objc/issues/249>`__)
 * It is now safe to open an asyncio event loop on a secondary thread. Previously
   this would work, but would intermittently fail with a segfault when then loop
   was closed. (`#250 <https://github.com/beeware/rubicon-objc/issues/250>`__)
 * A potential race condition that would lead to duplicated creation on
-  ObjCInstance wrapper objects has been resolved. (`#251
+  ``ObjCInstance`` wrapper objects has been resolved. (`#251
   <https://github.com/beeware/rubicon-objc/issues/251>`__)
-* A race condition associated with populating the ObjCClass method/property
+* A race condition associated with populating the ``ObjCClass`` method/property
   cache has been resolved. (`#252
   <https://github.com/beeware/rubicon-objc/issues/252>`__)
 
 
 Misc
 ----
 
@@ -50,24 +81,21 @@
 
 0.4.3 (2022-12-05)
 ==================
 
 Features
 --------
 
-* Support for Python 3.11 has been added. (`#224
-  <https://github.com/beeware/rubicon-objc/issues/224>`__)
-* Support for Python 3.12 has been added. (`#231
-  <https://github.com/beeware/rubicon-objc/issues/231>`__)
+* Support for Python 3.11 has been added. (`#224 <https://github.com/beeware/rubicon-objc/pull/224>`__)
+* Support for Python 3.12 has been added. (`#231 <https://github.com/beeware/rubicon-objc/pull/231>`__)
 
 Bugfixes
 --------
 
-* Enforce usage of `argtypes` when calling `send_super`. (`#220
-  <https://github.com/beeware/rubicon-objc/issues/220>`__)
+* Enforce usage of `argtypes` when calling `send_super`. (`#220 <https://github.com/beeware/rubicon-objc/pull/220>`__)
 * The check identifying the architecture on which Rubicon is running has been
   corrected for x86_64 simulators using a recent Python-Apple-support releases.
   (`#235 <https://github.com/beeware/rubicon-objc/issues/235>`__)
 
 Misc
 ----
 
@@ -77,82 +105,59 @@
 0.4.2 (2021-11-14)
 ------------------
 
 Features
 ^^^^^^^^
 
 * Added ``autoreleasepool`` context manager to mimic Objective-C
-  ``@autoreleasepool`` blocks. (`#213
-  <https://github.com/beeware/rubicon-objc/issues/213>`__)
-
+  ``@autoreleasepool`` blocks. (`#213 <https://github.com/beeware/rubicon-objc/pull/213>`__)
 * Allow storing Python objects in Objective-C properties declared with
-  ``@objc_property``. (`#214
-  <https://github.com/beeware/rubicon-objc/issues/214>`__)
-
-* Added support for Python 3.10. (`#218
-  <https://github.com/beeware/rubicon-objc/issues/218>`__)
+  ``@objc_property``. (`#214 <https://github.com/beeware/rubicon-objc/pull/214>`__)
+* Added support for Python 3.10. (`#218 <https://github.com/beeware/rubicon-objc/pull/218>`__)
 
 Bugfixes
 ^^^^^^^^
 
 * Raise ``TypeError`` when trying to declare a weak property of a non-object
-  type. (`#215 <https://github.com/beeware/rubicon-objc/issues/215>`__)
+  type. (`#215 <https://github.com/beeware/rubicon-objc/pull/215>`__)
 
 * Corrected handling of methods when a class overrides a method defined in a
   grandparent. (`#216 <https://github.com/beeware/rubicon-objc/issues/216>`__)
 
 
 0.4.1 (2021-07-25)
 ------------------
 
 Features
 ^^^^^^^^
 
-* Added official support for Python 3.9. (`#193
-  <https://github.com/beeware/rubicon-objc/issues/193>`__)
-
-* Added official support for macOS 11 (Big Sur). (`#195
-  <https://github.com/beeware/rubicon-objc/issues/195>`__)
-
+* Added official support for Python 3.9. (`#193 <https://github.com/beeware/rubicon-objc/pull/193>`__)
+* Added official support for macOS 11 (Big Sur). (`#195 <https://github.com/beeware/rubicon-objc/pull/195>`__)
 * Autorelease Objective-C instances when the corresponding Python instance is
   destroyed. (`#200 <https://github.com/beeware/rubicon-objc/issues/200>`__)
-
 * Improved memory management when a Python instance is assigned to a new
-  ``ObjCInstance`` attribute. (`#209
-  <https://github.com/beeware/rubicon-objc/issues/209>`__)
-
-* Added support to declare weak properties on custom Objective-C classes. (`#210
-  <https://github.com/beeware/rubicon-objc/issues/210>`__)
+  ``ObjCInstance`` attribute. (`#209 <https://github.com/beeware/rubicon-objc/pull/209>`__)
+* Added support to declare weak properties on custom Objective-C classes. (`#210 <https://github.com/beeware/rubicon-objc/issues/210>`__)
 
 Bugfixes
 ^^^^^^^^
 
 * Fixed incorrect behavior of :class:`~rubicon.objc.api.Block` when trying to
   create a block with no arguments and using explicit types. This previously
-  caused an incorrect exception about missing argument types; now a no-arg block
-  is created as expected. (`#153
-  <https://github.com/beeware/rubicon-objc/issues/153>`__)
-
+  caused an incorrect exception about missing argument types; now a ``no-arg``
+  block is created as expected. (`#153 <https://github.com/beeware/rubicon-objc/issues/153>`__)
 * Fixed handling of type annotations when passing a bound Python method into
-  :class:`~rubicon.objc.api.Block`. (`#153
-  <https://github.com/beeware/rubicon-objc/issues/153>`__)
-
+  :class:`~rubicon.objc.api.Block`. (`#153 <https://github.com/beeware/rubicon-objc/issues/153>`__)
 * A cooperative entry point for starting event loop has been added. This corrects
-  a problem seen when using Python 3.8 on iOS. (`#182
-  <https://github.com/beeware/rubicon-objc/issues/182>`__)
-
-* Improved performance of Objective-C method calls and
-  :class:`~rubicon.objc.api.ObjCInstance` creation in many cases. (`#183
-  <https://github.com/beeware/rubicon-objc/issues/183>`__)
-
-* Fix calling of signal handlers added to the asyncio loop with CFRunLoop
+  a problem seen when using Python 3.8 on iOS. (`#182 <https://github.com/beeware/rubicon-objc/pull/182>`__)
+* Improved performance of Objective-C method calls and :class:`~rubicon.objc.api.ObjCInstance` creation in many cases.
+  (`#183 <https://github.com/beeware/rubicon-objc/issues/183>`__)
+* Fix calling of signal handlers added to the asyncio loop with ``CFRunLoop``
   integration. (`#202 <https://github.com/beeware/rubicon-objc/issues/202>`__)
-
-* Allow restarting a stopped event loop. (`#205
-  <https://github.com/beeware/rubicon-objc/issues/205>`__)
+* Allow restarting a stopped event loop. (`#205 <https://github.com/beeware/rubicon-objc/pull/205>`__)
 
 Deprecations and Removals
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 * Removed automatic conversion of Objective-C numbers (``NSNumber`` and
   ``NSDecimalNumber``) to Python numbers when received from Objective-C (i.e.
   returned from an Objective-C method or property or passed into an Objective-C
@@ -180,94 +185,89 @@
   but will probably be removed relatively soon.
   Automatic tests on macOS 10.15 and 11.0 are unaffected
   as they run on a different CI service (GitHub Actions).
 
   Rubicon will continue to support macOS 10.14 and earlier on a best-effort
   basis, even though compatibility is no longer tested automatically. If you
   encounter any bugs or other problems with Rubicon on these older macOS
-  versions, please report them! (`#197
-  <https://github.com/beeware/rubicon-objc/issues/197>`__)
+  versions, please report them! (`#197 <https://github.com/beeware/rubicon-objc/issues/197>`__)
 
 Misc
 ^^^^
 
-* `#185 <https://github.com/beeware/rubicon-objc/issues/185>`_,
-  `#189 <https://github.com/beeware/rubicon-objc/issues/189>`_,
-  `#194 <https://github.com/beeware/rubicon-objc/issues/194>`_,
-  `#196 <https://github.com/beeware/rubicon-objc/issues/196>`_,
-  `#208 <https://github.com/beeware/rubicon-objc/issues/208>`_
+* #185, #189, #194, #196, #208
 
 
 0.4.0 (2020-07-04)
 ------------------
 
 Features
 ^^^^^^^^
 
 * Added macOS 10.15 (Catalina) to the test matrix.
-  (`#145 <https://github.com/beeware/rubicon-objc/issues/145>`__)
-* Added :pep:`517` and :pep:`518` build system metadata to pyproject.toml.
-  (`#156 <https://github.com/beeware/rubicon-objc/issues/156>`__)
+  (`#145 <https://github.com/beeware/rubicon-objc/pull/145>`__)
+* Added :pep:`517` and :pep:`518` build system metadata to ``pyproject.toml``.
+  (`#156 <https://github.com/beeware/rubicon-objc/pull/156>`__)
 * Added official support for Python 3.8.
-  (`#162 <https://github.com/beeware/rubicon-objc/issues/162>`__)
+  (`#162 <https://github.com/beeware/rubicon-objc/pull/162>`__)
 * Added a ``varargs`` keyword argument to
   :func:`~rubicon.objc.runtime.send_message` to allow calling variadic methods
-  more safely. (`#174 <https://github.com/beeware/rubicon-objc/issues/174>`__)
+  more safely. (`#174 <https://github.com/beeware/rubicon-objc/pull/174>`__)
 * Changed ``ObjCMethod`` to call methods using
   :func:`~rubicon.objc.runtime.send_message` instead of calling
   :class:`~rubicon.objc.runtime.IMP`\s directly. This is mainly an internal
   change and should not affect most existing code, although it may improve
   compatibility with Objective-C code that makes heavy use of runtime
   reflection and method manipulation (such as swizzling).
-  (`#177 <https://github.com/beeware/rubicon-objc/issues/177>`__)
+  (`#177 <https://github.com/beeware/rubicon-objc/pull/177>`__)
 
 Bugfixes
 ^^^^^^^^
 
 * Fixed Objective-C method calls in "flat" syntax accepting more arguments than
   the method has. The extra arguments were previously silently ignored.
   An exception is now raised if too many arguments are passed.
   (`#123 <https://github.com/beeware/rubicon-objc/issues/123>`__)
 * Fixed :func:`ObjCInstance.__str__ <rubicon.objc.api.ObjCInstance.__str__>`
   throwing an exception if the object's Objective-C ``description`` is ``nil``.
   (`#125 <https://github.com/beeware/rubicon-objc/issues/125>`__)
 * Corrected a slow memory leak caused every time an asyncio timed event handler
   triggered. (`#146 <https://github.com/beeware/rubicon-objc/issues/146>`__)
 * Fixed various minor issues in the build and packaging metadata.
-  (`#156 <https://github.com/beeware/rubicon-objc/issues/156>`__)
+  (`#156 <https://github.com/beeware/rubicon-objc/pull/156>`__)
 * Removed unit test that attempted to pass a struct with bit fields into a C
   function by value. Although this has worked in the past on x86 and x86_64,
   :mod:`ctypes` never officially supported this, and started generating an
   error in Python 3.7.6 and 3.8.1
   (see `bpo-39295 <https://bugs.python.org/issue39295>`__).
-  (`#157 <https://github.com/beeware/rubicon-objc/issues/157>`__)
+  (`#157 <https://github.com/beeware/rubicon-objc/pull/157>`__)
 * Corrected the invocation of ``NSApplication.terminate()`` when the
   :class:`~rubicon.objc.eventloop.CocoaLifecycle` is ended.
   (`#170 <https://github.com/beeware/rubicon-objc/issues/170>`__)
 * Fixed :func:`~rubicon.objc.runtime.send_message` not accepting
   :class:`~rubicon.objc.runtime.SEL` objects for the ``selector`` parameter.
   The documentation stated that this is allowed, but actually doing so caused
-  a type error. (`#177 <https://github.com/beeware/rubicon-objc/issues/177>`__)
+  a type error. (`#177 <https://github.com/beeware/rubicon-objc/pull/177>`__)
 
 Improved Documentation
 ^^^^^^^^^^^^^^^^^^^^^^
 
 * Added detailed :doc:`reference documentation </reference/index>` for all
   public APIs of :mod:`rubicon.objc`.
-  (`#118 <https://github.com/beeware/rubicon-objc/issues/118>`__)
+  (`#118 <https://github.com/beeware/rubicon-objc/pull/118>`__)
 * Added a :doc:`how-to guide for calling regular C functions
   </how-to/c-functions>` using :mod:`ctypes` and :mod:`rubicon.objc`.
-  (`#147 <https://github.com/beeware/rubicon-objc/issues/147>`__)
+  (`#147 <https://github.com/beeware/rubicon-objc/pull/147>`__)
 
 Deprecations and Removals
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 * Removed the i386 architecture from the test matrix. It is still supported on
   a best-effort basis, but compatibility is not tested automatically.
-  (`#139 <https://github.com/beeware/rubicon-objc/issues/139>`__)
+  (`#139 <https://github.com/beeware/rubicon-objc/pull/139>`__)
 * Tightened the API of :func:`~rubicon.objc.runtime.send_message`, removing
   some previously allowed shortcuts and features that were rarely used, or
   likely to be used by accident in an unsafe way.
 
   .. note::
 
       In most cases, Rubicon's high-level method call syntax provided by
@@ -298,46 +298,38 @@
   ``restype`` and ``argtypes`` keyword arguments. Every
   :func:`~rubicon.objc.runtime.send_message` call now needs to have its return
   and argument types set explicitly. This ensures that all arguments and the
   return value are converted correctly between (Objective-)C and Python.
 * Disallowed passing more argument values than there are argument types in
   ``argtypes``. This was previously allowed to support calling variadic methods
   - any arguments beyond the types set in ``argtypes`` would be passed as
-  varargs. However, this feature was easy to misuse by accident, as it allowed
+  ``varargs``. However, this feature was easy to misuse by accident, as it allowed
   passing extra arguments to *any* method, even though most Objective-C methods
   are not variadic. Extra arguments passed this way were silently ignored
   without causing an error or a crash.
 
   To prevent accidentally passing too many arguments like this, the number of
   arguments now has to exactly match the number of ``argtypes``. Variadic
-  methods can still be called, but the varargs now need to be passed as a list
-  into the separate ``varargs`` keyword arugment.
-  (`#174 <https://github.com/beeware/rubicon-objc/issues/174>`__)
+  methods can still be called, but the ``varargs`` now need to be passed as a
+  list into the separate ``varargs`` keyword argument.
+  (`#174 <https://github.com/beeware/rubicon-objc/pull/174>`__)
 * Removed the ``rubicon.objc.core_foundation`` module. This was an internal
   module with few remaining contents and should not have any external uses. If
   you need to call Core Foundation functions in your code, please load the
   framework yourself using ``load_library('CoreFoundation')`` and define the
   types and functions that you need.
-  (`#175 <https://github.com/beeware/rubicon-objc/issues/175>`__)
+  (`#175 <https://github.com/beeware/rubicon-objc/pull/175>`__)
 * Removed the ``ObjCMethod`` class from the public API, as there was no good
   way to use it from external code.
-  (`#177 <https://github.com/beeware/rubicon-objc/issues/177>`__)
+  (`#177 <https://github.com/beeware/rubicon-objc/pull/177>`__)
 
 Misc
 ^^^^
 
-* `#143 <https://github.com/beeware/rubicon-objc/issues/143>`_,
-  `#145 <https://github.com/beeware/rubicon-objc/issues/145>`_,
-  `#155 <https://github.com/beeware/rubicon-objc/issues/155>`_,
-  `#158 <https://github.com/beeware/rubicon-objc/issues/158>`_,
-  `#159 <https://github.com/beeware/rubicon-objc/issues/159>`_,
-  `#164 <https://github.com/beeware/rubicon-objc/issues/164>`_,
-  `#173 <https://github.com/beeware/rubicon-objc/issues/173>`_,
-  `#178 <https://github.com/beeware/rubicon-objc/issues/178>`_,
-  `#179 <https://github.com/beeware/rubicon-objc/issues/179>`_
+* #143, #145, #155, #158, #159, #164, #173, #178, #179
 
 
 0.3.1
 -----
 
 * Added a workaround for `bpo-36880 <https://bugs.python.org/issue36880>`_,
   which caused a "deallocating None" crash when returning structs from methods
@@ -361,24 +353,24 @@
   automatic conversion.
 
   In most cases, this change will not affect existing code, because
   ``NSString`` objects now support operations similar to ``str``. If an actual
   ``str`` object is required, the ``NSString`` object can be wrapped in a
   ``str`` call to convert it.
 * Added support for ``objc_property``\s with non-object types.
-* Added public ``get_ivar`` and ``set_ivar`` functions for manipulating ivars.
-* Changed the implementation of ``objc_property`` to use ivars instead of
+* Added public ``get_ivar`` and ``set_ivar`` functions for manipulating ``ivars``.
+* Changed the implementation of ``objc_property`` to use ``ivars`` instead of
   Python attributes for storage. This fixes name conflicts in some situations.
 * Added the :func:`~rubicon.objc.runtime.load_library` function for loading
   :class:`~ctypes.CDLL`\s by their name instead of their full path.
-* Split the high-level Rubicon API (:class:`ObjCInstance`, :class:`ObjCClass`,
-  etc.) out of :mod:`rubicon.objc.runtime` into a separate
-  :mod:`rubicon.objc.api` module. The :mod:`~rubicon.objc.runtime` module now
-  only contains low-level runtime interfaces like
-  :data:`~rubicon.objc.runtime.libobjc`.
+* Split the high-level Rubicon API (:class:`~rubicon.objc.api.ObjCInstance`,
+  :class:`~rubicon.objc.api.ObjCClass`, etc.) out of :mod:`rubicon.objc.runtime`
+  into a separate :mod:`rubicon.objc.api` module. The
+  :mod:`~rubicon.objc.runtime` module now only contains low-level runtime
+  interfaces like :data:`~rubicon.objc.runtime.libobjc`.
 
   This is mostly an internal change, existing code will not be affected unless
   it imports names directly from :mod:`rubicon.objc.runtime`.
 * Moved :class:`~rubicon.objc.types.c_ptrdiff_t` from
   :mod:`rubicon.objc.runtime` to :mod:`rubicon.objc.types`.
 * Removed some rarely used names (:class:`~rubicon.objc.runtime.IMP`,
   :class:`~rubicon.objc.runtime.Class`, :class:`~rubicon.objc.runtime.Ivar`,
@@ -405,15 +397,15 @@
   lengths. Previously this incorrectly returned ``True`` if the shorter sequence
   was a prefix of the longer one, now ``False`` is returned.
 * Fixed calling ``popitem`` on an empty Objective-C dictionary. Previously
   this crashed Python, now a ``KeyError`` is raised.
 * Fixed calling ``update`` with both a mapping and keyword arguments on an
   Objective-C dictionary. Previously the kwargs were incorrectly ignored if a
   mapping was given, now both are respected.
-* Fixed calling methods using kwarg syntax if a superclass and subclass define
+* Fixed calling methods using ``kwarg`` syntax if a superclass and subclass define
   methods with the same prefix, but different names. For example, if a
   superclass had a method ``initWithFoo:bar:`` and the subclass
   ``initWithFoo:spam:``, the former could not be called on instances of the
   subclass.
 * Fixed the internal ``ctypes_patch`` module so it no longer depends on a
   non-public CPython function.
 
@@ -438,30 +430,30 @@
   systems.
 * Renamed the ``async`` support package to ``eventloop`` to avoid a Python 3.5+
   keyword clash.
 
 0.2.9
 -----
 
-* Improved handling of boolean types.
+* Improved handling of Boolean types.
 * Added support for using primitives as object values (e.g, as the key/value in
-  an NSDictonary).
-* Added support for passing Python lists as Objective-C NSArray arguments, and
-  Python dicts as Objective-C NSDictionary arguments.
+  an ``NSDictonary``).
+* Added support for passing Python lists as Objective-C ``NSArray`` arguments, and
+  Python dictionaries as Objective-C ``NSDictionary`` arguments.
 * Corrected support to storing strings and other objects as properties on
   Python-defined Objective-C classes.
 * Added support for creating Objective-C blocks from Python callables. (ojii)
 * Added support for returning compound values (structures and unions) from
   Objective-C methods defined in Python.
 * Added support for creating, extending and conforming to Objective-C protocols.
 * Added an ``objc_const`` convenience function to look up global Objective-C
   object constants in a DLL.
 * Added support for registering custom ``ObjCInstance`` subclasses to be used
   to represent Objective-C objects of specific classes.
-* Added support for integrating NSApplication and UIApplication event loops
+* Added support for integrating ``NSApplication`` and ``UIApplication`` event loops
   with Python's asyncio event loop.
 
 0.2.8
 -----
 
 * Added support for using native Python sequence/mapping syntax with
   ``NSArray`` and ``NSDictionary``. (jeamland)
@@ -486,15 +478,15 @@
 * Removed the encoding constants. Use ``encoding_for_ctype`` to get the encoding
   of a type.
 
 0.2.7
 -----
 
 * (#40) Added the ability to explicitly declare no-attribute methods as
-  properties. This is to enable a workaround when Apple introduces readonly
+  properties. This is to enable a workaround when Apple introduces read-only
   properties as a way to access these methods.
 
 0.2.6
 -----
 
 * Added a more compact syntax for calling Objective-C methods, using Python
   keyword arguments. (The old syntax is still fully supported and will *not*
```

### Comparing `rubicon-objc-0.4.5rc1/docs/conf.py` & `rubicon-objc-0.4.6/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc", "sphinx_tabs.tabs"]
+extensions = ["sphinx.ext.autodoc", "sphinx_tabs.tabs", "sphinx.ext.intersphinx"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
 
@@ -44,15 +44,17 @@
 copyright = "2014, Russell Keith-Magee"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-version = metadata_version("rubicon-objc")
+release = metadata_version("rubicon-objc")
+# The short X.Y version
+version = ".".join(release.split(".")[:2])
 
 autoclass_content = "both"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
@@ -82,28 +84,41 @@
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
+intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
+
+nitpick_ignore = [
+    # These functions do not have documentation
+    ("py:func", "rubicon.objc.types.CGPointMake"),
+    ("py:func", "rubicon.objc.types.CGRectMake"),
+    ("py:func", "rubicon.objc.types.CGSizeMake"),
+    ("py:func", "rubicon.objc.types.NSEdgeInsetsMake"),
+    ("py:func", "rubicon.objc.types.NSMakePoint"),
+    ("py:func", "rubicon.objc.types.NSMakeRect"),
+    ("py:func", "rubicon.objc.types.NSMakeSize"),
+    ("py:func", "rubicon.objc.types.UIEdgeInsetsMake"),
+]
 
 # -- Options for HTML output ---------------------------------------------------
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-# html_title = None
+html_title = f"Rubicon {release}"
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 # html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
 html_logo = "_static/images/rubicon.png"
@@ -242,23 +257,24 @@
 
 # -- Options for spelling -------------------------------------------
 
 # Spelling check needs an additional module that is not installed by default.
 # Add it only if spelling check is requested so docs can be generated without it.
 if "spelling" in sys.argv:
     extensions.append("sphinxcontrib.spelling")
+    # Load the enchant package here before `ctypes` is mocked out.
+    # Otherwise, it will not be able to load its external library later.
+    import enchant  # noqa: F401, E402
 
 # Spelling language.
 spelling_lang = "en_US"
 
 # Location of word list.
 spelling_word_list_filename = "spelling_wordlist"
 
-spelling_ignore_pypi_package_names = True
-
 # We mock the ctypes and ctypes.util modules during the documentation build,
 # so that Sphinx autodoc is able to import and inspect rubicon.objc even on systems without an Objective-C runtime.
 # For more details, see the docstring of _mocked_modules/ctypes/__init__.py.
 sys.path.insert(0, os.path.abspath("_mocked_modules"))
 sys.modules.pop("ctypes", None)
 sys.modules.pop("ctypes.util", None)
 import ctypes.util  # noqa: F401, E402
```

### Comparing `rubicon-objc-0.4.5rc1/docs/how-to/async.rst` & `rubicon-objc-0.4.6/docs/how-to/async.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 =====================================
 Asynchronous Programming with Rubicon
 =====================================
 
 One of the banner features of Python 3 is the introduction of native
-asychronous programming, implemented in the `asyncio`.
+asynchronous programming, implemented in the `asyncio`.
 
 For an introduction to the use of asynchronous programming, see `the
 documentation for the asyncio module
-<https://docs.python.org/3/library/asyncio.html>`__, or `this introductory
-tutorial to asynchronous programming with asyncio
-<http://asyncio.readthedocs.io/en/latest/index.html>`__.
+<https://docs.python.org/3/library/asyncio.html>`__.
 
 Integrating asyncio with CoreFoundation
 =======================================
 
 The asyncio module provides an event loop to coordinate asynchronous features.
-However, if you're running an Objective C GUI applicaiton, you probably
+However, if you're running an Objective C GUI application, you probably
 already have an event loop - the one provided by CoreFoundation. This
 CoreFoundation event loop is then wrapped by `NSApplication` or
 `UIApplication` in end-user code.
 
 However, you can't have two event loops running at the same time, so you need
 a way to integrate the two. Luckily, `asyncio` provides a way to customize
 it's event loop so it can be integrated with other event sources.
@@ -40,20 +38,20 @@
     loop = asyncio.new_event_loop()
     loop.run_forever()
 
 The last call (``loop.run_forever()``) will, as the name suggests, run forever
 - or, at least, until an event handler calls ``loop.stop()`` to terminate the
 event loop.
 
-Integrating asyncio with AppKit and NSApplication
-=================================================
+Integrating asyncio with AppKit and ``NSApplication``
+=====================================================
 
 If you're using AppKit and NSApplication, you don't just need to start the
-CoreFoundation event loop - you need to start the full NSApplication
-lifecycle. To do this, you pass the application instance into the call to
+CoreFoundation event loop - you need to start the full ``NSApplication``
+life cycle. To do this, you pass the application instance into the call to
 ``loop.run_forever()``::
 
     # Import the Event Loop Policy and lifecycle
     from rubicon.objc.eventloop import EventLoopPolicy, CocoaLifecycle
 
     # Install the event loop policy
     asyncio.set_event_loop_policy(EventLoopPolicy())
@@ -74,15 +72,15 @@
 Again, this will run "forever" -- until either ``loop.stop()`` is called, or
 ``terminate:`` is invoked on the NSApplication.
 
 Integrating asyncio with iOS and UIApplication
 ==============================================
 
 If you're using UIKit and UIApplication on iOS, you need to use the iOS
-lifecycle. To do this, you pass an ``iOSLifecycle`` object into the call to
+life cycle. To do this, you pass an ``iOSLifecycle`` object into the call to
 ``loop.run_forever()``::
 
     # Import the Event Loop Policy and lifecycle
     from rubicon.objc.eventloop import EventLoopPolicy, iOSLifecycle
 
     # Install the event loop policy
     asyncio.set_event_loop_policy(EventLoopPolicy())
```

### Comparing `rubicon-objc-0.4.5rc1/docs/how-to/c-functions.rst` & `rubicon-objc-0.4.6/docs/how-to/c-functions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,19 @@
     Even though the constants use the type name ``NSCalendarIdentifier``, their actual type is still ``NSString *``, based on the ``typedef`` before.
 
     In some cases, constants use a ``typedef`` from a different header (or even a different library) than the one defining the constants, which can make it even harder to tell that they are actually Objective-C objects.
 
 A complex example: ``dispatch_get_main_queue``
 ----------------------------------------------
 
-As a final example, we'll look at the function ``dispatch_get_main_queue`` from the libdispatch library. This is a very complex function definition, which involves many of the concepts introduced above, as well as heavy use of C preprocessor macros. If you don't have a lot of experience with the C preprocessor, you may want to skip this section.
+As a final example, we'll look at the function ``dispatch_get_main_queue`` from
+the ``libdispatch`` library. This is a very complex function definition, which
+involves many of the concepts introduced above, as well as heavy use of C
+pre-processor macros. If you don't have a lot of experience with the C
+pre-processor, you may want to skip this section.
 
 .. This example is based on the response to a question from the beeware/general Gitter chat: https://gitter.im/beeware/general?at=5b54e95357f4f664b794cde2
 
 First, we need to look at the function's definition, which is found in the header ``<dispatch/queue.h>``:
 
 .. code-block:: objc
 
@@ -369,10 +373,10 @@
     def dispatch_get_main_queue():
         return ObjCInstance(cast(byref(_dispatch_main_q), objc_id))
 
 Further information
 -------------------
 
 * `cdecl.org <https://cdecl.org/>`_: An online service to translate C type syntax into more understandable English.
-* `cppreference.com <https://en.cppreference.com/>`_: A reference site about the standard C and C++ languages and libraries.
+* `cppreference.com <https://en.cppreference.com/w/>`_: A reference site about the standard C and C++ languages and libraries.
 * `Apple's reference documentation <https://developer.apple.com/documentation/>`_: Official API documentation for Apple platforms. Make sure to change the language to Objective-C in the top-right corner, otherwise you'll get Swift documentation, which can differ significantly from Objective-C.
 * macOS man pages, sections 2 and 3: Documentation for the C functions provided by macOS. View these using the ``man`` command, or by typing a function name into the search box of the macOS Terminal's Help menu.
```

### Comparing `rubicon-objc-0.4.5rc1/docs/how-to/contribute-code.rst` & `rubicon-objc-0.4.6/docs/how-to/contribute-code.rst`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     trim trailing whitespace.................................................Passed
     isort....................................................................Passed
     pyupgrade................................................................Passed
     docformatter.............................................................Passed
     [bugfix e3e0f73] Minor change
     1 file changed, 4 insertions(+), 2 deletions(-)
 
-Rubicon uses `tox <https://tox.readthedocs.io/en/latest/>`__ to manage the
+Rubicon uses `tox <https://tox.wiki/en/latest/>`__ to manage the
 testing process. To set up a testing environment and run the full test suite,
 run:
 
 .. code-block:: sh
 
     (venv) $ tox
```

### Comparing `rubicon-objc-0.4.5rc1/docs/how-to/internal/release.rst` & `rubicon-objc-0.4.6/docs/how-to/internal/release.rst`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       service monitoring as PyPI-proper, so it sometimes has problems. However,
       it's also not critical to the release process; if this step fails, you can
       perform Step 6 by manually downloading the "packages" artifact from the
       GitHub workflow instead.
    b. Something else fails in the build process. If the problem can be fixed
       without a code change to the Rubicon-ObjC repository (e.g., a transient
       problem with build machines not being available), you can re-run the
-      action that failed through the Github Actions GUI. If the fix requires a
+      action that failed through the GitHub Actions GUI. If the fix requires a
       code change, delete the old tag, make the code change, and re-tag the
       release.
 
 5. Create a clean virtual environment, install the new release from Test PyPI, and
    perform any pre-release testing that may be appropriate::
 
     $ python3 -m venv testvenv
@@ -70,16 +70,17 @@
     (testvenv) $ ... any other manual checks you want to perform ...
 
 6. Log into ReadTheDocs, visit the `Versions tab
    <https://readthedocs.org/projects/rubicon-objc/versions/>`__, and activate the
    new version. Ensure that the build completes; if there's a problem, you
    may need to correct the build configuration, roll back and re-tag the release.
 
-7. Edit the GitHub release. Add release notes (you can use the text generated
-   by towncrier). Check the pre-release checkbox (if necessary).
+7. Edit the GitHub release to add release notes. You can use the text generated
+   by Towncrier, but you'll need to update the format to Markdown, rather than
+   ReST. If necessary, check the pre-release checkbox.
 
 8. Double check everything, then click Publish. This will trigger a
    `publication workflow on GitHub
    <https://github.com/beeware/rubicon-objc/actions?query=workflow%3A%22Upload+Python+Package%22>`__.
 
 7. Wait for the `package to appear on PyPI
 <https://pypi.org/project/rubicon-objc/>`__.
```

### Comparing `rubicon-objc-0.4.5rc1/docs/how-to/memory-management.rst` & `rubicon-objc-0.4.6/docs/how-to/memory-management.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 When enabling automatic reference counting (ARC), the appropriate calls for
 memory management will be inserted for you at compile-time. However, since
 Rubicon Objective-C operates at runtime, it cannot make use of ARC.
 
 Reference counting in Rubicon Objective-C
 -----------------------------------------
 
-You won't have to manage reference counts in Python, Rubicon Objective-C will
-do that work for you. It does so by tracking when you gain ownership of an
-object. This is the case when you create an Objective-C instance using a method
-whose name begins with "alloc", "new", "copy", or "mutableCopy". Rubicon
+You won't have to manage reference counts in Python, Rubicon Objective-C will do
+that work for you. It does so by tracking when you gain ownership of an object.
+This is the case when you create an Objective-C instance using a method whose
+name begins with ``alloc``, ``new``, ``copy``, or ``mutableCopy``. Rubicon
 Objective-C will then insert a ``release`` call when the Python variable that
 corresponds to the Objective-C instance is deallocated.
 
 An exception to this is when you manually ``retain`` an object. Rubicon
 Objective-C will not keep track of such retain calls and you will be
 responsible to insert appropriate ``release`` calls yourself.
```

### Comparing `rubicon-objc-0.4.5rc1/docs/how-to/protocols.rst` & `rubicon-objc-0.4.6/docs/how-to/protocols.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/how-to/type-mapping.rst` & `rubicon-objc-0.4.6/docs/how-to/type-mapping.rst`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     :class:`~rubicon.objc.api.NSString` internally have the class
     ``ObjCStrInstance``, and you will see this name in the :func:`repr` of
     :class:`~rubicon.objc.api.NSString` objects. This is an implementation
     detail - you should not refer to the ``ObjCStrInstance`` class explicitly
     in your code.
 
 If you have an :class:`~rubicon.objc.api.NSString`, and you need to pass it to
-a method that does a specific typecheck for :class:`str`, you can use
+a method that does a specific type check for :class:`str`, you can use
 ``str(nsstring)`` to convert the :class:`~rubicon.objc.api.NSString` to
 :class:`str`:
 
 .. code-block:: python
 
     # Convert the Objective-C string to a Python string.
     >>> str(NSBundle.mainBundle.bundlePath)
@@ -193,17 +193,18 @@
 
 .. note::
 
     :class:`~rubicon.objc.api.NSString` objects behave slightly differently
     than Python :class:`str` objects in some cases. For technical reasons,
     :class:`~rubicon.objc.api.NSString`\s are not hashable in Python, which
     means they cannot be used as :class:`dict` keys (but they *can* be used as
-    :class:`NSDictionary` keys). :class:`~rubicon.objc.api.NSString` also
-    handles Unicode code points above ``U+FFFF`` differently than Python
-    :class:`str`, because the former is based on UTF-16.
+    :class:`~rubicon.objc.api.NSDictionary` keys).
+    :class:`~rubicon.objc.api.NSString` also handles Unicode code points above
+    ``U+FFFF`` differently than Python :class:`str`, because the former is
+    based on UTF-16.
 
 Lists
 ^^^^^
 
 :class:`~rubicon.objc.api.NSArray` objects behave like any other Python
 sequence - they can be indexed, sliced, etc. and standard operations like
 :func:`len` and ``in`` are supported:
```

### Comparing `rubicon-objc-0.4.5rc1/docs/index.rst` & `rubicon-objc-0.4.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/make.bat` & `rubicon-objc-0.4.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc-api.rst` & `rubicon-objc-0.4.6/docs/reference/rubicon-objc-api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -327,16 +327,16 @@
 
 Before being passed to the Python method, any object parameters (:class:`~rubicon.objc.runtime.objc_id`) are automatically converted to :class:`ObjCInstance`. If the method returns an Objective-C object, it is converted using :func:`ns_from_py` before being returned to Objective-C. These automatic conversions can be disabled by using :func:`objc_rawmethod` instead of :func:`objc_method`.
 
 The implicit ``_cmd`` parameter is not passed to the Python method, as it is normally redundant and not needed. If needed, the ``_cmd`` parameter can be accessed by using :func:`objc_rawmethod` instead of :func:`objc_method`.
 
 .. autofunction:: objc_rawmethod
 
-Defining properties and ivars
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Defining properties and ``ivars``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. autofunction:: objc_property
 .. autofunction:: objc_ivar
 .. autofunction:: get_ivar
 .. autofunction:: set_ivar
 
 .. _objc_blocks:
@@ -381,15 +381,15 @@
             res = SomeClass.someMethod()
             result_handler(res)
 
 .. note::
 
     These automatic conversions are mostly equivalent to the manual conversions described in the next section. There are internal technical differences between automatic and manual conversions, but they are not noticeable to most users.
 
-    The internals of automatic conversion and :class:`objc_block` handling may change in the future, so if you need more control over the block conversion process, you should use the manual conversions described in the next section.
+    The internals of automatic conversion and :class:`~rubicon.objc.runtime.objc_block` handling may change in the future, so if you need more control over the block conversion process, you should use the manual conversions described in the next section.
 
 Manual conversion
 ^^^^^^^^^^^^^^^^^
 
 These classes are used to manually convert blocks to Python callables and vice versa. You may need to use them to perform these conversions outside of Objective-C method calls, or if you need more control over the block's type signature.
 
 .. autoclass:: ObjCBlock(pointer, [return_type, *arg_types])
```

### Comparing `rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc-eventloop.rst` & `rubicon-objc-0.4.6/docs/reference/rubicon-objc-eventloop.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc-runtime.rst` & `rubicon-objc-0.4.6/docs/reference/rubicon-objc-runtime.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc-types.rst` & `rubicon-objc-0.4.6/docs/reference/rubicon-objc-types.rst`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 .. class:: NSUInteger([value])
 
     The `NSUInteger <https://developer.apple.com/documentation/objectivec/nsuinteger?language=objc>`__ type from ``<objc/NSObjCRuntime.h>``. Equivalent to :class:`~ctypes.c_ulong` on 64-bit systems and :class:`~ctypes.c_uint` on 32-bit systems.
 
 .. class:: CGFloat([value])
 
-    The `CGFloat <https://developer.apple.com/documentation/coregraphics/cgfloat?language=objc>`__ type from ``<CoreGraphics/CGBase.h>``. Equivalent to :class:`~ctypes.c_double` on 64-bit systems and :class:`~ctypes.c_float` on 32-bit systems.
+    The `CGFloat <https://developer.apple.com/documentation/corefoundation/cgfloat?language=objc>`__ type from ``<CoreGraphics/CGBase.h>``. Equivalent to :class:`~ctypes.c_double` on 64-bit systems and :class:`~ctypes.c_float` on 32-bit systems.
 
 .. class:: NSPoint([x, y])
 
     The `NSPoint <https://developer.apple.com/documentation/foundation/nspoint?language=objc>`__ structure from ``<Foundation/NSGeometry.h>``.
 
     .. note::
 
@@ -39,15 +39,15 @@
         x
         y
 
         The X and Y coordinates as :class:`CGFloat`\s.
 
 .. class:: CGPoint([x, y])
 
-    The `CGPoint <https://developer.apple.com/documentation/coregraphics/cgpoint?language=objc>`__ structure from ``<CoreGraphics/CGGeometry.h>``.
+    The `CGPoint <https://developer.apple.com/documentation/corefoundation/cgpoint?language=objc>`__ structure from ``<CoreGraphics/CGGeometry.h>``.
 
     .. attribute::
         x
         y
 
         The X and Y coordinates as :class:`CGFloat`\s.
 
@@ -63,15 +63,15 @@
         width
         height
 
         The width and height as :class:`CGFloat`\s.
 
 .. class:: CGSize([width, height])
 
-    The `CGSize <https://developer.apple.com/documentation/coregraphics/cgsize?language=objc>`__ structure from ``<CoreGraphics/CGGeometry.h>``.
+    The `CGSize <https://developer.apple.com/documentation/corefoundation/cgsize?language=objc>`__ structure from ``<CoreGraphics/CGGeometry.h>``.
 
     .. attribute::
         width
         height
 
         The width and height as :class:`CGFloat`\s.
 
@@ -89,15 +89,15 @@
 
     .. attribute:: size
 
         The size as a :class:`NSSize`.
 
 .. class:: CGRect([origin, size])
 
-    The `CGRect <https://developer.apple.com/documentation/coregraphics/cgrect?language=objc>`__ structure from ``<CoreGraphics/CGGeometry.h>``.
+    The `CGRect <https://developer.apple.com/documentation/corefoundation/cgrect?language=objc>`__ structure from ``<CoreGraphics/CGGeometry.h>``.
 
     .. attribute:: origin
 
         The origin as a :class:`CGPoint`.
 
     .. attribute:: size
 
@@ -227,51 +227,51 @@
 .. autofunction:: split_method_encoding
 .. autofunction:: ctypes_for_method_encoding
 
 Default registered type encodings
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The following table lists Objective-C's standard type encodings for primitive types, and the corresponding registered
-ctypes. These mappings can be considered stable, but nonetheless users should not hardcode these encodings unless
+ctypes. These mappings can be considered stable, but nonetheless users should not hard code these encodings unless
 necessary. Instead, the :func:`encoding_for_ctype` function should be used to encode types, because it is less
 error-prone and more readable than typing encodings out by hand.
 
-============================= ========================== =====
-Ctype                         Type encoding              Notes
-============================= ========================== =====
-``None`` (``void``)           ``v``
-:class:`~ctypes.c_bool`       ``B``                      This refers to the ``bool`` type from C99 and C++. It is not necessarily the same as the :class:`BOOL` type, which may be either :class:`~ctypes.c_byte` or :class:`~ctypes.c_bool` depending on the system and architecture.
-:class:`~ctypes.c_byte`       ``c``
-:class:`~ctypes.c_ubyte`      ``C``
-:class:`~ctypes.c_short`      ``s``
-:class:`~ctypes.c_ushort`     ``S``
-:class:`~ctypes.c_long`       ``l``
-:class:`~ctypes.c_ulong`      ``L``
-:class:`~ctypes.c_int`        ``i``                      On 32-bit systems, :class:`~ctypes.c_int` is an alias for :class:`~ctypes.c_long`, and will be encoded as such.
-:class:`~ctypes.c_uint`       ``I``                      On 32-bit systems, :class:`~ctypes.c_uint` is an alias for :class:`~ctypes.c_ulong`, and will be encoded as such.
-:class:`~ctypes.c_longlong`   ``q``                      On 64-bit systems, :class:`~ctypes.c_longlong` is an alias for :class:`~ctypes.c_long`, and will be encoded as such.
-:class:`~ctypes.c_ulonglong`  ``Q``                      On 64-bit systems, :class:`~ctypes.c_ulonglong` is an alias for :class:`~ctypes.c_ulong`, and will be encoded as such.
-:class:`~ctypes.c_float`      ``f``
-:class:`~ctypes.c_double`     ``d``
-:class:`~ctypes.c_longdouble` ``D``                      On ARM, :class:`~ctypes.c_longdouble` is an alias for :class:`~ctypes.c_double`, and will be encoded as such.
-:class:`~ctypes.c_char`       ``c``                      Only when encoding. Decoding ``c`` produces :class:`~ctypes.c_byte`, to allow using ``signed char`` as a boolean value.
-:class:`~ctypes.c_char_p`     ``*``
-``POINTER(c_char)``           ``*``                      Only when encoding. Decoding ``*`` produces :class:`~ctypes.c_char_p` for easier use of C strings.
-``POINTER(c_byte)``           ``*``                      Only when encoding. Decoding ``*`` produces :class:`~ctypes.c_char_p` for easier use of C strings.
-``POINTER(c_ubyte)``          ``*``                      Only when encoding. Decoding ``*`` produces :class:`~ctypes.c_char_p` for easier use of C strings.
-:class:`~ctypes.c_wchar`      ``i``                      Only when encoding. Decoding ``i`` produces :class:`~ctypes.c_int`.
-:class:`~ctypes.c_wchar_p`    ``^i``                     Only when encoding. Decoding ``^i`` produces ``POINTER(c_int)``.
-:class:`~ctypes.c_void_p`     ``^v``
-:class:`UnknownPointer`       ``^?``                     This encoding stands for a pointer to a type that cannot be encoded, which in practice means a function pointer.
-:class:`UnknownPointer`       ``^{?}``, ``^(?)``         Only when decoding. These encodings stand for pointers to a structure or union with unknown name and fields.
-:class:`objc_id`              ``@``                      Class name suffixes in the encoding (e. g. ``@"NSString"``) are ignored.
-:class:`objc_block`           ``@?``                     Block signature suffixes in the encoding (e. g. ``@?<v@?>``) are ignored.
-:class:`SEL`                  ``:``
-:class:`Class`                ``#``
-============================= ========================== =====
+========================================= ========================== =====
+`Ctype`                                   Type encoding              Notes
+========================================= ========================== =====
+``None`` (``void``)                       ``v``
+:class:`~ctypes.c_bool`                   ``B``                      This refers to the ``bool`` type from C99 and C++. It is not necessarily the same as the `BOOL` type, which may be either :class:`~ctypes.c_byte` or :class:`~ctypes.c_bool` depending on the system and architecture.
+:class:`~ctypes.c_byte`                   ``c``
+:class:`~ctypes.c_ubyte`                  ``C``
+:class:`~ctypes.c_short`                  ``s``
+:class:`~ctypes.c_ushort`                 ``S``
+:class:`~ctypes.c_long`                   ``l``
+:class:`~ctypes.c_ulong`                  ``L``
+:class:`~ctypes.c_int`                    ``i``                      On 32-bit systems, :class:`~ctypes.c_int` is an alias for :class:`~ctypes.c_long`, and will be encoded as such.
+:class:`~ctypes.c_uint`                   ``I``                      On 32-bit systems, :class:`~ctypes.c_uint` is an alias for :class:`~ctypes.c_ulong`, and will be encoded as such.
+:class:`~ctypes.c_longlong`               ``q``                      On 64-bit systems, :class:`~ctypes.c_longlong` is an alias for :class:`~ctypes.c_long`, and will be encoded as such.
+:class:`~ctypes.c_ulonglong`              ``Q``                      On 64-bit systems, :class:`~ctypes.c_ulonglong` is an alias for :class:`~ctypes.c_ulong`, and will be encoded as such.
+:class:`~ctypes.c_float`                  ``f``
+:class:`~ctypes.c_double`                 ``d``
+:class:`~ctypes.c_longdouble`             ``D``                      On ARM, :class:`~ctypes.c_longdouble` is an alias for :class:`~ctypes.c_double`, and will be encoded as such.
+:class:`~ctypes.c_char`                   ``c``                      Only when encoding. Decoding ``c`` produces :class:`~ctypes.c_byte`, to allow using ``signed char`` as a Boolean value.
+:class:`~ctypes.c_char_p`                 ``*``
+``POINTER(c_char)``                       ``*``                      Only when encoding. Decoding ``*`` produces :class:`~ctypes.c_char_p` for easier use of C strings.
+``POINTER(c_byte)``                       ``*``                      Only when encoding. Decoding ``*`` produces :class:`~ctypes.c_char_p` for easier use of C strings.
+``POINTER(c_ubyte)``                      ``*``                      Only when encoding. Decoding ``*`` produces :class:`~ctypes.c_char_p` for easier use of C strings.
+:class:`~ctypes.c_wchar`                  ``i``                      Only when encoding. Decoding ``i`` produces :class:`~ctypes.c_int`.
+:class:`~ctypes.c_wchar_p`                ``^i``                     Only when encoding. Decoding ``^i`` produces ``POINTER(c_int)``.
+:class:`~ctypes.c_void_p`                 ``^v``
+:class:`UnknownPointer`                   ``^?``                     This encoding stands for a pointer to a type that cannot be encoded, which in practice means a function pointer.
+:class:`UnknownPointer`                   ``^{?}``, ``^(?)``         Only when decoding. These encodings stand for pointers to a structure or union with unknown name and fields.
+:class:`~rubicon.objc.runtime.objc_id`    ``@``                      Class name suffixes in the encoding (e. g. ``@"NSString"``) are ignored.
+:class:`~rubicon.objc.runtime.objc_block` ``@?``                     Block signature suffixes in the encoding (e. g. ``@?<v@?>``) are ignored.
+:class:`~rubicon.objc.runtime.SEL`        ``:``
+:class:`~rubicon.objc.runtime.Class`      ``#``
+========================================= ========================== =====
 
 .. autoclass:: UnknownPointer
 
 In addition, the following types defined by Rubicon are registered, but their encodings may vary depending on the system
 and architecture:
 
 .. hlist::
@@ -313,17 +313,17 @@
 .. autofunction:: get_ctype_for_type_map
 
 Default registered mappings
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The following mappings are registered by default by Rubicon.
 
-===================== =====
-Python type           Ctype
-===================== =====
-:class:`int`          :class:`~ctypes.c_int`
-:class:`float`        :class:`~ctypes.c_float`
-:class:`bool`         :class:`~ctypes.c_bool`
-:class:`bytes`        :class:`~ctypes.c_char_p`
-:class:`ObjCInstance` :class:`objc_id`
-:class:`ObjCClass`    :class:`Class`
-===================== =====
+======================================= =======
+Python type                             `Ctype`
+======================================= =======
+:class:`int`                            :class:`~ctypes.c_int`
+:class:`float`                          :class:`~ctypes.c_float`
+:class:`bool`                           :class:`~ctypes.c_bool`
+:class:`bytes`                          :class:`~ctypes.c_char_p`
+:class:`~rubicon.objc.api.ObjCInstance` :class:`~rubicon.objc.runtime.objc_id`
+:class:`~rubicon.objc.api.ObjCClass`    :class:`~rubicon.objc.runtime.Class`
+======================================= =======
```

### Comparing `rubicon-objc-0.4.5rc1/docs/reference/rubicon-objc.rst` & `rubicon-objc-0.4.6/docs/reference/rubicon-objc.rst`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/docs/tutorial/tutorial-1.rst` & `rubicon-objc-0.4.6/docs/tutorial/tutorial-1.rst`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     >>> from rubicon.objc import ObjCClass
     >>> NSURL = ObjCClass("NSURL")
 
 This gives us an `NSURL` class in Python which is transparently bridged to the
 `NSURL` class in the Objective-C runtime. Any method or property described in
 `Apple's documentation on NSURL
-<https://developer.apple.com/reference/foundation/nsurl?language=objc>`__  can
+<https://developer.apple.com/documentation/foundation/nsurl?language=objc>`__  can
 be accessed over this bridge.
 
 Let's create an instance of an `NSURL` object. The `NSURL` documentation
 describes a static constructor `+URLWithString:`; we can invoke this
 constructor as::
 
     >>> base = NSURL.URLWithString("https://beeware.org/")
```

### Comparing `rubicon-objc-0.4.5rc1/docs/tutorial/tutorial-2.rst` & `rubicon-objc-0.4.6/docs/tutorial/tutorial-2.rst`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 names.
 
 What, no `__init__()`?
 ======================
 
 You'll also notice that our example code *doesn't* have an `__init__()` method
 like you'd normally expect of Python code. As we're defining an Objective-C
-class, we need to follow the Objective-C object lifecycle - which means
+class, we need to follow the Objective-C object life cycle - which means
 defining initializer methods that are visible to the Objective-C runtime, and
 invoking them over that bridge.
 
 Next steps
 ==========
 
 ???
```

### Comparing `rubicon-objc-0.4.5rc1/setup.cfg` & `rubicon-objc-0.4.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -27,43 +27,46 @@
 	LICENSE
 description = A bridge between an Objective C runtime environment and Python.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 
 [options]
 python_requires = >=3.7
-packages = find:
+packages = find_namespace:
 package_dir = 
 	= src
 install_requires = 
 	importlib_metadata >= 4.4; python_version < "3.8"
 
 [options.packages.find]
 where = src
+include = rubicon.*
 
 [options.extras_require]
 dev = 
-	pre-commit == 2.21.0
-	pytest == 7.2.1
+	pre-commit == 2.21.0; python_version < "3.8"
+	pre-commit == 3.2.2; python_version >= "3.8"
+	pytest == 7.3.0
 	pytest-tldr == 0.2.5
 	setuptools_scm[toml] == 7.1.0
-	tox == 4.3.5
+	tox == 4.4.11
 docs = 
-	furo == 2022.12.7
+	furo == 2023.3.27
 	pyenchant == 3.2.2
 	sphinx == 6.1.3
 	sphinx_tabs == 3.4.1
 	sphinx-autobuild == 2021.3.14
-	sphinxcontrib-spelling == 7.7.0
+	sphinxcontrib-spelling == 8.0.0
 
 [flake8]
 exclude = \
 	venv*/*,\
 	local/*,\
 	.tox/*
-max-complexity = 20
-ignore = E203,E266,E501,W503
+max-line-length = 119
+extend-ignore = 
+	E203,
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon/objc/__init__.py` & `rubicon-objc-0.4.6/src/rubicon/objc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     __version__ = get_version("../../..", relative_to=__file__)  # pragma: no cover
 except (ModuleNotFoundError, LookupError):
     # If setuptools_scm isn't in the environment, the call to import will fail.
     # If it *is* in the environment, but the code isn't a git checkout (e.g.,
     # it's been pip installed non-editable) the call to get_version() will fail.
     # If either of these occurs, read version from the installer metadata.
 
-    # importlib.metadata.versoin was added in Python 3.8
+    # importlib.metadata.version was added in Python 3.8
     try:
         from importlib.metadata import version
     except ModuleNotFoundError:
         from importlib_metadata import version
 
     __version__ = version("rubicon-objc")
```

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon/objc/api.py` & `rubicon-objc-0.4.6/src/rubicon/objc/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             restype=self.restype,
             argtypes=self.method_argtypes,
         )
 
         if not convert_result:
             return result
 
-        # Convert result to python type if it is a instance or class pointer.
+        # Convert result to python type if it is an instance or class pointer.
         if self.restype is not None and issubclass(self.restype, objc_id):
             result = ObjCInstance(result)
 
         # Mark for release if we acquire ownership of an object. Do not autorelease here because
         # we might retain a Python reference while the Obj-C reference goes out of scope.
         if self.name.startswith((b"alloc", b"new", b"copy", b"mutableCopy")):
             result._needs_release = True
@@ -256,15 +256,16 @@
             # Add "" to rest to indicate that the method takes arguments
             rest = frozenset(kwargs) | frozenset(("",))
 
         try:
             name, order = self.methods[rest]
         except KeyError:
             raise ValueError(
-                f"No method was found starting with {self.name_start!r} and with keywords {set(kwargs)}\nKnown keywords are:\n"
+                f"No method was found starting with {self.name_start!r} and with keywords {set(kwargs)}\n"
+                f"Known keywords are:\n"
                 + "\n".join(repr(keywords) for keywords in self.methods)
             )
 
         meth = receiver.objc_class._cache_method(name)
         args += [kwargs[name] for name in order]
         return meth(receiver, *args)
 
@@ -389,27 +390,27 @@
     def protocol_register(self, proto_ptr, attr_name):
         name = attr_name.replace("_", ":")
         types = b"".join(encoding_for_ctype(ctype_for_type(tp)) for tp in self.encoding)
         libobjc.protocol_addMethodDescription(proto_ptr, SEL(name), types, True, False)
 
 
 class objc_ivar:
-    """Defines an ivar in a custom Objective-C class.
+    """Defines an ``ivar`` in a custom Objective-C class.
 
     If you want to store additional data on a custom Objective-C class, it is
-    recommended to use properties (:func:`objc_property`) instead of ivars.
+    recommended to use properties (:func:`objc_property`) instead of ``ivars``.
     Properties are a more modern and high-level Objective-C feature, which
     automatically deal with reference counting for objects, and creation of
     getters and setters.
 
-    The ivar type may be any :mod:`ctypes` type.
+    The ``ivar`` type may be any :mod:`ctypes` type.
 
-    Unlike properties, the contents of an ivar cannot be accessed or modified
-    using Python attribute syntax. Instead, the :func:`get_ivar` and
-    :func:`set_ivar` functions need to be used.
+    Unlike properties, the contents of an ``ivar`` cannot be accessed or
+    modified using Python attribute syntax. Instead, the :func:`get_ivar`
+    and :func:`set_ivar` functions need to be used.
     """
 
     def __init__(self, vartype):
         self.vartype = vartype
 
     def class_register(self, class_ptr, attr_name):
         return add_ivar(class_ptr, attr_name, self.vartype)
@@ -433,15 +434,15 @@
     Python types accepted by :func:`~rubicon.objc.types.ctype_for_type`.
 
     Defining a property automatically defines a corresponding getter and setter.
     Following standard Objective-C naming conventions, for a property ``name``
     the getter is called ``name`` and the setter is called ``setName:``.
 
     In a custom Objective-C class, implementations for the getter and setter are
-    also generated, which store the property's value in an ivar called
+    also generated, which store the property's value in an ``ivar`` called
     ``_name``. If the property has an object type, the generated setter keeps
     the stored object retained, and releases it when it is replaced.
 
     In a custom Objective-C protocol, only the metadata for the property is
     generated.
 
     If ``weak`` is ``True``, the property will be created as a weak property.
@@ -478,15 +479,14 @@
         ]
         if self._is_objc_object:
             reference = b"W" if self.weak else b"&"
             attrs.append(objc_property_attribute_t(reference, b""))
         return (objc_property_attribute_t * len(attrs))(*attrs)
 
     def class_register(self, class_ptr, attr_name):
-
         ivar_name = "_" + attr_name
 
         add_ivar(class_ptr, ivar_name, self.vartype)
 
         # Implementation note:
         # 1. Objective-C objects are stored as strong or weak references in the
         #    ivar if the property was declared as strong or weak, respectively.
@@ -515,15 +515,14 @@
             if self.weak and self._is_py_object:
                 # Unpack the Python weakref.
                 value = value()
 
             return value
 
         def _objc_setter(objc_self, _cmd, new_value):
-
             if self._is_py_object and self.weak:
                 # Don't store the object itself but only a Python weakref.
                 new_value = weakref.ref(new_value)
 
             if not isinstance(new_value, self.vartype):
                 # If vartype is a primitive, then new_value may be unboxed. If
                 # that is the case, box it manually.
@@ -571,15 +570,14 @@
             [None, ObjCInstance, SEL, self.vartype],
         )
 
         attrs = self._get_property_attributes()
         libobjc.class_addProperty(class_ptr, ensure_bytes(attr_name), attrs, len(attrs))
 
     def dealloc_callback(self, objc_self, attr_name):
-
         ivar_name = "_" + attr_name
 
         if self._ivar_weak:
             # Clean up weak reference.
             set_ivar(objc_self, ivar_name, self.vartype(None), weak=True)
         elif self._is_objc_object:
             # If the old value is a non-null object, release it. There is no
@@ -887,22 +885,28 @@
                 # case; (b) this flaw exists in pure Python and Objective-C as
                 # well, because default object identity is tied to memory
                 # allocation; and (c) the stale wrapper will *work*, because
                 # it's the correct class.
                 #
                 # Refs #249.
                 if cls == ObjCInstance or isinstance(cls, ObjCInstance):
-                    cached_class_name = ensure_bytes(cached.objc_class.name)
+                    cached_class_name = cached.objc_class.name
                     current_class_name = libobjc.class_getName(
                         libobjc.object_getClass(object_ptr)
-                    )
-                    if cached_class_name != current_class_name:
-                        # There has been a cache hit, but the object is a different class.
-                        # Purge the cache for this address, and treat it as a cache miss.
-                        del cls._cached_objects[object_ptr.value]
+                    ).decode("utf-8")
+                    if (
+                        current_class_name != cached_class_name
+                        and not current_class_name.endswith(f"_{cached_class_name}")
+                    ):
+                        # There has been a cache hit, but the object is a
+                        # different class, treat this as a cache miss. We don't
+                        # *just* look for an *exact* class name match, because
+                        # some Cocoa/UIKit classes undergo a class name change
+                        # between `alloc()` and `init()` (e.g., `NSWindow`
+                        # becomes `NSKVONotifying_NSWindow`). Refs #257.
                         raise KeyError(object_ptr.value)
 
                 return cached
             except KeyError:
                 pass
 
             # If the given pointer points to a class, return an ObjCClass instead (if we're not already creating one).
@@ -959,17 +963,17 @@
         """
         self._needs_release = False
         result = send_message(self, "autorelease", restype=objc_id, argtypes=[])
         return ObjCInstance(result)
 
     def __del__(self):
         """Release the corresponding objc instance if we own it, i.e., if it
-        was returned by by a method starting with 'alloc', 'new', 'copy', or
-        'mutableCopy' and it wasn't already explicitly released by calling
-        :meth:`release` or :meth:`autorelease`."""
+        was returned by a method starting with :meth:`alloc`, :meth:`new`,
+        :meth:`copy`, or :meth:`mutableCopy` and it wasn't already explicitly
+        released by calling :meth:`release` or :meth:`autorelease`."""
         if self._needs_release:
             send_message(self, "release", restype=objc_id, argtypes=[])
 
     def __str__(self):
         """Get a human-readable representation of ``self``.
 
         By default, ``self.description`` converted to a Python string is
@@ -1003,15 +1007,15 @@
         If ``self`` has a Python attribute with the given name, its value is
         returned.
 
         If there is an Objective-C property with the given name, its value is
         returned using its getter method. An attribute is considered a property
         if any of the following are true:
 
-        * A property with the name is present on the class (i. e. declared using
+        * A property with the name is present on the class (i.e. declared using
           ``@property`` in the source code)
         * There is both a getter and setter method for the name
         * The name has been declared as a property using
           :meth:`ObjCClass.declare_property`
 
         Otherwise, a method matching the given name is looked up.
         :class:`ObjCInstance` understands two syntaxes for calling Objective-C
@@ -1027,15 +1031,15 @@
           method. For example, the Objective-C method call ``[self initWithRed:r
           green:g blue:b]`` translates to ``self.initWithRed(r, green=g,
           blue=b)``.
 
         The "interleaved" syntax is usually preferred, since it looks more
         similar to normal Objective-C syntax. However, the "flat" syntax is also
         fully supported. Certain method names require the "flat" syntax, for
-        example if two arguments have the same label (e. g.
+        example if two arguments have the same label (e.g.
         ``performSelector:withObject:withObject:``), which is not supported by
         Python's keyword argument syntax.
 
         .. warning::
 
             The "interleaved" syntax currently ignores the ordering of its
             keyword arguments. However, in the interest of readability, the
@@ -1276,15 +1280,14 @@
 
         # Register any user-defined dealloc method. We treat dealloc differently to
         # inject our own cleanup code for properties, ivars, etc.
 
         user_dealloc = attrs.get("dealloc", None)
 
         def _new_delloc(objc_self, _cmd):
-
             # Invoke user-defined dealloc.
             if user_dealloc:
                 user_dealloc(objc_self, _cmd)
 
             # Invoke dealloc callback of each attribute. Currently
             # defined for properties only.
             for attr_name, obj in attrs.items():
@@ -1538,15 +1541,15 @@
             Such properties cause compatibility issues when accessed from
             Rubicon: ``obj.description()`` works on 10.9 but is a
             :class:`TypeError` on 10.10, whereas ``obj.description`` works on
             10.10 but returns a method object on 10.9. To solve this issue, the
             property can be declared explicitly using
             ``NSObject.declare_property('description')``, so that it can always
             be accessed using ``obj.description``.
-        """  # noqa: E501 # The links in the docstring above are too long to wrap to 120 chars.
+        """
 
         self.forced_properties.add(name)
 
     def declare_class_property(self, name):
         """Declare the class method ``name`` to be a property getter.
 
         This is equivalent to
@@ -1990,15 +1993,14 @@
 # WrappedPyObject itself are only applied after a restart of course.
 
 try:
     WrappedPyObject = ObjCClass("WrappedPyObject")
 except NameError:
 
     class WrappedPyObject(NSObject):
-
         wrapped_pointer = objc_ivar(c_void_p)
 
         @objc_rawmethod
         def initWithObjectId_(self, cmd, address):
             self = send_message(self, "init", restype=objc_id, argtypes=[])
             if self is not None:
                 pyo = cast(address, py_object)
```

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon/objc/collections.py` & `rubicon-objc-0.4.6/src/rubicon/objc/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
     def popitem(self):
         if len(self) == 0:
             raise KeyError(f"popitem(): {type(self).__name__} is empty")
 
         key = self.allKeys().firstObject()
         value = self.objectForKey_(key)
         self.removeObjectForKey_(key)
-        return (key, value)
+        return key, value
 
     def setdefault(self, key, default=None):
         value = self.objectForKey_(key)
         if value is None:
             value = default
         if value is not None:
             self.setObject_forKey_(default, key)
```

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon/objc/ctypes_patch.py` & `rubicon-objc-0.4.6/src/rubicon/objc/ctypes_patch.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon/objc/eventloop.py` & `rubicon-objc-0.4.6/src/rubicon/objc/eventloop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """PEP 3156 event loop based on CoreFoundation."""
 
-import sys
+import contextvars
 import threading
 from asyncio import (
     DefaultEventLoopPolicy,
     SafeChildWatcher,
     coroutines,
     events,
     tasks,
@@ -223,15 +223,15 @@
     # Create a CF-compatible callback for a source event
     def _cf_socket_callback(
         self, cfSocket, callbackType, ignoredAddress, ignoredData, context
     ):
         if self._fd not in self._loop._sockets:
             # Spurious notifications seem to be generated sometimes if you
             # CFSocketDisableCallBacks in the middle of an event.  I don't know
-            # about this FD, any more, so let's get rid of it.
+            # about this FD any more, so let's get rid of it.
             libcf.CFRunLoopRemoveSource(
                 self._loop._cfrunloop, self._src, kCFRunLoopCommonModes
             )
             self._src = None
             return
 
         if callbackType == kCFSocketReadCallBack and self._reader:
@@ -320,29 +320,21 @@
             libcf.CFRunLoopRemoveSource(
                 self._loop._cfrunloop, self._src, kCFRunLoopCommonModes
             )
             libcf.CFSocketInvalidate(self._cf_socket)
 
 
 def context_callback(context, callback):
-    # Python 3.7 introduced the idea of context variables.
-    # asyncio.call_{at,later,soon} need to run any callbacks
-    # *inside* the context provided.
-    if sys.version_info >= (3, 7):
-        import contextvars
-
-        if context is None:
-            context = contextvars.copy_context()
-
-        def _callback(*args):
-            context.run(callback, *args)
-
-        return _callback
-    else:
-        return callback
+    if context is None:
+        context = contextvars.copy_context()
+
+    def _callback(*args):
+        context.run(callback, *args)
+
+    return _callback
 
 
 class CFEventLoop(unix_events.SelectorEventLoop):
     def __init__(self, lifecycle=None):
         self._lifecycle = lifecycle
         self._cfrunloop = libcf.CFRetain(libcf.CFRunLoopGetCurrent())
         self._running = False
@@ -739,27 +731,27 @@
         libcf.CFRunLoopRun()
 
     def stop(self):
         libcf.CFRunLoopStop(self._cfrunloop)
 
 
 class CocoaLifecycle:
-    """A lifecycle manager for Cocoa (``NSApplication``) apps."""
+    """A life cycle manager for Cocoa (``NSApplication``) apps."""
 
     def __init__(self, application):
         self._application = application
 
     def start(self):
         self._application.run()
 
     def stop(self):
         self._application.terminate(None)
 
 
 class iOSLifecycle:
-    """A lifecycle manager for iOS (``UIApplication``) apps."""
+    """A life cycle manager for iOS (``UIApplication``) apps."""
 
     def start(self):
         libcf.CFRunLoopRun()
 
     def stop(self):
         libcf.CFRunLoopStop(libcf.CFRunLoopGetMain())
```

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon/objc/runtime.py` & `rubicon-objc-0.4.6/src/rubicon/objc/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,27 +77,27 @@
 def load_library(name):
     """Load and return the C library with the given name.
 
     If the library could not be found, a :class:`ValueError` is raised.
 
     Internally, this function uses :func:`ctypes.util.find_library` to search
     for the library in the system-standard locations. If the library cannot be
-    found this way, it is attempted to load the library from certain hardcoded
+    found this way, it is attempted to load the library from certain hard-coded
     locations, as a fallback for systems where ``find_library`` does not work
     (such as iOS).
     """
 
     path = util.find_library(name)
     if path is not None:
         return CDLL(path)
 
     # On iOS (and probably also watchOS and tvOS), ctypes.util.find_library
     # doesn't work and always returns None. This is because the sandbox hides
     # all system libraries from the filesystem and pretends they don't exist.
-    # However they can still be loaded if the path is known, so we try to load
+    # However, they can still be loaded if the path is known, so we try to load
     # the library from a few known locations.
 
     for loc in _lib_path:
         try:
             return CDLL(os.path.join(loc, "lib" + name + ".dylib"))
         except OSError:
             pass
@@ -190,15 +190,15 @@
 class Class(objc_id):
     """The `Class <https://developer.apple.com/documentation/objectivec/class?language=objc>`__
     type from ``<objc/objc.h>``.
     """
 
 
 class IMP(c_void_p):
-    """The `IMP <https://developer.apple.com/documentation/objectivec/objective_c_runtime/imp?language=objc>`__
+    """The `IMP <https://developer.apple.com/documentation/objectivec/objective-c_runtime/imp?language=objc>`__
     type from ``<objc/objc.h>``.
 
     An :class:`IMP` cannot be called directly --- it must be cast to the
     correct :func:`~ctypes.CFUNCTYPE` first, to provide the necessary
     information about its signature.
     """
 
@@ -220,15 +220,15 @@
     type from ``<objc/runtime.h>``.
     """
 
 
 class objc_property_attribute_t(Structure):
     """The `objc_property_attribute_t <https://developer.apple.com/documentation/objectivec/objc_property_attribute_t?language=objc>`__
     structure from ``<objc/runtime.h>``.
-    """
+    """  # noqa: E501
 
     _fields_ = [
         ("name", c_char_p),
         ("value", c_char_p),
     ]
 
 
@@ -541,15 +541,15 @@
 
 ######################################################################
 
 
 class objc_method_description(Structure):
     """The `objc_method_description <https://developer.apple.com/documentation/objectivec/objc_method_description?language=objc>`__
     structure from ``<objc/runtime.h>``.
-    """
+    """  # noqa: E501
 
     _fields_ = [
         ("name", SEL),
         ("types", c_char_p),
     ]
 
 
@@ -733,20 +733,20 @@
         if should_use_fpret(restype):
             send_name = "objc_msgSend_fpret"
         elif should_use_stret(restype):
             send_name = "objc_msgSend_stret"
         else:
             send_name = "objc_msgSend"
 
-        # Looking up a C function via attribute access (e. g.
+        # Looking up a C function via attribute access (e.g.
         # libobjc.objc_msgSend) always returns the same function object. Because
         # we need to set the function object's restype and argtypes, this would
         # not be thread safe, and it also makes it impossible to cache multiple
         # differently configured copies of the same function like we do here.
-        # Instead, we look up the C function using subscript syntax (e. g.
+        # Instead, we look up the C function using subscript syntax (e.g.
         # libobjc['objc_msgSend']), which returns a new function object every
         # time.
         send = libobjc[send_name]
         send.restype = restype
         send.argtypes = [objc_id, SEL] + argtypes
 
         # Cache the fully set up objc_msgSend function object to speed up future calls with the same types.
@@ -757,67 +757,68 @@
 def send_message(receiver, selector, *args, restype, argtypes=None, varargs=None):
     """Call a method on the receiver with the given selector and arguments.
 
     This is the equivalent of an Objective-C method call like ``[receiver sel:args]``.
 
     .. note::
 
-        Some Objective-C methods take variadic arguments (varargs), for example
+        Some Objective-C methods take variadic arguments (``varargs``), for example
         `+[NSString stringWithFormat:] <https://developer.apple.com/documentation/foundation/nsstring/1497275-stringwithformat?language=objc>`_.
         When using :func:`send_message`, variadic arguments are treated
         differently from regular arguments: they are not passed as normal
         function arguments in ``*args``, but as a list in a separate ``varargs``
         keyword argument.
 
         This explicit separation of regular and variadic arguments protects
         against accidentally passing too many arguments into a method. By
-        default these extra arguments would be considered varargs and passed on
-        to the method, even if the method in question doesn't take varargs.
+        default these extra arguments would be considered ``varargs`` and passed on
+        to the method, even if the method in question doesn't take ``varargs``.
         Because of how the Objective-C runtime and most C calling conventions
         work, this error would otherwise be silently ignored.
 
-        The types of varargs are not included in the ``argtypes`` list. Instead,
+        The types of ``varargs`` are not included in the ``argtypes`` list. Instead,
         the values are automatically converted to C types using the default
-        :mod:`ctypes` argument conversion rules. To ensure that all varargs are
+        :mod:`ctypes` argument conversion rules. To ensure that all ``varargs`` are
         converted to the expected C types, it is recommended to manually convert
-        all varargs to :mod:`ctypes` types instead of relying on automatic
+        all ``varargs`` to :mod:`ctypes` types instead of relying on automatic
         conversions. For example:
 
         .. code-block:: python
 
             send_message(
                 NSString,
                 "stringWithFormat:",
                 at("%i %s %@"),
                 restype=objc_id,
                 argtypes=[objc_id],
                 varargs=[c_int(123), cast(b"C string", c_char_p), at("ObjC string")],
             )
 
     :param receiver: The object on which to call the method, as an
-        :class:`ObjCInstance` or :class:`objc_id`.
+        :class:`~rubicon.objc.api.ObjCInstance` or :class:`.objc_id`.
     :param selector: The name of the method as a :class:`str`, :class:`bytes`,
         or :class:`SEL`.
     :param args: The method arguments.
     :param restype: The return type of the method.
     :param argtypes: The argument types of the method, as a :class:`list`.
         Defaults to ``[]``.
     :param varargs: Variadic arguments for the method, as a :class:`list`.
         Defaults to ``[]``. These arguments are converted according to the
         default :mod:`ctypes` conversion rules.
-    """
+    """  # noqa: E501
 
     try:
         receiver = receiver._as_parameter_
     except AttributeError:
         pass
 
     if not isinstance(receiver, objc_id):
         raise TypeError(
-            f"Receiver must be an ObjCInstance or objc_id, not {type(receiver).__module__}.{type(receiver).__qualname__}"
+            f"Receiver must be an ObjCInstance or objc_id, "
+            f"not {type(receiver).__module__}.{type(receiver).__qualname__}"
         )
 
     if not isinstance(selector, SEL):
         selector = SEL(selector)
 
     if argtypes is None:
         argtypes = []
@@ -831,17 +832,20 @@
         )
 
     send = _msg_send_for_types(restype, argtypes)
 
     try:
         result = send(receiver, selector, *args, *varargs)
     except ArgumentError as error:
-        # Add more useful info to argument error exceptions, then reraise.
-        error.args = f"{error.args[0]} (selector = {selector}, argtypes = {argtypes})"
-        raise
+        # Add more useful info to the default error message, then reraise.
+        err = error.args[0]
+        sel = selector.name.decode(errors="backslashreplace")
+        valid_args = ", ".join(t.__name__ for t in argtypes)
+        error.args = [f"{sel} {err}; argtypes: {valid_args}"]
+        raise error
 
     if restype == c_void_p:
         result = c_void_p(result)
     return result
 
 
 class objc_super(Structure):
@@ -887,17 +891,18 @@
 
     Although it is possible to pass other values than ``__class__`` and
     ``self`` for the first two parameters, this is strongly discouraged. Doing
     so is not supported by the Objective-C language, and relies on
     implementation details of the superclasses.
 
     :param cls: The class in whose context the ``super`` call is happening, as
-        an :class:`ObjCClass` or :class:`Class`.
+        an :class:`~rubicon.objc.api.ObjCClass` or :class:`Class`.
     :param receiver: The object on which to call the method, as an
-        :class:`ObjCInstance`, :class:`objc_id`, or :class:`~ctypes.c_void_p`.
+        :class:`~rubicon.objc.api.ObjCInstance`, :class:`.objc_id`, or
+        :class:`~ctypes.c_void_p`.
     :param selector: The name of the method as a :class:`str`, :class:`bytes`,
         or :class:`SEL`.
     :param args: The method arguments.
     :param restype: The return type of the method.
     :param argtypes: The argument types of the method, as a :class:`list`.
         Defaults to ``[]``.
     :param varargs: Variadic arguments for the method, as a :class:`list`.
@@ -994,15 +999,15 @@
 
 def add_method(cls, selector, method, encoding, replace=False):
     """Add a new instance method to the given class.
 
     To add a class method, add an instance method to the metaclass.
 
     :param cls: The Objective-C class to which to add the method, as an
-        :class:`ObjCClass` or :class:`Class`.
+        :class:`~rubicon.objc.api.ObjCClass` or :class:`Class`.
     :param selector: The name for the new method, as a :class:`str`,
         :class:`bytes`, or :class:`SEL`.
     :param method: The method implementation, as a Python callable or a C
         function address.
     :param encoding: The method's signature (return type and argument types) as
         a :class:`list`. The types of the implicit ``self`` and ``_cmd``
         parameters must be included in the signature.
@@ -1037,38 +1042,38 @@
             raise ValueError(f"A method with the name {selector.name!r} already exists")
 
     _keep_alive_imps.append(imp)
     return imp
 
 
 def add_ivar(cls, name, vartype):
-    """Add a new instance variable of type vartype to cls."""
+    """Add a new instance variable of type ``vartype`` to ``cls``."""
 
     return libobjc.class_addIvar(
         cls,
         ensure_bytes(name),
         sizeof(vartype),
         alignment(vartype),
         encoding_for_ctype(ctype_for_type(vartype)),
     )
 
 
 def get_ivar(obj, varname, weak=False):
-    """Get the value of obj's ivar named varname.
+    """Get the value of obj's ``ivar`` named ``varname``.
 
     The returned object is a :mod:`ctypes` data object.
 
-    For non-object types (everything except :class:`objc_id` and subclasses),
-    the returned data object is backed by the ivar's actual memory. This means
+    For non-object types (everything except :class:`.objc_id` and subclasses),
+    the returned data object is backed by the ``ivar``'s actual memory. This means
     that the data object is only usable as long as the "owner" object is alive,
-    and writes to it will directly change the ivar's value.
+    and writes to it will directly change the ``ivar``'s value.
 
-    For object types, the returned data object is independent of the ivar's
-    memory. This is because object ivars may be weak, and thus cannot always be
-    accessed directly by their address.
+    For object types, the returned data object is independent of the ``ivar``'s
+    memory. This is because object ``ivars`` may be weak, and thus cannot always
+    be accessed directly by their address.
     """
 
     try:
         obj = obj._as_parameter_
     except AttributeError:
         pass
 
@@ -1083,19 +1088,19 @@
     elif issubclass(vartype, objc_id):
         return cast(libobjc.object_getIvar(obj, ivar), vartype)
     else:
         return vartype.from_address(obj.value + libobjc.ivar_getOffset(ivar))
 
 
 def set_ivar(obj, varname, value, weak=False):
-    """Set obj's ivar varname to value. If ``weak`` is ``True``, only a weak
+    """Set obj's ``ivar`` ``varname`` to value. If ``weak`` is ``True``, only a weak
     reference to the value is stored.
 
     value must be a :mod:`ctypes` data object whose type matches that of
-    the ivar.
+    the ``ivar``.
     """
 
     try:
         obj = obj._as_parameter_
     except AttributeError:
         pass
```

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon/objc/types.py` & `rubicon-objc-0.4.6/src/rubicon/objc/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
 
 __LP64__ = 8 * struct.calcsize("P") == 64
 
 # platform.processor() describes the CPU on which the code is running.
 #   * On a 64-bit Intel machine it is always "x86_64", even if Python is built as 32-bit.
 #   * M1 MacBooks return "arm"
 #   * iPhones (as of the late 2022 support packages) return "arm64"
-# This *wont'* work on older iOS support builds, as it relies on the customized
-# platform values added in https://github.com/beeware/Python-Apple-support/commit/2f42105838ab8f6f7e703ddb929d97758a36145e
+# This *won't* work on older iOS support builds, as it relies on the customized
+# platform values added in https://github.com/beeware/Python-Apple-support/commit/2f42105838ab8f6f7e703ddb929d97758a36145e  # noqa: E501
 _processor = platform.processor()
 _any_x86 = _processor in ("i386", "x86_64")
 __i386__ = _any_x86 and not __LP64__
 __x86_64__ = _any_x86 and __LP64__
 
 if _processor:
     _any_arm = _processor.startswith("arm")
@@ -119,40 +119,41 @@
     bool: c_bool,
     bytes: c_char_p,
     object: py_object,
 }
 
 
 def ctype_for_type(tp):
-    """Look up the ctype corresponding to the given Python type.
+    """Look up the C type corresponding to the given Python type.
 
-    This conversion is applied to types used in :class:`objc_method`
-    signatures, :class:`objc_ivar` types, etc. This function translates
+    This conversion is applied to types used in
+    :class:`~rubicon.objc.api.objc_method` signatures,
+    :class:`~rubicon.objc.api.objc_ivar` types, etc. This function translates
     Python built-in types and :mod:`rubicon.objc` classes to their
-    :mod:`ctypes` equivalents. Unregistered types (including types that
-    are already ctypes) are returned unchanged.
+    :mod:`ctypes` equivalents. Unregistered types (including types that are
+    already ctypes) are returned unchanged.
     """
 
     return _ctype_for_type_map.get(tp, tp)
 
 
 def register_ctype_for_type(tp, ctype):
-    """Register a conversion from a Python type to a ctype."""
+    """Register a conversion from a Python type to a C type."""
 
     _ctype_for_type_map[tp] = ctype
 
 
 def unregister_ctype_for_type(tp):
-    """Unregister a conversion from a Python type to a ctype."""
+    """Unregister a conversion from a Python type to a C type."""
 
     del _ctype_for_type_map[tp]
 
 
 def get_ctype_for_type_map():
-    """Get a copy of all currently registered type-to-ctype conversions as a
+    """Get a copy of all currently registered type-to-C type conversions as a
     mapping."""
 
     return dict(_ctype_for_type_map)
 
 
 _ctype_for_encoding_map = {}
 _encoding_for_ctype_map = {}
@@ -336,22 +337,22 @@
     elif encoding.startswith(b"A"):
         raise ValueError(f"Atomic types are not supported by ctypes: {encoding}")
     else:
         raise ValueError(f"Unknown encoding: {encoding}")
 
 
 def ctype_for_encoding(encoding):
-    """Return the ctype corresponding to an Objective-C type encoding.
+    """Return the C type corresponding to an Objective-C type encoding.
 
-    If a ctype has been registered for the encoding, that type is returned.
+    If a C type has been registered for the encoding, that type is returned.
     Otherwise, if the type encoding represents a compound type (pointer, array,
     structure, or union), the contained types are converted recursively. A new
-    ctype is then created from the converted ctypes, and is registered for the
-    encoding (so that future conversions of the same encoding return the same
-    ctype).
+    C type is then created from the converted ctypes, and is registered for
+    the encoding (so that future conversions of the same encoding return the
+    same C type).
 
     For example, the type encoding ``{spam=ic}`` is not registered by default.
     However, the contained types ``i`` and ``c`` are registered, so they are
     converted individually and used to create a new :class:`~ctypes.Structure`
     with two fields of the correct types. The new structure type is then
     registered for the original encoding ``{spam=ic}`` and returned.
 
@@ -368,17 +369,17 @@
     except KeyError:
         return _ctype_for_unknown_encoding(encoding)
 
 
 def encoding_for_ctype(ctype):
     """Return the Objective-C type encoding for the given ctypes type.
 
-    If a type encoding has been registered for the ctype, that encoding is
-    returned. Otherwise, if the ctype is a pointer type, its pointed-to type is
-    encoded and used to construct the pointer type encoding.
+    If a type encoding has been registered for the C type, that encoding is
+    returned. Otherwise, if the C type is a pointer type, its pointed-to type
+    is encoded and used to construct the pointer type encoding.
 
     Automatic encoding of other compound types (arrays, structures, and unions)
     is currently not supported. To encode such types, a type encoding must be
     manually provided for them using :func:`register_preferred_encoding` or
     :func:`register_encoding`.
 
     :raises ValueError: if the conversion fails at any point
@@ -391,140 +392,140 @@
             return b"^" + encoding_for_ctype(ctype._type_)
         except KeyError:
             raise ValueError(f"No type encoding known for ctype {ctype}")
 
 
 def register_preferred_encoding(encoding, ctype):
     """Register a preferred conversion between an Objective-C type encoding and
-    a ctype.
+    a C type.
 
     "Preferred" means that any existing conversions in each direction are
     overwritten with the new conversion. To register an encoding without
     overwriting existing conversions, use :func:`register_encoding`.
     """
 
     _ctype_for_encoding_map[encoding] = ctype
     _encoding_for_ctype_map[ctype] = encoding
 
 
 def with_preferred_encoding(encoding):
     """Register a preferred conversion between an Objective-C type encoding and
-    the decorated ctype.
+    the decorated C type.
 
     This is equivalent to calling :func:`register_preferred_encoding` on the
-    decorated ctype.
+    decorated C type.
     """
 
     def _with_preferred_encoding_decorator(ctype):
         register_preferred_encoding(encoding, ctype)
         return ctype
 
     return _with_preferred_encoding_decorator
 
 
 def register_encoding(encoding, ctype):
     """Register an additional conversion between an Objective-C type encoding
-    and a ctype.
+    and a C type.
 
     "Additional" means that any existing conversions in either direction are
     *not* overwritten with the new conversion. To register an encoding and
     overwrite existing conversions, use :func:`register_preferred_encoding`.
     """
 
     _ctype_for_encoding_map.setdefault(encoding, ctype)
     _encoding_for_ctype_map.setdefault(ctype, encoding)
 
 
 def with_encoding(encoding):
     """Register an additional conversion between an Objective-C type encoding
-    and the decorated ctype.
+    and the decorated C type.
 
     This is equivalent to calling :func:`register_encoding` on the
-    decorated ctype.
+    decorated C type.
     """
 
     def _with_encoding_decorator(ctype):
         register_encoding(encoding, ctype)
         return ctype
 
     return _with_encoding_decorator
 
 
 def unregister_encoding(encoding):
     """Unregister the conversion from an Objective-C type encoding to its
-    corresponding ctype.
+    corresponding C type.
 
     Note that this does not remove any conversions in the other direction (from
-    a ctype to this encoding). These conversions may be replaced with
+    a C type to this encoding). These conversions may be replaced with
     :func:`register_encoding`, or unregistered with :func:`unregister_ctype`. To
     remove all ctypes for an encoding, use :func:`unregister_encoding_all`.
 
     If the encoding was not registered previously, nothing happens.
     """
 
     _ctype_for_encoding_map.pop(encoding, None)
 
 
 def unregister_encoding_all(encoding):
     """Unregister all conversions between an Objective-C type encoding and all
     corresponding ctypes.
 
-    All conversions from any ctype to this encoding are removed recursively
+    All conversions from any C type to this encoding are removed recursively
     using :func:`unregister_ctype_all`.
 
     If the encoding was not registered previously, nothing happens.
     """
 
     _ctype_for_encoding_map.pop(encoding, None)
     for ct, enc in list(_encoding_for_ctype_map.items()):
         if enc == encoding:
             unregister_ctype_all(ct)
 
 
 def unregister_ctype(ctype):
-    """Unregister the conversion from a ctype to its corresponding Objective-C
-    type encoding.
+    """Unregister the conversion from a C type to its corresponding
+    Objective-C type encoding.
 
     Note that this does not remove any conversions in the other direction (from
-    an encoding to this ctype). These conversions may be replaced with
+    an encoding to this C type). These conversions may be replaced with
     :func:`register_encoding`, or unregistered with :func:`unregister_encoding`.
-    To remove all encodings for a ctype, use :func:`unregister_ctype_all`.
+    To remove all encodings for a C type, use :func:`unregister_ctype_all`.
 
-    If the ctype was not registered previously, nothing happens.
+    If the C type was not registered previously, nothing happens.
     """
 
     _encoding_for_ctype_map.pop(ctype, default=None)
 
 
 def unregister_ctype_all(ctype):
-    """Unregister all conversions between a ctype and all corresponding
+    """Unregister all conversions between a C type and all corresponding
     Objective-C type encodings.
 
-    All conversions from any type encoding to this ctype are removed recursively
-    using :func:`unregister_encoding_all`.
+    All conversions from any type encoding to this C type are removed
+    recursively using :func:`unregister_encoding_all`.
 
-    If the ctype was not registered previously, nothing happens.
+    If the C type was not registered previously, nothing happens.
     """
 
     _encoding_for_ctype_map.pop(ctype, default=None)
     for enc, ct in list(_ctype_for_encoding_map.items()):
         if ct == ctype:
             unregister_encoding_all(enc)
 
 
 def get_ctype_for_encoding_map():
-    """Get a copy of all currently registered encoding-to-ctype conversions as
-    a map."""
+    """Get a copy of all currently registered encoding-to-C type conversions
+    as a map."""
 
     return dict(_ctype_for_encoding_map)
 
 
 def get_encoding_for_ctype_map():
-    """Get a copy of all currently registered ctype-to-encoding conversions as
-    a map."""
+    """Get a copy of all currently registered C type-to-encoding conversions
+    as a map."""
 
     return dict(_encoding_for_ctype_map)
 
 
 def split_method_encoding(encoding):
     """Split a method signature encoding into a sequence of type encodings.
```

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon_objc.egg-info/PKG-INFO` & `rubicon-objc-0.4.6/src/rubicon_objc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubicon-objc
-Version: 0.4.5rc1
+Version: 0.4.6
 Summary: A bridge between an Objective C runtime environment and Python.
 Home-page: https://beeware.org/rubicon
 Author: Russell Keith-Magee
 Author-email: russell@keith-magee.com
 License: New BSD
 Project-URL: Funding, https://beeware.org/contributing/membership/
 Project-URL: Documentation, https://rubicon-objc.readthedocs.io/en/latest/
```

### Comparing `rubicon-objc-0.4.5rc1/src/rubicon_objc.egg-info/SOURCES.txt` & `rubicon-objc-0.4.6/src/rubicon_objc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 README.rst
 pyproject.toml
 setup.cfg
 tox.ini
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/dependabot-changenote.yml
+.github/workflows/pre-commit-update.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 changes/.gitignore
 changes/template.rst
 docs/Makefile
 docs/conf.py
 docs/index.rst
@@ -48,15 +49,14 @@
 docs/reference/rubicon-objc-eventloop.rst
 docs/reference/rubicon-objc-runtime.rst
 docs/reference/rubicon-objc-types.rst
 docs/reference/rubicon-objc.rst
 docs/tutorial/index.rst
 docs/tutorial/tutorial-1.rst
 docs/tutorial/tutorial-2.rst
-src/rubicon/__init__.py
 src/rubicon/objc/__init__.py
 src/rubicon/objc/api.py
 src/rubicon/objc/collections.py
 src/rubicon/objc/ctypes_patch.py
 src/rubicon/objc/eventloop.py
 src/rubicon/objc/runtime.py
 src/rubicon/objc/types.py
@@ -69,14 +69,16 @@
 tests/test_NSArray.py
 tests/test_NSDictionary.py
 tests/test_NSString.py
 tests/test_async.py
 tests/test_blocks.py
 tests/test_core.py
 tests/test_ctypes_patch.py
+tests/objc/Altered_Example.h
+tests/objc/Altered_Example.m
 tests/objc/BaseExample.h
 tests/objc/BaseExample.m
 tests/objc/Blocks.h
 tests/objc/Blocks.m
 tests/objc/Callback.h
 tests/objc/DescriptionTester.h
 tests/objc/DescriptionTester.m
```

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/BaseExample.h` & `rubicon-objc-0.4.6/tests/objc/BaseExample.h`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/BaseExample.m` & `rubicon-objc-0.4.6/tests/objc/BaseExample.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/Blocks.h` & `rubicon-objc-0.4.6/tests/objc/Blocks.h`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/Blocks.m` & `rubicon-objc-0.4.6/tests/objc/Blocks.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/DescriptionTester.m` & `rubicon-objc-0.4.6/tests/objc/DescriptionTester.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/Example.h` & `rubicon-objc-0.4.6/tests/objc/Example.h`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 +(int) staticIntField;
 +(void) setStaticIntField: (int) v;
 
 +(int) accessStaticIntField;
 +(void) mutateStaticIntFieldWithValue: (int) v;
 
 -(id) init;
+-(id) initWithClassChange;
 -(id) initWithIntValue: (int) v;
 -(id) initWithBaseIntValue: (int) b intValue: (int) v;
 
 -(int) accessIntField;
 -(void) mutateIntFieldWithValue: (int) v;
 
 -(void) setSpecialValue: (int) v;
```

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/Example.m` & `rubicon-objc-0.4.6/tests/objc/Example.m`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #import "Example.h"
+#import "Altered_Example.h"
 #import <stdio.h>
+#import <objc/runtime.h>
 
 NSString *const SomeGlobalStringConstant = @"Some global string constant";
 
 @implementation Example
 
 @synthesize intField = _intField;
 @synthesize thing = _thing;
@@ -56,14 +58,27 @@
     if (self) {
         [self setIntField:33];
     }
     _ambiguous = 42;
     return self;
 }
 
+-(id) initWithClassChange
+{
+    self = [super initWithIntValue:44];
+
+    if (self) {
+        [self setIntField:55];
+    }
+    _ambiguous = 37;
+
+    object_setClass(self, [Altered_Example class]);
+    return self;
+}
+
 -(id) initWithIntValue: (int) v
 {
     self = [super initWithIntValue:44];
 
     if (self) {
         [self setIntField:v];
     }
```

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/Makefile` & `rubicon-objc-0.4.6/tests/objc/Makefile`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/objc/Thing.m` & `rubicon-objc-0.4.6/tests/objc/Thing.m`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/test_NSArray.py` & `rubicon-objc-0.4.6/tests/test_NSArray.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/test_NSDictionary.py` & `rubicon-objc-0.4.6/tests/test_NSDictionary.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/test_NSString.py` & `rubicon-objc-0.4.6/tests/test_NSString.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/test_async.py` & `rubicon-objc-0.4.6/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/test_blocks.py` & `rubicon-objc-0.4.6/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `rubicon-objc-0.4.5rc1/tests/test_core.py` & `rubicon-objc-0.4.6/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import functools
 import gc
 import math
+import sys
 import threading
 import unittest
 import weakref
 from ctypes import (
+    ArgumentError,
     Structure,
     byref,
     c_char,
     c_double,
     c_float,
     c_int,
     c_void_p,
@@ -331,15 +333,15 @@
             issubclass(object(), NSSecureCoding)
         with self.assertRaises(TypeError):
             issubclass(object, NSSecureCoding)
         with self.assertRaises(TypeError):
             issubclass(NSObject.new(), NSSecureCoding)
 
     def test_field(self):
-        "A field on an instance can be accessed and mutated"
+        """A field on an instance can be accessed and mutated"""
 
         Example = ObjCClass("Example")
 
         obj = Example.alloc().init()
 
         self.assertEqual(obj.baseIntField, 22)
         self.assertEqual(obj.intField, 33)
@@ -347,15 +349,15 @@
         obj.baseIntField = 8888
         obj.intField = 9999
 
         self.assertEqual(obj.baseIntField, 8888)
         self.assertEqual(obj.intField, 9999)
 
     def test_method(self):
-        "An instance method can be invoked."
+        """An instance method can be invoked."""
         Example = ObjCClass("Example")
 
         obj = Example.alloc().init()
 
         self.assertEqual(obj.accessBaseIntField(), 22)
         self.assertEqual(obj.accessIntField(), 33)
 
@@ -377,14 +379,33 @@
 
         with self.assertRaises(TypeError):
             obj.mutateIntFieldWithValue_()
 
         with self.assertRaises(TypeError):
             obj.mutateIntFieldWithValue_(123, "extra argument")
 
+    def test_method_incorrect_argument_type(self):
+        """Attempting to call a method with the wrong type of argument throws an exception."""
+
+        Example = ObjCClass("Example")
+        obj = Example.alloc().init()
+
+        with self.assertRaisesRegex(
+            ArgumentError,
+            r"mutateIntFieldWithValue: argument 3: "
+            + (
+                r"TypeError: 'float' object cannot be interpreted as an integer; argtypes: c_int"
+                if sys.version_info >= (3, 12)
+                else r"TypeError: wrong type; argtypes: c_int"
+                if sys.version_info >= (3, 10)
+                else r"<class 'TypeError'>: wrong type; argtypes: c_int"
+            ),
+        ):
+            obj.mutateIntFieldWithValue_(1.234)
+
     def test_method_incorrect_argument_count_send(self):
         """Attempting to call a method with send_message with an incorrect
         number of arguments throws an exception."""
 
         Example = ObjCClass("Example")
         obj = Example.alloc().init()
 
@@ -421,15 +442,15 @@
             argtypes=[objc_id],
         )
         self.assertEqual(
             str(ObjCInstance(formatted)), "This is a string with placeholders"
         )
 
     def test_method_send(self):
-        "An instance method can be invoked with send_message."
+        """An instance method can be invoked with send_message."""
         Example = ObjCClass("Example")
 
         obj = Example.alloc().init()
 
         self.assertEqual(
             send_message(obj, "accessBaseIntField", restype=c_int, argtypes=[]), 22
         )
@@ -545,15 +566,15 @@
             argtypes=[c_int],
             restype=None,
         )
 
         self.assertEqual(obj.accessBaseIntField(), 11)
 
     def test_static_field(self):
-        "A static field on a class can be accessed and mutated"
+        """A static field on a class can be accessed and mutated"""
         Example = ObjCClass("Example")
 
         Example.mutateStaticBaseIntFieldWithValue_(1)
         Example.mutateStaticIntFieldWithValue_(11)
 
         self.assertEqual(Example.staticBaseIntField, 1)
         self.assertEqual(Example.staticIntField, 11)
@@ -561,25 +582,25 @@
         Example.staticBaseIntField = 1188
         Example.staticIntField = 1199
 
         self.assertEqual(Example.staticBaseIntField, 1188)
         self.assertEqual(Example.staticIntField, 1199)
 
     def test_static_method(self):
-        "A static method on a class can be invoked."
+        """A static method on a class can be invoked."""
         Example = ObjCClass("Example")
 
         Example.mutateStaticBaseIntFieldWithValue_(2288)
         Example.mutateStaticIntFieldWithValue_(2299)
 
         self.assertEqual(Example.accessStaticBaseIntField(), 2288)
         self.assertEqual(Example.accessStaticIntField(), 2299)
 
     def test_mutator_like_method(self):
-        "A method that looks like a mutator doesn't confuse issues."
+        """A method that looks like a mutator doesn't confuse issues."""
         Example = ObjCClass("Example")
 
         obj1 = Example.alloc().init()
 
         # setSpecialValue: looks like it might be a mutator
         # for a specialValue property, but this property doesn't exist.
 
@@ -593,15 +614,15 @@
         # ...until you set it explicitly...
         obj1.specialValue = 37
 
         # ...at which point it's fair game to be retrieved.
         self.assertEqual(obj1.specialValue, 37)
 
     def test_property_forcing(self):
-        "An instance or property method can be explicitly declared as a property."
+        """An instance or property method can be explicitly declared as a property."""
         Example = ObjCClass("Example")
         Example.declare_class_property("classMethod")
         Example.declare_class_property("classAmbiguous")
         Example.declare_property("instanceMethod")
         Example.declare_property("instanceAmbiguous")
 
         # A class method can be turned into a property
@@ -624,67 +645,67 @@
         NSBundle = ObjCClass("NSBundle")
         NSBundle.declare_class_property("mainBundle")
         self.assertFalse(
             callable(NSBundle.mainBundle), "NSBundle.mainBundle should not be a method"
         )
 
     def test_non_existent_field(self):
-        "An attribute error is raised if you invoke a non-existent field."
+        """An attribute error is raised if you invoke a non-existent field."""
         Example = ObjCClass("Example")
 
         obj1 = Example.alloc().init()
 
         # Non-existent fields raise an error.
         with self.assertRaises(AttributeError):
             obj1.field_doesnt_exist
 
         # Cache warming doesn't affect anything.
         with self.assertRaises(AttributeError):
             obj1.field_doesnt_exist
 
     def test_non_existent_method(self):
-        "An attribute error is raised if you invoke a non-existent method."
+        """An attribute error is raised if you invoke a non-existent method."""
         Example = ObjCClass("Example")
 
         obj1 = Example.alloc().init()
 
         # Non-existent methods raise an error.
         with self.assertRaises(AttributeError):
             obj1.method_doesnt_exist()
 
         # Cache warming doesn't affect anything.
         with self.assertRaises(AttributeError):
             obj1.method_doesnt_exist()
 
     def test_non_existent_static_field(self):
-        "An attribute error is raised if you invoke a non-existent static field."
+        """An attribute error is raised if you invoke a non-existent static field."""
         Example = ObjCClass("Example")
 
         # Non-existent fields raise an error.
         with self.assertRaises(AttributeError):
             Example.static_field_doesnt_exist
 
         # Cache warming doesn't affect anything.
         with self.assertRaises(AttributeError):
             Example.static_field_doesnt_exist
 
     def test_non_existent_static_method(self):
-        "An attribute error is raised if you invoke a non-existent static method."
+        """An attribute error is raised if you invoke a non-existent static method."""
         Example = ObjCClass("Example")
 
         # Non-existent methods raise an error.
         with self.assertRaises(AttributeError):
             Example.static_method_doesnt_exist()
 
         # Cache warming doesn't affect anything.
         with self.assertRaises(AttributeError):
             Example.static_method_doesnt_exist()
 
     def test_polymorphic_constructor(self):
-        "Check that the right constructor is activated based on arguments used"
+        """Check that the right constructor is activated based on arguments used"""
         Example = ObjCClass("Example")
 
         obj1 = Example.alloc().init()
         obj2 = Example.alloc().initWithIntValue_(2242)
         obj3 = Example.alloc().initWithBaseIntValue_intValue_(3342, 3337)
 
         self.assertEqual(obj1.baseIntField, 22)
@@ -697,43 +718,43 @@
         self.assertEqual(obj3.intField, 3337)
 
         # Protected constructors can't be invoked
         with self.assertRaises(AttributeError):
             Example.alloc().initWithString_("Hello")
 
     def test_static_access_non_static(self):
-        "An instance field/method cannot be accessed from the static context"
+        """An instance field/method cannot be accessed from the static context"""
         Example = ObjCClass("Example")
 
         obj = Example.alloc().init()
 
         with self.assertRaises(AttributeError):
             obj.staticIntField
 
         with self.assertRaises(AttributeError):
             obj.get_staticIntField()
 
     def test_non_static_access_static(self):
-        "A static field/method cannot be accessed from an instance context"
+        """A static field/method cannot be accessed from an instance context"""
         Example = ObjCClass("Example")
 
         with self.assertRaises(AttributeError):
             Example.intField
 
         with self.assertRaises(AttributeError):
             Example.accessIntField()
 
     def test_string_argument(self):
-        "A method with a string argument can be passed."
+        """A method with a string argument can be passed."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
         self.assertEqual(example.duplicateString_("Wagga"), "WaggaWagga")
 
     def test_enum_argument(self):
-        "An enumerated type can be used as an argument."
+        """An enumerated type can be used as an argument."""
         Example = ObjCClass("Example")
 
         obj = Example.alloc().init()
 
         self.assertEqual(obj.accessBaseIntField(), 22)
         self.assertEqual(obj.accessIntField(), 33)
 
@@ -752,62 +773,62 @@
         obj.baseIntField = MyEnum.value3
         obj.intField = MyEnum.value4
 
         self.assertEqual(obj.accessBaseIntField(), MyEnum.value3.value)
         self.assertEqual(obj.accessIntField(), MyEnum.value4.value)
 
     def test_string_return(self):
-        "If a method or field returns a string, you get a Python string back"
+        """If a method or field returns a string, you get a Python string back"""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
         self.assertEqual(example.toString(), "This is an ObjC Example object")
 
     def test_constant_string_return(self):
-        "If a method or field returns a *constant* string, you get a Python string back"
+        """If a method or field returns a *constant* string, you get a Python string back"""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
         self.assertEqual(example.smiley(), "%-)")
 
     def test_number_return(self):
-        "If a method or field returns a NSNumber, it is not automatically converted to a Python number."
+        """If a method or field returns a NSNumber, it is not automatically converted to a Python number."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
 
         answer = example.theAnswer()
         self.assertIsInstance(answer, ObjCInstance)
         self.assertEqual(py_from_ns(answer), 42)
         tau = example.twopi()
         self.assertIsInstance(tau, ObjCInstance)
         self.assertAlmostEqual(py_from_ns(tau), 2.0 * math.pi, 5)
 
     def test_float_method(self):
-        "A method with a float argument can be handled."
+        """A method with a float argument can be handled."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
         self.assertEqual(example.areaOfSquare_(1.5), 2.25)
 
     def test_float_method_send(self):
-        "A method with a float argument can be handled by send_message."
+        """A method with a float argument can be handled by send_message."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
         self.assertEqual(
             send_message(
                 example, "areaOfSquare:", 1.5, restype=c_float, argtypes=[c_float]
             ),
             2.25,
         )
 
     def test_double_method(self):
-        "A method with a double argument can be handled."
+        """A method with a double argument can be handled."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
         self.assertAlmostEqual(example.areaOfCircle_(1.5), 1.5 * math.pi, 5)
 
     def test_double_method_send(self):
-        "A method with a double argument can be handled by send_message."
+        """A method with a double argument can be handled by send_message."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
         self.assertAlmostEqual(
             send_message(
                 example, "areaOfCircle:", 1.5, restype=c_double, argtypes=[c_double]
             ),
             1.5 * math.pi,
@@ -815,26 +836,26 @@
         )
 
     @unittest.skipIf(
         OSX_VERSION and OSX_VERSION < (10, 10),
         "Property handling doesn't work on OS X 10.9 (Mavericks) and earlier",
     )
     def test_decimal_method(self):
-        "A method with a NSDecimalNumber arguments can be handled."
+        """A method with a NSDecimalNumber arguments can be handled."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
 
         result = example.areaOfTriangleWithWidth_andHeight_(
             Decimal("3.0"), Decimal("4.0")
         )
         self.assertIsInstance(result, ObjCClass("NSDecimalNumber"))
         self.assertEqual(py_from_ns(result), Decimal("6.0"))
 
     def test_auto_struct_creation(self):
-        "Structs from method signatures are created automatically."
+        """Structs from method signatures are created automatically."""
         Example = ObjCClass("Example")
 
         types.unregister_encoding_all(b"{simple=ii}")
         types.unregister_encoding_all(b"{simple}")
         types.unregister_encoding_all(b"{complex=[4s]^?{simple=ii}^{complex}}")
         types.unregister_encoding_all(b"{complex}")
 
@@ -854,39 +875,39 @@
         self.assertEqual(list(ret.field_0), [1, 2, 3, 4])
         self.assertEqual(ret.field_1.value, None)
         self.assertEqual(ret.field_2.field_0, 123)
         self.assertEqual(ret.field_2.field_1, 456)
         self.assertEqual(cast(ret.field_3, c_void_p).value, None)
 
     def test_sequence_arg_to_struct(self):
-        "Sequence arguments are converted to structures."
+        """Sequence arguments are converted to structures."""
         Example = ObjCClass("Example")
 
         ret = Example.extractSimpleStruct(([9, 8, 7, 6], None, (987, 654), None))
         struct_simple = types.ctype_for_encoding(b"{simple=ii}")
         self.assertIsInstance(ret, struct_simple)
         self.assertEqual(ret.field_0, 987)
         self.assertEqual(ret.field_1, 654)
 
     def test_struct_return(self):
-        "Methods returning structs of different sizes by value can be handled."
+        """Methods returning structs of different sizes by value can be handled."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
 
         types.register_encoding(b"{int_sized=[4c]}", struct_int_sized)
         self.assertEqual(example.intSizedStruct().x, b"abc")
 
         types.register_encoding(b"{oddly_sized=[5c]}", struct_oddly_sized)
         self.assertEqual(example.oddlySizedStruct().x, b"abcd")
 
         types.register_encoding(b"{large=[17c]}", struct_large)
         self.assertEqual(example.largeStruct().x, b"abcdefghijklmnop")
 
     def test_struct_return_send(self):
-        "Methods returning structs of different sizes by value can be handled when using send_message."
+        """Methods returning structs of different sizes by value can be handled when using send_message."""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
 
         self.assertEqual(
             send_message(
                 example, "intSizedStruct", restype=struct_int_sized, argtypes=[]
             ).x,
@@ -900,15 +921,15 @@
         )
         self.assertEqual(
             send_message(example, "largeStruct", restype=struct_large, argtypes=[]).x,
             b"abcdefghijklmnop",
         )
 
     def test_object_return(self):
-        "If a method or field returns an object, you get an instance of that type returned"
+        """If a method or field returns an object, you get an instance of that type returned"""
         Example = ObjCClass("Example")
         example = Example.alloc().init()
 
         Thing = ObjCClass("Thing")
         thing = Thing.alloc().initWithName_value_("This is thing", 2)
 
         example.thing = thing
@@ -976,29 +997,29 @@
         tester = DescriptionTester.alloc().initWithDescriptionString(
             None, debugDescriptionString=None
         )
         self.assertIsNot(str(tester), None)
         self.assertIsNot(repr(tester), None)
 
     def test_duplicate_class_registration(self):
-        "If you define a class name twice in the same runtime, you get an error."
+        """If you define a class name twice in the same runtime, you get an error."""
 
         # First definition should work.
         class MyClass(NSObject):
             pass
 
         # Second definition will raise an error.
         # Without protection, this is a segfault.
         with self.assertRaises(RuntimeError):
 
             class MyClass(NSObject):  # noqa: F811
                 pass
 
     def test_interface(self):
-        "An ObjC protocol implementation can be defined in Python."
+        """An ObjC protocol implementation can be defined in Python."""
 
         Callback = ObjCProtocol("Callback")
         results = {}
 
         class Handler(NSObject, protocols=[Callback]):
             @objc_method
             def initWithValue_(self, value: int):
@@ -1098,20 +1119,19 @@
         r = get_ivar(ivars, "rect")
         self.assertEqual(r.origin.x, 12)
         self.assertEqual(r.origin.y, 34)
         self.assertEqual(r.size.width, 56)
         self.assertEqual(r.size.height, 78)
 
     def test_class_properties(self):
-        "A Python class can have ObjC properties with synthesized getters and setters."
+        """A Python class can have ObjC properties with synthesized getters and setters."""
 
         NSURL = ObjCClass("NSURL")
 
         class URLBox(NSObject):
-
             url = objc_property(ObjCInstance)
             data = objc_property(ObjCInstance)
 
             @objc_method
             def getSchemeIfPresent(self):
                 if self.url is not None:
                     return self.url.scheme
@@ -1238,26 +1258,24 @@
         r = properties.rect
         self.assertEqual(r.origin.x, 12)
         self.assertEqual(r.origin.y, 34)
         self.assertEqual(r.size.width, 56)
         self.assertEqual(r.size.height, 78)
 
     def test_class_nonobject_properties_weak(self):
-
         with self.assertRaises(TypeError):
 
             class WeakNonObjectProperties(NSObject):
                 int = objc_property(c_int, weak=True)
 
     def test_class_properties_lifecycle_strong(self):
         class StrongObjectProperties(NSObject):
             object = objc_property(ObjCInstance)
 
         with autoreleasepool():
-
             properties = StrongObjectProperties.alloc().init()
 
             obj = NSObject.alloc().init()
             obj_pointer = obj.ptr.value  # store the object pointer for future use
 
             properties.object = obj
 
@@ -1268,15 +1286,14 @@
         self.assertEqual(properties.object.ptr.value, obj_pointer)
 
     def test_class_properties_lifecycle_weak(self):
         class WeakObjectProperties(NSObject):
             object = objc_property(ObjCInstance, weak=True)
 
         with autoreleasepool():
-
             properties = WeakObjectProperties.alloc().init()
 
             obj = NSObject.alloc().init()
             properties.object = obj
 
             self.assertIs(properties.object, obj)
 
@@ -1347,36 +1364,36 @@
             pass
 
         self.assertSequenceEqual(
             ProtocolExtendsProtocols.protocols, [NSObjectProtocol, ExampleProtocol]
         )
 
     def test_function_NSEdgeInsetsMake(self):
-        "Python can invoke NSEdgeInsetsMake to create NSEdgeInsets."
+        """Python can invoke NSEdgeInsetsMake to create NSEdgeInsets."""
 
         insets = NSEdgeInsets(0.0, 1.1, 2.2, 3.3)
         other_insets = NSEdgeInsetsMake(0.0, 1.1, 2.2, 3.3)
 
         # structs are NOT equal
         self.assertNotEqual(insets, other_insets)
 
         # but their values are
         self.assertEqual(insets.top, other_insets.top)
         self.assertEqual(insets.left, other_insets.left)
         self.assertEqual(insets.bottom, other_insets.bottom)
         self.assertEqual(insets.right, other_insets.right)
 
     def test_objc_const(self):
-        "objc_const works."
+        """objc_const works."""
 
         string_const = objc_const(rubiconharness, "SomeGlobalStringConstant")
         self.assertEqual(str(string_const), "Some global string constant")
 
     def test_interface_return_struct(self):
-        "An ObjC protocol implementation that returns values by struct can be defined in Python."
+        """An ObjC protocol implementation that returns values by struct can be defined in Python."""
 
         results = {}
         Thing = ObjCClass("Thing")
 
         class StructReturnHandler(Thing):
             @objc_method
             def initWithValue_(self, value):
@@ -1523,15 +1540,14 @@
         self.assertEqual(id(thing.python_object_2), python_object_2_id)
 
     def test_objcinstance_python_attribute_freed(self):
         """Python attributes on an ObjCInstance are freed after the instance is
         released."""
 
         with autoreleasepool():
-
             obj = NSObject.alloc().init()
 
             # Use a custom object as attribute value so that we can keep a weak reference.
 
             class TestO:
                 pass
 
@@ -1554,15 +1570,14 @@
             # Make sure that all Python objects are freed.
             del obj
             gc.collect()
 
         self.assertIsNone(wr_python_object())
 
     def test_objcinstance_release_owned(self):
-
         # Create an object which we own.
         obj = NSObject.alloc().init()
 
         # Check that it is marked for release.
         self.assertTrue(obj._needs_release)
 
         # Explicitly release the object.
@@ -1572,15 +1587,14 @@
         self.assertFalse(obj._needs_release)
 
         # Delete it and make sure that we don't segfault on garbage collection.
         del obj
         gc.collect()
 
     def test_objcinstance_autorelease_owned(self):
-
         # Create an object which we own.
         obj = NSObject.alloc().init()
 
         # Check that it is marked for release.
         self.assertTrue(obj._needs_release)
 
         # Explicitly release the object.
@@ -1645,29 +1659,29 @@
         self.assertTrue(obj._did_dealloc, "custom dealloc did not run")
         self.assertEqual(
             attr0.retainCount(), 1, "strong property value was not released"
         )
         self.assertEqual(attr1.retainCount(), 1, "weak property value was released")
 
     def test_partial_with_override(self):
-        "If one method in a partial is overridden, that doesn't impact lookup of other partial targets"
+        """If one method in a partial is overridden, that doesn't impact lookup of other partial targets"""
         SpecificExample = ObjCClass("SpecificExample")
 
         obj = SpecificExample.alloc().init()
 
         # The subclass implementation is invoked, not the base
         obj.method(2, withArg=3)
         self.assertEqual(obj.baseIntField, 5)
 
         # The base class implementation can still be found an invoked.
         obj.method(2)
         self.assertEqual(obj.baseIntField, 2)
 
     def test_stale_instance_cache(self):
-        "Instances returned by the ObjCInstance cache are checked for staleness (#249)"
+        """Instances returned by the ObjCInstance cache are checked for staleness (#249)"""
         # Wrap 2 classes with different method lists
         Example = ObjCClass("Example")
         Thing = ObjCClass("Thing")
 
         # Create objects of 2 different types.
         old = Example.alloc().init()
         thing = Thing.alloc().init()
@@ -1687,15 +1701,15 @@
             new_thing.computeSize(NSSize(37, 42))
         except AttributeError:
             # If a stale wrapper is returned, new_example will be of type Example,
             # so the expected method won't exist, causing an AttributeError.
             self.fail("Stale wrapper returned")
 
     def test_stale_instance_cache_implicit(self):
-        "Implicit instances returned by the ObjCInstance cache are checked for staleness (#249)"
+        """Implicit instances returned by the ObjCInstance cache are checked for staleness (#249)"""
         # Wrap 2 classes with different method lists
         Example = ObjCClass("Example")
         Thing = ObjCClass("Thing")
 
         # Create objects of 2 different types.
         old = Example.alloc().init()
         example = Example.alloc().init()
@@ -1722,16 +1736,34 @@
             # Try to access an method known to exist on Thing
             new_thing.computeSize(NSSize(37, 42))
         except AttributeError:
             # If a stale wrapper is returned, new_example will be of type Example,
             # so the expected method won't exist, causing an AttributeError.
             self.fail("Stale wrapper returned")
 
+    def test_compatible_class_name_change(self):
+        """If the class name changes in a compatible way, the wrapper isn't recreated (#257)"""
+        Example = ObjCClass("Example")
+
+        pre_init = Example.alloc()
+
+        # Call initWithClassChange(), which does an internal class name change.
+        # This mirrors what happens with NSWindow, where `init()` changes the
+        # class name to NSKVONotifying_NSWindow.
+        post_init = pre_init.initWithClassChange()
+
+        # Memory address hasn't changed
+        assert pre_init.ptr.value == post_init.ptr.value
+        # The class name hasn't changed either
+        assert pre_init.objc_class.name == post_init.objc_class.name == "Example"
+        # The wrapper is the same object
+        assert id(pre_init) == id(post_init)
+
     def test_threaded_wrapper_creation(self):
-        "If 2 threads try to create a wrapper for the same object, only 1 wrapper is created (#251)"
+        """If 2 threads try to create a wrapper for the same object, only 1 wrapper is created (#251)"""
         # Create an ObjC instance, and keep a track of the memory address
         Example = ObjCClass("Example")
         obj = Example.alloc().init()
         ptr = obj.ptr
 
         # The underlying problem is a race condition, so we need to try a
         # bunch of times to make it happen.
@@ -1762,15 +1794,16 @@
             # They should be pointing at the same memory address
             self.assertEqual(wrappers[0].ptr, wrappers[1].ptr)
 
             # They should be the same object (i.e., one came from the cache)
             self.assertEqual(id(wrappers[0]), id(wrappers[1]))
 
     def test_threaded_method_cache(self):
-        "If 2 threads try to access a method on the same object, there's no race condition populating the cache (#252)"
+        """If 2 threads try to access a method on the same object,
+        there's no race condition populating the cache (#252)"""
         # Wrap a class with lots of methods, and create the instance
         Example = ObjCClass("Example")
         obj = Example.alloc().init()
 
         for _ in range(0, 1000):
             # Manually clear the method/property cache on Example.
             # This returns the attributes set in ObjCClass.__new__
@@ -1794,15 +1827,16 @@
             # wait for both to complete.
             thread = threading.Thread(target=work)
             thread.start()
             work()
             thread.join()
 
     def test_threaded_accessor_cache(self):
-        "If 2 threads try to access an accessor on the same object, there's no race condition populating the cache (#252)"
+        """If 2 threads try to access an accessor on the same object,
+        there's no race condition populating the cache (#252)"""
         # Wrap a class with lots of methods, and create the instance
         Example = ObjCClass("Example")
         obj = Example.alloc().init()
 
         for _ in range(0, 1000):
             # Manually clear the method/property cache on Example.
             # This returns the attributes set in ObjCClass.__new__
@@ -1826,15 +1860,16 @@
             # wait for both to complete.
             thread = threading.Thread(target=work)
             thread.start()
             work()
             thread.join()
 
     def test_threaded_mutator_cache(self):
-        "If 2 threads try to access an mutator on the same object, there's no race condition populating the cache (#252)"
+        """If 2 threads try to access a mutator on the same object,
+        there's no race condition populating the cache (#252)"""
         # Wrap a class with lots of methods, and create the instance
         Example = ObjCClass("Example")
         obj = Example.alloc().init()
 
         for _ in range(0, 1000):
             # Manually clear the method/property cache on Example.
             # This returns the attributes set in ObjCClass.__new__
```

### Comparing `rubicon-objc-0.4.5rc1/tests/test_ctypes_patch.py` & `rubicon-objc-0.4.6/tests/test_ctypes_patch.py`

 * *Files identical despite different names*

