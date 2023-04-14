# Comparing `tmp/ignore_flake8_error-0.1.0.tar.gz` & `tmp/ignore_flake8_error-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignore_flake8_error-0.1.0.tar", last modified: Wed Jan 18 20:43:22 2023, max compression
+gzip compressed data, was "ignore_flake8_error-0.2.0.tar", last modified: Fri Apr 14 12:54:56 2023, max compression
```

## Comparing `ignore_flake8_error-0.1.0.tar` & `ignore_flake8_error-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 samuelsearles-bryant   (501) staff       (20)        0 2023-01-18 20:43:22.534597 ignore_flake8_error-0.1.0/
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     1078 2023-01-17 16:02:21.000000 ignore_flake8_error-0.1.0/LICENSE
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     1432 2023-01-18 20:43:22.534731 ignore_flake8_error-0.1.0/PKG-INFO
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)      845 2023-01-17 16:02:21.000000 ignore_flake8_error-0.1.0/README.md
-drwxr-xr-x   0 samuelsearles-bryant   (501) staff       (20)        0 2023-01-18 20:43:22.534271 ignore_flake8_error-0.1.0/ignore_flake8_error.egg-info/
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     1432 2023-01-18 20:43:22.000000 ignore_flake8_error-0.1.0/ignore_flake8_error.egg-info/PKG-INFO
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)      319 2023-01-18 20:43:22.000000 ignore_flake8_error-0.1.0/ignore_flake8_error.egg-info/SOURCES.txt
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)        1 2023-01-18 20:43:22.000000 ignore_flake8_error-0.1.0/ignore_flake8_error.egg-info/dependency_links.txt
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)       65 2023-01-18 20:43:22.000000 ignore_flake8_error-0.1.0/ignore_flake8_error.egg-info/entry_points.txt
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)       22 2023-01-18 20:43:22.000000 ignore_flake8_error-0.1.0/ignore_flake8_error.egg-info/requires.txt
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)       20 2023-01-18 20:43:22.000000 ignore_flake8_error-0.1.0/ignore_flake8_error.egg-info/top_level.txt
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     2668 2023-01-18 20:37:11.000000 ignore_flake8_error-0.1.0/ignore_flake8_error.py
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     1313 2023-01-18 20:43:22.535810 ignore_flake8_error-0.1.0/setup.cfg
--rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)       74 2023-01-17 16:02:21.000000 ignore_flake8_error-0.1.0/setup.py
+drwxr-xr-x   0 samuelsearles-bryant   (501) staff       (20)        0 2023-04-14 12:54:56.071680 ignore_flake8_error-0.2.0/
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     1078 2023-01-17 16:02:21.000000 ignore_flake8_error-0.2.0/LICENSE
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     1432 2023-04-14 12:54:56.071970 ignore_flake8_error-0.2.0/PKG-INFO
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)      845 2023-01-18 23:15:29.000000 ignore_flake8_error-0.2.0/README.md
+drwxr-xr-x   0 samuelsearles-bryant   (501) staff       (20)        0 2023-04-14 12:54:56.071073 ignore_flake8_error-0.2.0/ignore_flake8_error.egg-info/
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     1432 2023-04-14 12:54:56.000000 ignore_flake8_error-0.2.0/ignore_flake8_error.egg-info/PKG-INFO
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)      319 2023-04-14 12:54:56.000000 ignore_flake8_error-0.2.0/ignore_flake8_error.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)        1 2023-04-14 12:54:56.000000 ignore_flake8_error-0.2.0/ignore_flake8_error.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)       65 2023-04-14 12:54:56.000000 ignore_flake8_error-0.2.0/ignore_flake8_error.egg-info/entry_points.txt
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)       22 2023-04-14 12:54:56.000000 ignore_flake8_error-0.2.0/ignore_flake8_error.egg-info/requires.txt
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)       20 2023-04-14 12:54:56.000000 ignore_flake8_error-0.2.0/ignore_flake8_error.egg-info/top_level.txt
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     2733 2023-01-18 23:20:28.000000 ignore_flake8_error-0.2.0/ignore_flake8_error.py
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)     1313 2023-04-14 12:54:56.073337 ignore_flake8_error-0.2.0/setup.cfg
+-rw-r--r--   0 samuelsearles-bryant   (501) staff       (20)       74 2023-01-17 16:02:21.000000 ignore_flake8_error-0.2.0/setup.py
```

### Comparing `ignore_flake8_error-0.1.0/LICENSE` & `ignore_flake8_error-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ignore_flake8_error-0.1.0/PKG-INFO` & `ignore_flake8_error-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignore_flake8_error
-Version: 0.1.0
+Version: 0.2.0
 Summary: add `noqa` comments to ignore every occurrence of a flake8 error
 Home-page: https://github.com/samueljsb/ignore-flake8-error
 Author: Samuel Searles-Bryant
 Author-email: sam@samueljsb.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,18 +22,19 @@
 
 Install with pip:
 
 ```shell
 python -m pip install ignore-flake8-error
 ```
 
