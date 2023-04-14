# Comparing `tmp/taipy-gui-2.2.0.tar.gz` & `tmp/taipy-gui-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-gui-2.2.0.tar", last modified: Thu Apr 13 16:47:18 2023, max compression
+gzip compressed data, was "taipy-gui-2.2.1.tar", last modified: Fri Apr 14 16:25:56 2023, max compression
```

## Comparing `taipy-gui-2.2.0.tar` & `taipy-gui-2.2.1.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.797062 taipy-gui-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-13 16:47:18.797062 taipy-gui-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:47:18.797062 taipy-gui-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.749062 taipy-gui-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.749062 taipy-gui-2.2.0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.753062 taipy-gui-2.2.0/src/taipy/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/_gui_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/_gui_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/_page.py
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.757062 taipy-gui-2.2.0/src/taipy/gui/data/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/array_dict_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/content_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/data_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/data_scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.757062 taipy-gui-2.2.0/src/taipy/gui/data/decimator/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/decimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/decimator/lttb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/decimator/minmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/decimator/rdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/decimator/scatter_decimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/numpy_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/pandas_data_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.761062 taipy-gui-2.2.0/src/taipy/gui/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/extension/library.py
--rw-r--r--   0 runner    (1001) docker     (123)    89657 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/gui_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/icon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/partial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.761062 taipy-gui-2.2.0/src/taipy/gui/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.761062 taipy-gui-2.2.0/src/taipy/gui/renderers/_html/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_html/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_html/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.765062 taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/blocproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/postproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/preproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    39298 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/renderers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.769062 taipy-gui-2.2.0/src/taipy/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/_locals_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/_map_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/_runtime_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/_variable_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/chart_config_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/clientvarname.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/datatype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/expr_var_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/filename.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/filter_locals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/get_imported_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/get_module_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/getdatecolstrname.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/is_debugging.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/isnotebook.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/table_col_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/utils/varnamefromcontent.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-13 16:42:00.000000 taipy-gui-2.2.0/src/taipy/gui/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.789062 taipy-gui-2.2.0/src/taipy/gui/webapp/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-13 16:46:18.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/227.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)   204372 2023-04-13 16:46:18.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/499.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)  3585962 2023-04-13 16:46:18.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/660.taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 16:46:18.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.789062 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.789062 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/base/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/base/fontfaces.css
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/base/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.789062 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/blocks/layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.793062 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/button.css
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/chart.css
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/date.css
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/expandable.css
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/image.css
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/input.css
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/navbar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/number.css
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/selector.css
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/slider.css
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/table.css
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/toggle.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.793062 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/card.css
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/container.css
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/header.css
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/sidebar.css
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/stylekit.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.793062 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/typography.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.793062 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/colors.css
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/elements.css
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/misc.css
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/shapes.css
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/spacing.css
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/typography.css
--rw-r--r--   0 runner    (1001) docker     (123)   216882 2023-04-13 16:43:40.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)  5202264 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-deps.dll.js
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-13 16:43:40.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-dom.js
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)  1135101 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-13 16:46:18.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/taipy.status.json
--rw-r--r--   0 runner    (1001) docker     (123)    55978 2023-04-13 16:47:09.000000 taipy-gui-2.2.0/src/taipy/gui/webapp/viselements.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:47:18.797062 taipy-gui-2.2.0/src/taipy_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-13 16:47:18.000000 taipy-gui-2.2.0/src/taipy_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-13 16:47:18.000000 taipy-gui-2.2.0/src/taipy_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:47:18.000000 taipy-gui-2.2.0/src/taipy_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:47:11.000000 taipy-gui-2.2.0/src/taipy_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 16:47:18.000000 taipy-gui-2.2.0/src/taipy_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-13 16:47:18.000000 taipy-gui-2.2.0/src/taipy_gui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.720770 taipy-gui-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-14 16:25:56.720770 taipy-gui-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:25:56.720770 taipy-gui-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.692770 taipy-gui-2.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.692770 taipy-gui-2.2.1/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.696770 taipy-gui-2.2.1/src/taipy/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/_gui_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/_gui_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.696770 taipy-gui-2.2.1/src/taipy/gui/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/array_dict_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/content_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/data_scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.696770 taipy-gui-2.2.1/src/taipy/gui/data/decimator/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/decimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/decimator/lttb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/decimator/minmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/decimator/rdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/decimator/scatter_decimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/numpy_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/pandas_data_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.696770 taipy-gui-2.2.1/src/taipy/gui/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15522 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/extension/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89657 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/gui_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/partial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.696770 taipy-gui-2.2.1/src/taipy/gui/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.696770 taipy-gui-2.2.1/src/taipy/gui/renderers/_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_html/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_html/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.700770 taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/blocproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/postproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/preproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39365 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/renderers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.700770 taipy-gui-2.2.1/src/taipy/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/_locals_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/_map_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/_runtime_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/_variable_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/chart_config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/clientvarname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/expr_var_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/filter_locals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/get_imported_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/get_module_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/getdatecolstrname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/is_debugging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/isnotebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/table_col_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/utils/varnamefromcontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-14 16:21:51.000000 taipy-gui-2.2.1/src/taipy/gui/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.712770 taipy-gui-2.2.1/src/taipy/gui/webapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-14 16:25:09.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/227.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)   204372 2023-04-14 16:25:09.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/499.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3585962 2023-04-14 16:25:09.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/660.taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-14 16:25:09.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.712770 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.716770 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/base/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/base/fontfaces.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/base/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.716770 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/blocks/layout.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.716770 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/button.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/chart.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/date.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/expandable.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/image.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/input.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/navbar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/number.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/selector.css
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/table.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/toggle.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.716770 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/card.css
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/container.css
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/header.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/sidebar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/stylekit.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.716770 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/typography.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.716770 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/colors.css
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/elements.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/misc.css
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/shapes.css
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/spacing.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/typography.css
+-rw-r--r--   0 runner    (1001) docker     (123)   216882 2023-04-14 16:23:09.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-deps-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5202264 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-deps.dll.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-14 16:23:09.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-dom.js
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-dom.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)  1135118 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-14 16:25:09.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/taipy.status.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55978 2023-04-14 16:25:48.000000 taipy-gui-2.2.1/src/taipy/gui/webapp/viselements.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:25:56.720770 taipy-gui-2.2.1/src/taipy_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-14 16:25:56.000000 taipy-gui-2.2.1/src/taipy_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-04-14 16:25:56.000000 taipy-gui-2.2.1/src/taipy_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:25:56.000000 taipy-gui-2.2.1/src/taipy_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:25:49.000000 taipy-gui-2.2.1/src/taipy_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-14 16:25:56.000000 taipy-gui-2.2.1/src/taipy_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 16:25:56.000000 taipy-gui-2.2.1/src/taipy_gui.egg-info/top_level.txt
```

### Comparing `taipy-gui-2.2.0/LICENSE` & `taipy-gui-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/PKG-INFO` & `taipy-gui-2.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.2.0
+Version: 2.2.1
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-gui-2.2.0/README.md` & `taipy-gui-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/setup.py` & `taipy-gui-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/__init__.py` & `taipy-gui-2.2.1/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/__init__.py` & `taipy-gui-2.2.1/src/taipy/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/_default_config.py` & `taipy-gui-2.2.1/src/taipy/gui/_default_config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/_gui_cli.py` & `taipy-gui-2.2.1/src/taipy/gui/_gui_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/_gui_section.py` & `taipy-gui-2.2.1/src/taipy/gui/_gui_section.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/_page.py` & `taipy-gui-2.2.1/src/taipy/gui/_page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/config.py` & `taipy-gui-2.2.1/src/taipy/gui/config.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/__init__.py` & `taipy-gui-2.2.1/src/taipy/gui/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/array_dict_data_accessor.py` & `taipy-gui-2.2.1/src/taipy/gui/data/array_dict_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/content_accessor.py` & `taipy-gui-2.2.1/src/taipy/gui/data/content_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/data_accessor.py` & `taipy-gui-2.2.1/src/taipy/gui/data/data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/data_format.py` & `taipy-gui-2.2.1/src/taipy/gui/data/data_format.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/data_scope.py` & `taipy-gui-2.2.1/src/taipy/gui/data/data_scope.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/decimator/__init__.py` & `taipy-gui-2.2.1/src/taipy/gui/data/decimator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/decimator/lttb.py` & `taipy-gui-2.2.1/src/taipy/gui/data/decimator/lttb.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/decimator/minmax.py` & `taipy-gui-2.2.1/src/taipy/gui/data/decimator/minmax.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/decimator/rdp.py` & `taipy-gui-2.2.1/src/taipy/gui/data/decimator/rdp.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/decimator/scatter_decimator.py` & `taipy-gui-2.2.1/src/taipy/gui/data/decimator/scatter_decimator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/numpy_data_accessor.py` & `taipy-gui-2.2.1/src/taipy/gui/data/numpy_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/pandas_data_accessor.py` & `taipy-gui-2.2.1/src/taipy/gui/data/pandas_data_accessor.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/data/utils.py` & `taipy-gui-2.2.1/src/taipy/gui/data/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/extension/__init__.py` & `taipy-gui-2.2.1/src/taipy/gui/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/extension/library.py` & `taipy-gui-2.2.1/src/taipy/gui/extension/library.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/gui.py` & `taipy-gui-2.2.1/src/taipy/gui/gui.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/gui_actions.py` & `taipy-gui-2.2.1/src/taipy/gui/gui_actions.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/icon.py` & `taipy-gui-2.2.1/src/taipy/gui/icon.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/page.py` & `taipy-gui-2.2.1/src/taipy/gui/page.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/partial.py` & `taipy-gui-2.2.1/src/taipy/gui/partial.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/__init__.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_html/__init__.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_html/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_html/factory.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_html/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_html/parser.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_html/parser.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/__init__.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/blocproc.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/blocproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/control.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/control.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/factory.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/postproc.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/postproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/_markdown/preproc.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/_markdown/preproc.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/builder.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,14 +728,15 @@
             if self.__attributes.get("page"):
                 warnings.warn(
                     f"{self.__element_name} control: page and partial should not be defined at the same time."
                 )
             if isinstance(partial, Partial):
                 self.__attributes["page"] = partial._route
                 self.__set_react_attribute("partial", partial._route)
