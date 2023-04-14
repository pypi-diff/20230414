# Comparing `tmp/ipyautoui-0.4.8.tar.gz` & `tmp/ipyautoui-0.4.9.tar.gz`

## Comparing `ipyautoui-0.4.8.tar` & `ipyautoui-0.4.9.tar`

### file list

```diff
@@ -1,55 +1,59 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    12729 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    32390 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    26157 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0    21005 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0    13029 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14645 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/_dev_sys_path_append.py
--rw-r--r--   0        0        0    40878 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    25846 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30737 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0    13241 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/nested_items.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/LICENSE
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/README.md
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 ipyautoui-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    32390 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14140 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    40876 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    24911 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9392 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0    30629 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5478 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5838 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12971 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/_dev_sys_path_append.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/LICENSE
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/README.md
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 ipyautoui-0.4.9/PKG-INFO
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/__init__.py` & `ipyautoui-0.4.9/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/_utils.py` & `ipyautoui-0.4.9/src/ipyautoui/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import pathlib
 import json
 import yaml
 import importlib
 from typing import Type
 from markdown import markdown
 from math import log10, floor
@@ -259,51 +260,27 @@
 
     @validator("module_name", always=True)
     def _module_name(cls, v, values):
         return values["path"].stem
 
 
 def load_PyObj(obj: PyObj):
-    spec = importlib.util.spec_from_file_location(obj.module_name, obj.path)
+    submodule_search_locations = None
+    p = obj.path
+    if obj.path.is_dir():
+        p = p / "__main__.py"
+        submodule_search_locations = []
+    spec = importlib.util.spec_from_file_location(
+        obj.module_name, p, submodule_search_locations=submodule_search_locations
+    )
     foo = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(foo)
     return getattr(foo, obj.obj_name)
 
 
-def create_pydantic_json_file(pyobj: PyObj, path: pathlib.Path, **kwargs):
-    """
-    loads a pyobj (which must be a pydantic model) and then saves the default Json to file.
-    this requires defaults for all pydantic attributes.
-
-    Todo:
-        could extend the functionality to cover models that don't have defaults
-        using [pydantic-factories](https://github.com/Goldziher/pydantic-factories)
-
-    Args:
-        pyobj (PyObj): definition of where to get a pydantic model
-        path (pathlib.Path): where to save the pydantic json
-        **kwargs : passed to the pydantic model upon initiation
-
-    Returns:
-        path
-    """
-    obj = load_PyObj(pyobj)
-    assert (
-        str(type(obj)) == "<class 'pydantic.main.ModelMetaclass'>"
-    ), "the python object must be a pydantic model"
-    if not hasattr(obj, "file"):
-        setattr(obj, "file", file)
-    assert hasattr(
-        obj, "file"
-    ), "the pydantic BaseModel must be extended to have method 'file' for writing model to json"
-    myobj = obj(**kwargs)
-    myobj.file(path)
-    return path
-
-
 # TODO: use obj_to_importstr and obj_from_importstr rather than load_PyObj
 def obj_to_importstr(obj: ty.Callable):  # NOT IN USE
     """
     given a callable callable object this will return the
     import string to. From the string the object can be
     initiated again using importlib. This is useful for
     defining a function or class in a json serializable manner
@@ -438,7 +415,32 @@
 
 def check_installed(package_name):
     spec = importlib.util.find_spec(package_name)
     if spec is None:
         return False
     else:
         return True
+
+
+def html_link(url: str, description: str, color: str = "blue"):
+    """returns an html link string to open in new tab
+
+    Args:
+        url (url):
+        description (str): the text to display for the link
+        color (str, optional): color of description text. Defaults to "blue".
+
+    Returns:
+        str: html text
+    """
+    return f'<font color="{color}"><a href="{url}" target="blank" >{description}</a></font>'
+
+
+def get_user():
+    """get user. gets JUPYTERHUB_USER if present (i.e. if notebook served via a JupyterHub)"""
+    nm = "JUPYTERHUB_USER"
+    if nm in list(os.environ.keys()):
+        return os.environ[nm]
+    else:
+        from getpass import getuser
+
+        return getuser()
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.4.9/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/_version.py` & `ipyautoui-0.4.9/src/ipyautoui/_version.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/autodisplay.py` & `ipyautoui-0.4.9/src/ipyautoui/autodisplay.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.4.9/src/ipyautoui/autodisplay_renderers.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 import pandas as pd
 from IPython.display import display, Markdown, IFrame, clear_output, HTML, SVG
 import json
 import ipydatagrid as ipg
 import ipywidgets as w
 import traitlets as tr
 import typing as ty
-import traitlets_paths
 from io import StringIO, BytesIO
 from pydantic import HttpUrl, parse_obj_as
 
 
 #  local imports
 from ipyautoui.mydocstring_display import display_module_docstring
 from ipyautoui._utils import (
@@ -183,15 +182,15 @@
     byts = getbytes(path)
     df = pd.read_csv(StringIO(byts.decode()))
     df = del_matching(pd.read_csv(path), "Unnamed")
     return default_grid(df)
 
 
 class PreviewExcel(w.VBox):
-    path = traitlets_paths.Path()
+    path = tr.Instance(klass=pathlib.PurePath)
     xl = tr.Instance(klass="pandas.ExcelFile")
 
     def __init__(self, path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
         super().__init__()
 
         self.path = path
 
@@ -251,45 +250,57 @@
     """
     for l in li:
         l["grid"] = default_grid(l["df"])
         display(Markdown(mdheader(l)))
         display(l["grid"])
 
 
-def preview_json(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
-    js = json.loads(getbytes(path).decode())
+def preview_json_string(json_str):
     return Markdown(
         f"""
 ```json
-{json.dumps(js, indent=4)}
+{json.dumps(json_str, indent=4)}
 ```
 """
     )
 
 
-def preview_yaml(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
-    byts = getbytes(path)
+def preview_json(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
+    js = json.loads(getbytes(path).decode())
+    return preview_json_string(js)
+
+
+def preview_yaml_string(yaml_str):
     return Markdown(
         f"""
 ```yaml
-{byts.decode()}
+{yaml_str}
 ```
 """
     )
 
 
-def preview_plotly(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
+def preview_yaml(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
+    byts = getbytes(path)
+    return preview_yaml_string(byts.decode())
+
+
+def preview_plotly_json(plotly_str):
     package_name = "plotly"
     if check_installed(package_name):
-        byts = getbytes(path)
-        return pio.from_json(byts.decode())
+        return pio.from_json(plotly_str)
     else:
         return w.HTML(package_name + " is not installed")
 
 
+def preview_plotly(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
+    byts = getbytes(path)
+    return preview_plotly_json(byts.decode())
+
+
 def Vega(spec):
     """
     render Vega in jupyterlab
     https://github.com/jupyterlab/jupyterlab/blob/master/examples/vega/vega-extension.ipynb
     """
     bundle = {}
     bundle["application/vnd.vega.v5+json"] = spec
@@ -340,17 +351,25 @@
         elif isinstance(data["data"], dict):
             data["data"] = update_vega_data_url(data["data"], path)
         else:
             raise ValueError("vega data must be list or dict")
     return data
 
 
+def preview_vega_json(vega_json):
+    return Vega(vega_json)
+
+
 def preview_vega(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
     data = get_vega_data(path)
-    return Vega(data)
+    return preview_vega_json(data)
+
+
+def preview_vegalite_json(vegalite_json):
+    return VegaLite(vegalite_json)
 
 
 def preview_vegalite(path):
     data = get_vega_data(path)
     return VegaLite(data)
 
 
@@ -371,25 +390,31 @@
 
 def preview_audio(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable], *args, **kwargs):
     byts = getbytes(path)
     return w.Audio(value=byts, *args, **kwargs)
 
 
 ##############TODO: from here:###############################
-def preview_text(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
-    byts = getbytes(path)
+
+
+def preview_text_string(text_str):
     return Markdown(
         f"""
 ```
-{byts.decode()}
+{text_str}
 ```
 """
     )
 
 
+def preview_text(path: ty.Union[pathlib.Path, HttpUrl, ty.Callable]):
+    byts = getbytes(path)
+    return preview_text_string(byts.decode())
+
+
 def preview_dir(path: pathlib.Path):
     """preview folder"""
     # TODO: make recursive using AutoDisplay?
     li = path.glob("*")
     make_str = lambda p: f"📁 {p.stem}" if p.is_dir() else f"📄 {p.stem}"
     li = [make_str(l) for l in li]
     return HTML("<br>".join(li))
@@ -399,14 +424,15 @@
     """display path with ext == "" """
     if path.is_file():
         return preview_text(path)
     else:
         return preview_dir(path)
 
 
+# TODO: how to preview markdown not as a file, but as a string?
 def preview_markdown(path: pathlib.Path):
     import subprocess
 
     if not path.is_file():
         raise ValueError(
             f"path must be a valid pathlib.Path, not {path}. TODO: create render method."
         )
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.4.9/src/ipyautoui/autoipywidget.py`

 * *Files 14% similar despite different names*

