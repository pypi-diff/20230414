# Comparing `tmp/py-unused-deps-0.2.1.tar.gz` & `tmp/py-unused-deps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-unused-deps-0.2.1.tar", last modified: Sun Apr  9 20:36:41 2023, max compression
+gzip compressed data, was "py-unused-deps-0.3.0.tar", last modified: Fri Apr 14 07:04:17 2023, max compression
```

## Comparing `py-unused-deps-0.2.1.tar` & `py-unused-deps-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-09 20:36:41.323624 py-unused-deps-0.2.1/
--rw-r--r--   0 mjh       (1000) mjh       (1000)    18092 2023-01-07 15:04:16.000000 py-unused-deps-0.2.1/LICENSE
--rw-r--r--   0 mjh       (1000) mjh       (1000)     5952 2023-04-09 20:36:41.323624 py-unused-deps-0.2.1/PKG-INFO
--rw-r--r--   0 mjh       (1000) mjh       (1000)     5224 2023-01-07 14:57:55.000000 py-unused-deps-0.2.1/README.md
-drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-09 20:36:41.323624 py-unused-deps-0.2.1/py_unused_deps.egg-info/
--rw-r--r--   0 mjh       (1000) mjh       (1000)     5952 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/PKG-INFO
--rw-r--r--   0 mjh       (1000) mjh       (1000)      496 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/SOURCES.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)        1 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/dependency_links.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)       57 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/entry_points.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)       99 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/requires.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)       12 2023-04-09 20:36:41.000000 py-unused-deps-0.2.1/py_unused_deps.egg-info/top_level.txt
--rw-r--r--   0 mjh       (1000) mjh       (1000)     1682 2023-04-09 20:36:41.326957 py-unused-deps-0.2.1/setup.cfg
--rw-r--r--   0 mjh       (1000) mjh       (1000)       38 2022-09-30 21:07:55.000000 py-unused-deps-0.2.1/setup.py
-drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-09 20:36:41.323624 py-unused-deps-0.2.1/unused_deps/
--rw-r--r--   0 mjh       (1000) mjh       (1000)        9 2022-09-30 20:04:47.000000 py-unused-deps-0.2.1/unused_deps/__init__.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)       91 2022-10-02 15:27:05.000000 py-unused-deps-0.2.1/unused_deps/__main__.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)      356 2022-10-02 13:39:33.000000 py-unused-deps-0.2.1/unused_deps/compat.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)     2291 2023-01-03 11:03:42.000000 py-unused-deps-0.2.1/unused_deps/config.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)     2941 2022-12-16 22:04:00.000000 py-unused-deps-0.2.1/unused_deps/dist_info.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)      559 2022-12-16 22:04:00.000000 py-unused-deps-0.2.1/unused_deps/errors.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)     1526 2022-12-16 22:04:00.000000 py-unused-deps-0.2.1/unused_deps/files.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)      728 2022-12-16 22:04:00.000000 py-unused-deps-0.2.1/unused_deps/import_finder.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)     5540 2023-01-03 11:03:42.000000 py-unused-deps-0.2.1/unused_deps/main.py
--rw-r--r--   0 mjh       (1000) mjh       (1000)        0 2022-10-09 09:37:56.000000 py-unused-deps-0.2.1/unused_deps/py.typed
+drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-14 07:04:17.599928 py-unused-deps-0.3.0/
+-rw-r--r--   0 mjh       (1000) mjh       (1000)    18092 2023-01-07 15:04:16.000000 py-unused-deps-0.3.0/LICENSE
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     6370 2023-04-14 07:04:17.599928 py-unused-deps-0.3.0/PKG-INFO
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     5642 2023-04-13 21:14:49.000000 py-unused-deps-0.3.0/README.md
+drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-14 07:04:17.596595 py-unused-deps-0.3.0/py_unused_deps.egg-info/
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     6370 2023-04-14 07:04:17.000000 py-unused-deps-0.3.0/py_unused_deps.egg-info/PKG-INFO
+-rw-r--r--   0 mjh       (1000) mjh       (1000)      496 2023-04-14 07:04:17.000000 py-unused-deps-0.3.0/py_unused_deps.egg-info/SOURCES.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)        1 2023-04-14 07:04:17.000000 py-unused-deps-0.3.0/py_unused_deps.egg-info/dependency_links.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       57 2023-04-14 07:04:17.000000 py-unused-deps-0.3.0/py_unused_deps.egg-info/entry_points.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       99 2023-04-14 07:04:17.000000 py-unused-deps-0.3.0/py_unused_deps.egg-info/requires.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       12 2023-04-14 07:04:17.000000 py-unused-deps-0.3.0/py_unused_deps.egg-info/top_level.txt
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     1682 2023-04-14 07:04:17.599928 py-unused-deps-0.3.0/setup.cfg
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       38 2022-09-30 21:07:55.000000 py-unused-deps-0.3.0/setup.py
+drwxr-xr-x   0 mjh       (1000) mjh       (1000)        0 2023-04-14 07:04:17.599928 py-unused-deps-0.3.0/unused_deps/
+-rw-r--r--   0 mjh       (1000) mjh       (1000)        9 2022-09-30 20:04:47.000000 py-unused-deps-0.3.0/unused_deps/__init__.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)       91 2022-10-02 15:27:05.000000 py-unused-deps-0.3.0/unused_deps/__main__.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)      356 2022-10-02 13:39:33.000000 py-unused-deps-0.3.0/unused_deps/compat.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     2644 2023-04-13 21:14:49.000000 py-unused-deps-0.3.0/unused_deps/config.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     2941 2022-12-16 22:04:00.000000 py-unused-deps-0.3.0/unused_deps/dist_info.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)      559 2022-12-16 22:04:00.000000 py-unused-deps-0.3.0/unused_deps/errors.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     1677 2023-04-14 06:50:23.000000 py-unused-deps-0.3.0/unused_deps/files.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)      728 2022-12-16 22:04:00.000000 py-unused-deps-0.3.0/unused_deps/import_finder.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)     5856 2023-04-13 21:14:49.000000 py-unused-deps-0.3.0/unused_deps/main.py
+-rw-r--r--   0 mjh       (1000) mjh       (1000)        0 2022-10-09 09:37:56.000000 py-unused-deps-0.3.0/unused_deps/py.typed
```

### Comparing `py-unused-deps-0.2.1/LICENSE` & `py-unused-deps-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.1/PKG-INFO` & `py-unused-deps-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-unused-deps
-Version: 0.2.1
+Version: 0.3.0
 Summary: Find unused dependencies
 Home-page: https://github.com/matthewhughes934/py-unused-deps
 Author: Matthew Hughes
 Author-email: matthewhughes934@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,49 +20,58 @@
 # py-unused-deps
 
 Find unused dependencies in your Python projects.
 
 This application works by inspecting the metadata of your distribution and its
 dependencies. This means the current project **must be installed** and
 `py-unused-deps` must be run from within the same environment as the project,
