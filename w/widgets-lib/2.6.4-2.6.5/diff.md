# Comparing `tmp/widgets-lib-2.6.4.tar.gz` & `tmp/widgets-lib-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widgets-lib-2.6.4.tar", last modified: Sat Apr  8 15:33:25 2023, max compression
+gzip compressed data, was "widgets-lib-2.6.5.tar", last modified: Thu Apr 13 22:04:58 2023, max compression
```

## Comparing `widgets-lib-2.6.4.tar` & `widgets-lib-2.6.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.329379 widgets-lib-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-08 15:33:25.329379 widgets-lib-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 15:33:25.329379 widgets-lib-2.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.317379 widgets-lib-2.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.321380 widgets-lib-2.6.4/src/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.321380 widgets-lib-2.6.4/src/widgets/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21145 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/base/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/base/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.321380 widgets-lib-2.6.4/src/widgets/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.321380 widgets-lib-2.6.4/src/widgets/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.325379 widgets-lib-2.6.4/src/widgets/streamlit/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/expander.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.325379 widgets-lib-2.6.4/src/widgets/streamlit/resource/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/files/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/files/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/files/download_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.325379 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/selectstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/resource/values/textarea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.325379 widgets-lib-2.6.4/src/widgets/streamlit/widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/streamlit/widget/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.329379 widgets-lib-2.6.4/src/widgets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/templates/source.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/templates/streamlit_single.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/src/widgets/templates/streamlit_single.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.329379 widgets-lib-2.6.4/src/widgets_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-08 15:33:25.000000 widgets-lib-2.6.4/src/widgets_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-08 15:33:25.000000 widgets-lib-2.6.4/src/widgets_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 15:33:25.000000 widgets-lib-2.6.4/src/widgets_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-08 15:33:25.000000 widgets-lib-2.6.4/src/widgets_lib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-08 15:33:25.000000 widgets-lib-2.6.4/src/widgets_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 15:33:25.000000 widgets-lib-2.6.4/src/widgets_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 15:33:25.329379 widgets-lib-2.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/tests/test_duplicator.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/tests/test_source_parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-08 15:32:40.000000 widgets-lib-2.6.4/tests/test_streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.980206 widgets-lib-2.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-13 22:04:58.980206 widgets-lib-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:04:58.980206 widgets-lib-2.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.964206 widgets-lib-2.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.964206 widgets-lib-2.6.5/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.968206 widgets-lib-2.6.5/src/widgets/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21188 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/base/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.968206 widgets-lib-2.6.5/src/widgets/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.968206 widgets-lib-2.6.5/src/widgets/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.968206 widgets-lib-2.6.5/src/widgets/streamlit/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/expander.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.972206 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/files/download_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.972206 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/selectstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/resource/values/textarea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.972206 widgets-lib-2.6.5/src/widgets/streamlit/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/streamlit/widget/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.976206 widgets-lib-2.6.5/src/widgets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/templates/source.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/templates/streamlit_single.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/src/widgets/templates/streamlit_single.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.976206 widgets-lib-2.6.5/src/widgets_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 22:04:58.000000 widgets-lib-2.6.5/src/widgets_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:04:58.976206 widgets-lib-2.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_duplicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_source_parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-13 22:04:23.000000 widgets-lib-2.6.5/tests/test_streamlit.py
```

### Comparing `widgets-lib-2.6.4/LICENSE` & `widgets-lib-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/PKG-INFO` & `widgets-lib-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.6.4
+Version: 2.6.5
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.6.4/README.md` & `widgets-lib-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/pyproject.toml` & `widgets-lib-2.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/base/exceptions.py` & `widgets-lib-2.6.5/src/widgets/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/base/helpers.py` & `widgets-lib-2.6.5/src/widgets/base/helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/base/io.py` & `widgets-lib-2.6.5/src/widgets/base/io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/base/resource.py` & `widgets-lib-2.6.5/src/widgets/base/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         **kwargs
     ) -> None:
         """
         Set up the attributes which are used by all Resource objects.
         """
 
         # The 'id' cannot be empty
-        if len(id) == 0:
-            msg = "Must provide id for Resource"
+        if id is None or len(id) == 0:
+            msg = f"Must provide id for Resource ({self.__class__.__name__})"
             raise ResourceConfigurationException(msg)
 
         # Save the id and starting value for this particular resource
         self.id = id
 
         # If a value was provided
         if value is not None:
