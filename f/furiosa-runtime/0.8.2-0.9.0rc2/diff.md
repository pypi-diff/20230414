# Comparing `tmp/furiosa-runtime-0.8.2.tar.gz` & `tmp/furiosa-runtime-0.9.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furiosa-runtime-0.8.2.tar", last modified: Wed Nov  9 06:16:27 2022, max compression
+gzip compressed data, was "furiosa-runtime-0.9.0rc2.tar", last modified: Fri Apr 14 20:48:45 2023, max compression
```

## Comparing `furiosa-runtime-0.8.2.tar` & `furiosa-runtime-0.9.0rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      340 2022-07-09 17:15:10.784990 furiosa-runtime-0.8.2/Makefile
--rw-r--r--   0        0        0      193 2022-07-09 17:15:10.784990 furiosa-runtime-0.8.2/README.md
--rw-r--r--   0        0        0      589 2022-03-23 02:46:22.111317 furiosa-runtime-0.8.2/furiosa/runtime/__init__.py
--rw-r--r--   0        0        0      104 2022-03-23 02:46:22.111317 furiosa-runtime-0.8.2/furiosa/runtime/_api/__init__.py
--rw-r--r--   0        0        0     8157 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/furiosa/runtime/_api/v1.py
--rw-r--r--   0        0        0     1344 2022-03-23 02:46:22.111317 furiosa-runtime-0.8.2/furiosa/runtime/_util.py
--rw-r--r--   0        0        0     1665 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/furiosa/runtime/compiler.py
--rw-r--r--   0        0        0      301 2022-07-09 17:15:10.784990 furiosa-runtime-0.8.2/furiosa/runtime/consts.py
--rw-r--r--   0        0        0     1696 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/furiosa/runtime/envs.py
--rw-r--r--   0        0        0     7202 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/furiosa/runtime/errors.py
--rw-r--r--   0        0        0       15 2022-11-09 06:16:10.944066 furiosa-runtime-0.8.2/furiosa/runtime/git_version.txt
--rw-r--r--   0        0        0     4904 2022-10-27 05:41:38.768709 furiosa-runtime-0.8.2/furiosa/runtime/model.py
--rw-r--r--   0        0        0    11619 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/furiosa/runtime/profiler.py
--rw-r--r--   0        0        0        0 2022-03-23 02:46:22.111317 furiosa-runtime-0.8.2/furiosa/runtime/py.typed
--rw-r--r--   0        0        0    19853 2022-11-09 05:44:10.157830 furiosa-runtime-0.8.2/furiosa/runtime/session.py
--rw-r--r--   0        0        0     9264 2022-10-26 21:05:59.741773 furiosa-runtime-0.8.2/furiosa/runtime/tensor.py
--rw-r--r--   0        0        0     2444 2022-11-09 06:12:57.713127 furiosa-runtime-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      115 2022-03-23 02:46:22.111317 furiosa-runtime-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0     3296 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/tests/test_async_session.py
--rw-r--r--   0        0        0     3029 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/tests/test_base.py
--rw-r--r--   0        0        0      534 2022-05-04 06:07:47.319120 furiosa-runtime-0.8.2/tests/test_error.py
--rw-r--r--   0        0        0     1780 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/tests/test_profiler.py
--rw-r--r--   0        0        0     7713 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/tests/test_session.py
--rw-r--r--   0        0        0     5070 2022-11-03 20:35:29.971030 furiosa-runtime-0.8.2/tests/test_tensor.py
--rw-r--r--   0        0        0      559 2022-10-26 21:05:59.741773 furiosa-runtime-0.8.2/tests/test_version.py
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 furiosa-runtime-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/Makefile
+-rw-r--r--   0        0        0      193 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/README.md
+-rw-r--r--   0        0        0      589 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/__init__.py
+-rw-r--r--   0        0        0      104 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/_api/__init__.py
+-rw-r--r--   0        0        0     8334 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/_api/v1.py
+-rw-r--r--   0        0        0     1344 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/_util.py
+-rw-r--r--   0        0        0     1924 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/compiler.py
+-rw-r--r--   0        0        0      301 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/consts.py
+-rw-r--r--   0        0        0     1696 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/envs.py
+-rw-r--r--   0        0        0     7202 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/errors.py
+-rw-r--r--   0        0        0       17 2023-04-14 20:43:57.992533 furiosa-runtime-0.9.0rc2/furiosa/runtime/git_version.txt
+-rw-r--r--   0        0        0     4904 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/model.py
+-rw-r--r--   0        0        0    11619 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/profiler.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/py.typed
+-rw-r--r--   0        0        0    19965 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/session.py
+-rw-r--r--   0        0        0    10840 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/furiosa/runtime/tensor.py
+-rw-r--r--   0        0        0     2443 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0     3296 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_async_session.py
+-rw-r--r--   0        0        0     3029 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_base.py
+-rw-r--r--   0        0        0      534 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_error.py
+-rw-r--r--   0        0        0     1780 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_profiler.py
+-rw-r--r--   0        0        0     7713 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_session.py
+-rw-r--r--   0        0        0     5486 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_tensor.py
+-rw-r--r--   0        0        0      559 2023-04-14 20:42:32.781315 furiosa-runtime-0.9.0rc2/tests/test_version.py
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 furiosa-runtime-0.9.0rc2/PKG-INFO
```

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/__init__.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/_api/v1.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/_api/v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """C Native library binding"""
 
 import ctypes
-from ctypes import POINTER, c_bool, c_char_p, c_int, c_ulonglong, c_void_p
+from ctypes import POINTER, c_bool, c_char_p, c_double, c_int, c_int32, c_ulonglong, c_void_p
 import logging
 import os
 from typing import List
 
 from furiosa.common.native import LogLevel, find_native_libs
 from furiosa.runtime import consts
 
@@ -93,14 +93,17 @@
 
 LIBNUX.nux_tensor_axis.argtypes = [c_void_p, c_ulonglong]
 LIBNUX.nux_tensor_axis.restype = c_int
 
 LIBNUX.nux_tensor_dtype.argtypes = [c_void_p]
 LIBNUX.nux_tensor_dtype.restype = c_int
 
+LIBNUX.nux_tensor_quantization_parameter.argtypes = [c_void_p, POINTER(c_double), POINTER(c_int32)]
+LIBNUX.nux_tensor_quantization_parameter.restype = c_int
+
 LIBNUX.nux_session_create.argtypes = [c_void_p, c_ulonglong, c_void_p, POINTER(c_void_p)]
 LIBNUX.nux_session_create.restype = c_int
 
 LIBNUX.nux_session_get_model.argtypes = [c_void_p]
 LIBNUX.nux_session_get_model.restype = c_void_p
 
 LIBNUX.nux_session_run.argtypes = [c_void_p, c_void_p, c_void_p]
```

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/_util.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/_util.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/compiler.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/compiler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from datetime import datetime
 import logging
 from pathlib import Path
 import random
 import string
