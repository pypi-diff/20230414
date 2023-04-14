# Comparing `tmp/idefix_cli-1.1.3.tar.gz` & `tmp/idefix_cli-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-1.1.3.tar", last modified: Thu Apr  6 08:51:00 2023, max compression
+gzip compressed data, was "idefix_cli-1.2.0.tar", last modified: Fri Apr 14 09:54:36 2023, max compression
```

## Comparing `idefix_cli-1.1.3.tar` & `idefix_cli-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:51:00.335744 idefix_cli-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-06 08:51:00.331744 idefix_cli-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:51:00.327744 idefix_cli-1.1.3/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:51:00.331744 idefix_cli-1.1.3/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:51:00.331744 idefix_cli-1.1.3/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-06 08:51:00.000000 idefix_cli-1.1.3/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-06 08:51:00.000000 idefix_cli-1.1.3/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 08:51:00.000000 idefix_cli-1.1.3/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-06 08:51:00.000000 idefix_cli-1.1.3/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-06 08:51:00.000000 idefix_cli-1.1.3/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 08:51:00.000000 idefix_cli-1.1.3/idefix_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 08:51:00.335744 idefix_cli-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 08:51:00.331744 idefix_cli-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-06 08:50:47.000000 idefix_cli-1.1.3/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.342202 idefix_cli-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-14 09:54:36.342202 idefix_cli-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.338201 idefix_cli-1.2.0/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.338201 idefix_cli-1.2.0/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.338201 idefix_cli-1.2.0/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:54:36.342202 idefix_cli-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.342202 idefix_cli-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_write.py
```

### Comparing `idefix_cli-1.1.3/LICENSE` & `idefix_cli-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/PKG-INFO` & `idefix_cli-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 1.1.3
+Version: 1.2.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `idefix_cli-1.1.3/README.md` & `idefix_cli-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli/_backports.py` & `idefix_cli-1.2.0/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli/_commands/clean.py` & `idefix_cli-1.2.0/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli/_commands/clone.py` & `idefix_cli-1.2.0/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli/_commands/conf.py` & `idefix_cli-1.2.0/idefix_cli/_commands/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,22 @@
 
 
 @requires_idefix()
 def command(*args: str, directory: str, interactive: bool) -> int | NoReturn:
     python_cmd = ["python3", os.path.join(os.environ["IDEFIX_DIR"], "configure.py")]
     cmake_cmd = ["ccmake" if interactive else "cmake", os.environ["IDEFIX_DIR"]]
 
+    path = Path(directory)
+    setup_cpp = path.resolve().joinpath("setup.cpp")
+    if not setup_cpp.is_file():
+        # CMake is perfectly happy to run in empty directories, but we block it early
+        # to avoid confusing errors at compilation time
+        print_err("Cannot configure a directory that doesn't contain a setup.cpp")
+        return 1
+
     clargs = list(args)
     engine_req, st = _get_engine()
     if engine_req is None:
         print_err(st)
         return 1
     elif st is not None:
         print_warning(st)
@@ -289,11 +297,11 @@
         clargs = substitute_cmake_args(clargs)
     elif engine_req is EngineRequirement.PYTHON:
         cmd = python_cmd
     else:
         assert_never(engine_req)
 
     cmd.extend(clargs)
-    print_subcommand(cmd, loc=Path(directory))
+    print_subcommand(cmd, loc=path)
 
     with chdir(directory):
         os.execvp(cmd[0], cmd)
```

### Comparing `idefix_cli-1.1.3/idefix_cli/_commands/read.py` & `idefix_cli-1.2.0/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli/_commands/run.py` & `idefix_cli-1.2.0/idefix_cli/_commands/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 else:
     from typing_extensions import assert_never
 
     from idefix_cli._backports import StrEnum
     from idefix_cli.lib import chdir
 
 