```diff
@@ -216,72 +216,144 @@
 
 # +
 def make_bold(s: str) -> str:
     return f"<big><b>{s}</b></big>"
 
 
 class AutoObjectFormLayout(w.VBox):
+    """UI container for autoui form
 
+    Attributes:
+        title (str): form title
+        description (str): form description
+        show_description (bool, optional): show the description. Defaults to True.
+        show_title (bool, optional): show the title. Defaults to True.
+        show_savebuttonbar (bool, optional): show the savebuttonbar. Defaults to True.
+        show_raw (bool, optional): show the raw json. Defaults to False.
+        fn_onshowraw (callable): do not edit
+        fn_onhideraw (callable): do not edit
+        fns_onsave (callable): additional functions to be called on save
+        fns_onrevert (callable): additional functions to be called on revert
+    """
+
+    title = tr.Unicode(default_value="")
+    description = tr.Unicode(default_value="")
     show_description = tr.Bool(default_value=True)
     show_title = tr.Bool(default_value=True)
     show_savebuttonbar = tr.Bool(default_value=False)
+    show_raw = tr.Bool(default_value=False)
     fn_onshowraw = tr.Callable(default_value=lambda: "{'test':'json'}")
     fn_onhideraw = tr.Callable(default_value=lambda: None)
-    show_raw = tr.Bool(default_value=False)
+    fns_onsave = tr.List(trait=tr.Callable())
+    fns_onrevert = tr.List(trait=tr.Callable())
+
+    @tr.observe("title")
+    def _observe_title(self, change):
+        if not hasattr(self, "html_title"):
+            self.html_title = w.HTML()
+        self.html_title.value = f"<b>{self.title}</b>"
+
+    @tr.observe("description")
+    def _observe_description(self, change):
+        if not hasattr(self, "html_description"):
+            self.html_description = w.HTML()
+        self.html_description.value = self.description
 
     @tr.observe("show_raw")
     def _observe_show_raw(self, change):
         show_hide_widget(self.bn_showraw, self.show_raw)
 
     @tr.observe("show_description")
     def _observe_show_description(self, change):
-        show_hide_widget(self.description, self.show_description)
+        show_hide_widget(self.html_description, self.show_description)
 
     @tr.observe("show_title")
     def _observe_show_title(self, change):
-        show_hide_widget(self.title, self.show_title)
+        show_hide_widget(self.html_title, self.show_title)
 
     @tr.observe("show_savebuttonbar")
     def _observe_show_savebuttonbar(self, change):
         show_hide_widget(self.savebuttonbar, self.show_savebuttonbar)
 
-    def __init__(self, fns_onsave=None, fns_onrevert=None, **kwargs):
+    @tr.observe("fns_onsave")
+    def _observe_fns_onsave(self, change):
+        """NOTE: this observer will alway append actions.
+        to delete actions use
+            `self.savebuttonbar.fns_onsave = []`
+        then set with
+            `self.fns_onsave = [lambda: print('save-funcy')]`"""
+        value = change["new"]
+        if isinstance(value, list):
+            [self.savebuttonbar.fns_onsave_add_action(v) for v in value]
+        elif isinstance(value, ty.Callable):
+            self.savebuttonbar.fns_onsave_add_action(value)
+        else:
+            raise ValueError("fns_onsave must be a callable or list of callables")
+        return self.savebuttonbar.fns_onsave
+
+    @tr.observe("fns_onrevert")
+    def _observe_fns_onrevert(self, change):
+        """NOTE: this observer will alway append actions.
+        to delete actions use
+            `self.savebuttonbar.fns_onsave = []`
+        then set with
+            `self.fns_onrevert = [lambda: print('revert-funcy')]`"""
+        value = change["new"]
+        if isinstance(value, list):
+            [self.savebuttonbar.fns_onrevert_add_action(v) for v in value]
+        elif isinstance(value, ty.Callable):
+            self.savebuttonbar.fns_onrevert_add_action(value)
+        else:
+            raise ValueError("fns_onsave must be a callable or list of callables")
+        return self.savebuttonbar.fns_onrevert
+
+    @tr.default("fn_onshowraw")
+    def _default_fn_onshowraw(self):
+        return self.display_showraw
+
+    @tr.default("fn_onhideraw")
+    def _default_fn_onhideraw(self):
+        return self.display_ui
+
+    @tr.default("fns_onsave")
+    def _default_fns_onsave(self):
+        return self.savebuttonbar.fns_onsave
+
+    @tr.default("fns_onrevert")
+    def _default_fns_onrevert(self):
+        return self.savebuttonbar.fns_onsave
+
+    def __init__(self, **kwargs):
 
         self._init_form()
         self._init_bn_showraw_controls()
-        self.fn_onshowraw = self.display_showraw
-        self.fn_onhideraw = self.display_ui
-        if fns_onsave is not None:
-            self.fns_onsave = fns_onsave
-        if fns_onrevert is not None:
-            self.fns_onrevert = fns_onrevert
         super().__init__(
             layout=w.Layout(
                 width="100%",
                 display="flex",
                 flex="flex-grow",
             ),
             **kwargs,
         )
         self.children = [
             self.savebuttonbar,
             self.hbx_title,
-            self.description,
+            self.html_description,
             self.autowidget,
             self.vbx_showraw,
         ]
 
     def _init_form(self):
         self.autowidget = w.VBox()
         self.hbx_title = w.HBox()
         self.savebuttonbar = SaveButtonBar(layout={"display": "None"})  #
-        self.title = w.HTML()
+        self.html_title = w.HTML()
         self._init_bn_showraw()
-        self.hbx_title.children = [self.bn_showraw, self.title]
-        self.description = w.HTML()  #
+        self.hbx_title.children = [self.bn_showraw, self.html_title]
+        self.html_description = w.HTML()  #
 
     def _init_bn_showraw(self):
         self.bn_showraw = w.ToggleButton(
             icon="code",
             layout=w.Layout(width=BUTTON_WIDTH_MIN, display="None"),
             tooltip="show raw data",
             style={"font_weight": "bold", "button_color": None},
@@ -313,53 +385,27 @@
     def display_ui(self):
         self.autowidget.layout.display = ""
 
     def display_showraw(self):  # NOTE: this overwritten this in AutoObject
         self.autowidget.layout.display = "None"
         return '{"test": "json"}'
 
-    @property
-    def fns_onsave(self):
-        return self.savebuttonbar.fns_onsave
-
-    @fns_onsave.setter
-    def fns_onsave(self, value):
-        if isinstance(value, list):
-            [self.savebuttonbar.fns_onsave_add_action(v) for v in value]
-        elif isinstance(value, ty.Callable):
-            self.savebuttonbar.fns_onrevert_add_action(value)
-        else:
-            raise ValueError("fns_onsave must be a callable or list of callables")
-
-    @property
-    def fns_onrevert(self):
-        return self.savebuttonbar.fns_onrevert
-
-    @fns_onrevert.setter
-    def fns_onrevert(self, value):
-        if isinstance(value, list):
-            [self.savebuttonbar.fns_onrevert_add_action(v) for v in value]
-        elif isinstance(value, ty.Callable):
-            self.savebuttonbar.fns_onrevert_add_action(value)
-        else:
-            raise ValueError("fns_onrevert must be a callable or list of callables")
-
 
 if __name__ == "__main__":
     ui = AutoObjectFormLayout(description="description", show_savebuttonbar=True)
     display(ui)
 
 # +
 def demo_autoobject_form(title="test", description="a description of the title"):
     """for docs and testing only..."""
     from ipyautoui.custom.buttonbars import SaveButtonBar
 
     form = AutoObjectFormLayout()
-    form.title.value = make_bold(title)
-    form.description.value = description
+    form.title = make_bold(title)
+    form.description = description
     form.show_raw = True
     form.show_description = True
     form.show_title = True
     form.show_savebuttonbar = True
     form.savebuttonbar.layout = {"border": "solid red 2px"}
     form.savebuttonbar.children = [SaveButtonBar()]
     form.hbx_title.layout = {"border": "solid blue 2px"}
@@ -375,14 +421,17 @@
 
 
 if __name__ == "__main__":
     form = demo_autoobject_form()
     display(form)
 
 # +
+# form.title = "<b>asdfasdf</b>"
+
+# +
 # form.show_raw = True
 # -
 
 if __name__ == "__main__":
     form.show_savebuttonbar = False
     form.show_description = False
     form.show_title = False
@@ -401,81 +450,54 @@
 
 # +
 class AutoObject(AutoObjectFormLayout):  # w.VBox
     """creates an ipywidgets form from a json-schema or pydantic model.
     datatype must be "object"
 
     Attributes:
+
+        # AutoObjectFormLayout
+        # -------------------------
+        title (str): form title
+        description (str): form description
+        show_description (bool, optional): show the description. Defaults to True.
+        show_title (bool, optional): show the title. Defaults to True.
+        show_savebuttonbar (bool, optional): show the savebuttonbar. Defaults to True.
+        show_raw (bool, optional): show the raw json. Defaults to False.
+        fn_onshowraw (callable): do not edit
+        fn_onhideraw (callable): do not edit
+        fns_onsave (callable): additional functions to be called on save
+        fns_onrevert (callable): additional functions to be called on revert
+
+        # AutoObject
+        # -------------------------
         _value (dict): use `value` to set and get. the value of the form. this is a dict of the form {key: value}
         fdir (path, optional): fdir to work from. useful for widgets that link to files. Defaults to None.
         align_horizontal (bool, optional): aligns widgets horizontally. Defaults to True.
         nested_widgets (list, optional): allows user to indicate widgets that should be show / hide type. Defaults to [].
         auto_open (bool, optional): automatically opens the nested_widget. Defaults to True.
         order (list): allows user to re-specify the order for widget rows to appear by key name in self.di_widgets
         order_can_hide_rows (bool): allows user to hide rows by removing them from the order list.
         insert_rows (dict): e.g. {3:w.Button()}. allows user to insert a widget into the rows. its presence
             is ignored by the widget otherwise.
         disabled (bool, optional): disables all widgets. If widgets are disabled
             using schema kwargs this is remembered when re-enabled. Defaults to False.
 
-        # inherited from AutoObjectFormLayout
-
-        show_raw (bool, optional): show the raw json. Defaults to False.
-        show_description (bool, optional): show the description. Defaults to True.
-        show_title (bool, optional): show the title. Defaults to True.
-        show_savebuttonbar (bool, optional): show the savebuttonbar. Defaults to True.
-
     """
 
     _value = tr.Dict(allow_none=True)
     fdir = tr.Instance(klass=pathlib.PurePath, default_value=None, allow_none=True)
     align_horizontal = tr.Bool(default_value=True)
     auto_open = tr.Bool(default_value=True)
     nested_widgets = tr.List()
     order = tr.List(default_value=None, allow_none=True)
     order_can_hide_rows = tr.Bool(default_value=True)
     insert_rows = tr.Dict(default_value=None, allow_none=True)
     disabled = tr.Bool(default_value=False)
 
-    def __init__(
-        self,
-        schema,
-        by_alias=False,
-        value=None,
-        update_map_widgets=None,
-        fns_onsave=None,
-        fns_onrevert=None,
-        **kwargs,
-    ):
-        """creates a widget input form from schema. datatype must be "object"
-
-        Args:
-            schema (dict): json schema defining widget to generate
-            by_alias (bool, optional): use alias in schema. Defaults to False.
-            value (dict, optional): value of json. Defaults to None.
-            update_map_widgets (frozenmap, optional): frozen dict of widgets to map to schema items. Defaults to None.
-            fn_onsave (callable, optional): function to run on save. Defaults to None.
-            fn_onrevert (callable, optional): function to run on revert. Defaults to None.
-
-        Returns:
-            AutoObject(w.VBox)
-        """
-
-        self.update_map_widgets = update_map_widgets
-        self._init_schema(schema, by_alias=by_alias)  # TODO: make schema a trait
-        self._init_ui()
-        super().__init__(fns_onsave=fns_onsave, fns_onrevert=fns_onrevert, **kwargs)
-        self.title.value = make_bold(self.get_title())
-        self.description.value = self.get_description()
-        self._format_rows()
-        if value is not None:
-            self.value = value
-        else:
-            self._value = self.di_widgets_value
-
     @tr.validate("insert_rows")
     def validate_insert_rows(self, proposal):
         fn_checkisintkeys = (
             lambda di: True
             if [isinstance(l, int) == True for l in di.keys()]
             else False
         )
@@ -509,23 +531,25 @@
                             f"{k}: widget does not have a `disabled` traitlet"
                         )
 
     @tr.validate("order")
     def _order(self, proposal):
         v = proposal["value"]
         if v is not None:
+            if self.default_order is None:
+                return []
             for _ in v:
                 if _ not in self.default_order:
                     raise ValueError(f"ERROR: {_} not in {str(self.default_order)}")
             if not self.order_can_hide_rows:
                 if set(v) != set(self.default_order):
                     raise ValueError(
                         "set(v) != set(self.default_order)"
                         "if you want to use order to hide rows then set:"
-                        "`order_hides_rows = True`"
+                        "`order_can_hide_rows = True`"
                     )
         return v
 
     @tr.validate("order_can_hide_rows")
     def _order_can_hide_rows(self, proposal):
         if self.order_can_hide_rows != proposal["value"]:
             if self.order is not None:
@@ -555,17 +579,55 @@
         return [fn(p) for p in proposal["value"]]
 
     @tr.validate("_value")
     def _valid_value(self, proposal):
         # TODO: add validation?
         return proposal["value"]
 
+    def __init__(
+        self,
+        schema,
+        by_alias=False,
+        value=None,
+        update_map_widgets=None,
+        **kwargs,
+    ):
+        """creates a widget input form from schema. datatype must be "object"
+
+        Args:
+            schema (dict): json schema defining widget to generate
+            by_alias (bool, optional): use alias in schema. Defaults to False.
+            value (dict, optional): value of json. Defaults to None.
+            update_map_widgets (frozenmap, optional): frozen dict of widgets to map to schema items. Defaults to None.
+            fn_onsave (callable, optional): function to run on save. Defaults to None.
+            fn_onrevert (callable, optional): function to run on revert. Defaults to None.
+
+        Returns:
+            AutoObject(w.VBox)
+        """
+
+        self.update_map_widgets = update_map_widgets
+        self._init_schema(schema, by_alias=by_alias)  # TODO: make schema a trait
+        self._init_ui()
+        super().__init__(**kwargs)
+        self._update_traits_from_schema()
+        self._update_fdir()
+        self._format_rows()
+        if value is not None:
+            self.value = value
+        else:
+            self._value = self.di_widgets_value
+        self.savebuttonbar.unsaved_changes = False
+
     @property
     def default_order(self):
-        return list(self.di_widgets.keys())
+        try:
+            return list(self.di_widgets.keys())
+        except:
+            None
 
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, value):
@@ -612,14 +674,23 @@
         }
         self.contains_nullable = False
         for v in self.pr.values():
             if "nullable" in v.schema_:
                 self.contains_nullable = True
                 break
 
+    def _update_traits_from_schema(self):
+        traits = list(self.traits().keys())
+        for k, v in self.schema.items():
+            if k in traits:
+                setattr(self, k, v)
+            else:
+                pass
+
+    def _update_fdir(self):
         if self.fdir is not None:
             for v in self.pr.values():
                 v = add_fdir_to_widgetcaller(v, self.fdir)
 
     def _init_widgets(self):
         self.di_labels, self.di_widgets = _init_widgets_and_labels(self.pr)
 
@@ -724,39 +795,43 @@
         self._update_map_widgets = value
         self.widgets_map = aumap.get_widgets_map(value)
 
 
 if __name__ == "__main__":
     from ipyautoui.demo_schemas import CoreIpywidgets
 
+    fn = lambda: print("it works!")
+    fn.__name__ = "test-func"
     ui = AutoObject(
         CoreIpywidgets,
         order=["text", "int_text", "int_slider", "int_slider_nullable"],
-        show_description=False,
-        show_title=False,
-        show_savebuttonbar=False,
+        show_description=True,
+        show_title=True,
+        show_savebuttonbar=True,
         show_raw=False,
+        fns_onsave=[fn],
     )
     display(ui)
 # -
 
 if __name__ == "__main__":
+    ui.show_savebuttonbar = False
+    ui.show_title = True
+
+if __name__ == "__main__":
     from ipyautoui.demo_schemas import EditableGrid
 
-    ui = AutoObject(
+    ui_gr = AutoObject(
         EditableGrid,
         show_description=False,
         show_title=False,
         show_savebuttonbar=False,
         show_raw=False,
     )
-    display(ui)
-
-# +
-# ui.show_savebuttonbar = True
+    display(ui_gr)
 
 # +
 if __name__ == "__main__":
     order = [
         "text",
         "int_text",
         "int_slider",
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/automapschema.py` & `ipyautoui-0.4.9/src/ipyautoui/automapschema.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #     language: python
 #     name: python3
 # ---
 
 # +
 # %run _dev_sys_path_append.py
 # %run __init__.py
-#
 # %load_ext lab_black
 import typing as ty
 from pydantic import BaseModel, Field
 import ipywidgets as w
 import ipyautoui.autowidgets as auiwidgets
 from ipyautoui._utils import frozenmap, obj_from_importstr
 
@@ -82,15 +81,19 @@
     """
     if schema_base is None:
         schema_base = schema.copy()
         if "definitions" in schema_base.keys():
             schema_base["definitions"] = attach_schema_refs(
                 schema_base["definitions"], schema_base=schema_base
             )
-        # ^ TODO: how can i $refs be attached to definitions
+            schema_base["definitions"] = attach_schema_refs(
+                schema_base["definitions"], schema_base=schema_base
+            )
+            # ^ TODO: run twice to ensure nested refs in definitions are attached
+            #         come up with a more elegant implementation.
 
     try:
         schema = schema.copy()
     except:
         pass
     # ^ copying to avoid pydantic schema being modified "in-place"
 
@@ -586,27 +589,35 @@
     """
     try:
         if "nullable" in caller.schema_.keys() and caller.schema_["nullable"]:
             fn = auiwidgets.nullable(caller.autoui)
         else:
             fn = caller.autoui
         wi = fn(caller.schema_, *caller.args, **caller.kwargs)
-    except:
+    except Exception as e:
+
         if show_errors:
+            from ipyautoui.custom.widgetcaller_error import WidgetCallerError
+
             txt = f"""
 ERROR: widgetcaller
 -----
 widget:
 {str(caller.autoui)}
 
 schema: 
 {str(caller.schema_)}
+
+error:
+{str(e)}
 """
             # TODO: add logging
-            wi = w.Textarea(txt)
+            wi = WidgetCallerError(
+                widget=str(caller.autoui), schema=caller.schema_, error=str(e)
+            )
         else:
             return  # TODO: check this works
     return wi
 
 
 def update_widgets_map(widgets_map, di_update=None):
     """update the widget mapper frozen object
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/autoui.py` & `ipyautoui-0.4.9/src/ipyautoui/autoui.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,23 +25,21 @@
     ipywidgets UI. Currently nesting is not supported::
 
         from ipyautoui.constants import DISPLAY_AUTOUI_SCHEMA_EXAMPLE
         DISPLAY_AUTOUI_SCHEMA_EXAMPLE()
 """
 # %run _dev_sys_path_append.py
 # %run __init__.py
-#
 # %load_ext lab_black
 
 import pathlib
 from IPython.display import display
 from pydantic import BaseModel
 import json
 import traitlets as tr
-import traitlets_paths
 import typing as ty
 
 from ipyautoui.custom import SaveButtonBar  # removing makes circular import error
 from ipyautoui.autoipywidget import AutoObject, get_from_schema_root
 
 # +
 def rename_vjsf_schema_keys(obj, old="x_", new="x-"):
@@ -97,23 +95,18 @@
 # -
 
 
 class AutoUiFileMethods(tr.HasTraits):
     """AutoUiFileMethods is a mixin class that adds file methods to a AutoUi class
 
     Attributes:
-        path (traitlets_paths.Path): path to file
+        path (tr.Instance(klass=pathlib.PurePath)...): path to file
     """
 
-    path = traitlets_paths.Path(allow_none=True)
-
-    @tr.validate("path")
-    def _path(self, proposal):
-        if proposal["value"] is not None:
-            return pathlib.Path(proposal["value"])
+    path = tr.Instance(klass=pathlib.PurePath, default_value=None, allow_none=True)
 
     @tr.observe("path")
     def _observe_path(self, proposal):
         self.savebuttonbar.fns_onsave_add_action(self.file, to_beginning=True)
         self.savebuttonbar.fns_onrevert_add_action(self.load_file, to_beginning=True)
 
     def _get_path(self, path=None) -> pathlib.Path:
@@ -177,101 +170,87 @@
             unsaved_changes = True
         self.load_value(parse_json_file(p, model=self.model), unsaved_changes)
 
 
 class AutoRenderMethods:
     @classmethod
     def create_autoui_renderer(
-        cls,
-        schema: ty.Union[ty.Type[BaseModel], dict],
-        show_raw: bool = True,
-        path=None,
-        fns_onsave=None,
-        fns_onrevert=None,
+        cls, schema: ty.Union[ty.Type[BaseModel], dict], path=None, **kwargs
     ):
         if isinstance(schema, dict):
             docstring = f"AutoRenderer for {get_from_schema_root(schema, 'title')}"
         else:
             docstring = (
                 f"AutoRenderer for {get_from_schema_root(schema.schema(), 'title')}"
             )
 
         class AutoRenderer(cls):
             def __init__(self, path: pathlib.Path = path):
                 f"""{docstring}"""
                 if path is None:
                     raise ValueError("must give path")
-                super().__init__(
-                    schema,
-                    path=path,
-                    value=None,
-                    show_raw=show_raw,
-                    fns_onsave=fns_onsave,
-                    fns_onrevert=fns_onrevert,
-                )
+                super().__init__(schema, path=path, value=None, **kwargs)
 
         return AutoRenderer
 
     @classmethod
     def create_autodisplay_map(
-        cls,
-        schema: ty.Union[ty.Type[BaseModel], dict],
-        ext=".json",
-        show_raw: bool = True,
-        fns_onsave=None,
-        fns_onrevert=None,
+        cls, schema: ty.Union[ty.Type[BaseModel], dict], ext=".json", **kwargs
     ):
-        AutoRenderer = cls.create_autoui_renderer(
-            schema, show_raw=show_raw, fns_onsave=fns_onsave, fns_onrevert=fns_onrevert
-        )
+        AutoRenderer = cls.create_autoui_renderer(schema, **kwargs)
         return {ext: AutoRenderer}
 
 
 # +
 class AutoUi(AutoObject, AutoUiFileMethods, AutoRenderMethods):
     """extends AutoObject and AutoUiCommonMethods to create an
     AutoUi user-input form. The data that can be saved to a json
     file `path` and loaded from a json file.
 
     Attributes:
-        # inherited from AutoFileMethods
+
+        # AutoFileMethods
         # ------------------------------
-        path (traitlets_paths.Path): path to file
+        path (tr.Instance(klass=pathlib.PurePath, ... ): path to file
+
+        # AutoObjectFormLayout
+        # -------------------------
+        title (str): form title
+        description (str): form description
+        show_description (bool, optional): show the description. Defaults to True.
+        show_title (bool, optional): show the title. Defaults to True.
+        show_savebuttonbar (bool, optional): show the savebuttonbar. Defaults to True.
+        show_raw (bool, optional): show the raw json. Defaults to False.
+        fn_onshowraw (callable): do not edit
+        fn_onhideraw (callable): do not edit
+        fns_onsave (callable): additional functions to be called on save
+        fns_onrevert (callable): additional functions to be called on revert
 
-        # inherited from AutoObject
+        # AutoObject
         # -------------------------
         _value (dict): use `value` to set and get. the value of the form. this is a dict of the form {key: value}
         fdir (path, optional): fdir to work from. useful for widgets that link to files. Defaults to None.
         align_horizontal (bool, optional): aligns widgets horizontally. Defaults to True.
         nested_widgets (list, optional): allows user to indicate widgets that should be show / hide type. Defaults to [].
         auto_open (bool, optional): automatically opens the nested_widget. Defaults to True.
         order (list): allows user to re-specify the order for widget rows to appear by key name in self.di_widgets
         order_can_hide_rows (bool): allows user to hide rows by removing them from the order list.
         insert_rows (dict): e.g. {3:w.Button()}. allows user to insert a widget into the rows. its presence
             is ignored by the widget otherwise.
         disabled (bool, optional): disables all widgets. If widgets are disabled
             using schema kwargs this is remembered when re-enabled. Defaults to False.
 
-        # inherited from AutoObjectFormLayout
-        # ----------------------------------
-        show_raw (bool, optional): show the raw json. Defaults to False.
-        show_description (bool, optional): show the description. Defaults to True.
-        show_title (bool, optional): show the title. Defaults to True.
-        show_savebuttonbar (bool, optional): show the savebuttonbar. Defaults to True.
-
     """
 
     def __init__(
         self,
         schema: ty.Union[ty.Type[BaseModel], dict],
         value: dict = None,
         path: pathlib.Path = None,  # TODO: generalise data retrieval?
         update_map_widgets=None,
-        fns_onsave=None,
-        fns_onrevert=None,
         # validate_onchange=True,  # TODO: sort out how the validation works
         **kwargs,
     ):
         """initialises the AutoUi. in Jupyter hit "cntrl + I" to load "inspector"
         and see the attributes.
 
         Args:
@@ -281,26 +260,26 @@
             update_map_widgets (dict, optional): allows user to update the map_widgets. Defaults to None.
             fns_onsave (list, optional): list of functions to run on save. Defaults to None.
             fns_onrevert (list, optional): list of functions to run on revert. Defaults to None.
             **kwargs: passed to AutoObject. see attributes for details.
         """
 
         fdir = self.get_fdir(path=path, fdir=kwargs.get("fdir", None))
+        if fdir is not None:
+            kwargs = kwargs | {"fdir": fdir}
         # init app
         super().__init__(
             schema,
             value=None,
             update_map_widgets=update_map_widgets,
-            fdir=fdir,
-            fns_onsave=fns_onsave,
-            fns_onrevert=fns_onrevert,
             **kwargs,
         )
         self.path = path
         self.value = self._get_value(value, self.path)
+        self.savebuttonbar.unsaved_changes = False
 
     def get_fdir(self, path=None, fdir=None):
 
         if path is not None and fdir is None:
             return pathlib.Path(path).parent
         elif path is None and fdir is not None:
             return fdir
@@ -311,18 +290,19 @@
 
 
 if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic, TestAutoLogicSimple
 
     aui = AutoUi(
         TestAutoLogicSimple,
-        path="test.json",
-        show_description=False,
-        show_raw=True,  
-        show_savebuttonbar=False,
+        path=pathlib.Path("test.json"),
+        show_description=True,
+        show_raw=False,
+        show_savebuttonbar=True,
+        fns_onsave=[lambda: print("asdf")],
     )
     # aui.show_savebuttonbar = False
     display(aui)
 
 # +
 # aui.savebuttonbar.layout.display
 
@@ -346,34 +326,36 @@
 #  'dropdown_edge_case': 'female',
 #  'dropdown_simple': 'asd',
 #  'combobox': 'asd',
 #  'text': 'short text',
 #  'text_area': 'long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text long text ',
 #  'markdown': '\nSee details here: [__commonmark__](https://commonmark.org/help/)\n\nor press the question mark button. \n'}
 
-# +
-
 if __name__ == "__main__":
-    TestRenderer = AutoUi.create_autoui_renderer(TestAutoLogicSimple, path="test.json")
+    fn = lambda: print("it works!")
+    fn.__name__ = "test-func"
+    TestRenderer = AutoUi.create_autoui_renderer(
+        TestAutoLogicSimple,
+        path=pathlib.Path("test.json"),
+        fns_onsave=[fn],
+    )
     r = TestRenderer()
     r.show_savebuttonbar = True
     display(r)
 
-
 if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic, TestAutoLogicSimple
 
     aui = AutoUi(
         TestAutoLogicSimple,
-        path="test.json",
+        path=pathlib.Path("test.json"),
         show_raw=True,
         fn_onsave=lambda: print("test onsave"),
     )
     display(aui)
-# -
 
 if __name__ == "__main__":
     aui.show_description = False
     aui.show_title = False
     aui.show_raw = False
 
 # + tags=[]
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/autovjsf.py` & `ipyautoui-0.4.9/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/autowidgets.py` & `ipyautoui-0.4.9/src/ipyautoui/autowidgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,20 @@
         ValueError: if "value" trait not exist
     Returns:
         typing.Type: trait type of traitlet
     """
     try:
         return obj_with_traits.traits()["value"]
     except:
-        raise ValueError(f"{str(type(obj_with_traits))}: has no 'value' trait")
+        try:
+            return obj_with_traits.traits()["_value"]
+        except:
+            raise ValueError(
+                f"{str(type(obj_with_traits))}: has no 'value' or '_value' trait"
+            )
 
 
 def is_null(value):
     """
 
     Example:
         >>> [is_null(value) for value in [math.nan, np.nan, None, pd.NA, 3.3, "adsf"]]
@@ -74,29 +79,29 @@
 
 
 class Nullable(w.HBox):
     """class to allow widgets to be nullable. The widget that is extended is accessed
     using `self.widget`"""
 
     disabled = tr.Bool(default_value=False)
-    
+
     @tr.observe("disabled")
     def observe_disabled(self, on_change):
         """If disabled, ensure that the widget is disabled and the button is also."""
         if self.disabled:
             if self.widget.value is not None:
                 self.bn.value = False
             else:
                 self.bn.value = True
             self.bn.disabled = True
             self.widget.disabled = True
         else:
             self.bn.disabled = False
             self.widget.disabled = False
-    
+
     def __init__(self, widget_type, schema, *args, **kwargs):
         self.schema = schema
         self.caller = create_widget_caller(schema)
         # ^ TODO: should this be in a higher-level func?
         #         ui = nullable(w.IntSlider)(value=30) # this doesn't work bu maybe should...
         self.nullable = tr.Bool(default_value=True)
         self.bn = w.ToggleButton(icon="toggle-on", layout={"width": "40px"})
@@ -123,30 +128,36 @@
         trait_type = type(_get_value_trait(self.widget))
         self.add_traits(**{"_value": trait_type(allow_none=True)})
 
     @property
     def value(self):
         return self._value
 
+    def update_value(self, value):
+        self.bn.value = False
+        self.widget.value = value
+        # note. as the self.widget.value still exists in the background,
+        #       this may not trigger a change event...
+        #       so we'll manually do it too (below)
+        self._update("")
+
     @value.setter
     def value(self, value):
-        if pd.isnull(value):
+        if isinstance(value, dict) or isinstance(value, list):
+            self.update_value(value)
+        elif pd.isnull(value):
             self.bn.value = True
             self._value = None
         else:
-            self.bn.value = False
-            self.widget.value = value
-            # note. as the self.widget.value still exists in the background,
-            #       this may not trigger a change event...
-            #       so we'll manually do it too (below)
-            self._update("")
+            self.update_value(value)
 
     def _init_controls(self):
         self.bn.observe(self._toggle_none, "value")
         self.widget.observe(self._update, "value")
+        self.widget.observe(self._update, "_value")
         self.observe(self._observe_nullable, "nullable")
 
     def _observe_nullable(self, onchange):
         if self.nullable:
             self.bn.layout.display = ""
         else:
             self.bn.layout.display = "None"
@@ -496,9 +507,7 @@
 
 
 if __name__ == "__main__":
     import doctest
 
     doctest.testmod()
 # -
-
-
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/basemodel.py` & `ipyautoui-0.4.9/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/constants.py` & `ipyautoui-0.4.9/src/ipyautoui/constants.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/demo.py` & `ipyautoui-0.4.9/src/ipyautoui/demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import traitlets as tr
-from traitlets_paths import PurePath
 import typing as ty
 import ipywidgets as w
 import inspect
 from pydantic import BaseModel
 from IPython.display import display, clear_output, Markdown
 import json
 import pathlib
@@ -27,20 +26,20 @@
     li = [l for l in li if l[0] != "#"]
     li = [l.split("import ")[1] for l in li]
     return li
 
 
 class Demo(w.Tab, tr.HasTraits):
     pydantic_model = tr.Type(klass=BaseModel)
-    python_file: PurePath()
+    python_file = tr.Instance(klass=pathlib.PurePath)
 
     @tr.observe("pydantic_model")
     def _observe_pydantic_model(self, change):
         try:
-            self.python_file = inspect.getfile(self.pydantic_model)
+            self.python_file = pathlib.Path(inspect.getfile(self.pydantic_model))
         except:
             raise ValueError(
                 "for the Demo to work, the `pydantic_model` must"
                 " be defined in a separate python file."
             )
         self._update_autoui()
         self._update_pydantic()
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/env.py` & `ipyautoui-0.4.9/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.4.9/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/test_schema.py` & `ipyautoui-0.4.9/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/vjsf.vue` & `ipyautoui-0.4.9/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/autogrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 # +
 """defines a schema for a datagrid. this is used to build the datagrid and
 contains methods for validation, coercion, and default values. 
 
 defines AutoGrid, a datagrid generated from a jsonschema."""
 # %run _dev_sys_path_append.py
 # %run __init__.py
-#
 # %run ../__init__.py
 # %load_ext lab_black
 
 import typing as ty
 import traitlets as tr
 import logging
 import pandas as pd
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/buttonbars.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/editgrid.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #   jupytext:
 #     cell_metadata_filter: -all
 #     formats: py:light
 #     text_representation:
 #       extension: .py
 #       format_name: light
 #       format_version: '1.5'
-#       jupytext_version: 1.14.0
+#       jupytext_version: 1.14.5
 #   kernelspec:
 #     display_name: Python 3.9 (XPython)
 #     language: python
 #     name: xpython
 # ---
 
 # +
@@ -34,14 +34,15 @@
 from pydantic import BaseModel, Field
 
 import ipyautoui.autoipywidget as aui
 from ipyautoui.custom.buttonbars import CrudButtonBar
 from ipyautoui._utils import frozenmap
 from ipyautoui.constants import BUTTON_WIDTH_MIN
 from ipyautoui.custom.autogrid import AutoGrid
+from ipyautoui.custom.title_description import TitleDescription
 
 MAP_TRANSPOSED_SELECTION_MODE = frozenmap({True: "column", False: "row"})
 # TODO: rename "add" to "fn_add" so not ambiguous...
 # -
 
 
 class DataHandler(BaseModel):
@@ -233,34 +234,19 @@
 
 
 # +
 # TODO: refactor how the datahandler works...
 # TODO: add a test for the datahandler...
 
 
-class EditGrid(w.VBox):
+class EditGrid(w.VBox, TitleDescription):
     _value = tr.Tuple()  # using a tuple to guarantee no accidental mutation
     warn_on_delete = tr.Bool()
     show_copy_dialogue = tr.Bool()
     close_crud_dialogue_on_action = tr.Bool()
-    title = tr.Unicode(default_value=None, allow_none=True)
-    description = tr.Unicode(default_value=None, allow_none=True)
-    show_title = tr.Bool(default_value=True)
-
-    @tr.observe("title")
-    def observe_title(self, on_change):
-        self._update_title_description()
-
-    @tr.observe("description")
-    def observe_description(self, on_change):
-        self._update_title_description()
-
-    @tr.observe("show_title")
-    def observe_show_title(self, on_change):
-        self._update_title_description()
 
     @tr.observe("warn_on_delete")
     def observe_warn_on_delete(self, on_change):
         if self.warn_on_delete:
             self.ui_delete.layout.display = ""
         else:
             self.ui_delete.layout.display = "None"
@@ -295,27 +281,14 @@
     @transposed.setter
     def transposed(self, value: bool):
         self.grid.transposed = value
 
     def _update_value_from_grid(self):
         self._value = self.grid.records()
 
-    def _update_title_description(self):
-        if not self.show_title:
-            self.html_title.layout.display = "None"
-        else:
-            if self.title is None and self.description is None:
-                self.html_title.layout.display = "None"
-            else:
-                self.html_title.layout.display = ""
-                get = lambda v: "" if v is None else v
-                self.html_title.value = (
-                    f"<b>{get(self.title)}</b>, <i>{get(self.description)}</i>"
-                )
-
     def __init__(
         self,
         schema: ty.Union[dict, ty.Type[BaseModel]],
         value: ty.Optional[list[dict[str, ty.Any]]] = None,
         by_alias: bool = False,
         by_title: bool = True,
         datahandler: ty.Optional[DataHandler] = None,
@@ -327,26 +300,24 @@
         show_copy_dialogue: bool = False,
         close_crud_dialogue_on_action: bool = False,
         title: str = None,
         description: str = None,
         show_title: bool = True,
         **kwargs,
     ):
-        self.html_title = w.HTML("")
+        self.html_title = w.HTML()
         self.description = description
         self.title = title
         self.show_title = show_title
 
         self.by_title = by_title
         self.by_alias = by_alias
         self.datahandler = datahandler
-        getvalue = (
-            lambda value: None
-            if value is None or value == [{}]
-            else pd.DataFrame(value)
+        getvalue = lambda value: (
+            None if value is None or value == [{}] else pd.DataFrame(value)
         )
         self.grid = AutoGrid(
             schema, data=getvalue(value), by_alias=self.by_alias, **kwargs
         )
 
         self._init_form()
         if ui_add is None:
@@ -406,16 +377,16 @@
 
     @property
     def model(self):
         return self.grid.model
 
     def _init_form(self):
         super().__init__()
-        get_reload = (
-            lambda: None if self.datahandler is None else self._reload_datahandler
+        get_reload = lambda: (
+            None if self.datahandler is None else self._reload_datahandler
         )
         self.buttonbar_grid = CrudButtonBar(
             fn_add=self._add,
             fn_edit=self._edit,
             fn_copy=self._copy,
             fn_delete=self._delete,
             fn_reload=get_reload(),
@@ -435,18 +406,19 @@
     def _observe_order(self, on_change):
         if "order" in self.ui_add.traits() and self.grid.order is not None:
             self.ui_add.order = self.grid.order
         if "order" in self.ui_edit.traits() and self.grid.order is not None:
             self.ui_edit.order = self.grid.order
 
     def _observe_selections(self, onchange):
-        if self.buttonbar_grid.edit.value:
-            self._set_ui_edit_to_selected_row()
-        if self.buttonbar_grid.delete.value:
-            self._set_ui_delete_to_selected_row()
+        if self.grid.selections != []:
+            if self.buttonbar_grid.edit.value:
+                self._set_ui_edit_to_selected_row()
+            if self.buttonbar_grid.delete.value:
+                self._set_ui_delete_to_selected_row()
 
     # @debounce(0.1)  # TODO: make debounce work if too slow...
     def _grid_changed(self, onchange):
         # debouncer used to allow editing whole rows in 1 go
         # without updating the `value` on every cell edit.
         self._update_value_from_grid()
 
@@ -663,15 +635,15 @@
         __root__: ty.List[DataFrameCols] = Field(
             default=AUTO_GRID_DEFAULT_VALUE,
             format="dataframe",
             datagrid_index_name=("section", "title"),
         )
 
     title = "The Wonderful Edit Grid Application"
-    description = markdown("Useful for all editing purposes" " whatever they may be 👍")
+    description = markdown("Useful for all editing purposes whatever they may be 👍")
     editgrid = EditGrid(
         schema=TestDataFrame,
         title=title,
         description=description,
         ui_add=None,
         ui_edit=None,
         warn_on_delete=True,
@@ -684,24 +656,23 @@
 
 if __name__ == "__main__":
     editgrid.grid.order = ("floater", "string")
     # ^ NOTE: this will result in a value change in the grid
 
 
 if __name__ == "__main__":
-
     datahandler = DataHandler(
         fn_get_all_data=lambda: AUTO_GRID_DEFAULT_VALUE * random.randint(1, 10),
         fn_post=lambda v: print(v),
         fn_patch=lambda v: print(v),
         fn_delete=lambda v: print(v),
         fn_copy=lambda v: print(v),
     )
     title = "The Wonderful Edit Grid Application"
-    description = markdown("Useful for all editing purposes" " whatever they may be 👍")
+    description = markdown("Useful for all editing purposes whatever they may be 👍")
     editgrid = EditGrid(
         schema=TestDataFrame,
         title=title,
         description=description,
         datahandler=datahandler,
     )
     display(editgrid)
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/filechooser.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 #     language: python
 #     name: python3
 # ---
 
 """wrapper for ipyfilechooster.FileChooser"""
 # %run _dev_sys_path_append.py
 # %run __init__.py
-#
 # %load_ext lab_black
 
 import pathlib
 import traitlets as tr
-from traitlets_paths import PurePath  # TODO: create conda recipe for this package
+import typing as ty
 from ipyfilechooser import FileChooser
 
 
 def make_path(path):
     if type(path) == str:
         return pathlib.PurePath(path)
     else:
@@ -38,27 +37,26 @@
     follows the same convention as ipywidgets and therefore integrates
     better wiht ipyautoui
 
     Reference:
         https://github.com/crahan/ipyfilechooser
     """
 
-    # _value = PurePath()
     _value = tr.Unicode()
 
     @tr.default("_value")
     def _default_value(self):
         return str(pathlib.Path("."))
 
     @property
     def value(self):
         return self._value
 
     @value.setter
-    def value(self, value: PurePath):
+    def value(self, value: ty.Union[str, pathlib.Path]):
         """having the setter allows users to pass a new value field to the class which also updates the
         `selected` argument used by FileChooser"""
         self._value = str(value)
         p = pathlib.Path(self.value)
         if p.is_dir():
             self.reset(self.value, None)
         elif p.is_file():
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/fileupload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,85 +1,100 @@
+# -*- coding: utf-8 -*-
+# ---
+# jupyter:
+#   jupytext:
+#     cell_metadata_filter: -all
+#     formats: py:light
+#     text_representation:
+#       extension: .py
+#       format_name: light
+#       format_version: '1.5'
+#       jupytext_version: 1.14.0
+#   kernelspec:
+#     display_name: Python 3 (ipykernel)
+#     language: python
+#     name: python3
+# ---
+
 """file upload wrapper"""
 # %load_ext lab_black
 # %run _dev_sys_path_append.py
 # %run __init__.py
 # %run ../__init__.py
 
+# +
 import ipywidgets as w
 from markdown import markdown
 from IPython.display import display, clear_output
 from pydantic import BaseModel, validator, Field
 import pathlib
 import typing as ty
 import stringcase
 from datetime import datetime
 import traitlets as tr
 import json
 import logging
-
 from ipyautoui.constants import DELETE_BUTTON_KWARGS
 from ipyautoui._utils import getuser
 from ipyautoui.autodisplay import DisplayObject, DisplayPath
 from ipyautoui.custom.iterable import Array
 from ipyautoui.autodisplay_renderers import render_file
 from ipyautoui.env import Env
 
 IPYAUTOUI_ROOTDIR = Env().IPYAUTOUI_ROOTDIR
 IS_IPYWIDGETS8 = (lambda: True if "8" in w.__version__ else False)()
 logger = logging.getLogger(__name__)
 
+
+# +
 class File(BaseModel):
     name: str
     fdir: pathlib.Path = pathlib.Path(".")
     path: pathlib.Path = None
 
     @validator("path", always=True, pre=True)
     def _path(cls, v, values):
         return values["fdir"] / values["name"]
-
-
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
 
-
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
 
-
 def add_files(upld_value, fdir=pathlib.Path(".")):
     if not pathlib.Path(fdir).exists():
         pathlib.Path(fdir).mkdir(exist_ok=True)
     return add_files_ipywidgets8(upld_value, fdir=fdir)
 
-
 class FilesUploadToDir(Array):
     def __init__(
         self,
         value=None,
         fdir=pathlib.Path("."),
         kwargs_display_path: ty.Optional[dict] = None,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             add_remove_controls="remove_only",
             show_hash=None,
         )
         coerce_none = lambda v: {} if v is None else v
         self.kwargs_display_path = coerce_none(kwargs_display_path)
@@ -127,19 +142,23 @@
         kwargs_display_path: ty.Optional[dict] = None,
         **kwargs,
     ):
         super().__init__(
             value=value, fdir=fdir, kwargs_display_path=kwargs_display_path, **kwargs
         )
 
+
+# -
+
 if __name__ == "__main__":
     upld = FilesUploadToDir(
         ["/mnt/c/engDev/git_mf/test.PNG"], fdir=pathlib.Path("/mnt/c/engDev/git_mf")
     )
     display(upld)
+    # test
 
 if __name__ == "__main__":
     upld.value = ["EquipmentReferences-MaxFordhamStandard.pdf", "GenesisCroixDeFer.jpg"]
 
 if __name__ == "__main__":
     from pydantic import BaseModel, Field
     from ipyautoui.custom.fileupload import AutoUploadPaths
@@ -154,15 +173,14 @@
         )
 
     value = {"string": "string", "paths": ["bdns.csv"]}
     aui = AutoUi(Test, value=value, nested_widgets=[AutoUploadPaths])
     display(aui)
 
 
-# +
 class AutoUploadPathsValueString(w.VBox):
     _value = tr.Unicode()
 
     def __init__(
         self,
         schema=None,
         value=None,
@@ -204,15 +222,14 @@
     from ipyautoui import AutoUi
 
     class Test(BaseModel):
         paths: list[pathlib.Path] = Field(autoui="__main__.AutoUploadPathsValueString")
 
     aui = AutoUi(Test)
     display(aui)
-# -
 
 if __name__ == "__main__":
     upld = AutoUploadPathsValueString(
         fdir=pathlib.Path("/mnt/c/engDev/git_mf"),
     )
     display(upld)
 
@@ -222,9 +239,7 @@
     )
 
 if __name__ == "__main__":
     aui = AutoUploadPathsValueString(
         value='["EquipmentReferences-MaxFordhamStandard.pdf", "GenesisCroixDeFer.jpg"]'
     )
     display(aui)
-
-
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/iterable.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,18 +67,17 @@
         }
 
         arr = Array(**di_arr)
         display(arr)
 
 """
 # TODO: move iterable.py to root
-# TODO: review: https://github.com/widgetti/react-ipywidgets - it could simplify the code required below.
+# TODO: review: https://github.com/widgetti/reacton - it could simplify the code required below.
 # %run _dev_sys_path_append.py
 # %run __init__.py
-#
 # %load_ext lab_black
 import ipywidgets as w
 import traitlets as tr
 from traitlets import validate
 import typing as ty
 from IPython.display import display
 from ipyautoui.basemodel import BaseModel
@@ -94,22 +93,22 @@
     BUTTON_WIDTH_MIN,
     BUTTON_HEIGHT_MIN,
     BUTTON_MIN_SIZE,
 )
 from ipyautoui._utils import frozenmap
 from ipyautoui.autowidgets import create_widget_caller
 import logging
+from ipyautoui.custom.title_description import TitleDescription
 
 logger = logging.getLogger(__name__)
 BOX = frozenmap({True: w.HBox, False: w.VBox})
 TOGGLE_BUTTON_KWARGS = frozenmap(
     icon="",
     layout={"width": BUTTON_WIDTH_MIN, "height": BUTTON_HEIGHT_MIN},
 )
-# -
 
 # +
 class IterableItem(BaseModel):
     index: int
     key: ty.Union[UUID, str, int, float, bool] = None
     item: ty.Any = None
     add: ty.Any = None
@@ -168,19 +167,19 @@
             v.children[2].children = [values["item"]]
             return v
         else:
             return v
 
 
 # # +
-class Array(w.VBox):
+class Array(w.VBox, TitleDescription):
     """generic iterable. pass a list of items"""
 
     # -----------------------------------------------------------------------------------
-    _value = tr.List()
+    _value = tr.List(allow_none=True)
     _show_hash = tr.Unicode(allow_none=True)
     _add_remove_controls = tr.Unicode(allow_none=True)
     _sort_on = tr.Unicode(allow_none=True)
 
     @validate("show_hash")
     def _validate_show_hash(self, proposal):
         if proposal.value not in ["index", "key", None]:
@@ -197,18 +196,18 @@
             "append_only",
             "remove_only",
             None,
         ]:  # TODO: put this in an enum...
             raise ValueError(
                 f'{proposal} given. allowed values of _add_remove_controls are "add_remove", "append_only", "remove_only", None only'
             )
-        return proposal
+        return proposal.value
 
     @validate("_sort_on")
-    def _validate_add_remove_controls(self, proposal):
+    def _validate_sort_on(self, proposal):
         if proposal.value not in ["index", "key", None]:
             raise ValueError(
                 f'{proposal} given. allowed values of sort_on are "index", "key" and None only'
             )
         return proposal
 
     def _update_value(self, onchange):
@@ -217,14 +216,16 @@
     # -----------------------------------------------------------------------------------
     def __init__(
         self,
         value: ty.List = None,
         items: ty.List = None,
         toggle=False,
         title=None,
+        description=None,
+        show_title=True,
         fn_add: ty.Callable = lambda: display("add item"),
         fn_add_dialogue: ty.Callable = None,
         fn_remove: ty.Callable = lambda: display("remove item"),
         # fn_remove_dialogue: ty.Callable = lambda: display(f"are you sure you want to remove {item}"), #TODO
         watch_value: bool = True,
         minlen: int = 0,
         maxlen: int = 100,
@@ -246,14 +247,16 @@
         self.watch_value = watch_value
         self.zfill = 2
         value, items = self._init_value(value, items)
         self.iterable = self._init_iterable(items)
         self._init_form()
         self._toggle = toggle
         self.title = title
+        self.description = description
+        self.show_title = show_title
         self.add_remove_controls = add_remove_controls
         self.show_hash = show_hash
         self.sort_on = sort_on
         self._update_value("change")
 
     def _init_value(self, value, items):
         if value is None and items is None:
@@ -498,27 +501,14 @@
 
     @toggle.setter
     def toggle(self, value: bool):
         self._toggle = value
         self.toggle_button.value = True
         self._update_header()
 
-    @property
-    def title(self):
-        return self._title
-
-    @title.setter
-    def title(self, value: ty.Union[str, None]):
-        self._title = value
-        if self.title is None:
-            self.html_title = w.HTML(self.title)
-        else:
-            self.html_title = w.HTML(markdown(self.title))
-        self._update_header()
-
     def _update_header(self):
         header = []
         if self.toggle:
             header.append(self.toggle_button)
         if self.title is not None:
             header.append(self.html_title)
         self.title_box.children = header
@@ -881,14 +871,15 @@
     di_arr = {
         "items": [fn_add()],
         "fn_add": fn_add,
         "maxlen": 10,
         "show_hash": "index",
         "toggle": True,
         "title": "Array",
+        "description": "asdf",
         "add_remove_controls": "append_only",
         "orient_rows": False,
     }
 
     arr = Array(**di_arr)
     display(arr)
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/selectdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/showhide.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.4.9/src/ipyautoui/custom/workingdir.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,18 @@
 #
 # %load_ext lab_black
 
 # +
 from pydantic import BaseModel, validator, Field
 from ipyautoui.constants import LOAD_BUTTON_KWARGS, BUTTON_WIDTH_MIN
 from IPython.display import clear_output, Markdown
-from ipyautoui._utils import file
+from ipyautoui._utils import file, get_user
 import ipywidgets as w
 import traitlets as tr
 
-from getpass import getuser
-import os
 from halo import HaloNotebook
 from enum import Enum
 import pathlib
 from pydantic import BaseModel
 import typing as ty
 from datetime import datetime
 import logging
@@ -134,22 +132,14 @@
 class WorkingDirs(BaseModel):
     name: str = "working dirs"
     description: str = description
     dirs: ty.Dict[str, WorkingDir] = Field(default_factory=lambda: {})
 
 
 # + tags=[]
-def get_user():
-    """get user. gets JUPYTERHUB_USER if present (i.e. if notebook served via a JupyterHub)"""
-    nm = "JUPYTERHUB_USER"
-    if nm in list(os.environ.keys()):
-        return os.environ[nm]
-    else:
-        return getuser()
-
 
 def get_working_dirs(path=FPTH_WORKING_DIRS):
     """loads working dir from folder"""
     if path.exists():
         wdirs = WorkingDirs.parse_file(path)
     else:
         wdirs = WorkingDirs()
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from ipyautoui.basemodel import BaseModel
 from pydantic import Field, conint, constr
 import typing as ty
 
 DATAGRID_TEST_VALUE = [
     {
-        "string": "how long",
+        "string": "important string",
         "integer": 1,
         "floater": 3.14,
         "something_else": 324,
     },
-    # {"string": "update", "integer": 4, "floater": 3.12344, "something_else": 123},
-    # {"string": "evening", "integer": 5, "floater": 3.14, "something_else": 235},
-    # {"string": "morning", "integer": 5, "floater": 3.14, "something_else": 12},
-    # {"string": "number", "integer": 3, "floater": 3.14, "something_else": 123},
+    {"string": "update", "integer": 4, "floater": 3.12344, "something_else": 123},
+    {"string": "evening", "integer": 5, "floater": 3.14, "something_else": 235},
+    {"string": "morning", "integer": 5, "floater": 3.14, "something_else": 12},
+    {"string": "number", "integer": 3, "floater": 3.14, "something_else": 123},
 ]
 
 
 class DataFrameCols(BaseModel):
     string: str = Field("string", column_width=200)
     integer: int = Field(1)
     floater: float = Field(3.1415, column_width=70)
     something_else: float = Field(324, column_width=100)
 
 
-class EditableGrid(BaseModel):
-    __root__: ty.List[DataFrameCols] = Field(
+class NestedEditableGrid(BaseModel):
+    title: str = "My editable Dataframe"
+    reference: str = "some ref data"
+    grid: ty.List[DataFrameCols] = Field(
         default=DATAGRID_TEST_VALUE,
         # default_factory=lambda: DATAGRID_TEST_VALUE, # TODO: AutoUi isn't getting data when set using default_factory. make this work!
         format="DataFrame",
         global_decimal_places=2,
     )
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from ipyautoui.basemodel import BaseModel
 from pydantic import Field, conint, constr
 import typing as ty
 
 DATAGRID_TEST_VALUE = [
     {
-        "string": "important string",
+        "string": "how long",
         "integer": 1,
         "floater": 3.14,
         "something_else": 324,
     },
-    {"string": "update", "integer": 4, "floater": 3.12344, "something_else": 123},
-    {"string": "evening", "integer": 5, "floater": 3.14, "something_else": 235},
-    {"string": "morning", "integer": 5, "floater": 3.14, "something_else": 12},
-    {"string": "number", "integer": 3, "floater": 3.14, "something_else": 123},
+    # {"string": "update", "integer": 4, "floater": 3.12344, "something_else": 123},
+    # {"string": "evening", "integer": 5, "floater": 3.14, "something_else": 235},
+    # {"string": "morning", "integer": 5, "floater": 3.14, "something_else": 12},
+    # {"string": "number", "integer": 3, "floater": 3.14, "something_else": 123},
 ]
 
 
 class DataFrameCols(BaseModel):
     string: str = Field("string", column_width=200)
     integer: int = Field(1)
     floater: float = Field(3.1415, column_width=70)
     something_else: float = Field(324, column_width=100)
 
 
-class NestedEditableGrid(BaseModel):
-    title: str = "My editable Dataframe"
-    reference: str = "some ref data"
-    grid: ty.List[DataFrameCols] = Field(
+class EditableGrid(BaseModel):
+    __root__: ty.List[DataFrameCols] = Field(
         default=DATAGRID_TEST_VALUE,
         # default_factory=lambda: DATAGRID_TEST_VALUE, # TODO: AutoUi isn't getting data when set using default_factory. make this work!
         format="DataFrame",
+        warn_on_delete=True,  # TODO: this isn't being passed
         global_decimal_places=2,
     )
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/demo_schemas/nested_items.py` & `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nested.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 
 class RecursiveNest(BaseModel):
     """description in RecursiveNest docstring"""
 
     string1: str = Field(default="adsf", description="a description about my string")
     int_slider1: conint(ge=1, le=3) = 2
     int_text1: int = 1
-    nested: NestedObject = Field(default=None)
+    nested: NestedObject
 
 
 class Nested(BaseModel):
-    nested: NestedObject = Field(default=None)
-    # recursive_nest: RecursiveNest # TODO: fix this!
+    """demonstrates nested objects"""
+
+    nested: NestedObject
+    recursive_nest: RecursiveNest
     array_simple: list[str]
-    arrar_objects: list[NestedObject]
+    array_objects: list[NestedObject]
+    nullable_list: list[str] = None
+    nullable_object: NestedObject = None
```

