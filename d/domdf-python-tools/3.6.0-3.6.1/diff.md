# Comparing `tmp/domdf_python_tools-3.6.0.tar.gz` & `tmp/domdf_python_tools-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domdf_python_tools-3.6.0.tar", last modified: Tue Jan 17 07:57:32 2023, max compression
+gzip compressed data, was "domdf_python_tools-3.6.1.tar", last modified: Fri Apr 14 11:35:48 2023, max compression
```

## Comparing `domdf_python_tools-3.6.0.tar` & `domdf_python_tools-3.6.1.tar`

### file list

```diff
@@ -1,50 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 07:57:32.275147 domdf_python_tools-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-01-17 07:57:32.275147 domdf_python_tools-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5653 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/__pkginfo__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 07:57:32.271147 domdf_python_tools-3.6.0/domdf_python_tools/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/_is_match.py
--rw-r--r--   0 runner    (1001) docker     (122)    17722 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 07:57:32.275147 domdf_python_tools-3.6.0/domdf_python_tools/compat/
--rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/compat/importlib_metadata.py
--rw-r--r--   0 runner    (1001) docker     (122)     3509 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/compat/importlib_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/compat/importlib_resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/compat/importlib_resources.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10847 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/delegators.py
--rw-r--r--   0 runner    (1001) docker     (122)    12333 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/doctools.py
--rw-r--r--   0 runner    (1001) docker     (122)     7571 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/getters.py
--rw-r--r--   0 runner    (1001) docker     (122)    75153 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/google-10000-english-no-swears.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7786 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/import_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    11966 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/iterative.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 07:57:32.275147 domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/
--rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6136 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8803 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/sizes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8914 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/units.py
--rw-r--r--   0 runner    (1001) docker     (122)     3585 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    34632 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/paths.py
--rw-r--r--   0 runner    (1001) docker     (122)     8496 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/pretty_print.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)    14337 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/stringlist.py
--rw-r--r--   0 runner    (1001) docker     (122)     6519 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)     7372 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/typing.py
--rw-r--r--   0 runner    (1001) docker     (122)    17211 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/versions.py
--rw-r--r--   0 runner    (1001) docker     (122)    21784 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/domdf_python_tools/words.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-17 07:57:32.275147 domdf_python_tools-3.6.0/domdf_python_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-01-17 07:57:32.000000 domdf_python_tools-3.6.0/domdf_python_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-01-17 07:57:32.000000 domdf_python_tools-3.6.0/domdf_python_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 07:57:32.000000 domdf_python_tools-3.6.0/domdf_python_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-17 07:57:32.000000 domdf_python_tools-3.6.0/domdf_python_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-01-17 07:57:32.000000 domdf_python_tools-3.6.0/domdf_python_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-01-17 07:57:32.000000 domdf_python_tools-3.6.0/domdf_python_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-01-17 07:57:32.275147 domdf_python_tools-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-01-17 07:57:06.000000 domdf_python_tools-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 11:35:48.465410 domdf_python_tools-3.6.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-04-14 11:35:48.465410 domdf_python_tools-3.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5653 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/__pkginfo__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 11:35:48.461410 domdf_python_tools-3.6.1/domdf_python_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/_is_match.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17722 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 11:35:48.461410 domdf_python_tools-3.6.1/domdf_python_tools/compat/
+-rw-r--r--   0 runner    (1001) docker     (122)     5595 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/compat/importlib_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3509 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/compat/importlib_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/compat/importlib_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/compat/importlib_resources.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    10847 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4432 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/delegators.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12333 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/doctools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7571 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/getters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75153 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/google-10000-english-no-swears.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7786 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/import_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11966 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/iterative.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 11:35:48.461410 domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1780 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6136 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8803 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/sizes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8914 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/units.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3585 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34632 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8496 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14337 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/stringlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6519 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7372 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17211 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7941 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/versions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21784 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/domdf_python_tools/words.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 11:35:48.461410 domdf_python_tools-3.6.1/domdf_python_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-04-14 11:35:48.000000 domdf_python_tools-3.6.1/domdf_python_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-04-14 11:35:48.000000 domdf_python_tools-3.6.1/domdf_python_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 11:35:48.000000 domdf_python_tools-3.6.1/domdf_python_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-14 11:35:48.000000 domdf_python_tools-3.6.1/domdf_python_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-04-14 11:35:48.000000 domdf_python_tools-3.6.1/domdf_python_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-14 11:35:48.000000 domdf_python_tools-3.6.1/domdf_python_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     5026 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1441 2023-04-14 11:35:48.465410 domdf_python_tools-3.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-14 11:35:48.465410 domdf_python_tools-3.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     7089 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_bases.py
+-rw-r--r--   0 runner    (1001) docker     (122)      162 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12834 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2603 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_delegators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8969 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_dir_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1169 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12668 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_doctools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10904 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_getters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7169 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_import_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15576 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_namedlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29785 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17671 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_paths_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26929 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_pretty_print.py
+-rw-r--r--   0 runner    (1001) docker     (122)      903 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15460 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_stringlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3991 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2525 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_userlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14335 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12192 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8447 2023-04-14 11:35:21.000000 domdf_python_tools-3.6.1/tests/test_words.py
```

### Comparing `domdf_python_tools-3.6.0/LICENSE` & `domdf_python_tools-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/PKG-INFO` & `domdf_python_tools-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domdf_python_tools
-Version: 3.6.0
+Version: 3.6.1
 Summary: Helpful functions for Python 🐍 🛠️
 Home-page: https://github.com/domdfcoding/domdf_python_tools
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2019-2022 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
         OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
         OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/domdfcoding/domdf_python_tools
 Project-URL: Issue Tracker, https://github.com/domdfcoding/domdf_python_tools/issues
 Project-URL: Source Code, https://github.com/domdfcoding/domdf_python_tools
