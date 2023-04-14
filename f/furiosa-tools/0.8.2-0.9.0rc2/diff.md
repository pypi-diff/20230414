# Comparing `tmp/furiosa-tools-0.8.2.tar.gz` & `tmp/furiosa-tools-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-tools-0.8.2.tar", last modified: Wed Nov  9 06:15:55 2022, max compression
+gzip compressed data, was "furiosa-tools-0.9.0rc2.tar", last modified: Fri Apr 14 20:48:32 2023, max compression
```

## Comparing `furiosa-tools-0.8.2.tar` & `furiosa-tools-0.9.0rc2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      291 2022-07-09 17:15:10.784990 furiosa-tools-0.8.2/Makefile
--rw-r--r--   0        0        0      176 2022-07-09 17:15:10.784990 furiosa-tools-0.8.2/README.md
--rw-r--r--   0        0        0      112 2022-07-09 17:15:10.784990 furiosa-tools-0.8.2/furiosa/tools/__init__.py
--rw-r--r--   0        0        0       39 2022-07-09 17:15:10.784990 furiosa-tools-0.8.2/furiosa/tools/compiler/__init__.py
--rw-r--r--   0        0        0       84 2022-11-03 20:35:29.975030 furiosa-tools-0.8.2/furiosa/tools/compiler/api/__init__.py
--rw-r--r--   0        0        0     9145 2022-11-03 20:35:29.975030 furiosa-tools-0.8.2/furiosa/tools/compiler/api/v1.py
--rw-r--r--   0        0        0     6996 2022-11-09 06:11:58.366912 furiosa-tools-0.8.2/furiosa/tools/compiler/main.py
--rw-r--r--   0        0        0       30 2022-11-04 01:38:06.717787 furiosa-tools-0.8.2/furiosa/tools/git_version.txt
--rw-r--r--   0        0        0        0 2022-03-23 02:46:22.195319 furiosa-tools-0.8.2/furiosa/tools/py.typed
--rw-r--r--   0        0        0     2339 2022-11-09 06:13:13.105695 furiosa-tools-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      115 2022-03-23 02:46:22.195319 furiosa-tools-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0     6164 2022-11-09 05:44:10.157830 furiosa-tools-0.8.2/tests/tests_compile.py
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 furiosa-tools-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      291 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/Makefile
+-rw-r--r--   0        0        0      176 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/README.md
+-rw-r--r--   0        0        0      112 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/furiosa/tools/__init__.py
+-rw-r--r--   0        0        0       39 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/furiosa/tools/compiler/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/furiosa/tools/compiler/api/__init__.py
+-rw-r--r--   0        0        0     4170 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/furiosa/tools/compiler/api/errors.py
+-rw-r--r--   0        0        0     8458 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/furiosa/tools/compiler/api/v1.py
+-rw-r--r--   0        0        0     7260 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/furiosa/tools/compiler/main.py
+-rw-r--r--   0        0        0       17 2023-04-14 20:43:45.624647 furiosa-tools-0.9.0rc2/furiosa/tools/git_version.txt
+-rw-r--r--   0        0        0        0 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/furiosa/tools/py.typed
+-rw-r--r--   0        0        0     2345 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0     6164 2023-04-14 20:42:32.897314 furiosa-tools-0.9.0rc2/tests/tests_compile.py
+-rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 furiosa-tools-0.9.0rc2/PKG-INFO
```

### Comparing `furiosa-tools-0.8.2/furiosa/tools/compiler/api/v1.py` & `furiosa-tools-0.9.0rc2/furiosa/tools/compiler/api/v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """C Native library binding"""
 import ctypes
-from ctypes import CDLL, Structure, byref, c_bool, c_char_p, c_int, c_ulonglong, c_void_p
-from enum import IntEnum
+from ctypes import Structure, byref, c_bool, c_char_p, c_int, c_ulonglong, c_void_p
 import logging
 from pathlib import Path
-import sys
 from typing import Dict, Optional, Union
 
-from furiosa.common.error import FuriosaError, is_err
+from furiosa.common.error import is_err
 from furiosa.common.native import LogLevel, find_native_libs
 
+from .errors import CompilerApiError, InvalidTargetIrException, into_exception
+
 LOG = logging.getLogger(__name__)
 
 DEFAULT_ENCODING = "utf-8"
 DEFAULT_TARGET_NPU = "warboy-2pe"
 
 
 class FcBuffer(Structure):
@@ -101,56 +101,26 @@
 LIBCOMPILER.fc_options_enable_cache.argtypes = [c_void_p, c_bool]
 LIBCOMPILER.fc_options_enable_cache.restype = None
 
 # Register Ctrl-C signal handler to interrupt native side for long running job
 LIBCOMPILER.register_signal_handler()
 
 