### Comparing `ipyautoui-0.4.8/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.4.9/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,22 +12,14 @@
     "Pr_15_31_04": "Pr_15_31_04 - Applied cleaning and treatment products",
 }
 
 UniclassProducts = StrEnum("Uniclass Product Codes", DI_TEST)
 UniclassProducts.__doc__ = "A list of valid Uniclass Product codes"
 
 
-class UniclassProductsUi(BaseModel):
+class RootEnum(BaseModel):
     __root__: UniclassProducts = Field(
         None, autoui="ipyautoui.autowidgets.Combobox", layout={"width": "400px"}
     )
 
     class Config:
         arbitrary_types_allowed = True
-
-
-class RootArrayEnum(BaseModel):
-    """FIXME: **This is currently not working**. Due to nested definition in JSON-schema"""
-
-    products: list[UniclassProductsUi] = Field(
-        None, title=UniclassProducts.__name__, description=UniclassProducts.__doc__
-    )
```

### Comparing `ipyautoui-0.4.8/.gitignore` & `ipyautoui-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/LICENSE` & `ipyautoui-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.4.8/README.md` & `ipyautoui-0.4.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -138,14 +138,21 @@
 # assuming that you have `mamba` installed:
 $ mamba env create -f environment-dev.yml
 
 # run tests
 $ pytest
 ```
 
+```{note}
+[Jupytext](https://github.com/mwouts/jupytext) is used throughout to allow the `.py` files
+to be ran as notebooks to facillitate easy testing. You can use JupyterLab, or if you are 
+using VS Code then install the Jupytext extension. In the `.vscode/settings.json` file
+`"jupyter.notebookFileRoot": "${fileDirname}"` matching with the jupyterlab default. 
+```
+
 ## Packaging (restricted to core-maintainers)
 
 ```sh
 hatch build  # builds to local folder
 hatch publish  # publishes to pypi
 ```
```

### Comparing `ipyautoui-0.4.8/pyproject.toml` & `ipyautoui-0.4.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     "openpyxl",            # for excel fiel viewer
     "pandas",
     "pydantic",
     "pytest",
     "PyYAML",
     "stringcase",
     "traitlets",
-    "traitlets_paths",
     "wcmatch",
 ]
 
 [project.urls]
 Homepage = "https://github.com/maxfordham/ipyautoui"
 
 [tool.hatch.version]
