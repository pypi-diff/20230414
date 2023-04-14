# Comparing `tmp/ipyautoui-0.4.9.tar.gz` & `tmp/ipyautoui-0.5.0.tar.gz`

## Comparing `ipyautoui-0.4.9.tar` & `ipyautoui-0.5.0.tar`

### file list

```diff
@@ -1,59 +1,57 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    32390 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14140 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/_dev_sys_path_append.py
--rw-r--r--   0        0        0    40876 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    24911 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30629 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0    12971 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/_dev_sys_path_append.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/LICENSE
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/README.md
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    31400 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    40881 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    25164 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/README.md
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 ipyautoui-0.5.0/PKG-INFO
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/__init__.py` & `ipyautoui-0.5.0/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/_utils.py` & `ipyautoui-0.5.0/src/ipyautoui/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,31 +12,49 @@
 from pydantic import BaseModel, validator, Field
 import typing as ty
 import importlib.util
 import inspect
 import immutables
 import getpass
 
+
 frozenmap = immutables.Map
+try:
+    import maplocal
 
+    if maplocal.maplocal_openlocal_exists():
+        from maplocal import openlocal as open_path
+        from maplocal import maplocal as make_new_path
+    else:
 
-def make_new_path(path, *args, **kwargs):
-    return path
+        def make_new_path(path, *args, **kwargs):
+            return path
 
+        def open_path(path):
+            import subprocess
+            import sys
+
+            if sys.platform == "linux":
+                subprocess.call(["xdg-open", path])
+            else:
+                subprocess.call(["explorer.exe", path])
 
-try:
-    # TODO: remove these.
-    from mf_file_utilities import go as open_file
-    from mf_file_utilities.applauncher_wrapper import make_new_path
 except:
 
-    def open_file(path):
-        import subprocess
+    def make_new_path(path, *args, **kwargs):
+        return path
 
-        subprocess.call(["open", path])
+        def open_path(path):
+            import subprocess
+            import sys
+
+            if sys.platform == "linux":
+                subprocess.call(["xdg-open", path])
+            else:
+                subprocess.call(["explorer.exe", path])
 
 
 def getuser():
     try:
         return os.environ["JUPYTERHUB_USER"]
     except:
         return getpass.getuser()
@@ -215,17 +233,17 @@
     read yaml file.
 
     Ref:
         https://stackoverflow.com/questions/1773805/how-can-i-parse-a-yaml-file-in-python"""
     with open(fpth, encoding=encoding) as stream:
         try:
             data = yaml.safe_load(stream)
+            return data
         except yaml.YAMLError as exc:
             print(exc)
-    return data
 
 
 def file(self: Type[BaseModel], path: pathlib.Path, **json_kwargs):
     """
     this is a method that is added to the pydantic BaseModel within AutoUi using
     "setattr".
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.5.0/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/_version.py` & `ipyautoui-0.5.0/src/ipyautoui/_version.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/autodisplay.py` & `ipyautoui-0.5.0/src/ipyautoui/autodisplay.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 # %run _dev_sys_path_append.py
 # %run __init__.py
 # %load_ext lab_black
 
 # +
 import pathlib
 import functools
-from wcmatch.pathlib import Path as wcPath
 from IPython.display import (
     display,
     clear_output,
     Markdown,
 )
 import time
 import typing as ty
@@ -55,15 +54,15 @@
 
 #  local imports
 from ipyautoui.autodisplay_renderers import (
     DEFAULT_FILE_RENDERERS,
     handle_compound_ext,
 )
 from ipyautoui._utils import (
-    open_file,
+    open_path,
     make_new_path,
     frozenmap,
     get_ext,
     st_mtime_string,
 )
 from ipyautoui.constants import (
     #  BUTTON_WIDTH_MIN,
@@ -140,26 +139,25 @@
     if path.is_file() or path.is_dir():
         return True
     else:
         return False
 
 
 class DisplayFromPath(DisplayObjectActions):
-    newroot: pathlib.PureWindowsPath = pathlib.PureWindowsPath("J:/")
     path_new: pathlib.Path = None
     open_file: ty.Callable = None
     open_folder: ty.Callable = None
 
     @validator("path", always=True)
     def _path(cls, v, values):
         return pathlib.Path(v)
 
     @validator("path_new", always=True)
     def _path_new(cls, v, values):
-        return make_new_path(values["path"], newroot=values["newroot"])
+        return make_new_path(values["path"].absolute())
 
     @validator("name", always=True)
     def _name(cls, v, values):
         if values["path"] is not None:
             v = values["path"].name
         return v
 
@@ -185,26 +183,26 @@
         else:
             return None
 
     @validator("open_file", always=True)
     def _open_file(cls, v, values):
         p = values["path"]
         if p is not None:
-            fn = functools.partial(open_file, p, newroot=values["newroot"])
+            fn = functools.partial(open_path, p)
             return fn
         else:
             return lambda: "Error: path given is None"
 
     @validator("open_folder", always=True)
     def _open_folder(cls, v, values):
         p = values["path"]
         if not p.is_dir():
             p = p.parent
         if p is not None:
-            fn = functools.partial(open_file, p, newroot=values["newroot"])
+            fn = functools.partial(open_path, p)
             return fn
         else:
             return lambda: "Error: path given is None"
 
     class Config:
         arbitrary_types_allowed = True
 
@@ -357,25 +355,22 @@
     def _update_bx_bar(self, order):
         self.bx_bar.children = [getattr(self, l) for l in order]
 
     @classmethod
     def from_path(
         cls,
         path,
-        newroot=pathlib.PureWindowsPath("J:/"),
         renderers=None,
         extend_default_renderers=True,
         auto_open=False,
     ):
         renderers = get_renderers(
             renderers=renderers, extend_default_renderers=extend_default_renderers
         )
-        display_actions = DisplayFromPath(
-            path=path, newroot=newroot, renderers=renderers
-        )
+        display_actions = DisplayFromPath(path=path, renderers=renderers)
         return cls(display_actions=display_actions, auto_open=auto_open)
 
     @classmethod
     def from_request(
         cls,
         path,
         ext,
@@ -401,15 +396,15 @@
         renderers = get_renderers(
             renderers=renderers, extend_default_renderers=extend_default_renderers
         )
         display_actions = DisplayFromCallable(path=path, ext=ext, renderers=renderers)
         return cls(display_actions=display_actions, auto_open=auto_open)
 
     def tooltip_openpath(self, path):
-        return str(make_new_path(path, newroot=self.display_actions.newroot))
+        return str(make_new_path(path))
 
     def _init_form(self):
         self.exists = w.Valid(
             value=False,
             disabled=True,
             readout="-",
             tooltip="indicates if file exists",
@@ -498,46 +493,46 @@
 
 class DisplayPath(DisplayObject):
     _value = tr.Unicode(default_value="")
 
     def __init__(
         self,
         value,
-        newroot=pathlib.PureWindowsPath("J:/"),
         renderers=None,
         extend_default_renderers=True,
         **kwargs,
     ):
-        self.newroot = newroot
         self.renderers = get_renderers(
             renderers=renderers, extend_default_renderers=extend_default_renderers
         )
-        display_actions = DisplayFromPath(
-            path=value, newroot=self.newroot, renderers=self.renderers
-        )
+        display_actions = DisplayFromPath(path=value, renderers=self.renderers)
         super().__init__(display_actions=display_actions, **kwargs)
 
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, value):
         self._value = ""
-        self.display_actions = DisplayFromPath(
-            path=value, newroot=self.newroot, renderers=self.renderers
-        )
+        self.display_actions = DisplayFromPath(path=value, renderers=self.renderers)
 
 
 # -
 if __name__ == "__main__":
     d = DisplayFromPath(path="__init__.py")
     do = DisplayObject(d)
     display(do)
 
+# +
+# from maplocal import maplocal
+
+# maplocal(pathlib.Path("__init__.py"))
+# -
+
 if __name__ == "__main__":
     path = "https://catfact.ninja/fact"
     ext = ".json"
     display(DisplayFromRequest(path=path, ext=ext).renderer())
 
 
 if __name__ == "__main__":
@@ -615,19 +610,18 @@
 
     user_file_renderers = AutoUi.create_autodisplay_map(
         ext=".aui.json", schema=TestAutoLogic
     )
     path1 = tests_constants.PATH_TEST_AUI
 
     d = DisplayObject.from_path(path1, renderers=user_file_renderers)
+    d.order = ORDER_DEFAULT
     display(d)
 
 # +
-from wcmatch import fnmatch
-
 
 class AutoDisplay(tr.HasTraits):
     """
     displays the contents of a file in the notebook.
     comes with the following default renderers:
     DEFAULT_FILE_RENDERERS = {
         '.csv': csv_prev,
@@ -649,22 +643,14 @@
         '.pdf': pdf_prev,
     }
     user_file_renderers can be passed to class provided they have the correct
     dict format: user_file_renderers = {'.ext': myrenderer}
     notice that the class allows for "compound" filetypes, especially useful for .json files
     if you want to display the data in a specific way.
     """
-
-    #     _paths = tr.List()
-
-    #     @validate("_paths")
-    #     def _valid_value(self, proposal):
-    #         """makes path a wcmatch.Path (for enhanced pattern matching) and filters out directories"""
-    #         return [wcPath(p) for p in proposal["value"] if not pathlib.Path(p).is_dir()]
-
     def __init__(
         self,
         display_objects_actions: ty.List[DisplayObjectActions],
         patterns: ty.Union[
             str, ty.List, None
         ] = None,  # TODO: add pattern matching. currently only works with paths
         title: ty.Union[str, None] = None,
@@ -688,30 +674,28 @@
         self.display_showhide = display_showhide
         self.patterns = patterns
 
     @classmethod
     def from_paths(
         cls,
         paths: ty.List[pathlib.Path],
-        newroot=pathlib.PureWindowsPath("J:/"),  # TODO: maproots
         renderers=None,
         patterns: ty.Union[str, ty.List] = None,
         title: ty.Union[str, None] = None,
         display_showhide: bool = True,
     ):
         if renderers is not None:
             renderers = merge_default_renderers(renderers)
         else:
             renderers = DEFAULT_FILE_RENDERERS
         if not isinstance(paths, list):
             paths = [pathlib.Path(paths)]
 
         display_objects_actions = cls.actions_from_paths(
             paths=paths,
-            newroot=newroot,
             renderers=renderers,
         )
         return cls(
             display_objects_actions,
             patterns=patterns,
             title=title,
             display_showhide=display_showhide,
@@ -819,21 +803,17 @@
                 raise TypeError(f"expected pathlib.Path or dict, got {type(path)}")
 
         return [choose(path=path, renderers=renderers) for path in paths]
 
     @staticmethod
     def actions_from_paths(
         paths: ty.List[pathlib.Path],
-        newroot=pathlib.PureWindowsPath("J:/"),  # maproots
         renderers=None,
     ):
-        return [
-            DisplayFromPath(path=path, newroot=newroot, renderers=renderers)
-            for path in paths
-        ]
+        return [DisplayFromPath(path=path, renderers=renderers) for path in paths]
 
     @staticmethod
     def actions_from_requests(map_requests: ty.Dict[str, HttpUrl], renderers=None):
         return [
             DisplayFromRequest(path=v, ext=k, renderers=renderers)
             for k, v in map_requests.items()
         ]
@@ -846,25 +826,22 @@
             DisplayFromCallable(path=v, ext=k, renderers=renderers)
             for k, v in map_callables.items()
         ]
 
     def add_from_paths(
         self,
         paths,
-        newroot=pathlib.PureWindowsPath("J:/"),
         renderers=None,
     ):
         if renderers is not None:
             renderers = merge_default_renderers(renderers)
         else:
             renderers = DEFAULT_FILE_RENDERERS
         paths = [p for p in paths if p not in self.paths]
-        _new_actions = self.actions_from_paths(
-            paths=paths, newroot=newroot, renderers=renderers
-        )
+        _new_actions = self.actions_from_paths(paths=paths, renderers=renderers)
         actions = self.display_objects_actions + _new_actions
         self.display_objects_actions = actions
 
     @property
     def title(self):
         return self._title
 
@@ -997,20 +974,21 @@
     from ipyautoui.test_schema import TestAutoLogic
     from ipyautoui.autoui import AutoUi
     from ipyautoui.constants import load_test_constants
 
     tests_constants = load_test_constants()
     DIR_FILETYPES = load_test_constants().DIR_FILETYPES
     paths = list(pathlib.Path(DIR_FILETYPES).glob("*"))
-    ad = AutoDisplay.from_paths(
-        paths, newroot=pathlib.PureWindowsPath("C:/"), patterns="*.csv"
-    )
+    ad = AutoDisplay.from_paths(paths, patterns="*.csv")
     display(ad)
 # -
 if __name__ == "__main__":
+    ad.order = ORDER_DEFAULT
+
+if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic
 
     user_file_renderers = AutoUi.create_autodisplay_map(
         ext=".aui.json", schema=TestAutoLogic
     )
 
     test_ui = AutoDisplay.from_paths(
@@ -1073,9 +1051,7 @@
     path = "https://official-joke-api.appspot.com/random_joke"
     ext = ".json"
     d2 = DisplayFromRequest(path=path, ext=ext)
 
     test_display = AutoDisplay([d1, d2])
     display(Markdown("### From requests: "))
     display(test_display)
-
-
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.5.0/src/ipyautoui/autodisplay_renderers.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 """
 displayfile is used to display certain types of files.
 The module lets us preview a data retrieved from: file, request or callable (< TODO)
 """
 # %run _dev_sys_path_append.py
 # %run __init__.py
-#
 # %load_ext lab_black
 # +
 import os
 import pathlib
 import requests
 import pandas as pd
 from IPython.display import display, Markdown, IFrame, clear_output, HTML, SVG
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.5.0/src/ipyautoui/autoipywidget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/automapschema.py` & `ipyautoui-0.5.0/src/ipyautoui/automapschema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/autoui.py` & `ipyautoui-0.5.0/src/ipyautoui/autoui.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/autovjsf.py` & `ipyautoui-0.5.0/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/autowidgets.py` & `ipyautoui-0.5.0/src/ipyautoui/autowidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/basemodel.py` & `ipyautoui-0.5.0/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/constants.py` & `ipyautoui-0.5.0/src/ipyautoui/constants.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo.py` & `ipyautoui-0.5.0/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/env.py` & `ipyautoui-0.5.0/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.5.0/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/test_schema.py` & `ipyautoui-0.5.0/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/vjsf.vue` & `ipyautoui-0.5.0/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/autogrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 #   jupytext:
 #     cell_metadata_filter: -all
 #     formats: py:light
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.14.5
+#       jupytext_version: 1.14.0
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
 """defines a schema for a datagrid. this is used to build the datagrid and
 contains methods for validation, coercion, and default values. 
 
 defines AutoGrid, a datagrid generated from a jsonschema."""
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %run ../__init__.py
 # %load_ext lab_black
 
 import typing as ty
 import traitlets as tr
 import logging
@@ -1213,7 +1213,9 @@
 
 if __name__ == "__main__":
     grid.transposed = False
 
 if __name__ == "__main__":
     grid.set_item_value(0, {"string": "check", "integer": 2, "floater": 3.0})
 # -
+
+
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/buttonbars.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %load_ext lab_black
 
 import ipywidgets as w
 import traitlets as tr
 import typing as ty
 from ipyautoui.constants import (
@@ -27,14 +27,15 @@
 )
 
 from IPython.display import display
 from datetime import datetime
 from markdown import markdown
 import logging
 from enum import Enum
+
 logger = logging.getLogger(__name__)
 
 # +
 def merge_callables(callables: ty.Union[ty.Callable, ty.List[ty.Callable]]):
     if isinstance(callables, ty.Callable):
         return callables
     elif isinstance(callables, ty.List):
@@ -417,9 +418,7 @@
         fn_copy=copy,
         fn_delete=delete,
         fn_backward=backward,
         fn_reload=lambda: print("fn_reload"),
     )
 
     display(buttonbar)
-
-
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/decision_branch.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # ---
 
 # +
 """
 a UI element that loads a folder for data caching, whilst storing a record of folders in use
 """
 
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 #
 # %load_ext lab_black
 from pydantic import BaseModel
 import ipywidgets as w
 import typing as ty
 import traitlets as tr
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/editgrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 #     formats: py:light
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
 #       jupytext_version: 1.14.5
 #   kernelspec:
-#     display_name: Python 3.9 (XPython)
+#     display_name: Python 3 (ipykernel)
 #     language: python
-#     name: xpython
+#     name: python3
 # ---
 
 # +
 """General widget for editing data"""
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %run ../__init__.py
 # %load_ext lab_black
 # TODO: move editgrid.py to root ?
 
 import traitlets as tr
 import typing as ty
@@ -441,23 +441,28 @@
             raise ValueError(
                 "you must select an index (row if transposed==True, col if"
                 " transposed==True)"
             )
         self._check_one_row_selected()
 
     def _save_edit_to_grid(self):
+        selections = self.grid.selections  # Store current selection
+        self.grid.selections = []
+        # ^ HOTFIX: Have to set empty to reselect later on
+
         if self.datahandler is not None:
             self._reload_all_data()
         else:
-            changes = self.grid.set_item_value(
-                self.grid.selected_index, self.ui_edit.value
-            )
+            self.grid.set_item_value(self.grid.selected_index, self.ui_edit.value)
 
         if self.close_crud_dialogue_on_action:
             self.buttonbar_grid.edit.value = False
+        else:
+            # Reselect previous selection after reload.
+            self.grid.selections = selections
 
     def _set_ui_edit_to_selected_row(self):
         self.ui_edit.value = self.grid.selected
         self.ui_edit.savebuttonbar.unsaved_changes = False
 
     def _patch(self):
         if self.datahandler is not None:
@@ -656,18 +661,20 @@
 
 if __name__ == "__main__":
     editgrid.grid.order = ("floater", "string")
     # ^ NOTE: this will result in a value change in the grid
 
 
 if __name__ == "__main__":
+    import random
+
     datahandler = DataHandler(
-        fn_get_all_data=lambda: AUTO_GRID_DEFAULT_VALUE * random.randint(1, 10),
+        fn_get_all_data=lambda: AUTO_GRID_DEFAULT_VALUE * random.randint(1, 5),
         fn_post=lambda v: print(v),
-        fn_patch=lambda v: print(v),
+        fn_patch=lambda v: v,
         fn_delete=lambda v: print(v),
         fn_copy=lambda v: print(v),
     )
     title = "The Wonderful Edit Grid Application"
     description = markdown("Useful for all editing purposes whatever they may be 👍")
     editgrid = EditGrid(
         schema=TestDataFrame,
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/filechooser.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 """wrapper for ipyfilechooster.FileChooser"""
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %load_ext lab_black
 
 import pathlib
 import traitlets as tr
 import typing as ty
 from ipyfilechooser import FileChooser
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/filesindir.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #       jupytext_version: 1.11.5
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 #
 # %load_ext lab_black
 
 # +
 import pathlib
 from wcmatch.pathlib import Path as wcPath
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/fileupload.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 """file upload wrapper"""
 # %load_ext lab_black
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %run ../__init__.py
 
 # +
 import ipywidgets as w
 from markdown import markdown
 from IPython.display import display, clear_output
@@ -50,44 +50,48 @@
     name: str
     fdir: pathlib.Path = pathlib.Path(".")
     path: pathlib.Path = None
 
     @validator("path", always=True, pre=True)
     def _path(cls, v, values):
         return values["fdir"] / values["name"]
-    
+
+
 def read_file_upload_item(di: dict, fdir=pathlib.Path("."), added_by=None):
     if added_by is None:
         added_by = getuser()
     if IS_IPYWIDGETS8:
         _ = di
     else:
         _ = di["metadata"]
     _["fdir"] = fdir
     _["added_by"] = added_by
     return File(**_)
 
+
 def add_file(upld_item, fdir=pathlib.Path(".")):
     f = read_file_upload_item(upld_item, fdir=fdir)
     f.path.write_bytes(upld_item["content"])
     return f
 
 
 def add_files_ipywidgets8(upld_value, fdir=pathlib.Path(".")):
     di = {}
     for l in upld_value:
         f = add_file(l, fdir=fdir)
         di[l["name"]] = f
     return [v.path for v in di.values()]
 
+
 def add_files(upld_value, fdir=pathlib.Path(".")):
     if not pathlib.Path(fdir).exists():
         pathlib.Path(fdir).mkdir(exist_ok=True)
     return add_files_ipywidgets8(upld_value, fdir=fdir)
 
+
 class FilesUploadToDir(Array):
     def __init__(
         self,
         value=None,
         fdir=pathlib.Path("."),
         kwargs_display_path: ty.Optional[dict] = None,
         **kwargs,
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/iterable.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
         arr = Array(**di_arr)
         display(arr)
 
 """
 # TODO: move iterable.py to root
 # TODO: review: https://github.com/widgetti/reacton - it could simplify the code required below.
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %load_ext lab_black
 import ipywidgets as w
 import traitlets as tr
 from traitlets import validate
 import typing as ty
 from IPython.display import display
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/loadproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #     display_name: Python [conda env:ipyautoui]
 #     language: python
 #     name: ipyautoui
 # ---
 
 # %%
 """generic iterable object."""
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 #
 # %load_ext lab_black
 
 # %%
 import traitlets as tr
 import re
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/markdown_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 """simple markdown widget"""
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 #
 # %load_ext lab_black
 
 # +
 import ipywidgets as w
 import functools
@@ -229,9 +229,7 @@
 
     class Test(BaseModel):
         num: int
         label: str
         md: str = Field("adsf", format="markdown")
 
     display(AutoUi(Test))
-
-
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/outputlogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
 """simple set-up of outputting logging messages to widgets output."""
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 #
 # %run ../__init__.py
 # %load_ext lab_black
 
 import logging
 import ipywidgets as w
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/selectdir.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 #
 # %load_ext lab_black
 from IPython.display import display
 from ipyautoui.basemodel import BaseModel
 from ipyautoui.basemodel import file
 from ipyautoui._utils import file
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/showhide.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #       jupytext_version: 1.13.8
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 #
 # %run ../__init__.py
 # %load_ext lab_black
 
 # +
 import ipywidgets as w
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/title_description.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 """generic support for observed title and description"""
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %run ../__init__.py
 # %load_ext lab_black
 
 import traitlets as tr
 import ipywidgets as w
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/urlimagelink.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # +
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
-#
 # %load_ext lab_black
 
 from IPython.display import display, HTML, clear_output
 import ipywidgets as w
 import traitlets as t
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #     language: python
 #     name: python3
 # ---
 
 # %%
 """widget caller error"""
 # %load_ext lab_black
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %run ../__init__.py
 
 # %%
 import ipywidgets as w
 import traitlets as tr
 from IPython.display import clear_output
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.5.0/src/ipyautoui/custom/workingdir.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # ---
 
 # +
 """
 a UI element that loads a folder for data caching, whilst storing a record of folders in use
 """
 
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 #
 # %load_ext lab_black
 
 # +
 from pydantic import BaseModel, validator, Field
 from ipyautoui.constants import LOAD_BUTTON_KWARGS, BUTTON_WIDTH_MIN
@@ -133,14 +133,15 @@
     name: str = "working dirs"
     description: str = description
     dirs: ty.Dict[str, WorkingDir] = Field(default_factory=lambda: {})
 
 
 # + tags=[]
 
+
 def get_working_dirs(path=FPTH_WORKING_DIRS):
     """loads working dir from folder"""
     if path.exists():
         wdirs = WorkingDirs.parse_file(path)
     else:
         wdirs = WorkingDirs()
         wdirs.file(path)
```

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.5.0/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
 # %%
