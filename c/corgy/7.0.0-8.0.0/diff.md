# Comparing `tmp/corgy-7.0.0.tar.gz` & `tmp/corgy-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-7.0.0.tar", max compression
+gzip compressed data, was "corgy-8.0.0.tar", max compression
```

## Comparing `corgy-7.0.0.tar` & `corgy-8.0.0.tar`

### file list

```diff
@@ -1,42 +1,38 @@
--rw-r--r--   0        0        0    27949 2023-04-11 20:42:16.071329 corgy-7.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-04-11 20:42:16.071329 corgy-7.0.0/LICENSE
--rw-r--r--   0        0        0     4158 2023-04-11 20:42:16.071329 corgy-7.0.0/README.md
--rw-r--r--   0        0        0      395 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/__init__.py
--rw-r--r--   0        0        0     2329 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/_actions.py
--rw-r--r--   0        0        0      505 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/_annotations.py
--rw-r--r--   0        0        0    46721 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/_corgy.py
--rw-r--r--   0        0        0     6228 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/_corgyparser.py
--rw-r--r--   0        0        0    36993 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/_helpfmt.py
--rw-r--r--   0        0        0    17249 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/_meta.py
--rw-r--r--   0        0        0       64 2023-04-11 20:43:01.971882 corgy-7.0.0/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/py.typed
--rw-r--r--   0        0        0     1727 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/__init__.py
--rw-r--r--   0        0        0     5838 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_dir.py
--rw-r--r--   0        0        0     2382 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_expand.py
--rw-r--r--   0        0        0     3414 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_filepath.py
--rw-r--r--   0        0        0     3413 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_initargs.py
--rw-r--r--   0        0        0     2777 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_inputfile.py
--rw-r--r--   0        0        0     5464 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_keyvaluepairs.py
--rw-r--r--   0        0        0     5271 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_outputfile.py
--rw-r--r--   0        0        0     9846 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_subclass.py
--rw-r--r--   0        0        0    32375 2023-04-11 20:42:16.075329 corgy-7.0.0/docs/corgy.md
--rw-r--r--   0        0        0    14889 2023-04-11 20:42:16.075329 corgy-7.0.0/docs/corgy.types.md
--rw-r--r--   0        0        0      132 2023-04-11 20:42:16.075329 corgy-7.0.0/docs/index.md
--rw-r--r--   0        0        0     2679 2023-04-11 20:43:01.971882 corgy-7.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/__init__.py
--rw-r--r--   0        0        0    87305 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/test_corgy.py
--rw-r--r--   0        0        0    16513 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/test_corgyparser.py
--rw-r--r--   0        0        0      823 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/test_doctests.py
--rw-r--r--   0        0        0    47095 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/test_helpfmt.py
--rw-r--r--   0        0        0        0 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/__init__.py
--rw-r--r--   0        0        0      328 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/_pklclasses.py
--rw-r--r--   0        0        0     2002 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/_specialtmps.py
--rw-r--r--   0        0        0     3356 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/_test_file.py
--rw-r--r--   0        0        0     6023 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_dirs.py
--rw-r--r--   0        0        0     5365 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_filepaths.py
--rw-r--r--   0        0        0     2678 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_initargs.py
--rw-r--r--   0        0        0     2496 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_inputfiles.py
--rw-r--r--   0        0        0     5443 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_keyvaluepairs.py
--rw-r--r--   0        0        0     5085 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_outputfiles.py
--rw-r--r--   0        0        0     7082 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_subclass.py
--rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 corgy-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0    29010 2023-04-14 21:42:45.442256 corgy-8.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-04-14 21:42:45.442256 corgy-8.0.0/LICENSE
+-rw-r--r--   0        0        0     4158 2023-04-14 21:42:45.442256 corgy-8.0.0/README.md
+-rw-r--r--   0        0        0      395 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_annotations.py
+-rw-r--r--   0        0        0    48599 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_corgy.py
+-rw-r--r--   0        0        0     6228 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    36993 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    17249 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-04-14 21:43:27.343100 corgy-8.0.0/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/py.typed
+-rw-r--r--   0        0        0     1598 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/__init__.py
+-rw-r--r--   0        0        0     2382 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3413 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-04-14 21:42:45.442256 corgy-8.0.0/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    33057 2023-04-14 21:42:45.442256 corgy-8.0.0/docs/corgy.md
+-rw-r--r--   0        0        0    11884 2023-04-14 21:42:45.442256 corgy-8.0.0/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-04-14 21:42:45.442256 corgy-8.0.0/docs/index.md
+-rw-r--r--   0        0        0     2679 2023-04-14 21:43:27.339100 corgy-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 21:42:45.442256 corgy-8.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    89079 2023-04-14 21:42:45.442256 corgy-8.0.0/tests/test_corgy.py
+-rw-r--r--   0        0        0    16513 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      780 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/test_doctests.py
+-rw-r--r--   0        0        0    47095 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/_test_file.py
+-rw-r--r--   0        0        0     2678 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5122 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-04-14 21:42:45.446256 corgy-8.0.0/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 corgy-8.0.0/PKG-INFO
```

### Comparing `corgy-7.0.0/CHANGELOG.md` & `corgy-8.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,33 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [8.0.0](https://github.com/jayanthkoushik/corgy/compare/v7.0.0...v8.0.0) (2023-04-14)
+
+
+### ⚠ BREAKING CHANGES
+
+* The following path based types have been removed from
+`Corgy.types`: `ReadableFile`, `WritableFile`, `InputDirectory`,
+`OutputDirectory`, `LazyOutputDirectory`, `IODirectory`. The "promises"
+communicated by these types were only true when objects were created
+by calling the type--any operation could cause they types to have a value
+that did not satisfy the type's condition. For example, with
+`f: ReadableFile`, `f.parent` would be an object of type `ReadableFile`,
+but is not a file at all. For enforcing the conditions provided by the
+removed types in `Corgy` classes, custom parsers should be used instead.
+
+### Features
+
+* use `store_*` actions in `Corgy.add_args_to_parser` for single value literals ([88b0aa1](https://github.com/jayanthkoushik/corgy/commit/88b0aa15a6de4024b43185bd0ed09e54a3f3462b))
+
+
+* remove path sub-class types ([ac73147](https://github.com/jayanthkoushik/corgy/commit/ac7314733ffcca1c1f3be0173a3a9fff1c9a587d))
+
 ## [7.0.0](https://github.com/jayanthkoushik/corgy/compare/v6.0.0...v7.0.0) (2023-04-11)
 
 
 ### ⚠ BREAKING CHANGES
 
 * A few types in `corgy.types` accepted arbitrary keyword
 arguments. This was not consistent, not tested, and has been removed.
```

### Comparing `corgy-7.0.0/LICENSE` & `corgy-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/README.md` & `corgy-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/_actions.py` & `corgy-8.0.0/corgy/_actions.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/_corgy.py` & `corgy-8.0.0/corgy/_corgy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from __future__ import annotations
 
 import argparse
 import sys
-from argparse import _ActionsContainer, Action, ArgumentParser
+from argparse import (
+    _ActionsContainer,
+    _StoreConstAction,
+    _StoreFalseAction,
+    _StoreTrueAction,
+    Action,
+    ArgumentParser,
+)
 from collections import defaultdict
 from collections.abc import Sequence as AbstractSequence
 from functools import partial
 from importlib import import_module
 from typing import Any, Callable, Dict, IO, Mapping, Optional, Type, TypeVar, Union
 
 if sys.version_info >= (3, 9):
@@ -625,14 +632,34 @@
             options:
               --x T  ({T1/T2} optional)
 
         For types which specify choices by defining `__choices__`, the values are
         passed to the `choices` argument as with `Literal`, but no type inference is
         performed, and the base attribute type will be used as the argument type.
 
+        **Single-value Literals**
+        A special case for `Literal` types is when there is only one choice. In this
+        case, the argument is added as a `store_const` action, with the value as the
+        `const` argument. A further special case is when the choice is `True/False`,
+        in which case the action is `store_true`/`store_false` respectively::
+
+            >>> class A(Corgy):
+            ...     x: Literal[True]
+            ...     y: Literal[False]
+            ...     z: Literal[42]
+
+            >>> parser = ArgumentParser()
+            >>> A.add_args_to_parser(parser)
+            >>> parser.parse_args(["--x"])  # Note that `y` and `z` are absent
+            Namespace(x=True)
+            >>> parser.parse_args(["--y"])
+            Namespace(y=False)
+            >>> parser.parse_args(["--z"])
+            Namespace(z=42)
+
         *Corgy*
         Attributes which are themselves `Corgy` types are treated as argument groups.
         Group arguments are added to the command line parser with the group attribute
         name prefixed. Note that groups will ignore any custom flags when computing the
         prefix; elements within the group will use custom flags, but because they are
         prefixed with `--`, they will not be positional.
 
@@ -820,14 +847,36 @@
             else:
                 var_choices = None
 
             var_type_metavar: Optional[str] = getattr(
                 var_base_type, "__metavar__", None
             )
 
+            # Convert single choice attributes to `store_*` actions.
+            if (
+                var_choices is not None
+                and len(var_choices) == 1
+                and var_nargs is None
+                and var_action is None
+            ):
+                _choice = var_choices[0]
+                if _choice is True:
+                    var_action = _StoreTrueAction
+                    var_const = None
+                elif _choice is False:
+                    var_action = _StoreFalseAction
+                    var_const = None
+                else:
+                    var_action = _StoreConstAction
+                    var_const = _choice
+                var_choices = None
+                var_base_type = None
+            else:
+                var_const = None
+
             # Check if the variable is boolean. Boolean variables are converted to
             # `--<var-name>`/`--no-<var-name>` arguments.
             if (
                 var_base_type is bool
                 and var_nargs is None
                 and var_action is None
                 and var_choices is None
@@ -869,15 +918,19 @@
             elif var_required and not var_positional:
                 _kwargs["required"] = True
             elif not var_positional:
                 _kwargs["default"] = argparse.SUPPRESS
 
             if var_type_metavar is not None:
                 _kwargs["metavar"] = var_type_metavar
-            parser.add_argument(*var_flags, type=var_add_type, **_kwargs)
+            if var_add_type is not None:
+                _kwargs["type"] = var_add_type
+            if var_const is not None:
+                _kwargs["const"] = var_const
+            parser.add_argument(*var_flags, **_kwargs)
 
     def __init__(self, **args):
         if self.__class__ is Corgy:
             raise TypeError("`Corgy` is an abstract class and cannot be instantiated")
 
         setattr(self, f"_{self.__class__.__name__.lstrip('_')}__frozen", False)
```

### Comparing `corgy-7.0.0/corgy/_corgyparser.py` & `corgy-8.0.0/corgy/_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/_helpfmt.py` & `corgy-8.0.0/corgy/_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/_meta.py` & `corgy-8.0.0/corgy/_meta.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/types/__init__.py` & `corgy-8.0.0/corgy/types/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,38 +22,34 @@
     >>> a_subcls_obj = a_subcls()
     >>> a_subcls_obj  # doctest: +SKIP
     <B object at 0x106cd93d0>
 
     >>> import argparse
     >>> from argparse import ArgumentParser
     >>> from corgy import CorgyHelpFormatter
-    >>> from corgy.types import InputDirectory
+    >>> from corgy.types import InputFile
     >>> parser = ArgumentParser(
     ...     formatter_class=CorgyHelpFormatter,
     ...     add_help=False,
     ...     usage=argparse.SUPPRESS,
     ... )
-    >>> _ = parser.add_argument("--d", type=InputDirectory)
+    >>> _ = parser.add_argument("--f", type=InputFile)
     >>> parser.print_help()
     options:
-      --d dir  (default: None)
+      --f file  (default: None)
 
 """
 
-from ._dir import *
-from ._filepath import *
 from ._initargs import *
 from ._inputfile import *
 from ._keyvaluepairs import *
 from ._outputfile import *
 from ._subclass import *
 
 # pylint: disable=undefined-variable
 __all__ = (
-    _filepath.__all__  # type: ignore
-    + _outputfile.__all__  # type: ignore
+    _outputfile.__all__  # type: ignore
     + _inputfile.__all__  # type: ignore
-    + _dir.__all__  # type: ignore
     + _subclass.__all__  # type: ignore
     + _keyvaluepairs.__all__  # type: ignore
     + _initargs.__all__  # type: ignore
 )
```

### Comparing `corgy-7.0.0/corgy/types/_expand.py` & `corgy-8.0.0/corgy/types/_expand.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/types/_initargs.py` & `corgy-8.0.0/corgy/types/_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/types/_inputfile.py` & `corgy-8.0.0/corgy/types/_inputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/types/_keyvaluepairs.py` & `corgy-8.0.0/corgy/types/_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/types/_outputfile.py` & `corgy-8.0.0/corgy/types/_outputfile.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/corgy/types/_subclass.py` & `corgy-8.0.0/corgy/types/_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/docs/corgy.md` & `corgy-8.0.0/docs/corgy.md`

 * *Files 0% similar despite different names*

```diff
@@ -668,14 +668,36 @@
   --x T  ({T1/T2} optional)
 ```
 
 For types which specify choices by defining `__choices__`, the values are
 passed to the `choices` argument as with `Literal`, but no type inference is
 performed, and the base attribute type will be used as the argument type.
 
+**Single-value Literals**
+A special case for `Literal` types is when there is only one choice. In this
+case, the argument is added as a `store_const` action, with the value as the
+`const` argument. A further special case is when the choice is `True/False`,
+in which case the action is `store_true`/`store_false` respectively:
+
+```python
+>>> class A(Corgy):
+...     x: Literal[True]
+...     y: Literal[False]
+...     z: Literal[42]
+
+>>> parser = ArgumentParser()
+>>> A.add_args_to_parser(parser)
+>>> parser.parse_args(["--x"])  # Note that `y` and `z` are absent
+Namespace(x=True)
+>>> parser.parse_args(["--y"])
+Namespace(y=False)
+>>> parser.parse_args(["--z"])
+Namespace(z=42)
+```
+
 *Corgy*
 Attributes which are themselves `Corgy` types are treated as argument groups.
 Group arguments are added to the command line parser with the group attribute
 name prefixed. Note that groups will ignore any custom flags when computing the
 prefix; elements within the group will use custom flags, but because they are
 prefixed with `--`, they will not be positional.
```

### Comparing `corgy-7.0.0/docs/corgy.types.md` & `corgy-8.0.0/docs/corgy.types.md`

 * *Files 21% similar despite different names*

```diff
@@ -25,62 +25,27 @@
 >>> a_subcls_obj = a_subcls()
 >>> a_subcls_obj
 <B object at 0x106cd93d0>
 
 >>> import argparse
 >>> from argparse import ArgumentParser
 >>> from corgy import CorgyHelpFormatter
->>> from corgy.types import InputDirectory
+>>> from corgy.types import InputFile
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
 ...     usage=argparse.SUPPRESS,
 ... )
->>> _ = parser.add_argument("--d", type=InputDirectory)
+>>> _ = parser.add_argument("--f", type=InputFile)
 >>> parser.print_help()
 options:
-  --d dir  (default: None)
+  --f file  (default: None)
 ```
 
 
-### _class_ corgy.types.ReadableFile(path)
-`Path` sub-class representing a readable file.
-
-
-* **Parameters**
-
-    **path** – String or path-like object.
-
-
-The provided path must point to an existing file, and the file must be readable.
-`ValueError` is raised otherwise.
-
-User directory and environment variable expansion is performed on the path.
-To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
-to `False` respectively.
-
-
-### _class_ corgy.types.WritableFile(path)
-`Path` sub-class representing a writable file.
-
-
-* **Parameters**
-
-    **path** – String or path-like object.
-
-
-If the path exists, it must be a file, and it must be writable. If the path does
-not exist, the path’s directory must exist and be writable. `ValueError` is
-raised otherwise.
-
-User directory and environment variable expansion is performed on the path.
-To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
-to `False` respectively.
-
-
 ### _class_ corgy.types.OutputTextFile(path)
 `TextIOWrapper` sub-class representing an output file.
 
 
 * **Parameters**
 
     **path** – Path to a file.
@@ -171,77 +136,14 @@
 to close the file on program termination.
 
 User directory and environment variable expansion is performed on the path.
 To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
 to `False` respectively.
 
 
-### _class_ corgy.types.OutputDirectory(path)
-`Path` sub-class representing a directory to be written to.
-
-
-* **Parameters**
-
-    **path** – Path to a directory.
-
-
-If the path does not exist, a directory with the path name will be created
-(including any parent directories). `ValueError` is raised if this fails, or
-if the path is not a directory, or if the directory is not writable.
-
-User directory and environment variable expansion is performed on the path.
-To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
-to `False` respectively.
-
-
-### _class_ corgy.types.LazyOutputDirectory(path)
-`OutputDirectory` sub-class that does not auto-initialize.
-
-Useful for “default” folders, which only need to be created if an alternative is not
-provided. `init` must be called on instances to ensure that the directory exists.
-
-User directory and environment variable expansion is performed on the path.
-To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
-to `False` respectively.
-
-
-### _class_ corgy.types.InputDirectory(path)
-`Path` sub-class representing a directory to be read from.
-
-
-* **Parameters**
-
-    **path** – Path to a directory.
-
-
-The directory must exist, and will be checked to ensure it is readable.
-`ValueError` is raised if this is not the case.
-
-User directory and environment variable expansion is performed on the path.
-To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
-to `False` respectively.
-
-
-### _class_ corgy.types.IODirectory(path)
-`Path` sub-class representing an existing directory to be read from/written to.
-
-
-* **Parameters**
-
-    **path** – Path to a directory.
-
-
-The directory must exist, and will be checked to ensure it is readable and
-writeable. `ValueError` is raised if this is not the case.
-
-User directory and environment variable expansion is performed on the path.
-To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
-to `False` respectively.
-
-
 ### _class_ corgy.types.SubClass(name)
 Type representing a sub-class of a given class.
 
 Example:
 
 ```python
 >>> from corgy.types import SubClass
```

### Comparing `corgy-7.0.0/pyproject.toml` & `corgy-8.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corgy"
-version = "7.0.0"  # managed by `poetry-dynamic-versioning`
+version = "8.0.0"  # managed by `poetry-dynamic-versioning`
 description = "Elegant data classes"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
   { include = "corgy" },
```

### Comparing `corgy-7.0.0/tests/test_corgy.py` & `corgy-8.0.0/tests/test_corgy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # pylint: disable=abstract-class-instantiated
 import argparse
 import sys
-from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, ArgumentTypeError
+from argparse import (
+    _StoreConstAction,
+    _StoreFalseAction,
+    _StoreTrueAction,
+    ArgumentDefaultsHelpFormatter,
+    ArgumentParser,
+    ArgumentTypeError,
+)
 from collections.abc import Sequence as AbstractSequence
 from io import BytesIO
 from typing import ClassVar, List, Optional, Sequence, Set, Tuple
 from unittest import skipIf, TestCase
 from unittest.mock import MagicMock, patch
 
 SequenceType = Sequence
@@ -1732,14 +1739,50 @@
             x: A
 
         C.add_args_to_parser(self.parser)
         self.parser.add_argument.assert_called_once_with(
             "--x", type=A, required=True, choices=(1, 2, 3)
         )
 
+    def test_add_args_uses_store_const_action_for_single_choice_literal(self):
+        class A:
+            __choices__ = (42,)
+
+        for type_ in (A, Literal[42]):
+            with self.subTest(type=type_):
+
+                class C(Corgy):
+                    x: type_
+
+                self.setUp()
+                C.add_args_to_parser(self.parser)
+                self.parser.add_argument.assert_called_once_with(
+                    "--x", action=_StoreConstAction, const=42, required=True
+                )
+
+    def test_add_args_uses_store_true_false_action_for_true_false_literal(self):
+        for val in (True, False):
+
+            class A:
+                __choices__ = (val,)
+
+            for type_ in (A, Literal[val]):  # type: ignore
+                with self.subTest(val=val, type=type_):
+
+                    class C(Corgy):
+                        x: type_
+
+                    self.setUp()
+                    C.add_args_to_parser(self.parser)
+                    self.parser.add_argument.assert_called_once_with(
+                        "--x",
+                        action=(_StoreTrueAction if val else _StoreFalseAction),
+                        required=True,
+                    )
+
     def test_add_args_handles_user_defined_class_as_type(self):
         class T:
             ...
 
         class C(Corgy):
             x: T
 
@@ -2624,14 +2667,27 @@
             raise ArgumentTypeError(None, msg)
 
         self.parser.error = _raise_error
 
         with self.assertRaises(ArgumentTypeError):
             C.parse_from_cmdline(self.parser, add_help=False)
 
+    def test_parse_from_cmdline_handles_single_value_literal(self):
+        class C(Corgy):
+            x: Literal[42]
+
+        self.parser.parse_args = lambda: self.orig_parse_args(self.parser, ["--x"])
+        c = C.parse_from_cmdline(self.parser)
+        self.assertTrue(hasattr(c, "x"))
+
+        self.setUp()
+        self.parser.parse_args = lambda: self.orig_parse_args(self.parser, [])
+        c = C.parse_from_cmdline(self.parser)
+        self.assertFalse(hasattr(c, "x"))
+
 
 @skipIf(tomli is None, "`tomli` package not found")
 class TestCorgyTomlParsing(TestCase):
     def test_toml_file_parsed_to_corgy_object(self):
         class C(Corgy):
             x: int
```

### Comparing `corgy-7.0.0/tests/test_corgyparser.py` & `corgy-8.0.0/tests/test_corgyparser.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/tests/test_helpfmt.py` & `corgy-8.0.0/tests/test_helpfmt.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/tests/types/_specialtmps.py` & `corgy-8.0.0/tests/types/_specialtmps.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/tests/types/_test_file.py` & `corgy-8.0.0/tests/types/_test_file.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/tests/types/test_dirs.py` & `corgy-8.0.0/tests/types/test_outputfiles.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,163 +1,136 @@
 import os
+import sys
+from io import BufferedWriter, TextIOWrapper
 from pathlib import Path
-from stat import S_IEXEC, S_IREAD, S_IWRITE
+from stat import S_IREAD, S_IWRITE
 from tempfile import TemporaryDirectory
 from typing import Type, Union
-from unittest import skipIf, TestCase
+from unittest import skipIf
 from unittest.mock import MagicMock, patch
 
 from corgy.types import (
-    InputDirectory,
-    IODirectory,
-    LazyOutputDirectory,
-    OutputDirectory,
+    LazyOutputBinFile,
+    LazyOutputTextFile,
+    OutputBinFile,
+    OutputTextFile,
 )
 
-from ._specialtmps import temp_dir_in_home, temp_env_var_dir
+from ._test_file import TestFileWrapper
 
 
-class _TestDirectoryWrapper:
-    class TestDirectory(TestCase):
-        type: Union[Type[OutputDirectory], Type[InputDirectory], Type[IODirectory]]
+class _TestOutputFileWrapper:
+    class TestOutputFile(TestFileWrapper.TestFile):
+        def test_output_file_creates_dir_if_not_exists(self):
+            fname = os.path.join(self.tmp_dir.name, "foo", "bar", "baz.file")
+            with self.type(fname):
+                self.assertTrue(os.path.exists(fname))
+
+        def test_output_file_raises_if_dir_create_fails(self):
+            with patch(
+                "corgy.types._outputfile.os.makedirs", MagicMock(side_effect=OSError)
+            ):
+                with self.assertRaises(ValueError):
+                    self.type(os.path.join(self.tmp_dir.name, "foo", "bar", "baz.file"))
 
-        def setUp(self):
-            self.tmp_dir = TemporaryDirectory()  # pylint: disable=consider-using-with
-
-        def tearDown(self):
-            self.tmp_dir.cleanup()
-
-        def test_directory_returns_pathlib_path(self):
-            d = self.type(self.tmp_dir.name)
-            self.assertIsInstance(d, self.type)
-            self.assertIsInstance(d, Path)
-            self.assertEqual(str(d), self.tmp_dir.name)
-
-        def test_directory_raises_if_path_not_dir(self):
+        @skipIf(os.name == "nt", "`chmod` does not seem to work on Windows")
+        def test_output_file_fails_if_file_not_writeable(self):
             fname = os.path.join(self.tmp_dir.name, "foo.file")
             open(  # pylint: disable=unspecified-encoding,consider-using-with
                 fname, "x"
             ).close()
+            os.chmod(fname, S_IREAD)
             with self.assertRaises(ValueError):
                 self.type(fname)
+            os.chmod(fname, S_IREAD | S_IWRITE)
 
-        def test_directory_repr(self):
-            d = self.type(self.tmp_dir.name)
-            self.assertEqual(repr(d), f"{self.type.__name__}({self.tmp_dir.name!r})")
-            self.assertEqual(str(d), self.tmp_dir.name)
-
-        def test_directory_accepts_path(self):
-            d = self.type(Path(self.tmp_dir.name))
-            self.assertEqual(str(d), self.tmp_dir.name)
-
-        def test_directory_expands_user(self):
-            with temp_dir_in_home(self) as d:
-                td = self.type(os.path.join("~", d.name))
-                self.assertEqual(str(td), str(d))
-
-        def test_directory_does_not_expand_user_if_disabled(self):
-            class D(self.type):
-                do_expanduser = False
-
-            with temp_dir_in_home(self) as d:
-                if issubclass(self.type, OutputDirectory):
-                    td = D(os.path.join("~", d.name))
-                    td.init()
-                    self.assertNotEqual(str(td), str(d))
-                    os.rmdir(td)
-                    os.rmdir("~")
-                else:
-                    with self.assertRaises(ValueError):
-                        D(os.path.join("~", d.name))
-
-        def test_directory_expands_env_var(self):
-            with temp_env_var_dir(self) as (env_var, d):
-                td = self.type(f"${env_var}")
-                self.assertEqual(str(td), str(d))
-
-        def test_directory_does_not_expand_env_var_if_disabled(self):
-            class D(self.type):
-                do_expandvars = False
-
-            with temp_env_var_dir(self) as (env_var, d):
-                if issubclass(self.type, OutputDirectory):
-                    td = D(f"${env_var}")
-                    td.init()
-                    self.assertNotEqual(str(td), str(d))
-                    os.rmdir(td)
-                else:
-                    with self.assertRaises(ValueError):
-                        D(f"${env_var}")
-
-
-class TestOutputDirectory(_TestDirectoryWrapper.TestDirectory):
-    type = OutputDirectory
-
-    def test_output_directory_creates_dir_if_not_exists(self):
-        dname = os.path.join(self.tmp_dir.name, "foo", "bar", "baz")
-        self.type(dname)
-        self.assertTrue(os.path.exists(dname))
+        def test_output_file_handles_existing_file(self):
+            fname = os.path.join(self.tmp_dir.name, "foo.file")
+            with open(fname, "wb") as f:
+                f.write(b"foo")
+            of = self.type(fname)
+            with open(fname, "rb") as f:
+                self.assertEqual(f.read(), b"")
+            of.close()
+
+        def test_output_file_repr_str(self):
+            fname = os.path.join(self.tmp_dir.name, "foo.file")
+            with self.type(fname) as f:
+                self.assertEqual(repr(f), f"{self.type.__name__}({fname!r})")
+                self.assertEqual(str(f), fname)
+
+        def test_output_file_accepts_path(self):
+            fname = self.tmp_dir.name / Path("foo.file")
+            with self.type(fname):
+                self.assertTrue(fname.exists())
+
+
+class TestOutputTextFile(_TestOutputFileWrapper.TestOutputFile):
+    type = OutputTextFile
+
+    def test_output_text_file_type(self):
+        with self.type(os.path.join(self.tmp_dir.name, "foo.txt")) as f:
+            self.assertIsInstance(f, TextIOWrapper)
+
+    def test_output_text_file_stdouterr_wrappers(self):
+        for wrapper, buffer in zip(
+            [OutputTextFile.stdout_wrapper(), OutputTextFile.stderr_wrapper()],
+            [sys.__stdout__.buffer, sys.__stderr__.buffer],
+        ):
+            with self.subTest(wrapper=wrapper):
+                self.assertIsInstance(wrapper, OutputTextFile)
+                self.assertIs(wrapper.buffer, buffer)
+
+
+class TestOutputBinFile(_TestOutputFileWrapper.TestOutputFile):
+    type = OutputBinFile
+
+    def test_output_bin_file_type(self):
+        with self.type(os.path.join(self.tmp_dir.name, "foo.bin")) as f:
+            self.assertIsInstance(f, BufferedWriter)
+
+    def test_output_bin_file_stdouterr_wrappers(self):
+        for wrapper, buffer in zip(
+            [OutputBinFile.stdout_wrapper(), OutputBinFile.stderr_wrapper()],
+            [sys.__stdout__.buffer, sys.__stderr__.buffer],
+        ):
+            with self.subTest(wrapper=wrapper):
+                self.assertIsInstance(wrapper, OutputBinFile)
+                self.assertEqual(wrapper.fileno(), buffer.fileno())
+
+
+class _TestLazyOutputFileWrapper:
+    class TestLazyOutputFile(TestFileWrapper.TestFile):
+        type: Union[Type[LazyOutputTextFile], Type[LazyOutputBinFile]]
+
+        def test_lazy_output_file_does_not_auto_create_file(self):
+            fname = os.path.join(self.tmp_dir.name, "foo.file")
+            self.type(fname)
+            self.assertFalse(os.path.exists(fname))
+
+        def test_lazy_output_file_creates_on_calling_init(self):
+            fname = os.path.join(self.tmp_dir.name, "foo.file")
+            f = self.type(fname)
+            f.init()
+            self.assertTrue(os.path.exists(fname))
+            f.close()
+
+        def test_lazy_output_file_handles_existing_file(self):
+            with TemporaryDirectory() as tmp_dir:
+                fpath = os.path.join(tmp_dir, "foo.file")
+                with open(fpath, "wb") as f:
+                    f.write(b"foo")
+                lazyf = self.type(fpath)
+                with open(fpath, "rb") as f:
+                    self.assertEqual(f.read(), b"foo")
+                lazyf.init()
+                with open(fpath, "rb") as f:
+                    self.assertEqual(f.read(), b"")
+                lazyf.close()
+
+
+class TestLazyOutputTextFile(_TestLazyOutputFileWrapper.TestLazyOutputFile):
+    type = LazyOutputTextFile
 
-    def test_output_directory_raises_if_dir_create_fails(self):
-        with patch("corgy.types._dir.os.makedirs", MagicMock(side_effect=OSError)):
-            with self.assertRaises(ValueError):
-                self.type(os.path.join(self.tmp_dir.name, "foo", "bar", "baz"))
 
-    @skipIf(os.name == "nt", "`chmod` does not seem to work on Windows")
-    def test_output_directory_raises_if_dir_not_writeable(self):
-        dname = os.path.join(self.tmp_dir.name, "foo", "bar", "baz")
-        os.makedirs(dname)
-        os.chmod(dname, S_IREAD | S_IEXEC)
-        with self.assertRaises(ValueError):
-            self.type(dname)
-        os.chmod(dname, S_IREAD | S_IWRITE | S_IEXEC)
-
-
-class TestLazyOutputDirectory(TestCase):
-    def setUp(self):
-        self.tmp_dir = TemporaryDirectory()  # pylint: disable=consider-using-with
-
-    def tearDown(self):
-        self.tmp_dir.cleanup()
-
-    def test_lazy_output_directory_does_not_auto_create_dir(self):
-        dname = os.path.join(self.tmp_dir.name, "foo")
-        LazyOutputDirectory(dname)
-        self.assertFalse(os.path.exists(dname))
-
-    def test_lazy_output_directory_creates_dir_on_init(self):
-        dname = os.path.join(self.tmp_dir.name, "foo", "bar", "baz")
-        d = LazyOutputDirectory(dname)
-        d.init()
-        self.assertTrue(os.path.exists(dname))
-        self.assertEqual(str(d), dname)
-
-
-class TestInputDirectory(_TestDirectoryWrapper.TestDirectory):
-    type = InputDirectory
-
-    def test_input_directory_raises_if_dir_not_exists(self):
-        with self.assertRaises(ValueError):
-            self.type(os.path.join(self.tmp_dir.name, "nota.dir"))
-
-    @skipIf(os.name == "nt", "`chmod` does not seem to work on Windows")
-    def test_input_directory_raises_if_dir_not_readable(self):
-        dname = os.path.join(self.tmp_dir.name, "foo", "bar", "baz")
-        os.makedirs(dname)
-        os.chmod(dname, 0)
-        with self.assertRaises(ValueError):
-            self.type(dname)
-        os.chmod(dname, S_IREAD | S_IWRITE | S_IEXEC)
-
-
-class TestIODirectory(_TestDirectoryWrapper.TestDirectory):
-    type = IODirectory
-
-    test_io_directory_raises_if_dir_not_exists = (
-        TestInputDirectory.test_input_directory_raises_if_dir_not_exists
-    )
-    test_io_directory_raises_if_dir_not_readable = (
-        TestInputDirectory.test_input_directory_raises_if_dir_not_readable
-    )
-    test_io_directory_raises_if_dir_not_writeable = (
-        TestOutputDirectory.test_output_directory_raises_if_dir_not_writeable
-    )
+class TestLazyOutputBinFile(_TestLazyOutputFileWrapper.TestLazyOutputFile):
+    type = LazyOutputBinFile
```

### Comparing `corgy-7.0.0/tests/types/test_initargs.py` & `corgy-8.0.0/tests/types/test_initargs.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/tests/types/test_inputfiles.py` & `corgy-8.0.0/tests/types/test_inputfiles.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/tests/types/test_keyvaluepairs.py` & `corgy-8.0.0/tests/types/test_keyvaluepairs.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/tests/types/test_subclass.py` & `corgy-8.0.0/tests/types/test_subclass.py`

 * *Files identical despite different names*

### Comparing `corgy-7.0.0/PKG-INFO` & `corgy-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 7.0.0
+Version: 8.0.0
 Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
 Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
```