```

### Comparing `ipyautoui-0.4.8/PKG-INFO` & `ipyautoui-0.4.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.4.8
+Version: 0.4.9
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,14 @@
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: pydantic
 Requires-Dist: pytest
 Requires-Dist: pyyaml
 Requires-Dist: stringcase
 Requires-Dist: traitlets
-Requires-Dist: traitlets-paths
 Requires-Dist: wcmatch
 Description-Content-Type: text/markdown
 
 # ipyautoui
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/maxfordham/ipyautoui/HEAD) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![PyPI version](https://badge.fury.io/py/ipyautoui.svg)](https://badge.fury.io/py/ipyautoui)
 
@@ -169,14 +168,21 @@
 # assuming that you have `mamba` installed:
 $ mamba env create -f environment-dev.yml
 
 # run tests
 $ pytest
 ```
 
+```{note}
+[Jupytext](https://github.com/mwouts/jupytext) is used throughout to allow the `.py` files
+to be ran as notebooks to facillitate easy testing. You can use JupyterLab, or if you are 
+using VS Code then install the Jupytext extension. In the `.vscode/settings.json` file
+`"jupyter.notebookFileRoot": "${fileDirname}"` matching with the jupyterlab default. 
+```
+
 ## Packaging (restricted to core-maintainers)
 
 ```sh
 hatch build  # builds to local folder
 hatch publish  # publishes to pypi
 ```
```