-Project-URL: Documentation, https://domdf_python_tools.readthedocs.io/en/latest
+Project-URL: Documentation, https://domdf-python-tools.readthedocs.io/en/latest
 Keywords: utilities
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -83,16 +83,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/domdf_python_tools/latest?logo=read-the-docs
-	:target: https://domdf_python_tools.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/domdf-python-tools/latest?logo=read-the-docs
+	:target: https://domdf-python-tools.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/domdf_python_tools/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/domdf_python_tools/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/domdf_python_tools/workflows/Linux/badge.svg
@@ -154,15 +154,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/domdf_python_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.6.1
 	:target: https://github.com/domdfcoding/domdf_python_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/commit/master
 	:alt: GitHub last commit
```

### Comparing `domdf_python_tools-3.6.0/README.rst` & `domdf_python_tools-3.6.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/domdf_python_tools/latest?logo=read-the-docs
-	:target: https://domdf_python_tools.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/domdf-python-tools/latest?logo=read-the-docs
+	:target: https://domdf-python-tools.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/domdf_python_tools/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/domdf_python_tools/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/domdf_python_tools/workflows/Linux/badge.svg
@@ -96,15 +96,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/domdf_python_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.6.1
 	:target: https://github.com/domdfcoding/domdf_python_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/commit/master
 	:alt: GitHub last commit
```

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/__init__.py` & `domdf_python_tools-3.6.1/domdf_python_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 #  OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
 #  OR OTHER DEALINGS IN THE SOFTWARE.
 #
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2014-2020 Dominic Davis-Foster"
 __license__: str = "MIT"
-__version__: str = "3.6.0"
+__version__: str = "3.6.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __docs = False
```

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/_is_match.py` & `domdf_python_tools-3.6.1/domdf_python_tools/_is_match.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/bases.py` & `domdf_python_tools-3.6.1/domdf_python_tools/bases.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/compat/__init__.py` & `domdf_python_tools-3.6.1/domdf_python_tools/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/compat/importlib_metadata.pyi` & `domdf_python_tools-3.6.1/domdf_python_tools/compat/importlib_metadata.pyi`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/compat/importlib_resources.py` & `domdf_python_tools-3.6.1/domdf_python_tools/compat/importlib_resources.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/compat/importlib_resources.pyi` & `domdf_python_tools-3.6.1/domdf_python_tools/compat/importlib_resources.pyi`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/dates.py` & `domdf_python_tools-3.6.1/domdf_python_tools/dates.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/delegators.py` & `domdf_python_tools-3.6.1/domdf_python_tools/delegators.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/doctools.py` & `domdf_python_tools-3.6.1/domdf_python_tools/doctools.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/getters.py` & `domdf_python_tools-3.6.1/domdf_python_tools/getters.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/google-10000-english-no-swears.txt` & `domdf_python_tools-3.6.1/domdf_python_tools/google-10000-english-no-swears.txt`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/import_tools.py` & `domdf_python_tools-3.6.1/domdf_python_tools/import_tools.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/iterative.py` & `domdf_python_tools-3.6.1/domdf_python_tools/iterative.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/__init__.py` & `domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/__init__.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/classes.py` & `domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/classes.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/sizes.py` & `domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/sizes.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/units.py` & `domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/units.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/pagesizes/utils.py` & `domdf_python_tools-3.6.1/domdf_python_tools/pagesizes/utils.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/paths.py` & `domdf_python_tools-3.6.1/domdf_python_tools/paths.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/pretty_print.py` & `domdf_python_tools-3.6.1/domdf_python_tools/pretty_print.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/secrets.py` & `domdf_python_tools-3.6.1/domdf_python_tools/secrets.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/stringlist.py` & `domdf_python_tools-3.6.1/domdf_python_tools/stringlist.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/terminal.py` & `domdf_python_tools-3.6.1/domdf_python_tools/terminal.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/typing.py` & `domdf_python_tools-3.6.1/domdf_python_tools/typing.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/utils.py` & `domdf_python_tools-3.6.1/domdf_python_tools/utils.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/versions.py` & `domdf_python_tools-3.6.1/domdf_python_tools/versions.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools/words.py` & `domdf_python_tools-3.6.1/domdf_python_tools/words.py`

 * *Files identical despite different names*