-from typing import Union
+from typing import SupportsBytes, Union
 
 from . import envs
 from ._util import eprint
 
 LOG = logging.getLogger(__name__)
 
 
 def _read_file(path: Union[str, Path]):
     with open(path, 'rb') as file:
         contents = file.read()
         return contents
 
 
-def _model_image(model: Union[bytes, str, Path]) -> bytes:
+def _model_image(model: Union[bytes, SupportsBytes, str, Path]) -> bytes:
     if isinstance(model, bytes):
         model_image = model
     elif isinstance(model, (str, Path)):
         model_image = Path(model).read_bytes()
+    # isinstance(..., SupprotsBytes) must be checked after isinstance(..., Path) because Path has
+    # __bytes__.
+    elif isinstance(model, SupportsBytes):
+        model_image = bytes(model)
     else:
-        raise TypeError("'model' must be str or bytes, but it was " + repr(type(model)))
+        raise TypeError(
+            f"'model' must be bytes, SupportsBytes, str, or Path but was {type(model)!r}"
+        )
 
     return model_image
 
 
 def _generate_suffix(length: int) -> str:
     return ''.join(random.choice(string.ascii_lowercase + string.digits) for _ in range(length))
```

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/envs.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/envs.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/errors.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/errors.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/model.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/model.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/profiler.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/profiler.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/session.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Session and its asynchronous API for model inference"""
 
 import ctypes
 from ctypes import byref, c_int, c_void_p
 import logging
 from pathlib import Path
 import typing
-from typing import Dict, List, Mapping, Optional, Tuple, Union
+from typing import Dict, List, Mapping, Optional, SupportsBytes, Tuple, Union
 
 import numpy as np
 import yaml
 
 from furiosa import registry
 
 from . import envs
@@ -103,15 +103,15 @@
 
 
 class Session(Model):
     """Provides a blocking API to run an inference task with a given model"""
 
     def __init__(
         self,
-        model: Union[bytes, str, Path],
+        model: Union[bytes, SupportsBytes, str, Path],
         device: Optional[str] = None,
         worker_num: Optional[int] = None,
         batch_size: Optional[int] = None,
         compiler_hints: bool = True,
         compiler_config: Optional[Mapping[str, object]] = None,
     ):
         profiler_path = envs.profiler_output()
@@ -426,26 +426,27 @@
         self.close()
 
     def __del__(self):
         self.close()
 
 
 def create(
-    model: Union[bytes, str, Path, registry.Model],
+    model: Union[bytes, SupportsBytes, str, Path, registry.Model],
     device: str = None,
     worker_num: int = None,
     batch_size: int = None,
     compiler_config: Mapping[str, object] = None,
     compiler_hints: bool = True,
 ) -> Session:
     """Creates a session for a model
 
     Args:
-        model (bytes, str, Path, Model): a byte string containing a model image or \
-        a path string of a model image file or `furiosa.registry.Model`
+        model (bytes, SupportsBytes, str, Path, Model): a byte string
+            containing a model image, a path string of a model image
+            file, or furiosa.registry.Model
         device: NPU device (str) (e.g., npu0pe0, npu0pe0-1)
         worker_num: Number of workers
         batch_size: Batch size of input tensors
         compiler_config (Mapping[str, object]): Compile config
         compiler_hints: Print compiler hints if True (default: True)
 
     Returns:
@@ -477,29 +478,30 @@
         batch_size=batch_size,
         compiler_config=compiler_config,
         compiler_hints=compiler_hints,
     )
 
 
 def create_async(
-    model: Union[bytes, str, Path, registry.Model],
+    model: Union[bytes, SupportsBytes, str, Path, registry.Model],
     context_ty: Optional[type] = None,
     device: Optional[str] = None,
     worker_num: Optional[int] = None,
     batch_size: Optional[int] = None,
     compiler_hints: Optional[bool] = True,
     input_queue_size: Optional[int] = None,
     output_queue_size: Optional[int] = None,
     compiler_config: Optional[Mapping[str, object]] = None,
 ) -> Tuple[AsyncSession, CompletionQueue]:
     """Creates a pair of the asynchronous session and the completion queue for a given model
 
     Args:
-        model (bytes, str, Path, Model): a byte string containing a model image or \
-        a path string of a model image file or `furiosa.registry.Model`
+        model (bytes, SupportsBytes, str, Path, Model): a byte string
+            containing a model image, a path string of a model image
+            file, or furiosa.registry.Model
         context_ty (type): Type for passing context from AsyncSession to CompletionQueue
         device: NPU device (str) (e.g., npu0pe0, npu0pe0-1)
         worker_num: Number of workers
         batch_size: Batch size of input tensors
         compiler_hints: Print compiler hints if True (default: True)
         input_queue_size: The input queue size, and it must be > 0 and < 2^31.
         output_queue_size: The output queue size, and it must be be > 0 and < 2^31.
```