-Call the tool with an error code you want to add ignore comments for and the paths tothe files:
+Call the tool with an error code you want to add ignore comments for and the
+paths to the files:
 
 ```shell
-ignore-flake8-error F401 path/to/files/ path/to/more/files/s
+ignore-flake8-error F401 path/to/files/ path/to/more/files/
 ```
 
 ## Rationale
 
 When adding a new plugin (or enabling more rules) to flake8 on a large codebase,
 fixing the existing violations can be too large a task to do quickly. However,
 starting to check the rule sooner will prevent new violations fom being
```

### Comparing `ignore_flake8_error-0.1.0/README.md` & `ignore_flake8_error-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 Install with pip:
 
 ```shell
 python -m pip install ignore-flake8-error
 ```
 
-Call the tool with an error code you want to add ignore comments for and the paths tothe files:
+Call the tool with an error code you want to add ignore comments for and the
+paths to the files:
 
 ```shell
-ignore-flake8-error F401 path/to/files/ path/to/more/files/s
+ignore-flake8-error F401 path/to/files/ path/to/more/files/
 ```
 
 ## Rationale
 
 When adding a new plugin (or enabling more rules) to flake8 on a large codebase,
 fixing the existing violations can be too large a task to do quickly. However,
 starting to check the rule sooner will prevent new violations fom being
```

### Comparing `ignore_flake8_error-0.1.0/ignore_flake8_error.egg-info/PKG-INFO` & `ignore_flake8_error-0.2.0/ignore_flake8_error.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ignore-flake8-error
-Version: 0.1.0
+Version: 0.2.0
 Summary: add `noqa` comments to ignore every occurrence of a flake8 error
 Home-page: https://github.com/samueljsb/ignore-flake8-error
 Author: Samuel Searles-Bryant
 Author-email: sam@samueljsb.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,18 +22,19 @@
 
 Install with pip:
 
 ```shell
 python -m pip install ignore-flake8-error
 ```
 
-Call the tool with an error code you want to add ignore comments for and the paths tothe files:
+Call the tool with an error code you want to add ignore comments for and the
+paths to the files:
 
 ```shell
-ignore-flake8-error F401 path/to/files/ path/to/more/files/s
+ignore-flake8-error F401 path/to/files/ path/to/more/files/
 ```
 
 ## Rationale
 
 When adding a new plugin (or enabling more rules) to flake8 on a large codebase,
 fixing the existing violations can be too large a task to do quickly. However,
 starting to check the rule sooner will prevent new violations fom being
```

### Comparing `ignore_flake8_error-0.1.0/ignore_flake8_error.py` & `ignore_flake8_error-0.2.0/ignore_flake8_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         capture_output=True,
         text=True,
     )
 
     # extract filenames and line numbers
     results: dict[str, list[int]] = defaultdict(list)
     for line in proc.stdout.splitlines():
-        filename_, lineno_ = line.split()
+        filename_, lineno_ = line.rsplit(maxsplit=1)
         results[filename_].append(int(lineno_))
 
     return results
 
 
 def _add_code_to_comment(comment: str, code: str) -> str:
     if 'noqa: ' in comment:
@@ -70,14 +70,15 @@
     parser.add_argument('filenames', nargs='*')
     args = parser.parse_args(argv)
 
     print('-> running flake8', file=sys.stderr)
     violations = _run_flake8(args.code, args.filenames)
 
     if not violations:
+        print('no violations found', file=sys.stderr)
         return 0
 
     print(f'found violations in {len(violations)} files', file=sys.stderr)
 
     print('-> adding noqa comments', file=sys.stderr)
     ret = 0
     for filename, linenos in violations.items():
```

### Comparing `ignore_flake8_error-0.1.0/setup.cfg` & `ignore_flake8_error-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ignore_flake8_error
-version = 0.1.0
+version = 0.2.0
 description = add `noqa` comments to ignore every occurrence of a flake8 error
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/samueljsb/ignore-flake8-error
 author = Samuel Searles-Bryant
 author_email = sam@samueljsb.co.uk
 license = MIT
```