-and its dependencies, are installed within. For example using `setuptools`:
+and its dependencies, are installed within. For example running in on this repo:
 
 ``` console
 $ python -m venv .venv
 $ source .venv/bin/activate
-$ pip install --editable .
-$ pip install unused-deps
-$ py-unused-deps
+$ pip install .
+$ py-unused-deps --distribution py-unused-deps
 ```
 
 ## Usage
 
-    usage: py-unused-deps [-h] [-d DISTRIBUTION] [-v] [-i IGNORE] [-e EXTRAS] [-r REQUIREMENTS] [--include INCLUDE] [--exclude EXCLUDE]
-                          [--config-file CONFIG_FILE]
+    usage: py-unused-deps [-h] [-d DISTRIBUTION] [-n] [-v] [-i IGNORE] [-e EXTRAS] [-r REQUIREMENTS]
+                          [--include INCLUDE] [--exclude EXCLUDE] [--config-file CONFIG_FILE]
                           [filepaths ...]
     
     positional arguments:
       filepaths             Paths to scan for dependency usage
     
     options:
       -h, --help            show this help message and exit
       -d DISTRIBUTION, --distribution DISTRIBUTION
                             The distribution to scan for unused dependencies
+      -n, --no-distribution
       -v, --verbose
       -i IGNORE, --ignore IGNORE
