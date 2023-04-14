# Comparing `tmp/robocorp_logging-0.0.6.tar.gz` & `tmp/robocorp_logging-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_logging-0.0.6.tar", max compression
+gzip compressed data, was "robocorp_logging-0.0.7.tar", max compression
```

## Comparing `robocorp_logging-0.0.6.tar` & `robocorp_logging-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    10142 2023-04-13 13:57:55.411195 robocorp_logging-0.0.6/LICENSE
--rw-r--r--   0        0        0     1021 2023-04-13 13:57:55.411195 robocorp_logging-0.0.6/README.md
--rw-r--r--   0        0        0      936 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    12763 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/__init__.py
--rw-r--r--   0        0        0     8075 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_ast_utils.py
--rw-r--r--   0        0        0     4542 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_auto_logging_setup.py
--rw-r--r--   0        0        0     1857 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_config.py
--rw-r--r--   0        0        0      572 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_convert_units.py
--rw-r--r--   0        0        0     6297 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_decoder.py
--rw-r--r--   0        0        0     1915 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_lifecycle_hooks.py
--rw-r--r--   0        0        0      493 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_logger_instances.py
--rw-r--r--   0        0        0    10505 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0    12108 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12044 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_rewrite_importhook.py
--rw-r--r--   0        0        0     8184 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_robo_logger.py
--rw-r--r--   0        0        0    48322 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/_robo_output_impl.py
--rw-r--r--   0        0        0    41722 2023-04-13 13:58:49.275020 robocorp_logging-0.0.6/src/robo_log/index.py
--rw-r--r--   0        0        0    46480 2023-04-13 13:58:52.579013 robocorp_logging-0.0.6/src/robo_log/index_v2.py
--rw-r--r--   0        0        0      511 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/protocols.py
--rw-r--r--   0        0        0        0 2023-04-13 13:57:55.419195 robocorp_logging-0.0.6/src/robo_log/py.typed
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 robocorp_logging-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-14 17:04:10.498247 robocorp_logging-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1021 2023-04-14 17:04:10.498247 robocorp_logging-0.0.7/README.md
+-rw-r--r--   0        0        0      985 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    13329 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/__init__.py
+-rw-r--r--   0        0        0     8413 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_ast_utils.py
+-rw-r--r--   0        0        0     4311 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     2697 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_config.py
+-rw-r--r--   0        0        0      572 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_convert_units.py
+-rw-r--r--   0        0        0     6297 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_decoder.py
+-rw-r--r--   0        0        0     1915 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0      493 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_logger_instances.py
+-rw-r--r--   0        0        0    11842 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0    10726 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12161 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_rewrite_importhook.py
+-rw-r--r--   0        0        0     8412 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_robo_logger.py
+-rw-r--r--   0        0        0    48322 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/_robo_output_impl.py
+-rw-r--r--   0        0        0    41722 2023-04-14 17:04:48.498617 robocorp_logging-0.0.7/src/robo_log/index.py
+-rw-r--r--   0        0        0    46480 2023-04-14 17:04:50.826635 robocorp_logging-0.0.7/src/robo_log/index_v2.py
+-rw-r--r--   0        0        0      511 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/protocols.py
+-rw-r--r--   0        0        0        0 2023-04-14 17:04:10.502247 robocorp_logging-0.0.7/src/robo_log/py.typed
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 robocorp_logging-0.0.7/PKG-INFO
```

### Comparing `robocorp_logging-0.0.6/LICENSE` & `robocorp_logging-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.6/README.md` & `robocorp_logging-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.6/pyproject.toml` & `robocorp_logging-0.0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-logging"
-version = "0.0.6"
+version = "0.0.7"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Z. <fabio@robocorp.com>",
     "Ossi R. <ossi@robocorp.com>",
     "Kerkko P. <kerkko@robocorp.com>",
 ]
 readme = "README.md"
@@ -24,14 +24,15 @@
 
 [[tool.mypy.overrides]]
 module = "pytest_timeout.*"
 ignore_missing_imports = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
+tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pytest-xdist = "^3.2.1"
 pytest-regressions = "1.0.6"
```

### Comparing `robocorp_logging-0.0.6/src/robo_log/__init__.py` & `robocorp_logging-0.0.7/src/robo_log/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,24 @@
     List,
     Sequence,
     Dict,
     Union,
     Iterable,
     Literal,
 )
-from ._config import Filter
+from ._config import Filter, FilterKind
 from ._logger_instances import _get_logger_instances
 from .protocols import OptExcInfo, LogHTMLStyle, Status
 from robo_log.protocols import IReadLines
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
+    from ._rewrite_filtering import FilesFiltering
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 # --- Logging methods for custom messaging.
 
 
 def _log(level, message: str, html: bool = False) -> None:
@@ -361,15 +362,15 @@
         library_roots = [
             (f if isinstance(f, str) else str(f.absolute())) for f in untracked_folders
         ]
     else:
         library_roots = None
 
     return register_auto_logging_callbacks(
-        ConfigFilesFiltering(project_roots, library_roots, filters)
+        ConfigFilesFiltering(project_roots, library_roots, filters, set_as_global=True)
     )
 
 
 def add_log_output(
     output_dir: Optional[Union[str, Path]] = None,
     max_file_size: str = "1MB",
     max_files: int = 5,
@@ -415,7 +416,21 @@
     _get_logger_instances()[logger] = 1
 
     def _exit():
         _get_logger_instances().pop(logger, None)
         logger.close()
 
     return OnExitContextManager(_exit)
+
+
+# Not part of the API, used to determine whether a file is a project file
+# or a library file when running with the FilterKind.log_on_project_call kind.
+# Only set/used when setting up auto-logging (changed at runtime).
+def _in_project_roots(filename: str) -> bool:
+    return False
+
+
+def _caller_in_project_roots() -> bool:
+    try:
+        return _in_project_roots(sys._getframe(2).f_code.co_filename)
+    except ValueError:  # call stack is not deep enough
+        return False
```

### Comparing `robocorp_logging-0.0.6/src/robo_log/_ast_utils.py` & `robocorp_logging-0.0.7/src/robo_log/_ast_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,32 +230,44 @@
         return self._set_line_col(assign)
 
     def NameLoad(self, name: str) -> ast.Name:
         return self._set_line_col(ast.Name(name, ast.Load()))
 
     def NameTempStore(self) -> ast.Name:
         name = f"@tmp_{self.next_var_id()}"
+        return self.NameStore(name)
+
+    def NameStore(self, name) -> ast.Name:
         return self._set_line_col(ast.Name(name, ast.Store()))
 
     def Attribute(self, name: ast.AST, attr_name: str) -> ast.Attribute:
         return self._set_line_col(ast.Attribute(name, attr_name, ast.Load()))
 
-    def NameLoadBuiltin(self, builtin_name: str) -> ast.Attribute:
-        builtin_ref = self.NameLoad("@py_builtins")
+    def NameLoadRewriteCallback(self, builtin_name: str) -> ast.Attribute:
+        ref = self.NameLoad("@robocorp_rewrite_callbacks")
 
-        return self._set_line_col(self.Attribute(builtin_ref, builtin_name))
+        return self._set_line_col(self.Attribute(ref, builtin_name))
 
-    def NameLoadRewriteCallback(self, builtin_name: str) -> ast.Attribute:
-        builtin_ref = self.NameLoad("@robocorp_rewrite_callbacks")
+    def NameLoadRobo(self, builtin_name: str) -> ast.Attribute:
+        ref = self.NameLoad("@robo_log")
 
-        return self._set_line_col(self.Attribute(builtin_ref, builtin_name))
+        return self._set_line_col(self.Attribute(ref, builtin_name))
 
     def Str(self, s) -> ast.Str:
         return self._set_line_col(ast.Str(s))
 
+    def If(self, cond) -> ast.If:
+        return self._set_line_col(ast.If(cond))
+
+    def AndExpr(self, expr1, expr2) -> ast.Expr:
+        andop = self._set_line_col(ast.And())
+        bool_op = self._set_line_col(ast.BoolOp(op=andop, values=[expr1, expr2]))
+
+        return self.Expr(bool_op)
+
     def Expr(self, expr) -> ast.Expr:
         return self._set_line_col(ast.Expr(expr))
 
     def Try(self) -> ast.Try:
         try_node = ast.Try(handlers=[], orelse=[])
         return self._set_line_col(try_node)
```

### Comparing `robocorp_logging-0.0.6/src/robo_log/_auto_logging_setup.py` & `robocorp_logging-0.0.7/src/robo_log/_auto_logging_setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,19 +112,14 @@
         try:
             pop_package, pop_name, _curr_status = status_stack[-1]
         except IndexError:
             # oops, something bad happened, the stack is unsynchronized
             critical("On method except the status_stack was empty.")
             return
 
-        if pop_package != package or pop_name != name:
-            critical(
-                f"On method except status stack package/name was: {pop_package}.{pop_name}. Received: {package}.{name}."
-            )
-            return
         status_stack[-1][2] = Status.ERROR
 
         for robo_logger in _get_logger_instances():
             robo_logger.log_method_except(exc_info, unhandled=False)
 
     before_method.register(call_before_method)
     after_method.register(call_after_method)
```

### Comparing `robocorp_logging-0.0.6/src/robo_log/_convert_units.py` & `robocorp_logging-0.0.7/src/robo_log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.6/src/robo_log/_decoder.py` & `robocorp_logging-0.0.7/src/robo_log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.6/src/robo_log/_lifecycle_hooks.py` & `robocorp_logging-0.0.7/src/robo_log/_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.6/src/robo_log/_rewrite_ast_add_callbacks.py` & `robocorp_logging-0.0.7/src/robo_log/_rewrite_ast_add_callbacks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,305 @@
 import ast
-from typing import Optional, Any, Union, List
-import sys
+from typing import Any, Union, List, Optional, Tuple
 from . import _ast_utils
-from ._config import BaseConfig
+from ._config import BaseConfig, FilterKind
 
 DEBUG = False
 
 
 def is_rewrite_disabled(docstring: str) -> bool:
     return "NO_LOG" in docstring
 
 
+def _make_import_aliases_ast(lineno, filter_kind: FilterKind):
+    aliases = [
+        ast.alias(
+            "robo_log._lifecycle_hooks",
+            "@robocorp_rewrite_callbacks",
+            lineno=lineno,
+            col_offset=0,
+        ),
+    ]
+
+    if filter_kind == FilterKind.log_on_project_call:
+        aliases.append(ast.alias("robo_log", "@robo_log", lineno=lineno, col_offset=0))
+
+    imports = [ast.Import([alias], lineno=lineno, col_offset=0) for alias in aliases]
+    return imports
+
+
+def _get_function_and_class_name(stack) -> Optional[Tuple[Any, str]]:
+    if not stack:
+        return None
+    stack_it = reversed(stack)
+    for function in stack_it:
+        if function.__class__.__name__ != "FunctionDef":
+            continue
+        break
+    else:
+        return None
+
+    class_name = ""
+    try:
+        parent = next(stack_it)
+        if parent.__class__.__name__ == "ClassDef":
+            class_name = parent.name + "."
+    except StopIteration:
+        pass
+
+    return function, class_name
+
+
+def _rewrite_return(function, class_name, node) -> Optional[list]:
+    if function.name.startswith("_"):
+        return None
+
+    factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
+
+    result: list = []
+
+    call = factory.Call()
+    call.func = factory.NameLoadRewriteCallback("method_return")
+    call.args.append(factory.NameLoad("__package__"))
+    call.args.append(factory.NameLoad("__name__"))
+    call.args.append(factory.NameLoad("__file__"))
+    call.args.append(factory.Str(f"{class_name}{function.name}"))
+    call.args.append(factory.LineConstant())
+
+    if node.value:
+        assign = factory.Assign()
+        store_name = factory.NameTempStore()
+        assign.targets = [store_name]
+        assign.value = node.value
+
+        node.value = factory.NameLoad(store_name.id)
+
+        result.append(assign)
+        call.args.append(factory.NameLoad(store_name.id))
+    else:
+        call.args.append(factory.NoneConstant())
+
+    result.append(factory.Expr(call))
+    result.append(node)
+    return result
+
+
+_EMPTY_LIST: list = []
+
+
+def _create_before_method_ast(factory, class_name, function, filter_kind) -> list:
+    # Target code:
+    # def method(a, b):
+    #     before_method(__package__, __name, __file__, "method_name", 11, {'a': a, 'b': b})
+    stmts: list = []
+
+    if filter_kind == FilterKind.log_on_project_call:
+        # In this case we need to create a local variable signaling whether
+        # the caller is in the project (as if it's not we won't log the calls).
+        call = factory.Call()
+        call.func = factory.NameLoadRobo("_caller_in_project_roots")
+
+        assign = factory.Assign()
+        caller_in_proj_name = factory.NameStore("@caller_in_proj")
+        assign.targets = [caller_in_proj_name]
+        assign.value = call
+        stmts.append(assign)
+
+    call = factory.Call()
+    call.func = factory.NameLoadRewriteCallback("before_method")
+    call.args.append(factory.NameLoad("__package__"))
+    call.args.append(factory.NameLoad("__name__"))
+    call.args.append(factory.NameLoad("__file__"))
+    call.args.append(factory.Str(f"{class_name}{function.name}"))
+    call.args.append(factory.LineConstant())
+
+    dct = factory.Dict()
+    keys: list[Union[ast.expr, None]] = []
+    values: list[ast.expr] = []
+    for arg in function.args.args:
+        if class_name and arg.arg == "self":
+            continue
+        keys.append(factory.Str(arg.arg))
+        values.append(factory.NameLoad(arg.arg))
+
+    if function.args.vararg:
+        keys.append(factory.Str(function.args.vararg.arg))
+        values.append(factory.NameLoad(function.args.vararg.arg))
+
+    if function.args.kwarg:
+        keys.append(factory.Str(function.args.kwarg.arg))
+        values.append(factory.NameLoad(function.args.kwarg.arg))
+    dct.keys = keys
+    dct.values = values
+    call.args.append(dct)
+
+    if filter_kind == FilterKind.log_on_project_call:
+        stmts.append(factory.AndExpr(factory.NameLoad("@caller_in_proj"), call))
+    else:
+        stmts.append(factory.Expr(call))
+    return stmts
+
+
+def _create_except_handler_ast(
+    factory,
+    class_name: str,
+    function: ast.FunctionDef,
+    last_body_lineno,
+    filter_kind: FilterKind,
+):
+    # Target code:
+    #     import sys as @py_sys
+    #     method_except(@py_sys.exc_info())
+    #     raise
+    #
+    # ExceptHandler
+    #   Import
+    #   Expr
+    #     Call
+    #       Name
+    #         Load
+    #       Call
+    #         Attribute
+    #           Name
+    #             Load
+    #           Load
+    #   Raise
+    aliases = [
+        ast.alias("sys", "@py_sys", lineno=last_body_lineno, col_offset=0),
+    ]
+
+    imports = [
+        ast.Import([alias], lineno=last_body_lineno, col_offset=0) for alias in aliases
+    ]
+
+    except_handler = factory.ExceptHandler()
+
+    if filter_kind == FilterKind.log_on_project_call:
+        if_stmt = factory.If(factory.NameLoad("@caller_in_proj"))
+        add_to_body = if_stmt.body = []
+        if_stmt.orelse = []
+        except_handler.body.append(if_stmt)
+    else:
+        add_to_body = except_handler.body
+
+    exc_info_attr = factory.Attribute(factory.NameLoad("@py_sys"), "exc_info")
+    call_exc_info = factory.Call()
+    call_exc_info.func = exc_info_attr
+
+    method_except = factory.NameLoadRewriteCallback("method_except")
+    call_method_except = factory.Call()
+    call_method_except.func = method_except
+    call_method_except.args.append(factory.NameLoad("__package__"))
+    call_method_except.args.append(factory.NameLoad("__name__"))
+    call_method_except.args.append(factory.NameLoad("__file__"))
+    call_method_except.args.append(factory.Str(f"{class_name}{function.name}"))
+    call_method_except.args.append(factory.LineConstant())
+    call_method_except.args.append(call_exc_info)
+
+    add_to_body.extend(imports)
+    add_to_body.append(factory.Expr(call_method_except))
+
+    except_handler.body.append(factory.Raise())
+    return except_handler
+
+
+def _create_after_method_ast(factory, class_name, function, filter_kind):
+    call = factory.Call()
+    call.func = factory.NameLoadRewriteCallback("after_method")
+    call.args.append(factory.NameLoad("__package__"))
+    call.args.append(factory.NameLoad("__name__"))
+    call.args.append(factory.NameLoad("__file__"))
+    call.args.append(factory.Str(f"{class_name}{function.name}"))
+    call.args.append(factory.LineConstant())
+
+    if filter_kind == FilterKind.log_on_project_call:
+        return factory.AndExpr(factory.NameLoad("@caller_in_proj"), call)
+    else:
+        return factory.Expr(call)
+
+
+def _rewrite_funcdef(stack, node, filter_kind):
+    parent: Any
+    function: ast.FunctionDef = node
+    if function.name.startswith("_") and function.name != "__init__":
+        return
+
+    if not function.body:
+        return
+    # Only rewrite functions which actually have some content.
+
+    class_name = ""
+    if stack:
+        parent = stack[-1]
+        if parent.__class__.__name__ == "ClassDef":
+            class_name = parent.name + "."
+
+    first_non_constant_stmt_index = 0
+    for stmt in function.body:
+        if (
+            stmt.__class__.__name__ == "Expr"
+            and stmt.value.__class__.__name__ == "Constant"
+        ):
+            first_non_constant_stmt_index += 1
+            continue
+        break
+
+    function_body = function.body
+    function.body = None  # Proper value will be set later.
+
+    # Separate the docstring.
+    if first_non_constant_stmt_index > 0:
+        function_body_prefix = function_body[0:first_non_constant_stmt_index]
+        function_body = function_body[first_non_constant_stmt_index:]
+    else:
+        function_body_prefix = _EMPTY_LIST
+
+    if not function_body:
+        # We had just the docstring, no real contents here
+        # (so, just restore the docstring).
+        function.body = function_body_prefix
+        return
+
+    factory = _ast_utils.NodeFactory(
+        function_body[0].lineno, function_body[0].col_offset
+    )
+
+    before_method_stmts = _create_before_method_ast(
+        factory, class_name, function, filter_kind
+    )
+
+    for stmt in reversed(before_method_stmts):
+        function_body.insert(0, stmt)
+
+    try_finally = factory.Try()
+    try_finally.body = function_body
+
+    factory = _ast_utils.NodeFactory(
+        function_body[-1].lineno, function_body[-1].col_offset
+    )
+
+    after_expr = _create_after_method_ast(factory, class_name, function, filter_kind)
+    try_finally.finalbody = [after_expr]
+
+    except_handler = _create_except_handler_ast(
+        factory, class_name, function, function_body[-1].lineno, filter_kind
+    )
+
+    handlers: List[ast.ExceptHandler] = [except_handler]
+    try_finally.handlers = handlers
+
+    function.body = function_body_prefix + [try_finally]
+
+
 def rewrite_ast_add_callbacks(
     mod: ast.Module,
-    source: Optional[bytes] = None,
-    module_path: Optional[str] = None,
-    config: Optional[BaseConfig] = None,
+    filter_kind: FilterKind,
+    source: bytes,
+    module_path: str,
+    config: BaseConfig,
 ) -> None:
     """Rewrite the module as needed so that the logging is done automatically."""
 
     if not mod.body:
         # Nothing to do.
         return
 
@@ -53,237 +333,48 @@
     # Special case: for a decorated function, set the lineno to that of the
     # first decorator, not the `def`. Issue #4984.
     if isinstance(item, ast.FunctionDef) and item.decorator_list:
         lineno = item.decorator_list[0].lineno
     else:
         lineno = item.lineno
     # Now actually insert the special imports.
-    if sys.version_info >= (3, 10):
-        aliases = [
-            ast.alias("builtins", "@py_builtins", lineno=lineno, col_offset=0),
-            ast.alias(
-                "robo_log._lifecycle_hooks",
-                "@robocorp_rewrite_callbacks",
-                lineno=lineno,
-                col_offset=0,
-            ),
-        ]
-    else:
-        aliases = [
-            ast.alias("builtins", "@py_builtins"),
-            ast.alias("robo_log._lifecycle_hooks", "@robocorp_rewrite_callbacks"),
-        ]
-
-    imports = [ast.Import([alias], lineno=lineno, col_offset=0) for alias in aliases]
+    imports = _make_import_aliases_ast(lineno, filter_kind)
     mod.body[pos:pos] = imports
 
     it: Any = _ast_utils.iter_and_replace_nodes(mod)
     node: Any
-    parent: Any
-    function: Any
-
-    EMPTY_LIST: list = []
 
     while True:
         try:
             stack, node = next(it)
         except StopIteration:
             break
 
         if node.__class__.__name__ == "Return":
-            if not stack:
+            func_and_class_name = _get_function_and_class_name(stack)
+            if not func_and_class_name:
                 continue
-            stack_it = reversed(stack)
-            for function in stack_it:
-                if function.__class__.__name__ != "FunctionDef":
-                    continue
-                break
+            function, class_name = func_and_class_name
 
-            class_name = ""
             try:
-                parent = next(stack_it)
-                if parent.__class__.__name__ == "ClassDef":
-                    class_name = parent.name + "."
-            except StopIteration:
-                pass
+                result = _rewrite_return(function, class_name, node)
+            except Exception:
+                raise RuntimeError(
+                    f"Error when rewriting function return: {function.name} line: {node.lineno} at: {module_path}"
+                )
 
-            if function.name.startswith("_"):
+            if result is None:
                 continue
-
-            factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
-
-            result: list = []
-
-            call = factory.Call()
-            call.func = factory.NameLoadRewriteCallback("method_return")
-            call.args.append(factory.NameLoad("__package__"))
-            call.args.append(factory.NameLoad("__name__"))
-            call.args.append(factory.NameLoad("__file__"))
-            call.args.append(factory.Str(f"{class_name}{function.name}"))
-            call.args.append(factory.LineConstant())
-
-            if node.value:
-                assign = factory.Assign()
-                store_name = factory.NameTempStore()
-                assign.targets = [store_name]
-                assign.value = node.value
-
-                node.value = factory.NameLoad(store_name.id)
-
-                result.append(assign)
-                call.args.append(factory.NameLoad(store_name.id))
-            else:
-                call.args.append(factory.NoneConstant())
-
-            result.append(factory.Expr(call))
-            result.append(node)
-
             it.send(result)
 
         elif node.__class__.__name__ == "FunctionDef":
-            function = node
-            if function.name.startswith("_") and function.name != "__init__":
-                continue
-
-            if function.body:
-                class_name = ""
-                if stack:
-                    parent = stack[-1]
-                    if parent.__class__.__name__ == "ClassDef":
-                        class_name = parent.name + "."
-
-                function_body = function.body
-
-                first_non_constant_stmt_index = 0
-                for stmt in function_body:
-                    if (
-                        stmt.__class__.__name__ == "Expr"
-                        and stmt.value.__class__.__name__ == "Constant"
-                    ):
-                        first_non_constant_stmt_index += 1
-                        continue
-                    break
-                function.body = None  # Proper value will be set later.
-
-                # Separate the docstring.
-                if first_non_constant_stmt_index > 0:
-                    function_body_prefix = function_body[
-                        0:first_non_constant_stmt_index
-                    ]
-                    function_body = function_body[first_non_constant_stmt_index:]
-                else:
-                    function_body_prefix = EMPTY_LIST
-
-                factory = _ast_utils.NodeFactory(
-                    function_body[0].lineno, function_body[0].col_offset
-                )
-
-                # Only rewrite functions which actually have some content.
-                call = factory.Call()
-                call.func = factory.NameLoadRewriteCallback("before_method")
-                call.args.append(factory.NameLoad("__package__"))
-                call.args.append(factory.NameLoad("__name__"))
-                call.args.append(factory.NameLoad("__file__"))
-                call.args.append(factory.Str(f"{class_name}{function.name}"))
-                call.args.append(factory.LineConstant())
-
-                dct = factory.Dict()
-                keys: list[Union[ast.expr, None]] = []
-                values: list[ast.expr] = []
-                for arg in function.args.args:
-                    if class_name and arg.arg == "self":
-                        continue
-                    keys.append(factory.Str(arg.arg))
-                    values.append(factory.NameLoad(arg.arg))
-
-                if function.args.vararg:
-                    keys.append(factory.Str(function.args.vararg.arg))
-                    values.append(factory.NameLoad(function.args.vararg.arg))
-
-                if function.args.kwarg:
-                    keys.append(factory.Str(function.args.kwarg.arg))
-                    values.append(factory.NameLoad(function.args.kwarg.arg))
-                dct.keys = keys
-                dct.values = values
-                call.args.append(dct)
-
-                function_body.insert(0, factory.Expr(call))
-
-                try_finally = factory.Try()
-                try_finally.body = function_body
-
-                factory = _ast_utils.NodeFactory(
-                    function_body[-1].lineno, function_body[-1].col_offset
-                )
-                call = factory.Call()
-                call.func = factory.NameLoadRewriteCallback("after_method")
-                call.args.append(factory.NameLoad("__package__"))
-                call.args.append(factory.NameLoad("__name__"))
-                call.args.append(factory.NameLoad("__file__"))
-                call.args.append(factory.Str(f"{class_name}{function.name}"))
-                call.args.append(factory.LineConstant())
-
-                try_finally.finalbody = [factory.Expr(call)]
-
-                # Target code:
-                #     import sys as @py_sys
-                #     method_except(@py_sys.exc_info())
-                #     raise
-                #
-                # ExceptHandler
-                #   Import
-                #   Expr
-                #     Call
-                #       Name
-                #         Load
-                #       Call
-                #         Attribute
-                #           Name
-                #             Load
-                #           Load
-                #   Raise
-                if sys.version_info >= (3, 10):
-                    aliases = [
-                        ast.alias("sys", "@py_sys", lineno=lineno, col_offset=0),
-                    ]
-                else:
-                    aliases = [
-                        ast.alias("sys", "@py_sys"),
-                    ]
-
-                imports = [
-                    ast.Import([alias], lineno=lineno, col_offset=0)
-                    for alias in aliases
-                ]
-
-                exc_info_attr = factory.Attribute(
-                    factory.NameLoad("@py_sys"), "exc_info"
-                )
-                call_exc_info = factory.Call()
-                call_exc_info.func = exc_info_attr
-
-                method_except = factory.NameLoadRewriteCallback("method_except")
-                call_method_except = factory.Call()
-                call_method_except.func = method_except
-                call_method_except.args.append(factory.NameLoad("__package__"))
-                call_method_except.args.append(factory.NameLoad("__name__"))
-                call_method_except.args.append(factory.NameLoad("__file__"))
-                call_method_except.args.append(
-                    factory.Str(f"{class_name}{function.name}")
+            try:
+                _rewrite_funcdef(stack, node, filter_kind)
+            except Exception:
+                raise RuntimeError(
+                    f"Error when rewriting function: {node.name} line: {node.lineno} at: {module_path}"
                 )
-                call_method_except.args.append(factory.LineConstant())
-                call_method_except.args.append(call_exc_info)
-
-                except_handler = factory.ExceptHandler()
-                except_handler.body.extend(imports)
-                except_handler.body.append(factory.Expr(call_method_except))
-                except_handler.body.append(factory.Raise())
-
-                handlers: List[ast.ExceptHandler] = [except_handler]
-                try_finally.handlers = handlers
-
-                function.body = function_body_prefix + [try_finally]
 
     if DEBUG:
         print("\n============ New AST (with hooks in place) ==============\n")
         # Note: only python 3.9 onwards.
         print(ast.unparse(mod))  # type: ignore
```

### Comparing `robocorp_logging-0.0.6/src/robo_log/_rewrite_filtering.py` & `robocorp_logging-0.0.7/src/robo_log/_rewrite_filtering.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import fnmatch
-import glob
 import os.path
 import sys
 
 import platform
 import logging
-from typing import Sequence, Optional, List, Dict, Any
+from typing import Sequence, Optional, List, Dict
 import threading
-from ._config import Filter
+from ._config import Filter, FilterKind
 
 log = logging.getLogger(__name__)
 
 
 def normcase(s, NORMCASE_CACHE={}):
     try:
         return NORMCASE_CACHE[s]
@@ -33,73 +31,14 @@
     for root in roots:
         assert isinstance(root, str), "%s not str (found: %s)" % (root, type(root))
         if root:
             new_roots.append(root)
     return new_roots
 
 
-def _check_matches(patterns, paths):
-    if not patterns and not paths:
-        # Matched to the end.
-        return True
-
-    if (not patterns and paths) or (patterns and not paths):
-        return False
-
-    pattern = normcase(patterns[0])
-    path = normcase(paths[0])
-
-    if not glob.has_magic(pattern):
-        if pattern != path:
-            return False
-
-    elif pattern == "**":
-        if len(patterns) == 1:
-            return True  # if ** is the last one it matches anything to the right.
-
-        for i in range(len(paths)):
-            # Recursively check the remaining patterns as the
-            # current pattern could match any number of paths.
-            if _check_matches(patterns[1:], paths[i:]):
-                return True
-
-    elif not fnmatch.fnmatch(path, pattern):
-        # Current part doesn't match.
-        return False
-
-    return _check_matches(patterns[1:], paths[1:])
-
-
-def glob_matches_path(path, pattern, sep=os.sep, altsep=os.altsep):
-    if altsep:
-        pattern = pattern.replace(altsep, sep)
-        path = path.replace(altsep, sep)
-
-    drive = ""
-    if len(path) > 1 and path[1] == ":":
-        drive, path = path[0], path[2:]
-
-    if drive and len(pattern) > 1:
-        if pattern[1] == ":":
-            if drive.lower() != pattern[0].lower():
-                return False
-            pattern = pattern[2:]
-
-    patterns = pattern.split(sep)
-    paths = path.split(sep)
-    if paths:
-        if paths[0] == "":
-            paths = paths[1:]
-    if patterns:
-        if patterns[0] == "":
-            patterns = patterns[1:]
-
-    return _check_matches(patterns, paths)
-
-
 class FilesFiltering(object):
     """
     Usage is something as:
 
     files_filtering = FilesFiltering(...)
 
     if files_filtering.accept(mod.__file__, mod.__name__):
@@ -111,15 +50,17 @@
         project_roots: Optional[Sequence[str]] = None,
         library_roots: Optional[Sequence[str]] = None,
         filters: Sequence[Filter] = (),
     ):
         self._filters = filters
         self._project_roots: List[str] = []
         self._library_roots: List[str] = []
-        self._cache: Dict[Any, bool] = {}
+        self._cache_modname_to_kind: Dict[str, Optional[FilterKind]] = {}
+        self._cache_filename_to_kind: Dict[str, FilterKind] = {}
+        self._cache_in_project_roots: Dict[str, bool] = {}
 
         if project_roots is not None:
             self._set_project_roots(project_roots)
 
         if library_roots is None:
             library_roots = self._get_default_library_roots()
         self._set_library_roots(library_roots)
@@ -194,22 +135,29 @@
             path = self._absolute_normalized_path(root)
             if IS_WINDOWS:
                 new_roots.append(path + "\\")
             else:
                 new_roots.append(path + "/")
         return new_roots
 
-    def _absolute_normalized_path(self, filename):
+    def _absolute_normalized_path(self, filename, cache={}):
         """
         Provides a version of the filename that's absolute and normalized.
         """
+        try:
+            return cache[filename]
+        except KeyError:
+            pass
+
         if filename.startswith("<"):
-            return normcase(filename)
+            cache[filename] = normcase(filename)
+            return cache[filename]
 
-        return normcase(os.path.abspath(filename))
+        cache[filename] = normcase(os.path.abspath(filename))
+        return cache[filename]
 
     def _set_project_roots(self, project_roots):
         self._project_roots = self._fix_roots(project_roots)
         log.debug("IDE_PROJECT_ROOTS %s\n" % project_roots)
 
     def _get_project_roots(self):
         return self._project_roots
@@ -217,19 +165,17 @@
     def _set_library_roots(self, roots):
         self._library_roots = self._fix_roots(roots)
         log.debug("LIBRARY_ROOTS %s\n" % roots)
 
     def _get_library_roots(self):
         return self._library_roots
 
-    def _in_project_roots(self, received_filename):
+    def _in_project_roots(self, received_filename: str) -> bool:
         """
-        Note: don't call directly. Use PyDb.in_project_scope (there's no caching here and it doesn't
-        handle all possibilities for knowing whether a project is actually in the scope, it
-        just handles the heuristics based on the absolute_normalized_filename without the actual frame).
+        Note: uncached. Use `in_project_roots`.
         """
         DEBUG = False
 
         if received_filename.startswith(LIBRARY_CODE_BASENAMES_STARTING_WITH):
             if DEBUG:
                 log.debug(
                     "Not in in_project_roots - library basenames - starts with %s (%s)",
@@ -304,57 +250,63 @@
                             "Final in project (found in both): %s (%s)",
                             absolute_normalized_filename,
                             in_project,
                         )
 
         return in_project
 
-    def _exclude_by_filter(self, absolute_filename: Optional[str], module_name: str):
+    def in_project_roots(self, filename: str) -> bool:
+        try:
+            return self._cache_in_project_roots[filename]
+        except KeyError:
+            pass
+
+        in_project_roots = self._in_project_roots(filename)
+        self._cache_in_project_roots[filename] = in_project_roots
+        return in_project_roots
+
+    def _compute_filter_kind(self, module_name: str) -> Optional[FilterKind]:
         """
         :return: True if it should be excluded, False if it should be included and None
             if no rule matched the given file.
         """
-        for exclude_filter in self._filters:  # : :type exclude_filter: Filter
-            if exclude_filter.is_path:
-                if not absolute_filename:
-                    continue
-                if glob_matches_path(absolute_filename, exclude_filter.name):
-                    return exclude_filter.exclude
-            else:
-                # Module filter.
-                if exclude_filter.name == module_name or module_name.startswith(
-                    exclude_filter.name + "."
-                ):
-                    return exclude_filter.exclude
+        for exclude_filter in self._filters:
+            if exclude_filter.name == module_name or module_name.startswith(
+                exclude_filter.name + "."
+            ):
+                return exclude_filter.kind
         return None
 
-    def accept_module_name(self, module_name: str) -> bool:
+    def get_modname_filter_kind(self, module_name: str) -> Optional[FilterKind]:
         cache_key = module_name
         try:
-            return self._cache[cache_key]
+            return self._cache_modname_to_kind[cache_key]
         except KeyError:
             pass
 
-        exclude = self._exclude_by_filter(None, module_name)
-        if exclude is None:
-            exclude = False
-
-        accept = not exclude
-        self._cache[cache_key] = accept
-        return accept
+        filter_kind = self._compute_filter_kind(module_name)
+        self._cache_modname_to_kind[cache_key] = filter_kind
+        return filter_kind
+
+    def get_modname_or_file_filter_kind(
+        self, filename: str, module_name: str
+    ) -> FilterKind:
+        filter_kind = self.get_modname_filter_kind(module_name)
+        if filter_kind is not None:
+            return filter_kind
 
-    def accept(self, filename: str, module_name: str) -> bool:
         absolute_filename = self._absolute_normalized_path(filename)
 
-        cache_key = (absolute_filename, module_name)
+        cache_key = absolute_filename
         try:
-            return self._cache[cache_key]
+            return self._cache_filename_to_kind[cache_key]
         except KeyError:
             pass
 
-        exclude = self._exclude_by_filter(absolute_filename, module_name)
-        if exclude is None:
-            exclude = not self._in_project_roots(absolute_filename)
-
-        accept = not exclude
-        self._cache[cache_key] = accept
-        return accept
+        exclude = not self.in_project_roots(absolute_filename)
+        if exclude:
+            filter_kind = FilterKind.exclude
+        else:
+            filter_kind = FilterKind.full_log
+
+        self._cache_filename_to_kind[cache_key] = filter_kind
+        return filter_kind
```

### Comparing `robocorp_logging-0.0.6/src/robo_log/_rewrite_importhook.py` & `robocorp_logging-0.0.7/src/robo_log/_rewrite_importhook.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,25 +35,26 @@
 from typing import Callable
 from typing import Dict
 from typing import IO
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
-from ._config import BaseConfig
+from ._config import BaseConfig, FilterKind
 from ._rewrite_ast_add_callbacks import rewrite_ast_add_callbacks
 
 
 # caches rewritten pycs in pycache dirs
 # 0.0.1: Initial version
 # 0.0.2: Bugfix: docstrings must be kept as the first statement
 # 0.0.3: Support for exception handlers
 # 0.0.4: Add __name__
 # 0.0.5: Renames of internal modules.
-version = "0.0.5"
+# 0.0.6: Option to log just 1 level deep into library modules.
+version = "0.0.6"
 PYTEST_TAG = f"{sys.implementation.cache_tag}-robo_log-{version}"
 PYC_EXT = ".py" + (__debug__ and "c" or "o")
 PYC_TAIL = "." + PYTEST_TAG + PYC_EXT
 
 FORCE_CODE_GENERATION = False
 DEBUG = False
 
@@ -86,16 +87,23 @@
         self,
         name: str,
         path: Optional[Sequence[Union[str, bytes]]] = None,
         target: Optional[types.ModuleType] = None,
     ) -> Optional[importlib.machinery.ModuleSpec]:
         if self._writing_pyc:
             return None
-        if self._early_rewrite_bailout(name):
-            return None
+
+        filter_kind: Optional[FilterKind] = self.config.get_filter_kind_by_module_name(
+            name
+        )
+        if filter_kind is not None:
+            # Try to bail out as early as possible as the slow part is the "_find_spec".
+            if filter_kind == FilterKind.exclude:
+                return None
+
         trace("find_module called for: %s" % name)
 
         # Type ignored because mypy is confused about the `self` binding here.
         spec = self._find_spec(name, path)  # type: ignore
         if (
             # the import machinery could not find a file to import
             spec is None
@@ -107,16 +115,18 @@
             # if the file doesn't exist, we can't rewrite it
             or not os.path.exists(spec.origin)
         ):
             return None
         else:
             fn = spec.origin
 
-        if not self._should_rewrite(name, fn):
-            return None
+        if filter_kind is None:
+            filter_kind = self.config.get_filter_kind_by_module_name_and_path(name, fn)
+            if filter_kind == FilterKind.exclude:
+                return None
 
         return importlib.util.spec_from_file_location(
             name,
             fn,
             loader=self,
             submodule_search_locations=spec.submodule_search_locations,
         )
@@ -145,48 +155,40 @@
         cache_dir = get_cache_dir(fn)
         if write:
             ok = try_makedirs(cache_dir)
             if not ok:
                 write = False
                 trace(f"read only directory: {cache_dir}")
 
-        cache_name = fn.name[:-3] + PYC_TAIL
+        filter_kind: FilterKind = self.config.get_filter_kind_by_module_name_and_path(
+            module.__name__, module.__spec__.origin
+        )
+
+        cache_name = fn.name[:-3] + filter_kind.value + PYC_TAIL
+
         pyc = cache_dir / cache_name
         # Notice that even if we're in a read-only directory, I'm going
         # to check for a cached pyc. This may not be optimal...
         if FORCE_CODE_GENERATION:
             co = None
         else:
             co = _read_pyc(fn, pyc, trace)
         if co is None:
             trace(f"rewriting {fn!r}")
-            source_stat, co = _rewrite(fn, self.config)
+            source_stat, co, _tree = _rewrite(fn, self.config, filter_kind)
             if write:
                 self._writing_pyc = True
                 try:
                     _write_pyc(co, source_stat, pyc)
                 finally:
                     self._writing_pyc = False
         else:
             trace(f"found cached rewritten pyc for {fn}")
         exec(co, module.__dict__)
 
-    def _early_rewrite_bailout(self, module_name: str) -> bool:
-        """A fast way to get out of rewriting modules.
-
-        Profiling has shown that the call to PathFinder.find_spec (inside of
-        the find_spec from this class) is a major slowdown, so, this method
-        tries to filter what we're sure won't be rewritten before getting to
-        it.
-        """
-        return not self.config.can_rewrite_module_name(module_name)
-
-    def _should_rewrite(self, module_name: str, filename: str) -> bool:
-        return self.config.can_rewrite_module(module_name, filename)
-
     def get_data(self, pathname: Union[str, bytes]) -> bytes:
         """Optional PEP302 get_data API."""
         with open(pathname, "rb") as f:
             return f.read()
 
     if sys.version_info >= (3, 10):
         if sys.version_info >= (3, 12):
@@ -243,23 +245,25 @@
         # we ignore any failure to write the cache file
         # there are many reasons, permission-denied, pycache dir being a
         # file etc.
         return False
     return True
 
 
-def _rewrite(fn: Path, config: BaseConfig) -> Tuple[os.stat_result, types.CodeType]:
+def _rewrite(
+    fn: Path, config: BaseConfig, filter_kind: FilterKind
+) -> Tuple[os.stat_result, types.CodeType, ast.AST]:
     """Read and rewrite *fn* and return the code object."""
     stat = os.stat(fn)
     source = fn.read_bytes()
     strfn = str(fn)
     tree = ast.parse(source, filename=strfn)
-    rewrite_ast_add_callbacks(tree, source, strfn, config)
+    rewrite_ast_add_callbacks(tree, filter_kind, source, strfn, config)
     co = compile(tree, strfn, "exec", dont_inherit=True)
-    return stat, co
+    return stat, co, tree
 
 
 def _read_pyc(
     source: Path, pyc: Path, trace: Callable[[str], None] = lambda x: None
 ) -> Optional[types.CodeType]:
     """Possibly read a pytest pyc containing rewritten code.
```

### Comparing `robocorp_logging-0.0.6/src/robo_log/_robo_logger.py` & `robocorp_logging-0.0.7/src/robo_log/_robo_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from io import StringIO
 import functools
 from pathlib import Path
 from typing import Optional, Union, Sequence, Tuple
 import datetime
-from robo_log.protocols import OptExcInfo, LogHTMLStyle
+from robo_log.protocols import OptExcInfo, LogHTMLStyle, Status
+import sys
 
 
 def _log_error(func):
     @functools.wraps(func)
     def new_func(self, *args, **kwargs):
         import traceback
 
         try:
             return func(self, *args, **kwargs)
         except Exception as e:
             s = StringIO()
             traceback.print_exc(file=s)
             traceback.print_exc()
             self._robot_output_impl.log_message(
-                "ERROR",
+                Status.ERROR,
                 f"_RoboLogger internal error: {e}\n{s.getvalue()}",
-                self._robot_output_impl.get_time_delta(),
                 False,
+                __file__,
+                sys._getframe().f_lineno,
+                self._robot_output_impl.get_time_delta(),
             )
 
     return new_func
 
 
 class _RoboLogger:
     def __init__(
@@ -93,31 +96,35 @@
         return self._robot_output_impl.get_time_delta()
 
     def start_logging_methods(self):
         if self._skip_log_methods <= 0:
             self._robot_output_impl.log_message(
                 "ERROR",
                 f"_RoboLogger error: start_logging_methods() called before stop_logging_methods() (call is ignored as logging is already on).",
-                self._robot_output_impl.get_time_delta(),
                 False,
+                __file__,
+                sys._getframe().f_lineno,
+                self._robot_output_impl.get_time_delta(),
             )
             return
 
         self._skip_log_methods -= 1
 
     def stop_logging_methods(self):
         self._skip_log_methods += 1
 
     def start_logging_variables(self):
         if self._skip_log_arguments <= 0:
             self._robot_output_impl.log_message(
                 "ERROR",
                 f"_RoboLogger error: start_logging_variables() called before stop_logging_variables() (call is ignored as logging is already on).",
-                self._robot_output_impl.get_time_delta(),
                 False,
+                __file__,
+                sys._getframe().f_lineno,
+                self._robot_output_impl.get_time_delta(),
             )
             return
 
         self._skip_log_arguments -= 1
 
     def stop_logging_variables(self):
         self._skip_log_arguments += 1
```

### Comparing `robocorp_logging-0.0.6/src/robo_log/_robo_output_impl.py` & `robocorp_logging-0.0.7/src/robo_log/_robo_output_impl.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.6/src/robo_log/index.py` & `robocorp_logging-0.0.7/src/robo_log/index.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.6/src/robo_log/index_v2.py` & `robocorp_logging-0.0.7/src/robo_log/index_v2.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.6/PKG-INFO` & `robocorp_logging-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: robocorp-logging
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatic trace logging for Python
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11"
 Description-Content-Type: text/markdown
 
 # Logging for python based Robocorp projects
 
 Logging focused on RPA projects for Robocorp robots.
 
 > Note: The current version is still pre-alpha and the [format specified](/docs/format.md) may still change.
```