-class NativeError(IntEnum):
-    """Python object correspondnig to nux_error_t in furiosa-libcompiler C API"""
-
-    SUCCESS = 0
-    COMPILATION_ERROR = 1
-    IO_ERROR = 2
-    CONFIGURATION_MISMATCH = 3
-    INVALID_FORMAT = 4
-    INVALID_MODEL = 5
-    INVALID_NPUID = 6
-    OUT_OF_DRAM = 7
-    OUT_OF_SRAM = 8
-    OUT_OF_INSTUCTION_MEMORY = 9
-    TFLITE_TO_DFG = 10
-    USER_COMMAND = 11
-    INVALID_CONFIG = 12
-    OTHER = 13
-
-
-class CompilerApiError(FuriosaError):
-    def __init__(self, message: str, err_code: Optional[NativeError] = None):
-        self.native_err = err_code
-        super().__init__(message)
-
-
-class InvalidTargetIrException(CompilerApiError):
-    def __init__(self, format: str = None):
-        super().__init__(f"invalid target ir '{format}'", NativeError.INVALID_FORMAT)
-
-
 def __set_ga_param(options, key: str, value: object):
     if key.lower() == "population_size":
         if isinstance(value, int):
             LIBCOMPILER.fc_options_ga_population_size(options, value)
         else:
             raise CompilerApiError("population_size must be a positive integer")
 
     elif key.lower() == "generation_limit":
         if isinstance(value, int):
             LIBCOMPILER.fc_options_ga_generation_limit(options, value)
         else:
-            CompilerApiError("generation_limit must be a positive integer")
+            raise CompilerApiError("generation_limit must be a positive integer")
 
     elif key.lower() == "max_prefetch_size":
         if isinstance(value, int):
             LIBCOMPILER.fc_options_ga_max_prefetch_size(options, value)
         else:
             raise CompilerApiError("max_prefetch_size must be a positive integer")
 
@@ -190,39 +160,39 @@
 
 def __check_target_ir(target_ir: str):
     if not target_ir.lower().strip() in ["dfg", "ldfg", "cdfg", "gir", "sir", "lir", "enf"]:
         raise InvalidTargetIrException(target_ir)
 
 
 def compile(
-    input_path: Union[str, Path],
-    output_path: Union[str, Path] = None,
+    input_bytes: bytes,
     target_ir: str = "enf",
     dot_graph: Optional[Union[str, Path]] = None,
     analyze_memory: Optional[Union[str, Path]] = None,
     batch_size: Optional[int] = None,
     split_after_lower: Optional[bool] = None,
     auto_batch_size: Optional[bool] = None,
     ga_params: Optional[Dict[str, str]] = None,
     target_npu: str = DEFAULT_TARGET_NPU,
     cache_enabled: bool = True,
     verbose: bool = False,
-) -> int:
+) -> bytes:
+    """The compilation function. Takes an onnx/tflite/furiosa-ir and compiles it to target_ir."""
+
     if verbose:
         LIBCOMPILER.fc_enable_logging(LogLevel.INFO)
 
-    input_bytes = Path(input_path).read_bytes()
     input_buf = FcBuffer(ctypes.cast(input_bytes, c_void_p).value, len(input_bytes))
 
     __check_target_ir(target_ir)
 
     options = LIBCOMPILER.fc_create_options()
 
     LIBCOMPILER.fc_options_target_ir(options, target_ir.encode(DEFAULT_ENCODING))
-    LIBCOMPILER.fc_options_target_npu(options, target_npu.encode(DEFAULT_ENCODING))
+    LIBCOMPILER.fc_options_target_npu(options, apply_b0(target_npu).encode(DEFAULT_ENCODING))
     LIBCOMPILER.fc_options_enable_cache(options, cache_enabled)
 
     if analyze_memory:
         LIBCOMPILER.fc_options_memory_analysis(
             options, str(analyze_memory).encode(DEFAULT_ENCODING)
         )
     if dot_graph:
@@ -239,21 +209,28 @@
             value = ga_params[key]
             __set_ga_param(options, key, value)
 
     output_buf = FcBuffer()
     errno = LIBCOMPILER.fc_compile(options, None, None, byref(input_buf), byref(output_buf))
 
     if is_err(errno):
-        # it's ok because furiosa-compiler will print out the error message to stderr
-        return errno.value if isinstance(errno, ctypes.c_int) else errno
-
-    try:
-        with open(output_path, "wb") as output:
-            array_type = ctypes.c_ubyte * output_buf.len
-            buffer = array_type.from_address(output_buf.data)
-            output.write(buffer)
-            print(f"The output has been saved to {output_path}", file=sys.stderr)
-    finally:
-        LIBCOMPILER.fc_destroy_buffer(byref(output_buf))
+        raise into_exception(errno)
 
-    # Happy return
-    return 0
+    # Passing to `bytes` function makes copy
+    output_bytes = bytes((ctypes.c_ubyte * output_buf.len).from_address(output_buf.data))
+    # Destroy the buffer after copying it
+    LIBCOMPILER.fc_destroy_buffer(byref(output_buf))
+
+    return output_bytes
+
+
+def apply_b0(target_npu: str) -> str:
+    if target_npu == "warboy":
+        return "warboy-b0"
+    elif target_npu == "warboy-2pe":
+        return "warboy-b0-2pe"
+    elif target_npu == "warboy-a0":
+        return "warboy"
+    elif target_npu == "warboy-a0-2pe":
+        return "warboy-2pe"
+    else:
+        return target_npu
```

### Comparing `furiosa-tools-0.8.2/furiosa/tools/compiler/main.py` & `furiosa-tools-0.9.0rc2/furiosa/tools/compiler/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse
 import logging
 import os