### Comparing `domdf_python_tools-3.6.0/domdf_python_tools.egg-info/PKG-INFO` & `domdf_python_tools-3.6.1/domdf_python_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domdf-python-tools
-Version: 3.6.0
+Version: 3.6.1
 Summary: Helpful functions for Python 🐍 🛠️
 Home-page: https://github.com/domdfcoding/domdf_python_tools
 Author: Dominic Davis-Foster
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: Copyright (c) 2019-2022 Dominic Davis-Foster
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
         OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
         OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/domdfcoding/domdf_python_tools
 Project-URL: Issue Tracker, https://github.com/domdfcoding/domdf_python_tools/issues
 Project-URL: Source Code, https://github.com/domdfcoding/domdf_python_tools
-Project-URL: Documentation, https://domdf_python_tools.readthedocs.io/en/latest
+Project-URL: Documentation, https://domdf-python-tools.readthedocs.io/en/latest
 Keywords: utilities
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -83,16 +83,16 @@
 	* - Activity
 	  - |commits-latest| |commits-since| |maintained| |pypi-downloads|
 	* - QA
 	  - |codefactor| |actions_flake8| |actions_mypy|
 	* - Other
 	  - |license| |language| |requires|
 
-.. |docs| image:: https://img.shields.io/readthedocs/domdf_python_tools/latest?logo=read-the-docs
-	:target: https://domdf_python_tools.readthedocs.io/en/latest
+.. |docs| image:: https://img.shields.io/readthedocs/domdf-python-tools/latest?logo=read-the-docs
+	:target: https://domdf-python-tools.readthedocs.io/en/latest
 	:alt: Documentation Build Status
 
 .. |docs_check| image:: https://github.com/domdfcoding/domdf_python_tools/workflows/Docs%20Check/badge.svg
 	:target: https://github.com/domdfcoding/domdf_python_tools/actions?query=workflow%3A%22Docs+Check%22
 	:alt: Docs Check Status
 
 .. |actions_linux| image:: https://github.com/domdfcoding/domdf_python_tools/workflows/Linux/badge.svg
@@ -154,15 +154,15 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/domdf_python_tools
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.6.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/domdf_python_tools/v3.6.1
 	:target: https://github.com/domdfcoding/domdf_python_tools/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/domdf_python_tools
 	:target: https://github.com/domdfcoding/domdf_python_tools/commit/master
 	:alt: GitHub last commit
```

### Comparing `domdf_python_tools-3.6.0/pyproject.toml` & `domdf_python_tools-3.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools!=61.*,>=40.6.0", "wheel>=0.34.2",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "domdf_python_tools"
-version = "3.6.0"
+version = "3.6.1"
 description = "Helpful functions for Python 🐍 🛠️"
 readme = "README.rst"
 requires-python = ">=3.6"
 keywords = [ "utilities",]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -37,15 +37,15 @@
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/domdfcoding/domdf_python_tools"
 "Issue Tracker" = "https://github.com/domdfcoding/domdf_python_tools/issues"
 "Source Code" = "https://github.com/domdfcoding/domdf_python_tools"
-Documentation = "https://domdf_python_tools.readthedocs.io/en/latest"
+Documentation = "https://domdf-python-tools.readthedocs.io/en/latest"
 
 [project.optional-dependencies]
 dates = [ "pytz>=2019.1",]
 testing = []
 all = [ "pytz>=2019.1",]
 
 [tool.mkrecipe]
```

### Comparing `domdf_python_tools-3.6.0/setup.cfg` & `domdf_python_tools-3.6.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = domdf_python_tools
-version = 3.6.0
+version = 3.6.1
 author = Dominic Davis-Foster
 author_email = dominic@davis-foster.co.uk
 license = MIT License
 keywords = utilities
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 platforms = Windows, macOS, Linux
 url = https://github.com/domdfcoding/domdf_python_tools
 project_urls = 
-	Documentation = https://domdf_python_tools.readthedocs.io/en/latest
+	Documentation = https://domdf-python-tools.readthedocs.io/en/latest
 	Issue Tracker = https://github.com/domdfcoding/domdf_python_tools/issues
 	Source Code = https://github.com/domdfcoding/domdf_python_tools
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

### Comparing `domdf_python_tools-3.6.0/setup.py` & `domdf_python_tools-3.6.1/setup.py`

 * *Files identical despite different names*