```

### Comparing `widgets-lib-2.6.4/src/widgets/base/widget.py` & `widgets-lib-2.6.5/src/widgets/base/widget.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/cli/main.py` & `widgets-lib-2.6.5/src/widgets/cli/main.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/__init__.py` & `widgets-lib-2.6.5/src/widgets/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/base.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/columns.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/columns.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/duplicator.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/expander.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/expander.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/files/base.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/files/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/files/dataframe.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/files/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """DataFrame resource used in a Streamlit-based widget."""
 
     value = pd.DataFrame()
     kwargs = dict()
 
     def __init__(
         self,
-        id=None,
+        id="dataframe",
         value=None,
         label=None,
         help: Union[str, None] = None,
         disabled: bool = False,
         label_visibility: str = "visible",
         kwargs={},
         sidebar=True,
```

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/files/download_dataframe.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/files/download_dataframe.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/markdown.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/markdown.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/selector.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+from copy import deepcopy
 from typing import List, Union
 from widgets.streamlit.resource.base import StResource
 from widgets.streamlit.resource.values.selectstring import StSelectString
 from widgets.base.exceptions import ResourceConfigurationException
 
 
 class StSelector(StResource):
     """
     Present a drop-down menu to the user, and only show the child
     element which they select (based on the label).
     """
 
+    options = []
+
     def __init__(
         self,
         id="selector",
         label="Select Resource",
         options: List[StResource] = None,
         value: Union[str, None] = None,
         **kwargs
     ):
 
         # The user must have provided a list of Resources to select from
         if options is None:
-            msg = f"Selector must have options provided ({id})"
-            raise ResourceConfigurationException(msg)
+            if self.__class__.options is None:
+                msg = f"Selector must have options provided ({id})"
+                raise ResourceConfigurationException(msg)
+            else:
+                options = deepcopy(self.__class__.options)
 
         if not isinstance(options, list):
             msg = f"Selector options must be a list ({id})"
             raise ResourceConfigurationException(msg)
 
         if any([isinstance(i, StResource) is False for i in options]):
             msg = f"Selector options must be a list of Resources ({id})"
@@ -39,15 +45,15 @@
             msg = "Selector options must have unique labels"
             raise ResourceConfigurationException(msg)
 
         # Attach the options
         self.options = options
 
         # If no value was provided
-        if value is None:
+        if value is None and len(self.options) > 0:
 
             # The value is the label of the first one
             value = options[0].label
 
         # If a value was provided
         else:
```

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/base.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/checkbox.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/checkbox.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/float.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/float.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/integer.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/integer.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/multiselect.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/multiselect.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/selectstring.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/selectstring.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/slider.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/slider.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/string.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/string.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/resource/values/textarea.py` & `widgets-lib-2.6.5/src/widgets/streamlit/resource/values/textarea.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/streamlit/widget/base.py` & `widgets-lib-2.6.5/src/widgets/streamlit/widget/base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets/templates/streamlit_single.html.j2` & `widgets-lib-2.6.5/src/widgets/templates/streamlit_single.html.j2`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/src/widgets_lib.egg-info/PKG-INFO` & `widgets-lib-2.6.5/src/widgets_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: widgets-lib
-Version: 2.6.4
+Version: 2.6.5
 Summary: Merging code and data in webpages
 Author-email: Samuel Minot <sminot@fredhutch.org>
 Project-URL: Homepage, https://github.com/FredHutch/widgets
 Project-URL: Bug Tracker, https://github.com/FredHutch/widgets/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `widgets-lib-2.6.4/src/widgets_lib.egg-info/SOURCES.txt` & `widgets-lib-2.6.5/src/widgets_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/tests/test_base.py` & `widgets-lib-2.6.5/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/tests/test_cli.py` & `widgets-lib-2.6.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/tests/test_duplicator.py` & `widgets-lib-2.6.5/tests/test_duplicator.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/tests/test_helpers.py` & `widgets-lib-2.6.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/tests/test_io.py` & `widgets-lib-2.6.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/tests/test_source_parents.py` & `widgets-lib-2.6.5/tests/test_source_parents.py`

 * *Files identical despite different names*

### Comparing `widgets-lib-2.6.4/tests/test_streamlit.py` & `widgets-lib-2.6.5/tests/test_streamlit.py`

 * *Files identical despite different names*