+import pathlib
 import sys
 from typing import Dict
 
 from furiosa.tools import __version__
 from furiosa.tools.compiler.api import CompilerApiError, VersionInfo, compile, version_string
 
 logging.basicConfig(level=os.environ.get('FURIOSA_LOG_LEVEL', 'INFO').upper())
@@ -19,15 +20,15 @@
     furiosa compile foo.onnx -o foo.enf
 
     # In addition to compilation, analyze the memory allocation and write the HTML report to bar.html
     furiosa compile foo.onnx -o foo.enf --analyze-memory bar.html
 
     # In addition to compilation, write the dot graph of the model graph into to bar.dot
     furiosa compile foo.onnx -o foo.enf --dot-graph bar.dot
-    
+
     # Set the genetic algorithm parameters for optimization
     furiosa compile foo.onnx -o foo.enf -ga population_size=100,generation_limit=500
 """
 
 NPU_IDS = ["warboy", "warboy-2pe"]
 
 
@@ -75,15 +76,14 @@
             raise CommandArgError("init_tactic must be either 'random' or 'heuristic'")
 
     else:
         raise CommandArgError(f"unknown genetic algorithm parameter: '{key}'")
 
 
 def ga_options(ga_params_str: str) -> Dict[str, object]:
-
     ga_params: Dict[str, object] = {}
 
     for kv in [part.strip() for part in ga_params_str.split(",")]:
         parts = kv.split("=")
         if len(parts) == 2:
             ga_params[parts[0]] = convert_ga_param(parts[0], parts[1])
         else:
@@ -182,31 +182,38 @@
         )
 
         ga_params = None
         if self.args.genetic_optimization:
             ga_params = ga_options(self.args.genetic_optimization)
 
         if self.args.output is None:
-            output = f"output.{self.args.target_ir}"
+            output_path = f"output.{self.args.target_ir.lower()}"
         else:
-            output = self.args.output
+            output_path = self.args.output
+
+        input_bytes = pathlib.Path(self.args.source).read_bytes()
 
-        return compile(
-            self.args.source,
-            output_path=output,
+        output_bytes = compile(
+            input_bytes,
             target_ir=self.args.target_ir,
             dot_graph=self.args.dot_graph,
             analyze_memory=self.args.analyze_memory,
             batch_size=self.args.batch_size,
             auto_batch_size=self.args.auto_batch_size,
             ga_params=ga_params,
             target_npu=self.args.target_npu,
             verbose=self.args.verbose,
         )
 
+        with open(output_path, "wb") as output_path:
+            output_path.write(output_bytes)
+            print(f"The output has been saved to {output_path}", file=sys.stderr)
+
+        return 0
+
 
 def main():
     try:
         exit(CommandCompile().run())
     except (CommandArgError, CompilerApiError) as e:
         print(f"ERROR: {e.message}", file=sys.stderr)
         exit(255)
```

### Comparing `furiosa-tools-0.8.2/pyproject.toml` & `furiosa-tools-0.9.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-tools"
-version = "0.8.2"
+version = "0.9.0.rc2"
 authors = [{ name = "FurioaAI, Inc.", email = "pkg@furiosa.ai" }]
 readme = "README.md"
 license = { text = "Apache License 2.0" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dynamic = ["description"]
-requires-python = "~=3.7"
+requires-python = "~=3.8"
 dependencies = ["pyyaml~=6.0.0"]
 
 [project.optional-dependencies]
 test = []
 
 [project.urls]
 Home = "https://furiosa.ai"
@@ -41,15 +41,15 @@
 
 [project.scripts]
 furiosa-compile = "furiosa.tools.compiler.main:main"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 100
-target-version = ["py37", "py38", "py39"]
+target-version = ["py38", "py39", "py310"]
 extend-exclude = "/generated/"
 
 [tool.isort]
 force_sort_within_sections = true
 known_first_party = ["furiosa"]
 line_length = 100
 profile = "black"
```

### Comparing `furiosa-tools-0.8.2/tests/tests_compile.py` & `furiosa-tools-0.9.0rc2/tests/tests_compile.py`

 * *Files identical despite different names*

### Comparing `furiosa-tools-0.8.2/PKG-INFO` & `furiosa-tools-0.9.0rc2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: furiosa-tools
-Version: 0.8.2
+Version: 0.9.0rc2
 Summary: FuriosaAI tools
 Author-email: "FurioaAI, Inc." <pkg@furiosa.ai>
-Requires-Python: ~=3.7
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: pyyaml~=6.0.0
 Project-URL: Bug Tracker, https://github.com/furiosa-ai/furiosa-sdk/issues
 Project-URL: Documentation, https://furiosa-ai.github.io/docs
 Project-URL: Home, https://furiosa.ai
 Project-URL: Source Code, https://github.com/furiosa-ai/furiosa-sdk
```