+                self.__set_react_attribute("defaultPartial", True)
         return self
 
     def _set_propagate(self):
         val = self.__get_boolean_attribute("propagate", self.__gui._config.config.get("propagate"))
         return self if val else self.set_boolean_attribute("propagate", False)
 
     def __set_refresh_on_update(self):
```

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/factory.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/factory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/json.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/json.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/renderers/utils.py` & `taipy-gui-2.2.1/src/taipy/gui/renderers/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/server.py` & `taipy-gui-2.2.1/src/taipy/gui/server.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/state.py` & `taipy-gui-2.2.1/src/taipy/gui/state.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/types.py` & `taipy-gui-2.2.1/src/taipy/gui/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/__init__.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/_adapter.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/_attributes.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/_attributes.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/_bindings.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/_bindings.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/_evaluator.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/_evaluator.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/_locals_context.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/_locals_context.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/_map_dict.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/_map_dict.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/_runtime_manager.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/_runtime_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/_variable_directory.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/_variable_directory.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/boolean.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/boolean.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/chart_config_builder.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/chart_config_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/clientvarname.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/clientvarname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/datatype.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/datatype.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/date.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/date.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/expr_var_name.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/expr_var_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/filename.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/filename.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/filter_locals.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/filter_locals.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/get_imported_var.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/get_imported_var.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/get_module_name.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/get_module_name.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/getdatecolstrname.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/getdatecolstrname.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/html.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/html.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/is_debugging.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/is_debugging.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/isnotebook.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/isnotebook.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/singleton.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/table_col_builder.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/table_col_builder.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/types.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/types.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/utils/varnamefromcontent.py` & `taipy-gui-2.2.1/src/taipy/gui/utils/varnamefromcontent.py`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/227.taipy-gui.js` & `taipy-gui-2.2.1/src/taipy/gui/webapp/227.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/499.taipy-gui.js` & `taipy-gui-2.2.1/src/taipy/gui/webapp/499.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/660.taipy-gui.js` & `taipy-gui-2.2.1/src/taipy/gui/webapp/660.taipy-gui.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt` & `taipy-gui-2.2.1/src/taipy/gui/webapp/660.taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/favicon.ico` & `taipy-gui-2.2.1/src/taipy/gui/webapp/favicon.ico`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/favicon.png` & `taipy-gui-2.2.1/src/taipy/gui/webapp/favicon.png`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/index.html` & `taipy-gui-2.2.1/src/taipy/gui/webapp/index.html`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/base/base.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/base/base.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/base/fontfaces.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/base/fontfaces.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/base/typography.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/base/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/blocks/layout.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/blocks/layout.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/button.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/button.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/chart.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/chart.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/date.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/date.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/expandable.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/expandable.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/image.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/image.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/input.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/input.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/navbar.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/navbar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/number.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/number.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/selector.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/selector.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/slider.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/slider.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/table.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/table.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/controls/toggle.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/controls/toggle.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/card.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/card.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/container.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/container.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/header.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/header.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/elements/sidebar.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/elements/sidebar.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/stylekit.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/stylekit.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/colors.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/misc.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/spacing.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/utilities/typography.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/utilities/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/colors.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/colors.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/elements.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/elements.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/misc.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/misc.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/shapes.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/shapes.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/spacing.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/spacing.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/stylekit/variables/typography.css` & `taipy-gui-2.2.1/src/taipy/gui/webapp/stylekit/variables/typography.css`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-deps-manifest.json` & `taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-deps-manifest.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-deps.dll.js` & `taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-deps.dll.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt` & `taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-deps.dll.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui-dom.js` & `taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui-dom.js`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui.d.ts` & `taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui.d.ts`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui.js` & `taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -48994,33 +48994,34 @@
                             }))]
                         })) : null
                     },
                     Part: e => {
                         const {
                             id: r,
                             children: o,
-                            partial: i
+                            partial: i,
+                            defaultPartial: a
                         } = e, {
-                            state: a
-                        } = (0, n.useContext)(lc), s = vc(e.libClassName, e.dynamicClassName, e.className), l = uc(e.render, e.defaultRender, !0), c = uc(e.page, e.defaultPage, ""), u = (0, n.useMemo)((() => {
-                            if (c && !i) {
-                                if (/^https?\:\/\//.test(c)) return !0;
-                                const e = "/" + c;
-                                return !Object.keys(a.locations || {}).some((t => e === t))
+                            state: s
+                        } = (0, n.useContext)(lc), l = vc(e.libClassName, e.dynamicClassName, e.className), c = uc(e.render, e.defaultRender, !0), u = uc(e.page, e.defaultPage, ""), d = (0, n.useMemo)((() => {
+                            if (u && !a) {
+                                if (/^https?\:\/\//.test(u)) return !0;
+                                const e = "/" + u;
+                                return !Object.keys(s.locations || {}).some((t => e === t))
                             }
                             return !1
-                        }), [a.locations, c, i]);
-                        return l ? (0, t.jsxs)(ld, Object.assign({
+                        }), [s.locations, u, a]);
+                        return c ? (0, t.jsxs)(ld, Object.assign({
                             id: r,
-                            className: s
+                            className: l
                         }, {
-                            children: [u ? (0, t.jsx)("iframe", {
-                                src: c
-                            }) : c ? (0, t.jsx)(Gj, {
-                                path: "/" + c,
+                            children: [d ? (0, t.jsx)("iframe", {
+                                src: u
+                            }) : u ? (0, t.jsx)(Gj, {
+                                path: "/" + u,
                                 partial: i,
                                 fromBlock: !0
                             }) : null, o]
                         })) : null
                     },
                     Selector: e => {
                         const {
```

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt` & `taipy-gui-2.2.1/src/taipy/gui/webapp/taipy-gui.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy/gui/webapp/viselements.json` & `taipy-gui-2.2.1/src/taipy/gui/webapp/viselements.json`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy_gui.egg-info/PKG-INFO` & `taipy-gui-2.2.1/src/taipy_gui.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-gui
-Version: 2.2.0
+Version: 2.2.1
 Summary: Low-code library to create graphical user interfaces on the Web for your Python applications.
 Home-page: https://github.com/avaiga/taipy-gui
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-gui
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-gui-2.2.0/src/taipy_gui.egg-info/SOURCES.txt` & `taipy-gui-2.2.1/src/taipy_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-gui-2.2.0/src/taipy_gui.egg-info/requires.txt` & `taipy-gui-2.2.1/src/taipy_gui.egg-info/requires.txt`

 * *Files identical despite different names*