-class RecompileMode(StrEnum):
+class RebuildMode(StrEnum):
     ALWAYS = auto()
     PROMPT = auto()
 
 
 # known end messages in Idefix
 KNOWN_SUCCESS: Final = (
     "Main: Job completed successfully.",
@@ -49,23 +49,23 @@
 KNOWN_FAIL: Final = (
     "Main: Job was interrupted before completion.",
     "Main: Job was aborted because of an unrecoverable error.",
 )
 
 
 @requires_idefix()
-def make(directory) -> int:
+def build_idefix(directory) -> int:
     ncpus = 2 ** min(3, cpu_count().bit_length())
     cmd = ["make", "-j", str(ncpus)]
     print_subcommand(cmd, loc=Path(directory))
     try:
         with chdir(directory):
             return check_call(cmd)
     except CalledProcessError as exc:
-        print_err("failed to compile idefix")
+        print_err("failed to build idefix")
         return exc.returncode
 
 
 def add_arguments(parser) -> None:
     parser.add_argument("--dir", dest="directory", default=".", help="target directory")
     parser.add_argument(
         "-i",
@@ -174,32 +174,32 @@
                     "configuration file seems malformed, "
                     "expected 'Output' to be a section title, not a parameter name."
                 )
                 return 1
             for entry in output_types:
                 output_sec[entry] = time_step
 
-    recompile_mode_str: str = get_option("idfx run", "recompile") or "always"
+    rebuild_mode_str: str = get_option("idfx run", "recompile") or "always"
 
     try:
-        recompile_mode = RecompileMode(recompile_mode_str)
+        rebuild_mode = RebuildMode(rebuild_mode_str)
     except ValueError:
         print_warning(
-            f"Expected [idfx run].recompile to be any of {[str(_) for _ in RecompileMode]}"
-            f"Got {recompile_mode} from {get_config_file()}\n"
+            f"Expected [idfx run].recompile to be any of {[str(_) for _ in RebuildMode]}"
+            f"Got {rebuild_mode} from {get_config_file()}\n"
         )
         print_warning("Falling back to 'prompt' mode.")
-        recompile_mode = RecompileMode.PROMPT
+        rebuild_mode = RebuildMode.PROMPT
 
-    compilation_is_required: bool
-    if recompile_mode is RecompileMode.ALWAYS:
-        compilation_is_required = True
-    elif recompile_mode is RecompileMode.PROMPT:
+    build_is_required: bool
+    if rebuild_mode is RebuildMode.ALWAYS:
+        build_is_required = True
+    elif rebuild_mode is RebuildMode.PROMPT:
         if exe.is_file():
-            last_compilation_time = os.stat(exe).st_mtime
+            last_build_time = os.stat(exe).st_mtime
             source_patterns = (
                 "**/*.hpp",
                 "**/*.cpp",
                 "**/*.h",
                 "**/*.c",
                 "**/CMakeLists.txt",
                 "**/Makefile.cmake",
@@ -227,33 +227,33 @@
                     set(git_indexed_idefix_files).intersection(source_files)
                 )
 
             source_edit_times = tuple(
                 (file, os.stat(file).st_mtime) for file in files_to_check
             )
             time_deltas = tuple(
-                (file, edit_time - last_compilation_time)
+                (file, edit_time - last_build_time)
                 for file, edit_time in source_edit_times
             )
             if updated_since_compilation := tuple(
                 file for file, td in time_deltas if td > 0
             ):
                 print_warning(
                     "The following files were updated since last successful compilation:",
                 )
                 print("\n".join(updated_since_compilation), file=sys.stderr)
-                compilation_is_required = Confirm.ask(
-                    "Would you like to recompile before running the program ?"
+                build_is_required = Confirm.ask(
+                    "Would you like to rebuild before running the program ?"
                 )
             else:
-                compilation_is_required = False
+                build_is_required = False
     else:
-        assert_never(recompile_mode)
+        assert_never(rebuild_mode)
 
-    if compilation_is_required and (ret := make(directory)) != 0:
+    if build_is_required and (ret := build_idefix(directory)) != 0:
         return ret
 
     if time_step is not None:
         conf["TimeIntegrator"]["first_dt"] = time_step
     if duration is not None:
         conf["TimeIntegrator"]["tstop"] = duration
```

### Comparing `idefix_cli-1.1.3/idefix_cli/_commands/stamp.py` & `idefix_cli-1.2.0/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli/_commands/write.py` & `idefix_cli-1.2.0/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli/_main.py` & `idefix_cli-1.2.0/idefix_cli/_main.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli/lib.py` & `idefix_cli-1.2.0/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-1.2.0/idefix_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 1.1.3
+Version: 1.2.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `idefix_cli-1.1.3/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-1.2.0/idefix_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/pyproject.toml` & `idefix_cli-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idefix_cli"
-version = "1.1.3"
+version = "1.2.0"
 description = "A CLI to automate mundane tasks with Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
```

### Comparing `idefix_cli-1.1.3/tests/test_app_structure.py` & `idefix_cli-1.2.0/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/tests/test_clean.py` & `idefix_cli-1.2.0/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/tests/test_clone.py` & `idefix_cli-1.2.0/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/tests/test_commons.py` & `idefix_cli-1.2.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/tests/test_conf.py` & `idefix_cli-1.2.0/tests/test_conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 from packaging.version import Version
 from pytest_check import check
 
 from idefix_cli._commands.conf import substitute_cmake_args
 from idefix_cli._main import main
 
 
+def test_conf_without_setup_cpp(capsys, tmp_path, monkeypatch):
+    tmp_idefix_dir = tmp_path / "idefix"
+    os.makedirs(tmp_idefix_dir / ".git")
+    monkeypatch.setenv("IDEFIX_DIR", str(tmp_idefix_dir))
+
+    monkeypatch.chdir(tmp_path)
+    ret = main(["conf"])
+    with check:
+        assert ret != 0
+
+    out, err = capsys.readouterr()
+    with check:
+        assert out == ""
+    with check:
+        assert "💥 Cannot configure a directory that doesn't contain a setup.cpp" in err
+
+
 def test_setup_requiring_cmake_in_bad_env(capsys, tmp_path, monkeypatch):
     tmp_idefix_dir = tmp_path / "idefix"
     os.makedirs(tmp_idefix_dir / ".git")
     monkeypatch.setenv("IDEFIX_DIR", str(tmp_idefix_dir))
 
     monkeypatch.chdir(tmp_path)
     usr_config = tmp_path / "idefix.cfg"
@@ -21,14 +38,15 @@
     # not going to test every possible case, but we want to make sure that
     # the requirements are not met for this test, so we mock (almost)
     # impossible conditions.
     mock_requirements = {"cmake": Version("9001.0.1"), "idefix": Version("9001.0.1")}
     monkeypatch.setattr(
         "idefix_cli._commands.conf.CMAKE_MIN_VERSIONS", mock_requirements
     )
+    (tmp_path / "setup.cpp").touch()
 
     ret = main(["conf"])
     with check:
         assert ret != 0
 
     out, err = capsys.readouterr()
     with check:
```

### Comparing `idefix_cli-1.1.3/tests/test_read.py` & `idefix_cli-1.2.0/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/tests/test_stamp.py` & `idefix_cli-1.2.0/tests/test_stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/tests/test_ux.py` & `idefix_cli-1.2.0/tests/test_ux.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.1.3/tests/test_write.py` & `idefix_cli-1.2.0/tests/test_write.py`

 * *Files identical despite different names*

