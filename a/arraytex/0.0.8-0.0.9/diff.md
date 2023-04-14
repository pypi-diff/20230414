# Comparing `tmp/arraytex-0.0.8.tar.gz` & `tmp/arraytex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraytex-0.0.8.tar", max compression
+gzip compressed data, was "arraytex-0.0.9.tar", max compression
```

## Comparing `arraytex-0.0.8.tar` & `arraytex-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-04-13 09:33:23.806359 arraytex-0.0.8/LICENSE
--rw-r--r--   0        0        0     2982 2023-04-13 09:33:23.806359 arraytex-0.0.8/README.md
--rw-r--r--   0        0        0     2389 2023-04-13 09:33:49.310519 arraytex-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-13 09:33:23.806359 arraytex-0.0.8/src/arraytex/__init__.py
--rw-r--r--   0        0        0      206 2023-04-13 09:33:23.806359 arraytex-0.0.8/src/arraytex/__main__.py
--rw-r--r--   0        0        0     5033 2023-04-13 09:33:49.310519 arraytex-0.0.8/src/arraytex/api.py
--rw-r--r--   0        0        0      243 2023-04-13 09:33:23.806359 arraytex-0.0.8/src/arraytex/errors.py
--rw-r--r--   0        0        0        0 2023-04-13 09:33:23.806359 arraytex-0.0.8/src/arraytex/py.typed
--rw-r--r--   0        0        0     1776 2023-04-13 09:33:49.314519 arraytex-0.0.8/src/arraytex/utils.py
--rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 arraytex-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-14 16:20:20.920270 arraytex-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3135 2023-04-14 16:20:38.312520 arraytex-0.0.9/README.md
+-rw-r--r--   0        0        0     2389 2023-04-14 16:20:38.312520 arraytex-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-14 16:20:20.920270 arraytex-0.0.9/src/arraytex/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-14 16:20:20.920270 arraytex-0.0.9/src/arraytex/__main__.py
+-rw-r--r--   0        0        0     4986 2023-04-14 16:20:38.312520 arraytex-0.0.9/src/arraytex/api.py
+-rw-r--r--   0        0        0      243 2023-04-14 16:20:20.920270 arraytex-0.0.9/src/arraytex/errors.py
+-rw-r--r--   0        0        0        0 2023-04-14 16:20:20.920270 arraytex-0.0.9/src/arraytex/py.typed
+-rw-r--r--   0        0        0     1776 2023-04-14 16:20:20.920270 arraytex-0.0.9/src/arraytex/utils.py
+-rw-r--r--   0        0        0     4098 1970-01-01 00:00:00.000000 arraytex-0.0.9/PKG-INFO
```

### Comparing `arraytex-0.0.8/LICENSE` & `arraytex-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arraytex-0.0.8/README.md` & `arraytex-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,31 @@
 >>> import arraytex as atx
 >>> A = np.array([[1, 2, 3], [4, 5, 6]])
 >>> print(atx.to_matrix(A))
 \begin{bmatrix}
 1 & 2 & 3 \\
 4 & 5 & 6 \\
 \end{bmatrix}
+>>> print(atx.to_tabular(A))
+\begin{tabular}{c c c}
+\toprule
+Col 1 & Col 2 & Col 3 \\
+\midrule
+1 & 2 & 3 \\
+4 & 5 & 6 \\
+\bottomrule
+\end{tabular}
 ```
 
 Inspired by [@josephcslater](https://github.com/josephcslater)'s
 [array_to_latex](https://github.com/josephcslater/array_to_latex).
 
 ## Features
 
-- Support for different matrix environment delimiters, (`bmatrix`, `pmatrix`, etc.)
+- Support for matrix environments with different delimiters (`bmatrix`, `pmatrix`, etc.).
 - Support for tabular environments.
 - Support for builtin number formats (`:.2f`, `:.3e`, etc.).
 - Fully tested and typed.
 
 ## Requirements
 
 - `python >= 3.8`
```