### Comparing `furiosa-runtime-0.8.2/furiosa/runtime/tensor.py` & `furiosa-runtime-0.9.0rc2/furiosa/runtime/tensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Tensor object and its utilities"""
 
 import ctypes
 from ctypes import POINTER, byref, c_uint8, c_uint64, c_void_p
 from enum import IntEnum
-from typing import Optional, Union
+from typing import Optional, Tuple, Union
 
 import numpy as np
 
 from ._api import LIBNUX
 from ._util import list_to_dict
-from .errors import UnsupportedTensorType
+from .errors import UnsupportedTensorType, is_err
 
 
 class Axis(IntEnum):
     """Axis of Tensor"""
 
     WIDTH = 0
     HEIGHT = 1
@@ -124,14 +124,25 @@
         return DataType(LIBNUX.nux_tensor_dtype(self))
 
     @property
     def numpy_dtype(self):
         """Return numpy dtype"""
         return self.dtype.numpy_dtype
 
+    @property
+    def quantization_parameter(self) -> Tuple[ctypes.c_double, ctypes.c_int32]:
+        """Return the quantization parameter for this tensor"""
+        scale = ctypes.c_double(0.0)
+        zero_point = ctypes.c_int32(0)
+
+        err = LIBNUX.nux_tensor_quantization_parameter(self, byref(scale), byref(zero_point))
+        if is_err(err):
+            raise into_exception(err)
+        return (scale, zero_point)
+
     def __repr__(self) -> str:
         repr = self.__class__.__name__ + "("
         if self.name:
             repr += f"name=\"{self.name}\", "
 
         repr += (
             f"shape={self.shape}, dtype={self.dtype.__repr__()}, "
@@ -166,14 +177,20 @@
         return self.desc.dtype
 
     @property
     def numpy_dtype(self):
         """Return numpy dtype"""
         return self.desc.numpy_dtype
 
+    @property
+    def quantization_parameter(self) -> Tuple[ctypes.c_double, ctypes.c_int32]:
+        """Return the quantization parameter for this tensor"""
+
+        return self.desc.quantization_parameter
+
     def copy_from(self, data: Union[np.ndarray, np.generic]):
         """Copy the contents of Numpy ndarray to this tensor"""
         if isinstance(data, np.ndarray):
             data = np.ascontiguousarray(data)
         if isinstance(data, (np.ndarray, np.generic)):
             buf_ptr = data.ctypes.data_as(POINTER(c_uint8))
             buf_size_in_bytes = data.nbytes
@@ -213,19 +230,29 @@
         if self.desc.name:
             repr += f'name="{self.desc.name}", '
 
         repr += f"shape={self.desc.shape}, dtype={self.desc.dtype.__repr__()})"
 
         return repr
 
-    def __del__(self):
+    # _LIBNUX is meant to keep a valid reference to the Nux library at
+    # interpreter shutdown. From https://bugs.python.org/issue5099#msg80855:
+    #
+    # > At interpreter shutdown, the module's global variables are set to None
+    # > before the module itself is released. __del__ methods may be called in
+    # > those precarious circumstances, and should not rely on any global
+    # > state.
+    def _close(self, _LIBNUX=LIBNUX):
         if self.allocated and self.ref:
-            LIBNUX.nux_tensor_destroy(self.ref)
+            _LIBNUX.nux_tensor_destroy(self.ref)
             self.allocated = False
 
+    def __del__(self):
+        self._close()
+
     def __eq__(self, other):
         if isinstance(other, Tensor):
             return np.array_equal(self.numpy(), other.numpy())
 
         return False
 
 
@@ -294,19 +321,29 @@
         """Convert TensorArray to a list of numpy.ndarray"""
         array = []
         for idx in range(self.len):
             array.append(self[idx].numpy())
 
         return array
 
-    def __del__(self):
+    # _LIBNUX is meant to keep a valid reference to the Nux library at
+    # interpreter shutdown. From https://bugs.python.org/issue5099#msg80855:
+    #
+    # > At interpreter shutdown, the module's global variables are set to None
+    # > before the module itself is released. __del__ methods may be called in
+    # > those precarious circumstances, and should not rely on any global
+    # > state.
+    def _close(self, _LIBNUX=LIBNUX):
         if self.should_drop and self.ref:
-            LIBNUX.nux_tensor_array_destroy(self.ref)
+            _LIBNUX.nux_tensor_array_destroy(self.ref)
             self.should_drop = False
 
+    def __del__(self):
+        self._close()
+
     def __repr__(self):
         return list_to_dict(self).__repr__()
 
 
 def numpy_dtype(value):
     """Return numpy dtype from any eligible object of Nux"""
     if isinstance(value, (np.ndarray, np.generic)):
```

### Comparing `furiosa-runtime-0.8.2/pyproject.toml` & `furiosa-runtime-0.9.0rc2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,58 +2,58 @@
 # Custom backend from https://gitlab.com/ileixe/flit_ext to use setuptools-scm
 # Upstream flit does not support it. See https://github.com/pypa/flit/issues/257
 requires = ["flit_ext"]
 build-backend = "flit_ext:buildapi"
 
 [project]
 name = "furiosa-runtime"
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
 dependencies = [
-    "furiosa-common == 0.8.*",
-    "furiosa-registry == 0.8.*",
+    "furiosa-common == 0.9.*",
+    "furiosa-registry == 0.9.*",
     "cffi ~= 1.14",
-    "numpy ~= 1.19",
-    "pydantic ~= 1.9",
+    "numpy ~= 1.24",
+    "pydantic",
     "pandas ~= 1.3",
 ]
 
 [project.optional-dependencies]
-test = ["mnist", "onnxruntime ~= 1.12.1"]
+test = ["mnist", "onnxruntime ~= 1.13.1"]
 
 [project.urls]
 Home = "https://furiosa.ai"
 Documentation = "https://furiosa-ai.github.io/docs"
 "Bug Tracker" = "https://github.com/furiosa-ai/furiosa-sdk/issues"
 "Source Code" = "https://github.com/furiosa-ai/furiosa-sdk"
 
 [tool.flit.module]
 name = "furiosa.runtime"
 
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

### Comparing `furiosa-runtime-0.8.2/tests/test_async_session.py` & `furiosa-runtime-0.9.0rc2/tests/test_async_session.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/tests/test_base.py` & `furiosa-runtime-0.9.0rc2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/tests/test_error.py` & `furiosa-runtime-0.9.0rc2/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/tests/test_profiler.py` & `furiosa-runtime-0.9.0rc2/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/tests/test_session.py` & `furiosa-runtime-0.9.0rc2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/tests/test_tensor.py` & `furiosa-runtime-0.9.0rc2/tests/test_tensor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ctypes import c_double, c_int32
 import random
 import unittest
 
 import mnist
 import numpy as np
 
 from furiosa.runtime import session
@@ -32,14 +33,16 @@
 
     def test_tensor_desc(self):
         tensor = self.sess.input(0)
         self.assertEqual(4, tensor.ndim)
         self.assertEqual("NCHW", tensor.format)
         self.assertEqual((1, 1, 28, 28), tensor.shape)
         self.assertEqual(DataType.FLOAT32, tensor.dtype)
+        self.assertEqual(c_double(1.0).value, tensor.quantization_parameter[0].value)
+        self.assertEqual(c_int32(0).value, tensor.quantization_parameter[1].value)
         self.assertEqual(np.float32, numpy_dtype(tensor))
         self.assertEqual(784, tensor.length)
         self.assertEqual(3136, tensor.size)
         self.assertEqual(
             tensor.__repr__(),
             'TensorDesc(name="Input3", shape=(1, 1, 28, 28), dtype=FLOAT32, format=NCHW, size=3136, len=784)',
         )
@@ -113,14 +116,18 @@
         cls.sess.close()
 
     def test_tensor_desc(self):
         tensor = self.sess.output(0)
         self.assertEqual(6, tensor.ndim)
         self.assertEqual(DataType.INT8, tensor.dtype)
         self.assertEqual(np.int8, numpy_dtype(tensor))
+        self.assertEqual(
+            c_double(0.02242703177034855).value, tensor.quantization_parameter[0].value
+        )
+        self.assertEqual(c_int32(-128).value, tensor.quantization_parameter[1].value)
         self.assertLess(tensor.length * np.dtype(tensor.numpy_dtype).itemsize, tensor.size)
 
     def test_tensor_numpy(self):
         tensor = self.sess.output(0)
 
         strides = []
         stride = 1
```

### Comparing `furiosa-runtime-0.8.2/tests/test_version.py` & `furiosa-runtime-0.9.0rc2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `furiosa-runtime-0.8.2/PKG-INFO` & `furiosa-runtime-0.9.0rc2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: furiosa-runtime
-Version: 0.8.2
+Version: 0.9.0rc2
 Summary: Provide high-level Python APIs to access Furiosa AI's NPUs and its eco-system
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
-Requires-Dist: furiosa-common == 0.8.*
-Requires-Dist: furiosa-registry == 0.8.*
+Requires-Dist: furiosa-common == 0.9.*
+Requires-Dist: furiosa-registry == 0.9.*
 Requires-Dist: cffi ~= 1.14
-Requires-Dist: numpy ~= 1.19
-Requires-Dist: pydantic ~= 1.9
+Requires-Dist: numpy ~= 1.24
+Requires-Dist: pydantic
 Requires-Dist: pandas ~= 1.3
 Requires-Dist: mnist ; extra == "test"
-Requires-Dist: onnxruntime ~= 1.12.1 ; extra == "test"
+Requires-Dist: onnxruntime ~= 1.13.1 ; extra == "test"
 Project-URL: Bug Tracker, https://github.com/furiosa-ai/furiosa-sdk/issues
 Project-URL: Documentation, https://furiosa-ai.github.io/docs
 Project-URL: Home, https://furiosa.ai
 Project-URL: Source Code, https://github.com/furiosa-ai/furiosa-sdk
 Provides-Extra: test
 
 # Package `furiosa.runtime`
```