-# %run _dev_sys_path_append.py
+# %run ../_dev_sys_path_append.py
 # %run __init__.py
 # %run ../__init__.py
 # %load_ext lab_black
 
 from enum import Enum
 from pydantic import BaseModel, Field
 from ipyautoui import AutoUi
```

### Comparing `ipyautoui-0.4.9/.gitignore` & `ipyautoui-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/LICENSE` & `ipyautoui-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.9/README.md` & `ipyautoui-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,15 @@
 using VS Code then install the Jupytext extension. In the `.vscode/settings.json` file
 `"jupyter.notebookFileRoot": "${fileDirname}"` matching with the jupyterlab default. 
 ```
 
 ## Packaging (restricted to core-maintainers)
 
 ```sh
+mamba activate hatcher # or conda env with hatch installed
 hatch build  # builds to local folder
 hatch publish  # publishes to pypi
 ```
 
 ## Contributions
 
 AutoVjsf is a very thin wrapper where ipyvuetify and vuetify-jsonschema-form are doing all the work.
```

### Comparing `ipyautoui-0.4.9/pyproject.toml` & `ipyautoui-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "pandas",
     "pydantic",
     "pytest",
     "PyYAML",
     "stringcase",
     "traitlets",
     "wcmatch",
+    "maplocal==0.1.1",
 ]
 
 [project.urls]
 Homepage = "https://github.com/maxfordham/ipyautoui"
 
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `ipyautoui-0.4.9/PKG-INFO` & `ipyautoui-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.4.9
+Version: 0.5.0
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: immutables
 Requires-Dist: ipydatagrid>=1.1.14
 Requires-Dist: ipyfilechooser
 Requires-Dist: ipython
 Requires-Dist: ipyvuetify
 Requires-Dist: ipywidgets>8
+Requires-Dist: maplocal==0.1.1
 Requires-Dist: markdown
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: pydantic
 Requires-Dist: pytest
 Requires-Dist: pyyaml
@@ -178,14 +179,15 @@
 using VS Code then install the Jupytext extension. In the `.vscode/settings.json` file
 `"jupyter.notebookFileRoot": "${fileDirname}"` matching with the jupyterlab default. 
 ```
 
 ## Packaging (restricted to core-maintainers)
 
 ```sh
+mamba activate hatcher # or conda env with hatch installed
 hatch build  # builds to local folder
 hatch publish  # publishes to pypi
 ```
 
 ## Contributions
 
 AutoVjsf is a very thin wrapper where ipyvuetify and vuetify-jsonschema-form are doing all the work.
```