### Comparing `arraytex-0.0.8/pyproject.toml` & `arraytex-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arraytex"
-version = "0.0.8"
+version = "0.0.9"
 description = "ArrayTeX"
 authors = ["Dom Batten <dominic.batten@googlemail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dbatten5/arraytex"
 repository = "https://github.com/dbatten5/arraytex"
 documentation = "https://arraytex.readthedocs.io"
```

### Comparing `arraytex-0.0.8/src/arraytex/api.py` & `arraytex-0.0.9/src/arraytex/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,30 +55,30 @@
 @use_clipboard
 def to_tabular(
     arr: NDArray[Any],
     num_format: Optional[str] = None,
     scientific_notation: bool = False,
     col_align: Union[List[str], str] = "c",
     col_names: Optional[List[str]] = None,
-    col_index: Optional[List[str]] = None,
+    index: Optional[List[str]] = None,
     to_clp: bool = False,
 ) -> str:
     """Convert a numpy.NDArray to LaTeX tabular environment.
 
     Args:
         arr: the array to be converted
         num_format: a number formatter string, e.g. ".2f"
         scientific_notation: a flag to determine whether 1 x 10^3 should be used,
             otherwise e-notation is used (1e3)
         col_align: set the alignment of the columns, usually "c", "r" or "l". If a
             single character is provided then it will be broadcast to all columns. If a list
             is provided then each item will be assigned to each column, list size and
             number of columns must match
         col_names: an optional list of column names, otherwise generic names will be assigned
-        col_index: an optional list of column indices, i.e. row identifiers
+        index: an optional table index, i.e. row identifiers
         to_clp: copy the output to the system clipboard
 
     Returns:
         the LaTeX tabular string representation of the array
 
     Raises:
         TooManyDimensionsError: when the supplied array has more than 2 dimensions
@@ -92,29 +92,29 @@
     elif n_dims == 1:
         n_cols = arr.shape[0]
     elif n_dims == 2:
         n_cols = arr.shape[1]
     else:
         raise TooManyDimensionsError
 
-    if not col_index:
+    if not index:
         if isinstance(col_align, list) and len(col_align) != n_cols:
             raise DimensionMismatchError(
                 f"Number of `col_align` items ({len(col_align)}) "
                 + f"doesn't match number of columns ({n_cols})"
             )
 
         if col_names and len(col_names) != n_cols:
             raise DimensionMismatchError(
                 f"Number of `col_names` items ({len(col_names)}) "
                 + f"doesn't match number of columns ({n_cols})"
             )
 
     if (
-        col_index
+        index
         and col_names
         and isinstance(col_align, list)
         and len(col_names) != len(col_align)
     ):
         raise DimensionMismatchError(
             f"Number of `col_align` items ({len(col_align)}) "
             + f"doesn't match number of columns ({len(col_names)})"
@@ -124,29 +124,29 @@
         col_align = [col_align for _ in range(n_cols)]
 
     if not col_names:
         col_names = [f"Col {i + 1}" for i in range(n_cols)]
 
     lines = _parse_lines(arr, num_format, scientific_notation)
 
-    if col_index:
-        if len(col_index) != len(lines):
+    if index:
+        if len(index) != len(lines):
             raise DimensionMismatchError(
-                f"Number of `col_index` items ({len(col_index)}) "
+                f"Number of `index` items ({len(index)}) "
                 + f"doesn't match number of rows ({len(lines)})"
             )
 
         if len(col_align) == n_cols:
             col_align.insert(0, "l")
 
         if len(col_names) == n_cols:
             col_names.insert(0, "Index")
 
         for idx, line in enumerate(lines):
-            lines[idx] = f"{col_index[idx]} & " + line.strip()
+            lines[idx] = f"{index[idx]} & " + line.strip()
 
     rv = [f"\\begin{{tabular}}{{{' '.join(col_align)}}}"]
     rv += [r"\toprule"]
     rv += [" & ".join(col_names) + r" \\"]
     rv += [r"\midrule"]
     rv += [line.strip() + r" \\" for line in lines]
     rv += [r"\bottomrule"]
```

### Comparing `arraytex-0.0.8/src/arraytex/utils.py` & `arraytex-0.0.9/src/arraytex/utils.py`

 * *Files identical despite different names*

### Comparing `arraytex-0.0.8/PKG-INFO` & `arraytex-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arraytex
-Version: 0.0.8
+Version: 0.0.9
 Summary: ArrayTeX
 Home-page: https://github.com/dbatten5/arraytex
 License: MIT
 Author: Dom Batten
 Author-email: dominic.batten@googlemail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -53,22 +53,31 @@
 >>> import arraytex as atx
 >>> A = np.array([[1, 2, 3], [4, 5, 6]])
 >>> print(atx.to_matrix(A))
 \begin{bmatrix}
 1 & 2 & 3 \\
 4 & 5 & 6 \\
 \end{bmatrix}
+>>> print(atx.to_tabular(A))
+\begin{tabular}{c c c}
+\toprule
+Col 1 & Col 2 & Col 3 \\
+\midrule
+1 & 2 & 3 \\
+4 & 5 & 6 \\
+\bottomrule
+\end{tabular}
 ```
 
 Inspired by [@josephcslater](https://github.com/josephcslater)'s
 [array_to_latex](https://github.com/josephcslater/array_to_latex).
 
 ## Features
 
-- Support for different matrix environment delimiters, (`bmatrix`, `pmatrix`, etc.)
+- Support for matrix environments with different delimiters (`bmatrix`, `pmatrix`, etc.).
 - Support for tabular environments.
 - Support for builtin number formats (`:.2f`, `:.3e`, etc.).
 - Fully tested and typed.
 
 ## Requirements
 
 - `python >= 3.8`
```