-                            Dependencies to ignore when scanning for usage. For example, you might want to ignore a linter that you run but don't import
+                            Dependencies to ignore when scanning for usage. For example, you might want to
+                            ignore a linter that you run but don't import
       -e EXTRAS, --extra EXTRAS
                             Extra environment to consider when loading dependencies
       -r REQUIREMENTS, --requirement REQUIREMENTS
                             File listing extra requirements to scan for
       --include INCLUDE     Pattern to match on files when measuring usage
       --exclude EXCLUDE     Pattern to match on files or directory to exclude when measuring usage
       --config-file CONFIG_FILE
                             File to load config from
 
+### Specifying a Distribution
+
+There are to ways to scan for unused dependencies, if you have an installable
+project you can specify it with the `--dependency` flag. Otherwise, if you just
+have a list Python files and some dependencies e.g. in a `requirements.txt` file
+you can use the `--no-distribution` flag. Exactly one of these flags must be
+specified.
+
 ### File Discovery
 
 The positional `filepaths` provides the location to search for files. Files
 under this path are matched according to the `--include` argument. This can be
 given multiple times and arguments are used interpreted as wildcard patterns
 (specifically, they are parsed to
 [`fnmatch.fnmatch`](https://docs.python.org/3/library/fnmatch.html#fnmatch.fnmatch).
```

### Comparing `py-unused-deps-0.2.1/README.md` & `py-unused-deps-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 # py-unused-deps
 
 Find unused dependencies in your Python projects.
 
 This application works by inspecting the metadata of your distribution and its
 dependencies. This means the current project **must be installed** and
 `py-unused-deps` must be run from within the same environment as the project,
-and its dependencies, are installed within. For example using `setuptools`:
+and its dependencies, are installed within. For example running in on this repo:
 
 ``` console
 $ python -m venv .venv
 $ source .venv/bin/activate
-$ pip install --editable .
-$ pip install unused-deps
-$ py-unused-deps
+$ pip install .
+$ py-unused-deps --distribution py-unused-deps
 ```
 
 ## Usage
 
-    usage: py-unused-deps [-h] [-d DISTRIBUTION] [-v] [-i IGNORE] [-e EXTRAS] [-r REQUIREMENTS] [--include INCLUDE] [--exclude EXCLUDE]
-                          [--config-file CONFIG_FILE]
+    usage: py-unused-deps [-h] [-d DISTRIBUTION] [-n] [-v] [-i IGNORE] [-e EXTRAS] [-r REQUIREMENTS]
+                          [--include INCLUDE] [--exclude EXCLUDE] [--config-file CONFIG_FILE]
                           [filepaths ...]
     
     positional arguments:
       filepaths             Paths to scan for dependency usage
     
     options:
       -h, --help            show this help message and exit
       -d DISTRIBUTION, --distribution DISTRIBUTION
                             The distribution to scan for unused dependencies
+      -n, --no-distribution
       -v, --verbose
       -i IGNORE, --ignore IGNORE
-                            Dependencies to ignore when scanning for usage. For example, you might want to ignore a linter that you run but don't import
+                            Dependencies to ignore when scanning for usage. For example, you might want to
+                            ignore a linter that you run but don't import
       -e EXTRAS, --extra EXTRAS
                             Extra environment to consider when loading dependencies
       -r REQUIREMENTS, --requirement REQUIREMENTS
                             File listing extra requirements to scan for
       --include INCLUDE     Pattern to match on files when measuring usage
       --exclude EXCLUDE     Pattern to match on files or directory to exclude when measuring usage
       --config-file CONFIG_FILE
                             File to load config from
 
+### Specifying a Distribution
+
+There are to ways to scan for unused dependencies, if you have an installable
+project you can specify it with the `--dependency` flag. Otherwise, if you just
+have a list Python files and some dependencies e.g. in a `requirements.txt` file
+you can use the `--no-distribution` flag. Exactly one of these flags must be
+specified.
+
 ### File Discovery
 
 The positional `filepaths` provides the location to search for files. Files
 under this path are matched according to the `--include` argument. This can be
 given multiple times and arguments are used interpreted as wildcard patterns
 (specifically, they are parsed to
 [`fnmatch.fnmatch`](https://docs.python.org/3/library/fnmatch.html#fnmatch.fnmatch).
```

### Comparing `py-unused-deps-0.2.1/py_unused_deps.egg-info/PKG-INFO` & `py-unused-deps-0.3.0/py_unused_deps.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-unused-deps
-Version: 0.2.1
+Version: 0.3.0
 Summary: Find unused dependencies
 Home-page: https://github.com/matthewhughes934/py-unused-deps
 Author: Matthew Hughes
 Author-email: matthewhughes934@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -20,49 +20,58 @@
 # py-unused-deps
 
 Find unused dependencies in your Python projects.
 
 This application works by inspecting the metadata of your distribution and its
 dependencies. This means the current project **must be installed** and
 `py-unused-deps` must be run from within the same environment as the project,
-and its dependencies, are installed within. For example using `setuptools`:
+and its dependencies, are installed within. For example running in on this repo:
 
 ``` console
 $ python -m venv .venv
 $ source .venv/bin/activate
-$ pip install --editable .
-$ pip install unused-deps
-$ py-unused-deps
+$ pip install .
+$ py-unused-deps --distribution py-unused-deps
 ```
 
 ## Usage
 
-    usage: py-unused-deps [-h] [-d DISTRIBUTION] [-v] [-i IGNORE] [-e EXTRAS] [-r REQUIREMENTS] [--include INCLUDE] [--exclude EXCLUDE]
-                          [--config-file CONFIG_FILE]
+    usage: py-unused-deps [-h] [-d DISTRIBUTION] [-n] [-v] [-i IGNORE] [-e EXTRAS] [-r REQUIREMENTS]
+                          [--include INCLUDE] [--exclude EXCLUDE] [--config-file CONFIG_FILE]
                           [filepaths ...]
     
     positional arguments:
       filepaths             Paths to scan for dependency usage
     
     options:
       -h, --help            show this help message and exit
       -d DISTRIBUTION, --distribution DISTRIBUTION
                             The distribution to scan for unused dependencies
+      -n, --no-distribution
       -v, --verbose
       -i IGNORE, --ignore IGNORE
-                            Dependencies to ignore when scanning for usage. For example, you might want to ignore a linter that you run but don't import
+                            Dependencies to ignore when scanning for usage. For example, you might want to
+                            ignore a linter that you run but don't import
       -e EXTRAS, --extra EXTRAS
                             Extra environment to consider when loading dependencies
       -r REQUIREMENTS, --requirement REQUIREMENTS
                             File listing extra requirements to scan for
       --include INCLUDE     Pattern to match on files when measuring usage
       --exclude EXCLUDE     Pattern to match on files or directory to exclude when measuring usage
       --config-file CONFIG_FILE
                             File to load config from
 
+### Specifying a Distribution
+
+There are to ways to scan for unused dependencies, if you have an installable
+project you can specify it with the `--dependency` flag. Otherwise, if you just
+have a list Python files and some dependencies e.g. in a `requirements.txt` file
+you can use the `--no-distribution` flag. Exactly one of these flags must be
+specified.
+
 ### File Discovery
 
 The positional `filepaths` provides the location to search for files. Files
 under this path are matched according to the `--include` argument. This can be
 given multiple times and arguments are used interpreted as wildcard patterns
 (specifically, they are parsed to
 [`fnmatch.fnmatch`](https://docs.python.org/3/library/fnmatch.html#fnmatch.fnmatch).
```

### Comparing `py-unused-deps-0.2.1/setup.cfg` & `py-unused-deps-0.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py-unused-deps
-version = 0.2.1
+version = 0.3.0
 author = Matthew Hughes
 author_email = matthewhughes934@gmail.com
 description = Find unused dependencies
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/matthewhughes934/py-unused-deps
 classifiers =
```

### Comparing `py-unused-deps-0.2.1/unused_deps/config.py` & `py-unused-deps-0.3.0/unused_deps/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "pyproject.toml",
 )
 
 
 class Config(NamedTuple):
     filepaths: list[str]
     distribution: str | None = None
+    no_distribution: bool = False
     ignore: list[str] | None = None
     extras: list[str] | None = None
     requirements: list[str] | None = None
     include: list[str] | None = None
     exclude: list[str] | None = None
     verbose: int = 0
     config_file: str | None = None
@@ -45,14 +46,23 @@
             k: v
             for (k, v) in chain(config_from_file.items(), vars(args).items())
             if v is not None
         }
     )
 
 
+def validate_config(config: Config) -> None:
+    if (config.distribution is None and not config.no_distribution) or (
+        config.distribution is not None and config.no_distribution
+    ):
+        raise InternalError(
+            "You must specify exactly one of '--distribution' or '--no-distribution'"
+        )
+
+
 def load_config_from_file(path: str | None) -> dict[str, object] | None:
     if path is not None:
         config = _read_config(path)
         if config is None:
             raise InternalError(f"Could not read config from {path}")
         else:
             return config
```

### Comparing `py-unused-deps-0.2.1/unused_deps/dist_info.py` & `py-unused-deps-0.3.0/unused_deps/dist_info.py`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.1/unused_deps/errors.py` & `py-unused-deps-0.3.0/unused_deps/errors.py`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.1/unused_deps/files.py` & `py-unused-deps-0.3.0/unused_deps/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from __future__ import annotations
 
 import logging
 import os
 from collections.abc import Generator, Sequence
 from fnmatch import fnmatch
 
+from unused_deps.errors import InternalError
+
 logger = logging.getLogger("unused-deps")
 
 
 def find_files(
     path: str, *, exclude: Sequence[str], include: Sequence[str]
 ) -> Generator[str, None, None]:
     return (
         filename
         for filename in _walk_path(path, exclude)
         if _include(filename, include)
     )
 
 
 def _walk_path(path: str, exclude: Sequence[str]) -> Generator[str, None, None]:
+    if not os.path.exists(path):
+        raise InternalError(f"Can't scan '{path}': file doesn't exist")
     if os.path.isdir(path):
         for root, sub_directories, files in os.walk(path):
             for directory in tuple(sub_directories):
                 joined = os.path.join(root, directory)
                 if _exclude(joined, exclude):
                     logger.debug("Excluding directory: %s", joined)
                     sub_directories.remove(directory)
```

### Comparing `py-unused-deps-0.2.1/unused_deps/import_finder.py` & `py-unused-deps-0.3.0/unused_deps/import_finder.py`

 * *Files identical despite different names*

### Comparing `py-unused-deps-0.2.1/unused_deps/main.py` & `py-unused-deps-0.3.0/unused_deps/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 import logging
 import sys
 from collections.abc import Generator, Iterable, Sequence
 from itertools import chain
 
 from unused_deps.compat import importlib_metadata
-from unused_deps.config import build_config, load_config_from_file
+from unused_deps.config import build_config, load_config_from_file, validate_config
 from unused_deps.dist_info import (
     distribution_packages,
     parse_requirement,
     required_dists,
 )
 from unused_deps.errors import InternalError, log_error
 from unused_deps.files import find_files
@@ -26,33 +26,36 @@
 
     parser = _build_arg_parser()
     args = parser.parse_args(argv)
 
     try:
         config_from_file = load_config_from_file(args.config_file)
         config = build_config(args, config_from_file)
+        validate_config(config)
         _configure_logging(config.verbose)
 
         python_paths = chain.from_iterable(
             find_files(path, exclude=args.exclude, include=args.include)
             for path in args.filepaths
         )
         imported_packages = frozenset(
             chain.from_iterable(get_import_bases(path) for path in python_paths)
         )
 
         if not imported_packages:
             logger.info("Could not find any source files")
 
         success = True
-        package_dists = (
-            _requirements_from_dist(args.distribution, args.extras)
-            if args.distribution is not None
-            else []
-        )
+
+        package_dists: Iterable[importlib_metadata.Distribution]
+        if args.distribution is not None:
+            package_dists = _requirements_from_dist(args.distribution, args.extras)
+        else:
+            package_dists = []
+
         requirement_dists = (
             (
                 dist
                 for dist in _read_requirements(args.requirements, args.extras)
                 if dist is not None
             )
             if args.requirements is not None
@@ -109,14 +112,21 @@
     parser.add_argument(
         "-d",
         "--distribution",
         required=False,
         help="The distribution to scan for unused dependencies",
     )
     parser.add_argument(
+        "-n",
+        "--no-distribution",
+        required=False,
+        action="store_true",
+        help="Run without scanning any distribution for dependencies",
+    )
+    parser.add_argument(
         "-v",
         "--verbose",
         default=0,
         action="count",
     )
     parser.add_argument(
         "-i",
```

