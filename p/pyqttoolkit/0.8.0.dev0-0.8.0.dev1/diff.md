# Comparing `tmp/pyqttoolkit-0.8.0.dev0.tar.gz` & `tmp/pyqttoolkit-0.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyqttoolkit-0.8.0.dev0.tar", last modified: Thu Oct  6 16:06:52 2022, max compression
+gzip compressed data, was "dist/pyqttoolkit-0.8.0.dev1.tar", last modified: Fri Apr 14 08:09:15 2023, max compression
```

## Comparing `pyqttoolkit-0.8.0.dev0.tar` & `pyqttoolkit-0.8.0.dev1.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/application/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      849 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/application/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4190 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/application/application.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2369 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/application/garbage_collector.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/colors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3093 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/colors/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1002 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      944 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1228 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/composite.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1108 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/default.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1152 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/environment.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3177 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/multi_json_file.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1158 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/with_signal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1190 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/with_value_changed.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      914 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      915 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/bits.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2024 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/cache.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1158 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/interval.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/names.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/datetime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/datetime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2563 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/datetime/datetime.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2290 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/datetime/qdatetime.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/dependencies/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2077 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/dependencies/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/errors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/errors/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/filesystem/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1009 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/filesystem/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/logs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3596 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/logs/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1081 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4826 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/dataframe_metadata_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2881 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/dict_metadata_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      961 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/id_generator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1967 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/metadata_manager_base.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1192 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1522 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/code_text.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5155 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/dataframetable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5774 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/dictpropertytree.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5013 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/dicttable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1770 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/json_text.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2073 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/list_model.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1052 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/module.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      922 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/roles.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2061 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/series_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1120 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/span.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1033 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/validation.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1161 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/add_signal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/module_opening.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1076 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/rejectable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      867 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1549 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/launcher_config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3395 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/module.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/properties/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      931 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/properties/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8611 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/properties/auto.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2673 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/properties/throttled.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1222 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/script_context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3852 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/script_runner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1551 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/script_template.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1504 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1416 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/autosave.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/email.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/event_registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2383 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/file_dialog.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4378 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/hotkey_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5637 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/link_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2635 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/message_board.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5764 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/module_service.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/object_converter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5020 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/project_updater.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9127 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/task_runner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1919 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/theme_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1978 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/tool_window_service.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/viewmanagers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      798 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/viewmanagers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      939 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/viewmanagers/tool.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/code/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      856 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/code/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9791 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/code/code_edit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8404 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/code/python_syntax.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1033 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/collabsible.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2015 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/group_box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4085 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/group_panel.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1179 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/lines.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1552 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/link.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      967 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39316 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3404 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/colorbar.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2078 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/colormap.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2230 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/font.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1094 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4229 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/legend_control.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9921 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/plot_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6113 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/plot_toolbar_options.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1432 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/size.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      908 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/tool_type.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4203 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/toolbar.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2264 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4520 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/bulk_value_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1374 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/check_box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3962 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/combo_box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2223 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/count_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4130 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/datetime.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7356 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/datetime_range_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/default_text_line_edit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5202 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/delegates.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4180 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/dtype_edit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1861 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/editable_combo_box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1958 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/file_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2916 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/icon.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4895 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/icon_button.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/json_edit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1234 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/labelled.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2148 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/line_edit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1687 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/linkable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1888 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/list_view.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3048 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/main_window.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3190 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/metadata_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2401 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/modulewindow.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1710 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/popout.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1609 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/popup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1102 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/property_tree.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1391 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/shrunk_push_button.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2690 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/steppable_combo_box.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1293 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/styleable.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6439 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/table.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1234 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/text_edit.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1475 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/tool_window.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      857 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      502 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit/_version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4632 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/pyqttoolkit.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       54 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1141 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    68611 2022-10-06 16:06:11.000000 pyqttoolkit-0.8.0.dev0/versioneer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2022-10-06 16:06:52.000000 pyqttoolkit-0.8.0.dev0/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/application/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      849 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/application/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3873 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/application/application.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2417 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/application/garbage_collector.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/colors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3093 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/colors/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1002 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      944 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1228 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/composite.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1108 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/default.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1152 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/environment.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3177 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/multi_json_file.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1162 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/with_signal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1208 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/with_value_changed.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      914 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      915 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/bits.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2024 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/cache.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1158 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/interval.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      982 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/names.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/datetime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      764 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/datetime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2563 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/datetime/datetime.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2225 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/datetime/qdatetime.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/dependencies/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2233 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/dependencies/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/errors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      889 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/errors/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/filesystem/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1009 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/filesystem/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/logs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3596 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/logs/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1081 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4826 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/dataframe_metadata_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2881 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/dict_metadata_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      961 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/id_generator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1967 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/metadata_manager_base.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1192 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1492 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/code_text.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5101 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/dataframetable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5709 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/dictpropertytree.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4983 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/dicttable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1705 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/json_text.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2043 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/list_model.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1052 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/module.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      922 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/roles.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2061 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/series_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1090 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/span.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1033 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/validation.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1161 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/add_signal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      911 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/module_opening.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1046 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/rejectable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      867 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1519 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/launcher_config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3449 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/module.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/properties/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      931 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/properties/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8611 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/properties/auto.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2673 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/properties/throttled.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1222 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/script_context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3852 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/script_runner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1551 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/script_template.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1504 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1416 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/autosave.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/email.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/event_registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2345 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/file_dialog.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4313 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/hotkey_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5630 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/link_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2573 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/message_board.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5942 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/module_service.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1804 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/object_converter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4958 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/project_updater.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9026 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/task_runner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1919 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/theme_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1916 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/tool_window_service.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/viewmanagers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      798 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/viewmanagers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      939 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/viewmanagers/tool.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/code/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      856 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/code/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10075 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/code/code_edit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8404 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/code/python_syntax.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1089 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2392 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/collabsible.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2012 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/group_box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6825 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/group_panel.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1152 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/lines.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1559 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/link.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      967 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    39267 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3404 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/colorbar.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2078 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/colormap.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2230 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/font.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1094 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4208 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/legend_control.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9883 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/plot_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6110 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/plot_toolbar_options.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1432 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/size.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      908 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/tool_type.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4176 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/toolbar.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2263 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4735 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/bulk_value_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1371 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/check_box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3873 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/combo_box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2219 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/count_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4092 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/datetime.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7267 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/datetime_range_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1786 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/default_text_line_edit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5099 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/delegates.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4142 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/dtype_edit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1861 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/editable_combo_box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1955 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/file_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2980 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/icon.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4898 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/icon_button.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      890 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/json_edit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1241 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/labelled.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2118 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/line_edit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1660 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/linkable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1885 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/list_view.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3134 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/main_window.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3187 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/metadata_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2637 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/modulewindow.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1694 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/popout.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1606 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/popup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/property_tree.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1361 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/shrunk_push_button.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2660 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/steppable_combo_box.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1362 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/styleable.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6424 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/table.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1254 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/text_edit.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1448 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/tool_window.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      857 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      502 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit/_version.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4632 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/pyqttoolkit.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       54 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2023-04-14 08:08:30.000000 pyqttoolkit-0.8.0.dev1/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1141 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    68611 2023-04-14 08:08:31.000000 pyqttoolkit-0.8.0.dev1/versioneer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2023-04-14 08:09:15.000000 pyqttoolkit-0.8.0.dev1/PKG-INFO
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/application/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/application/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/application/application.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/application/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,28 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 import sys
 import logging
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QApplication, QWidget, pyqtSignal
-#pyline: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import QApplication, QWidget
 
 from pyqttoolkit.services import MessageBoard, TaskRunner, ToolWindowService, EventRegistry, ObjectConverter
 from pyqttoolkit.dependencies import DependencyContainer
 from .garbage_collector import GarbageCollector
 
 LOGGER = logging.getLogger(__name__)
 
 class Application(QApplication):
     def __init__(self, argv):
         QApplication.__init__(self, argv)
         self._dependency_container = DependencyContainer()
-        self._garbage_collector = GarbageCollector(self)
+        self._garbage_collector = GarbageCollector(self, None)
 
         self._module_service = None
         self._message_board = None
         self._project_manager = None
 
         self._handling_exception = False
 
@@ -50,22 +49,14 @@
 
         if filename:
             self._project_manager.load_project(filename)
         
         self.mainWindowLoaded.emit(self._module_service.openModule('Base'))
         return self.exec_()
     
-    def notify(self, receiver, event):
-        try:
-            return QApplication.notify(self, receiver, event)
-        #pylint: disable=broad-except
-        except Exception as e:
-            self._handle_exception(type(e), e, e.__traceback__)
-            return True
-    
     def _handle_exception(self, ex_type, ex_value, traceback_obj):
         LOGGER.error('Application Exception: %s, %s', ex_type, ex_value)
         if self._handling_exception:
             return
         self._handling_exception = True
         self._perform_exception_handling(ex_type, ex_value, traceback_obj)
         self._handling_exception = False
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/application/garbage_collector.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/application/garbage_collector.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,52 +13,52 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 import gc
 import logging
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QObject, QTimer
-#pyline: enable=no-name-in-module
+from PyQt5.QtCore import QObject, QTimer
 
 from pyqttoolkit.logs import TRACE
 
 LOGGER = logging.getLogger(__name__)
 
 class GarbageCollector(QObject):
     '''
     Disable automatic garbage collection and instead collect manually
     every INTERVAL milliseconds.
 
     This is done to ensure that garbage collection only happens in the GUI
     thread, as otherwise Qt can crash.
     '''
 
-    def __init__(self, parent, interval=10000):
-        QObject.__init__(self, parent)
+    def __init__(self, parent, interval=60000):
+        super().__init__(parent)
         self._interval = interval
-
-        self._timer = QTimer(self)
-        self._timer.timeout.connect(self.check)
-
         self._threshold = gc.get_threshold()
         gc.disable()
-        self._timer.start(self._interval)
 
-    def check(self):
+        if self._interval:
+            self._timer = QTimer(self)
+            self._timer.timeout.connect(self.check)
+            self._timer.start(self._interval)
+        else:
+            self._timer = None
+
+    def check(self, full=False):
         l0, l1, l2 = gc.get_count()
         LOGGER.log(TRACE, 'gc_check called: l0=%d, l1=%d, l2=%d', l0, l1, l2)
-        if l0 > self._threshold[0]:
+        if full or l0 > self._threshold[0]:
             num = gc.collect(0)
             LOGGER.log(TRACE, 'Collecting gen 0, found: %d unreachable', num)
-            if l1 > self._threshold[1]:
+            if full or l1 > self._threshold[1]:
                 num = gc.collect(1)
                 LOGGER.log(TRACE, 'Collecting gen 1, found: %d unreachable', num)
-                if l2 > self._threshold[2]:
+                if full or l2 > self._threshold[2]:
                     num = gc.collect(2)
                     LOGGER.log(TRACE, 'Collecting gen 2, found: %d unreachable', num)
 
     def debug_cycles(self):
         gc.set_debug(gc.DEBUG_SAVEALL)
         gc.collect()
         for obj in gc.garbage:
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/colors/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/base.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/base.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/composite.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/composite.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/default.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/default.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/environment.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/environment.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/multi_json_file.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/multi_json_file.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/with_signal.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/with_value_changed.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import pyqtSignal, QObject
+from PyQt5.QtCore import pyqtSignal, QObject
 
 class WithValueChangedConfiguration(QObject):
-    def __init__(self, inner):
+    def __init__(self, parent, inner):
+        super().__init__(parent)
         self._inner = inner
     
     onValueChanged = pyqtSignal(str, object)
     
     def get_value(self, key):
         return self._inner.get_value(key)
 
     def set_value(self, key, value):
         self._inner.set_value(key, value)
-        self.onValueChanged(key, value)
+        self.onValueChanged.emit(key, value)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/config/with_value_changed.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/config/with_signal.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,22 +10,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import pyqtSignal, QObject
+from PyQt5.QtCore import pyqtSignal, QObject
 
 class WithValueChangedConfiguration(QObject):
     def __init__(self, inner):
-        super().__init__()
         self._inner = inner
     
     onValueChanged = pyqtSignal(str, object)
     
     def get_value(self, key):
         return self._inner.get_value(key)
 
     def set_value(self, key, value):
         self._inner.set_value(key, value)
-        self.onValueChanged.emit(key, value)
+        self.onValueChanged(key, value)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/bits.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/bits.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/cache.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/cache.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/interval.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/interval.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/data/names.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/data/names.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/datetime/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/datetime/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/datetime/datetime.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/datetime/qdatetime.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/datetime/qdatetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from datetime import datetime, timedelta
 from .datetime import round_timedelta
 
 import pandas as pd
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QDateTime, QDate, QTime
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QDateTime, QDate, QTime
 
 def q_datetime_to_datetime(q_datetime: QDateTime):
     if q_datetime is None or not q_datetime.isValid():
         return None
 
     return datetime(
         q_datetime.date().year(), q_datetime.date().month(), q_datetime.date().day(),
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/dependencies/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/dependencies/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,22 @@
 
     def get_instance(self, name):
         return self._instances[name]
 
     def resolve(self, type_, extras=None, none_for_missing=False):
         args = self._get_args(type_)
         all_dependencies = {**self._instances, **(extras or {})}
-        for a in args:
-            if a not in all_dependencies.keys():
-                if none_for_missing:
-                    all_dependencies[a] = None
+        for arg_name, arg in args.items():
+            if arg_name not in all_dependencies:
+                if arg.default != inspect.Parameter.empty:
+                    all_dependencies[arg_name] = arg.default
+                elif none_for_missing:
+                    all_dependencies[arg_name] = None
                 else:
-                    raise MissingDependency(type_, a)
+                    raise MissingDependency(type_, arg_name)
         return type_(**{a: all_dependencies[a] for a in args})
     
     def resolve_for(self, type_for, base_type, extras=None):
         type_to_resolve = self._types[type_for][base_type]
         return self.resolve(type_to_resolve, extras)
     
     @staticmethod
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/errors/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/filesystem/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/logs/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/dataframe_metadata_manager.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/dataframe_metadata_manager.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/dict_metadata_manager.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/dict_metadata_manager.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/id_generator.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/id_generator.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/metadata/metadata_manager_base.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/metadata/metadata_manager_base.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/code_text.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/code_text.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QObject, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QObject, pyqtSignal
 
 from pyqttoolkit.properties import AutoProperty
 
 class CodeTextModel(QObject):
     def __init__(self, parent, validator):
         QObject.__init__(self, parent)
         self.textChanged.connect(self._validate)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/dataframetable.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/dataframetable.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.Qt import QAbstractTableModel, Qt, QVariant, QModelIndex, QItemSelectionModel
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal, QAbstractTableModel, Qt, QVariant, QModelIndex, QItemSelectionModel
 
 class DataFrameTableModel(QAbstractTableModel):
     def __init__(self, parent, data, display_column=None, editable=False, row_headers=False):
         QAbstractTableModel.__init__(self, parent)
         self._data = data.copy()
         self._display_column_index = (
             0 if display_column is None
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/dictpropertytree.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/dictpropertytree.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from enum import Enum
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import Qt, QAbstractItemModel, pyqtSignal, QModelIndex, QVariant
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import Qt, QAbstractItemModel, pyqtSignal, QModelIndex, QVariant
 
 class DictPropertyTreeModel(QAbstractItemModel):
     def __init__(self, parent, data):
         QAbstractItemModel.__init__(self, parent)
         self._data = data
         self._nodes = []
         self._indexes = {}
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/dicttable.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/dicttable.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import Qt, QAbstractTableModel, pyqtSignal, QModelIndex
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import Qt, QAbstractTableModel, pyqtSignal, QModelIndex
 
 from pyqttoolkit.models.roles import DataRole
 
 class DictTableModel(QAbstractTableModel):
     def __init__(self, parent, value):
         if not isinstance(value, dict):
             raise TypeError('value must be dict')
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/json_text.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/json_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from json import loads, dumps, JSONDecodeError
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QObject, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QObject, pyqtSignal
 
 from pyqttoolkit.properties import AutoProperty
 
 class JsonTextModel(QObject):
     def __init__(self, parent):
         QObject.__init__(self, parent)
         self.textChanged.connect(self._set_data)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/list_model.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/list_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import Qt, QAbstractListModel, QStringListModel
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import Qt, QAbstractListModel, QStringListModel
 
 from pyqttoolkit.models.roles import DataRole
 
 class ListModel(QAbstractListModel):
     def __init__(self, parent, items, display_name_map=None):
         QAbstractListModel.__init__(self, parent)
         self._items = items
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/module.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/module.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/roles.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/roles.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/series_data.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/series_data.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/span.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/models/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,23 +10,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QObject
+from PyQt5.QtCore import QObject
 #pylint: enable=no-name-in-module
 
-class SpanModel(QObject):
-    def __init__(self, parent, left, right):
+class ValidationModel(QObject):
+    def __init__(self, parent, error):
         QObject.__init__(self, parent)
-        self._left = left
-        self._right = right
-    
-    @property
-    def left(self):
-        return self._left
+        self._error = error
 
     @property
-    def right(self):
-        return self._right
+    def error(self):
+        return self._error
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/models/validation.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/rejectable.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from PyQt5.QtCore import QObject
-#pylint: enable=no-name-in-module
-
-class ValidationModel(QObject):
-    def __init__(self, parent, error):
-        QObject.__init__(self, parent)
-        self._error = error
 
+class RejectableEvent(QObject):
+    def __init__(self):
+        QObject.__init__(self)
+        self._accepted = True
+    
     @property
-    def error(self):
-        return self._error
+    def accepted(self):
+        return self._accepted
+    
+    def reject(self):
+        self._accepted = False
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/add_signal.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/add_signal.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/module_opening.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/events/module_opening.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/events/rejectable.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/styleable.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QObject
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QStyleOption, QStyle
+from PyQt5.QtGui import QPainter
+
+opt = QStyleOption()
+
+def make_styleable(cls):
+    global opt
+    class Styleable(cls):
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self._painter = None
+        
+        def paintEvent(self, event):
+            self._painter = QPainter(self)
+            opt.initFrom(self)
+            self.style().drawPrimitive(QStyle.PE_Widget, opt, self._painter, self)
+            self._painter.end()
+            return super().paintEvent(event)
+
+    return Styleable
 
-class RejectableEvent(QObject):
-    def __init__(self):
-        QObject.__init__(self)
-        self._accepted = True
-    
-    @property
-    def accepted(self):
-        return self._accepted
-    
-    def reject(self):
-        self._accepted = False
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/launcher_config.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/launcher_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QObject, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QObject, pyqtSignal
 
 from pyqttoolkit.properties import AutoProperty
 
 class LauncherConfig(QObject):
     def __init__(self):
         QObject.__init__(self)
         self.enabled = False
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/modules/module.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/modules/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QObject, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QObject, pyqtSignal
 
 from .events import ModuleOpeningEvent
 
 class ModuleBase(QObject):
     def __init__(self, id_, launcher_config=None):
         QObject.__init__(self)
         self._id = id_
         self._launcher_config = launcher_config
+        if self._launcher_config:
+            self._launcher_config.setParent(self)
     
     opening = pyqtSignal(ModuleOpeningEvent)
     opened = pyqtSignal()
 
     @property
     def id(self):
         return self._id
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/properties/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/properties/auto.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/properties/auto.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/properties/throttled.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/properties/throttled.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/script_context.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/script_context.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/script_runner.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/script_runner.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/scripting/script_template.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/scripting/script_template.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/autosave.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/autosave.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/email.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/email.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/event_registry.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/event_registry.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/file_dialog.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/file_dialog.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from os import path
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QStandardPaths, QFileDialog
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QStandardPaths
+from PyQt5.QtWidgets import QFileDialog
 
 class FileDialogService:
     def __init__(self, project_manager, application_configuration):
         self._project_manager = project_manager
         self._application_configuration = application_configuration
     
     def get_save_filename(self, parent, filter_, default_name=None):
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/hotkey_manager.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/hotkey_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from enum import Enum
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import Qt
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import Qt
 
 class HotkeyEvents(Enum):
     next_instance_y = 0
     previous_instance_y = 1
     next_instance_x = 2
     previous_instance_x = 3
     next_t = 4
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/link_manager.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/link_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QPalette, QColor, Qt, QObject
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import Qt, QObject
+from PyQt5.QtGui import QColor, QPalette
 
 from pyqttoolkit.views import ModuleWindow
 from . import MessageType
 from ..colors import rgb_to_hex
 
 class IncompatibleWidgets(Exception):
     def __init__(self):
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/message_board.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/message_board.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,16 @@
 class MessageResponse(IntEnum):
     ok = 1
     cancel = 2
     save = 4
     discard = 8
     ignore = 16
 
-class MessageArgs(QObject):
-    def __init__(self, parent, message_type, message, checkbox_message, response_type):
-        QObject.__init__(self, parent)
+class MessageArgs:
+    def __init__(self, message_type, message, checkbox_message, response_type):
         self._message_type = message_type
         self._message = message
         self._checkbox_message = checkbox_message
         self._response_type = response_type
         self._response = None
         self._checkbox_value = None
     
@@ -77,13 +76,13 @@
         self._checkbox_value = value
 
 class MessageBoard(QObject):
     def __init__(self, parent):
         QObject.__init__(self, parent)
     
     def post(self, message_type, message, response_type=MessageResponse.ok, checkbox_message=None):
-        self.message = MessageArgs(self, message_type, message, checkbox_message, response_type)
+        self.message = MessageArgs(message_type, message, checkbox_message, response_type)
         return self.message
 
     messageChanged = pyqtSignal(MessageArgs)
 
     message = AutoProperty(MessageArgs)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/module_service.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/module_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,46 +14,46 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 """:mod:`module_service`
 The module service, creates and manages qt widget modules
 """
 from weakref import ref
-from functools import partial
+import weakref
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QObject, pyqtSlot
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QObject, pyqtSlot, QTimer, Qt
 
 from pyqttoolkit.modules import Module, CommandModule
 from pyqttoolkit.views import ModuleWindow
 from pyqttoolkit.modules.events import ModuleOpeningEvent
 
 class ModuleService(QObject):
     """class::ModuleService
     This class creates and displays modules (views, models and view managers)
     """
 
-    def __init__(self, dependency_container, theme_manager, project_updater, project_manager):
-        QObject.__init__(self, None)
+    def __init__(self, dependency_container, theme_manager, project_updater, project_manager, garbage_collector):
+        super().__init__(None)
         self._theme_manager = theme_manager
         self._dependency_container = dependency_container
         self._view_manager_refs = {}
         self._window_refs = {}
         self._model_refs = {}
         self._view_managers = {}
         self._windows = {}
         self._models = {}
         self._registered_modules = {}
         self._project_updater = project_updater
         self._project_manager = project_manager
+        self._garbage_collector = garbage_collector
     
     def register(self, module):
         if module.id in self._registered_modules:
             raise ValueError('module')
+        module.setParent(self)
         self._registered_modules[module.id] = module
         if module.launcher_config and self._project_updater is not None and self._project_manager is not None:
             self._project_updater.projectUpdated.connect(self._project_update_handler(module))
         
     def _project_update_handler(self, module):
         def _handler():
             module.handle_project_updated(self._project_manager.project)
@@ -71,19 +71,20 @@
             elif isinstance(module, Module):
                 result = self._create_module(name).show()
             else:
                 raise ValueError('Invalid module type')
             self._module_opened(name)
             return result
         return None
-    
+
     def closeModules(self):
         for id_, window in list(self._windows.items()):
-            if id_ != 'root':
-                window.close()
+            if id_ != 'root' and not window.forceClose():
+                return False
+        return True
             
     def modules(self):
         return self._registered_modules
     
     def _init_module(self, id_):
         module = self._registered_modules[id_]
         opening_event = ModuleOpeningEvent()
@@ -99,40 +100,48 @@
         if self._registered_modules[id_].is_root:
             return self._create_root_module(id_)
         else:
             return self._create_sub_module(id_)
     
     def _create_root_module(self, id_):
         window = self._dependency_container.resolve(self._registered_modules[id_].view_type)
-        model = self._dependency_container.resolve(self._registered_modules[id_].model_type, {'parent': window})
+        model = self._dependency_container.resolve(self._registered_modules[id_].model_type)
+        model.setParent(window)
         view_manager = self._registered_modules[id_].view_manager_type(window, model)
         self._windows['root'] = window
         self._models['root'] = model
         self._view_managers['root'] = view_manager
         return window
 
     def _create_sub_module(self, id_):
-        window = ModuleWindow(self._theme_manager, self._registered_modules[id_].title)
+        singleton = self._registered_modules[id_].singleton
+        window = ModuleWindow(self._theme_manager, self._registered_modules[id_].title, singleton)
+        window.setAttribute(Qt.WA_DeleteOnClose)
         model = self._dependency_container.resolve(
             self._registered_modules[id_].model_type,
             {'parent': window, 'module_id': id_}
         )
         view = self._dependency_container.resolve(self._registered_modules[id_].view_type, {'parent': window})
-        if hasattr(model, 'handle_view_closed'):
-            garbage_collector = self._dependency_container.get_instance('garbage_collector')
-            view.destroyed.connect(partial(model.handle_view_closed, garbage_collector))
         window.setModuleView(view)
         view_manager = self._registered_modules[id_].view_manager_type(view, model)
 
         self._view_managers[window.moduleId] = model
         self._windows[window.moduleId] = window
         self._models[window.moduleId] = model
         self._view_manager_refs[window.moduleId] = ref(view_manager)
         self._window_refs[window.moduleId] = ref(window)
         self._model_refs[window.moduleId] = ref(model)
         window.closing.connect(self._remove_module)
         return window
-
+    
     def _remove_module(self, module_id):
         self._view_managers.pop(module_id)
-        self._windows.pop(module_id).setParent(None)
-        self._models.pop(module_id).setParent(None)
+        window = self._windows.pop(module_id)
+        self._models.pop(module_id)
+        window.deleteLater()
+        window.destroyed.connect(self._schedule_gc)
+    
+    def _schedule_gc(self):
+        QTimer.singleShot(0, self._gc)
+    
+    def _gc(self):
+        self._garbage_collector.check(full=True)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/object_converter.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/object_converter.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/project_updater.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/project_updater.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 """:mod:`project_updater`
 Defines the ProjectUpdater class, which enables the project to be updated
 """
 import inspect
 from threading import Lock
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QObject, pyqtSignal, QTimer, QCoreApplication, QEvent, QSemaphore, QThread
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QObject, pyqtSignal, QEvent, QSemaphore, QThread
+from PyQt5.QtWidgets import QApplication
 
 def _check_attribute(name, fields, project):
     if not name in fields:
         raise ValueError(f'Could not access property {name} of project {type(project)}')
 
 
 class ProjectProxy:
@@ -78,15 +77,15 @@
 
 class UpdateEvent(QEvent):
     def __init__(self, updater):
         super().__init__(QEvent.User)
         self._updater = updater
         self._result = None
         self._semaphore = QSemaphore(1)
-        if QCoreApplication.instance().thread() != QThread.currentThread():
+        if QApplication.instance().thread() != QThread.currentThread():
             self._semaphore.acquire()
     
     def exec(self):
         try:
             self._result = self._updater(None)
         finally:
             self._semaphore.release()
@@ -127,18 +126,18 @@
         result = update_function(None)
         if updated_properties:
             for prop in updated_properties:
                 self._on_project_updated(prop)
         else:
             self._on_project_updated(None)
         if on_completed:
-            QCoreApplication.postEvent(self, UpdateCompleteEvent(on_completed, result))
+            QApplication.postEvent(self, UpdateCompleteEvent(on_completed, result))
     
     def _on_project_updated(self, prop):
-        QCoreApplication.postEvent(self, PropertyUpdatedEvent(prop))
+        QApplication.postEvent(self, PropertyUpdatedEvent(prop))
     
     def event(self, event):
         if isinstance(event, PropertyUpdatedEvent):
             self.projectUpdated.emit(event.prop)
             return True
         if isinstance(event, UpdateCompleteEvent):
             event.exec()
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/task_runner.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/task_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,16 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 """:mod:`task_runner`
 Defines the task runner
 """
 import logging
 import inspect
 
-#pylint: disable=no-name-in-module
-from PyQt5.QtCore import QObject, pyqtSignal, pyqtSlot
-from PyQt5.Qt import QThreadPool, QRunnable, QThread, QSemaphore, QEvent, QCoreApplication
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QObject, pyqtSignal, QEvent
+from PyQt5.QtWidgets import QApplication
 
 from concurrent.futures import ThreadPoolExecutor
 
 from ..properties import AutoProperty
 
 LOGGER = logging.getLogger(__name__)
 
@@ -85,25 +83,25 @@
         self._on_completed = on_completed
         self._on_cancelled = on_cancelled
         self._on_error = on_error
         self._error_description = error_description
     
     def run(self):
         if self._busy_args:
-            QCoreApplication.postEvent(self._task_runner, BusyEvent(self._busy_args))
+            QApplication.postEvent(self._task_runner, BusyEvent(self._busy_args))
         try:
             result = self._f(*self._args.args, **self._args.kwargs)
         except TaskCancelled:
-            QCoreApplication.postEvent(self._task_runner, CancelledEvent(self._on_cancelled))
+            QApplication.postEvent(self._task_runner, CancelledEvent(self._on_cancelled))
         #pylint: disable=broad-except
         except Exception as e:
-            QCoreApplication.postEvent(self._task_runner, ErrorEvent(e, self._on_error, self._error_description))
+            QApplication.postEvent(self._task_runner, ErrorEvent(e, self._on_error, self._error_description))
         #pylint: enable=broad-except
         else:
-            QCoreApplication.postEvent(self._task_runner, ResultEvent(result, self._on_completed))
+            QApplication.postEvent(self._task_runner, ResultEvent(result, self._on_completed))
 
 class ProgressUpdatedEvent(QEvent):
     def __init__(self, progress, message):
         super().__init__(QEvent.User)
         self._progress = progress
         self._message = message
     
@@ -174,15 +172,15 @@
 class TaskRunner(QObject):
     """class::TaskRunner
     Runs tasks on a background thread
     """
     def __init__(self, parent):
         QObject.__init__(self, parent)
         self._is_cancelled = False
-        self._executor = ThreadPoolExecutor(max_workers=1)
+        self._executor = ThreadPoolExecutor(max_workers=1, thread_name_prefix='TaskRunner_Thread')
 
     def run_task(self, task_function, task_args=None, on_completed=None, on_cancelled=None, on_error=None, description=None, error_description=None, show_progress=True, cancellable=False, **kwargs):
         """function::runTask(self, task_function, task_args, on_completed, on_error)
         :param task_function: The function to execute
         :param task_args: The arguments to pass to the function
         :param on_completed: The function to execute when the task completes
         :param on_error: The function to execute when the task errors
@@ -207,15 +205,15 @@
             busy_args=busy_args, on_completed=on_completed,
             on_cancelled=on_cancelled, on_error=on_error,
             error_description=error_description
         )
         self._executor.submit(worker.run)
     
     def update_progress(self, percent, message):
-        QCoreApplication.postEvent(self, ProgressUpdatedEvent(float(percent), message))
+        QApplication.postEvent(self, ProgressUpdatedEvent(float(percent), message))
     
     def event(self, event):
         if isinstance(event, ProgressUpdatedEvent):
             if self.busy is not None:
                 self.busy.updateProgress(float(event.progress), event.message)
             return True
         elif isinstance(event, BusyEvent):
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/theme_manager.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/theme_manager.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/services/tool_window_service.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/services/tool_window_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QWidget
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget
 
 from pyqttoolkit.views import ToolWindow
 from pyqttoolkit.viewmanagers import ToolViewManager
 
 class ToolWindowService:
     def __init__(self, dependency_contianer):
         self._dependency_container = dependency_contianer
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/viewmanagers/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/viewmanagers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/viewmanagers/tool.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/viewmanagers/tool.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/code/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/code/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/code/code_edit.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/code/code_edit.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,22 +10,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import (
-    Qt, QWidget, QGridLayout, QPlainTextEdit, QColor,
-    QPalette, pyqtSignal, QFont, QTextOption, QSplitter,
-    QTextBrowser, QLabel, QSize, QRect, QPainter,
-    QFontMetrics, QPointF, QTextEdit, QTextFormat,
-    QEvent
+import weakref
+from PyQt5.QtCore import Qt, pyqtSignal, QSize, QRect
+from PyQt5.QtWidgets import (
+    QWidget, QGridLayout, QPlainTextEdit,
+    QSplitter, QTextBrowser,
+    QLabel, QTextEdit
+)
+from PyQt5.QtGui import (
+    QPainter, QColor, QPalette, QFont,
+    QTextOption, QFontMetrics, QTextFormat
 )
-#pylint: enable=no-name-in-module
 
 from .python_syntax import PythonHighlighter
 
 class LineNumberArea(QWidget):
     def __init__(self, editor):
         QWidget.__init__(self, editor)
         self._editor = editor
@@ -151,15 +154,15 @@
         self._output_pane = QTextBrowser(self)
         self._output_pane.document().setDefaultFont(QFont('Courier', pointSize=7))
         self._output_pane.setWordWrapMode(QTextOption.NoWrap)
 
         self._output_pane_container = QWidget(self)
         self._output_pane_layout = QGridLayout(self._output_pane_container)
         self._output_pane_layout.setContentsMargins(0, 16, 0, 0)
-        self._output_pane_layout.addWidget(QLabel(self.tr('Script Output')), 0, 0)
+        self._output_pane_layout.addWidget(QLabel(self.tr('Script Output'), self), 0, 0)
         self._output_pane_layout.addWidget(self._output_pane)
 
         self._splitter = QSplitter(Qt.Vertical, self)
 
         self._splitter.addWidget(self._text_edit)
         self._splitter.addWidget(self._output_pane_container)
         self._splitter.setStretchFactor(0, 3)
@@ -196,24 +199,30 @@
             self._output_pane.setVisible(True)
         else:
             self._output_pane_container.setVisible(False)
         self.editComplete.connect(self._handle_text_changed(model))
         model.validationMessageChanged.connect(self._handle_validation_message)
     
     def _set_text(self, widget, scroll_to_end=False):
+        widget_ref = weakref.ref(widget)
         def _(text):
-            if widget.toPlainText() != text:
-                widget.setPlainText(text)
-                if scroll_to_end:
-                    widget.verticalScrollBar().setSliderPosition(widget.verticalScrollBar().maximum())
+            widget_inst = widget_ref()
+            if widget_inst:
+                if widget_inst.toPlainText() != text:
+                    widget_inst.setPlainText(text)
+                    if scroll_to_end:
+                        widget_inst.verticalScrollBar().setSliderPosition(widget_inst.verticalScrollBar().maximum())
         return _
 
     def _handle_text_changed(self, model):
+        model_ref = weakref.ref(model)
         def _setter(value):
-            model.text = value
+            model_inst = model_ref()
+            if model_inst:
+                model_inst.text = value
         return _setter
 
     def _handle_validation_message(self, message):
         if message:
             palette = self.palette()
             invalid_color = QColor(Qt.red)
             invalid_color.setAlphaF(0.2)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/code/python_syntax.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/code/python_syntax.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from .lines import HLine, VLine
-from .group_panel import GroupPanelLayout, VGroupPanelLayout, HGroupPanelLayout
+from .group_panel import GroupPanelLayout, VGroupPanelLayout, HGroupPanelLayout, GroupPanelWidget, HGroupPanelWidget, VGroupPanelWidget
 from .group_box import wrap_in_group_box, wrap_many_in_group_box
 from .collabsible import HCollapsibleLayout, VCollapsibleLayout
 from .link import LinkWidget
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/collabsible.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/collabsible.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QBoxLayout, QToolButton, Qt
-#pylint: enable=no-name-in-module
-
-from .lines import HLine, VLine
+from PyQt5.QtWidgets import QBoxLayout, QToolButton
+from PyQt5.QtCore import Qt
 
 class CollapsibleLayout(QBoxLayout):
     def __init__(self, parent, direction):
         QBoxLayout.__init__(self, direction, parent)
         self._index = 0
         self._widgets = []
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/group_box.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/group_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QGroupBox, QGridLayout, Qt, QVBoxLayout
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QGroupBox, QGridLayout, QVBoxLayout
+from PyQt5.QtCore import Qt
 
 class LinkGroupBox(QGroupBox):
     def __init__(self, name, parent, linkable_widget):
         QGroupBox.__init__(self, name, parent)
         self._linkable_widget = linkable_widget
         if hasattr(self._linkable_widget, 'setLinkDisplay'):
             self._linkable_widget.setLinkDisplay(self)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/lines.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/lines.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QFrame
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QFrame
 
 class HLine(QFrame):
     def __init__(self, parent):
         QFrame.__init__(self, parent)
         self.setFrameShape(QFrame.HLine)
         self.setFrameShadow(QFrame.Sunken)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/layout/link.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/layout/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QWidget
+from PyQt5.QtWidgets import QWidget
 
 class LinkWidget(QWidget):
     def __init__(self, parent, linkable_widget):
         super().__init__(parent)
         self._linkable_widget = linkable_widget
         if hasattr(self._linkable_widget, 'setLinkDisplay'):
             self._linkable_widget.setLinkDisplay(self)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/base.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from io import BytesIO
 import numpy as np
 from datetime import datetime
-from functools import partial
 
-#pylint: disable=no-name-in-module
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.Qt import QVBoxLayout, QWidget, QSize, QTimer, QMenu, QAction, QApplication, QImage, QKeySequence
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal, QSize, QTimer
+from PyQt5.QtWidgets import QVBoxLayout, QWidget, QMenu, QAction, QApplication
+from PyQt5.QtGui import QKeySequence, QImage
 
 import matplotlib
 from matplotlib.legend import DraggableLegend
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.figure import Figure
 from matplotlib.widgets import RectangleSelector, SpanSelector
 from mpl_toolkits.axes_grid1 import Size, Divider
@@ -76,23 +74,23 @@
             self.extents = x, x, y, y
         RectangleSelector._press(self, event)
 
 class MatPlotLibBase(QWidget):
     def __init__(self,
         parent, file_dialog_service,
         h_margin=(0.8, 0.1), v_margin=(0.5, 0.15),
-        h_axes=[Size.Scaled(1.0)], v_axes=[Size.Scaled(1.0)],
+        h_axes=None, v_axes=None,
         nx_default=1, ny_default=1
         ):
         QWidget.__init__(self, parent)
         self._file_dialog_service = file_dialog_service
         self._figure = Figure()
         self._canvas = FigureCanvas(self._figure)
-        h = [Size.Fixed(h_margin[0]), *h_axes, Size.Fixed(h_margin[1])]
-        v = [Size.Fixed(v_margin[0]), *v_axes, Size.Fixed(v_margin[1])]
+        h = [Size.Fixed(h_margin[0]), *(h_axes or [Size.Scaled(1.0)]), Size.Fixed(h_margin[1])]
+        v = [Size.Fixed(v_margin[0]), *(v_axes or [Size.Scaled(1.0)]), Size.Fixed(v_margin[1])]
         self._divider = Divider(self._figure, (0.0, 0.0, 1.0, 1.0), h, v, aspect=False)
         self._axes = Axes(self._figure, self._divider.get_position())
         self._axes.set_axes_locator(self._divider.new_locator(nx=nx_default, ny=ny_default))
         self._axes.set_zorder(2)
         self._axes.patch.set_visible(False)
         for spine in ['top', 'right']:
             self._axes.spines[spine].set_visible(False)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/colorbar.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/colorbar.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/colormap.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/colormap.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/matplotlib/font.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/matplotlib/font.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/legend_control.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/legend_control.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QWidget, pyqtSignal, QGridLayout, QLabel, QColor, QPalette
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget, QGridLayout, QLabel
+from PyQt5.QtCore import pyqtSignal
 
 from pyqttoolkit.properties import AutoProperty, bind
 from pyqttoolkit.views import BindableCheckBox, BindableLineEdit
 from pyqttoolkit.colors import format_color, ColorFormat
 
 class LegendControlView(QWidget):
     def __init__(self, parent):
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/plot_options.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/plot_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 import numpy as np
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QWidget, pyqtSignal, QGridLayout, QLabel
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget, QGridLayout, QLabel
+from PyQt5.QtCore import pyqtSignal
 
 from pyqttoolkit.properties import AutoProperty, bind
 from pyqttoolkit.views import BindableCheckBox, AutoFloatLineEdit
 
 class PlotOptionsView(QWidget):
     def __init__(self, parent, grid_lines=True, x_limits=True, y_limits=True, secondary_x_limits=False, secondary_y_limits=False):
         QWidget.__init__(self, parent)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/plot_toolbar_options.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/plot_toolbar_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QWidget, QGridLayout, Qt, QSizePolicy, QVBoxLayout
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget, QGridLayout, QSizePolicy, QVBoxLayout
+from PyQt5.QtCore import Qt
 
 from pyqttoolkit.views import PopoutWidget, make_styleable
 from pyqttoolkit.colors import interpolate_rgb, format_color, ColorFormat
 from pyqttoolkit.views.layout import HLine
 
 from .tool_type import ToolType
 from .toolbar import PlotToolbarWidget
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/size.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/size.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/tool_type.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/tool_type.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/plot/toolbar.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/plot/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.Qt import QWidget, Qt, QSize
+from PyQt5.QtCore import pyqtSignal, Qt, QSize
+from PyQt5.QtWidgets import QWidget
 from PyQt5.QtWidgets import QVBoxLayout
-#pylint: enable=no-name-in-module
 
 from pyqttoolkit.views import IconButton, make_styleable
 from .tool_type import ToolType
 
 class PlotToolbarWidget(QWidget):
     tool_icons = {
         ToolType.zoom: 'zoom.svg',
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 from .datetime_range_selector import DatetimeRangeSelectorWidget
 from .count_selector import CountSelectorWidget
 from .list_view import ListView
 from .styleable import make_styleable
 from .popout import PopoutWidget
 from .popup import Popup
 from .delegates import ComboBoxItemDelegate, DateTimeItemDelegate, BulkValueSelectorItemDelegate
-from .labelled import make_labelled
+from .labelled import make_labelled
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/bulk_value_selector.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/bulk_value_selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,38 +10,46 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.QtCore import pyqtSignal, QItemSelectionModel
-from PyQt5.Qt import QWidget, QGridLayout, QAbstractItemModel, QStringListModel, Qt
-#pylint: enable=no-name-in-module
+import weakref
+from PyQt5.QtCore import pyqtSignal, QItemSelectionModel, QAbstractItemModel, QStringListModel, Qt
+from PyQt5.QtWidgets import QWidget, QGridLayout
 
 from pyqttoolkit.properties import auto_property
 from pyqttoolkit.models.roles import DataRole
 from .list_view import ListView
 
 class BulkValueSelectorWidget(QWidget):
     def __init__(self, parent):
         QWidget.__init__(self, parent)
         self._value_selector = ListView(self)
         self._value_selector.setSelectionMode(ListView.ExtendedSelection)
-        self._value_selector.selectedItemsChanged.connect(lambda: self.selectedValuesChanged.emit(self.selectedValues))
+        self._value_selector.selectedItemsChanged.connect(self._handle_selected_items_changed())
 
         self._layout = QGridLayout(self)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self._layout.addWidget(self._value_selector)
         self.setLayout(self._layout)
 
     valuesChanged = pyqtSignal(QAbstractItemModel)
     selectedValuesChanged = pyqtSignal(list)
     dataCommitted = pyqtSignal(list)
 
+    def _handle_selected_items_changed(self):
+        widget_ref = weakref.ref(self)
+        def _():
+            widget = widget_ref()
+            if widget:
+                widget.selectedValuesChanged.emit(widget.selectedValues)
+        return _
+
     @auto_property(QAbstractItemModel)
     def values(self):
         return self._value_selector.model()
     
     @values.setter
     def values(self, value):
         self._value_selector.setModel(value)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/check_box.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/check_box.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QCheckBox, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import QCheckBox
 
 from pyqttoolkit.properties import AutoProperty
 from pyqttoolkit.views.styleable import make_styleable
 
 class BindableCheckBox(QCheckBox):
     def __init__(self, label, parent):
         QCheckBox.__init__(self, label, parent)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/combo_box.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/combo_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,16 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 """:mod:`combo_box`
 Defines the ComboBox class
 """
 from enum import Enum
 
-#pylint: disable=no-name-in-module
 from PyQt5.QtWidgets import QComboBox
-from PyQt5.Qt import pyqtSignal
-from PyQt5.QtCore import Qt
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import Qt, pyqtSignal
 
 from pyqttoolkit.properties import AutoProperty
 from pyqttoolkit.models.roles import DataRole
 from pyqttoolkit.views.styleable import make_styleable
 
 class ComboBox(QComboBox):
     def __init__(self, parent, padding=20):
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/count_selector.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/count_selector.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from PyQt5.QtCore import pyqtSignal, Qt
-from PyQt5.Qt import QWidget, QHBoxLayout, QScrollBar, QLineEdit, QIntValidator
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget, QHBoxLayout, QScrollBar, QLineEdit
+from PyQt5.QtGui import QIntValidator
 
 class CountSelectorWidget(QWidget):
     def __init__(self, parent, minimum, maximum, initial=0):
         QWidget.__init__(self, parent)
 
         self._slider = QScrollBar(Qt.Horizontal, self)
         self._slider.setMinimum(minimum)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/datetime.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/datetime.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 """:mod:`datetime`
 Defines the DateTimeEdit class
 """
 from enum import Enum
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QDateTimeEdit, QDateTime, QTime, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QDateTime, QTime, pyqtSignal
+from PyQt5.QtWidgets import QDateTimeEdit
 
 from pyqttoolkit.properties import auto_property, AutoProperty
 
 from .styleable import make_styleable
 
 class DateTimeEdit(QDateTimeEdit):
     class Limit(Enum):
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/datetime_range_selector.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/datetime_range_selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,16 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 """:mod:`datetime_range_selector`
 Defines the DatetimeRangeSelectorWidget
 """
-#pylint: disable=no-name-in-module
-from PyQt5.QtCore import pyqtSignal
-from PyQt5.Qt import QDateTime, QSize, QMenu, QAction
-from PyQt5.QtWidgets import QGridLayout, QSizePolicy
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal, QDateTime, QSize
+from PyQt5.QtWidgets import QGridLayout, QSizePolicy, QMenu, QAction
 
 from datetime import timedelta
 
 from pyqttoolkit.properties import auto_property, bind, unbind
 from pyqttoolkit.datetime.qdatetime import step_qdatetime
 from pyqttoolkit.services.link_manager import IncompatibleWidgets
 from .linkable import LinkableWidget
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/default_text_line_edit.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/default_text_line_edit.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/delegates.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/delegates.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,19 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from enum import Enum
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QStyledItemDelegate, QTableView, QTreeView, QStringListModel, QStyle, QStyleOptionViewItem, QWidget, QHBoxLayout, QPushButton, QPoint, Qt, QDateTime
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QStringListModel, Qt, QDateTime
+from PyQt5.QtWidgets import QStyledItemDelegate, QTableView, QWidget, QHBoxLayout, QPushButton
 
 from pyqttoolkit.models.roles import DataRole, EditorAuxDataRole
-from pyqttoolkit.views import BindableComboBox, DateTimeEdit, BulkValueSelectorWidget, Popup, make_styleable
+from pyqttoolkit.views import BindableComboBox, DateTimeEdit, BulkValueSelectorWidget, Popup
 
 class ComboBoxItemDelegate(QStyledItemDelegate):
     def __init__(self, parent):
         super().__init__(parent)
     
     def setComboBoxModel(self, model):
         self._combo_box_model = model
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/dtype_edit.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/dtype_edit.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 from math import isnan, isfinite
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QDoubleValidator, pyqtSignal, Qt
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal, Qt
+from PyQt5.QtGui import QDoubleValidator
 
 from pyqttoolkit.properties import AutoProperty
 from pyqttoolkit.views import LineEdit
 
 def _type_editor(dtype, default_value):
     class _TypeEdit(LineEdit):
         def __init__(self, parent):
             LineEdit.__init__(self, parent)
-            self.setValidator(QDoubleValidator())
+            self.setValidator(QDoubleValidator(self))
             self.editComplete.connect(self._set_value)
             self.valueChanged.connect(self._set_text)
         
         valueChanged = pyqtSignal(dtype)
 
         value = AutoProperty(dtype)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/editable_combo_box.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/editable_combo_box.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/file_selector.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/file_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QWidget, QLineEdit, QHBoxLayout, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget, QLineEdit, QHBoxLayout
+from PyQt5.QtCore import pyqtSignal
 
 from pyqttoolkit.properties import auto_property
 
 from . import ShrunkPushButton
 
 class FileSelector(QWidget):
     def __init__(self, parent, filter_, file_dialog_service):
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/icon.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/icon.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QFile, QHBoxLayout, QSize, Qt, QWidget
+from PyQt5.QtWidgets import QHBoxLayout, QWidget
+from PyQt5.QtCore import QFile, QSize, Qt
 from PyQt5.QtSvg import QSvgWidget
 from PyQt5.QtXml import QDomDocument
-#pylint: enable=no-name-in-module
 
 from pyqttoolkit.colors import format_color, ColorFormat
 from pyqttoolkit.services.theme_manager import ThemeManager
 from .styleable import make_styleable
 
 class Icon(QWidget):
     def __init__(self, parent, icon, size=None, padding=None, color=None):
@@ -29,38 +29,39 @@
         padding = padding or 0
         self._theme_manager = ThemeManager.get(self)
         
         self._color = format_color(color or self._theme_manager.get_color('button_foreground'), ColorFormat.rgb_string_256)
 
         self._svgdoc = QDomDocument()
         self._icon_widget = QSvgWidget(self)
-
         self.loadIcon(icon)
 
         if size:
             self._icon_widget.setFixedSize(QSize(size.width() - 2 * padding, size.height() - 2 * padding))
 
         self._layout = QHBoxLayout(self)
         self._layout.setContentsMargins(padding, padding, padding, padding)
         self._layout.addWidget(self._icon_widget, Qt.AlignCenter)
     
     def loadIcon(self, icon):
-        file = QFile(f'icons:{icon}')
-        file.open(QFile.ReadOnly)
-        self._svgdoc.setContent(file.readAll())
-        self._svgdoc.documentElement().setAttribute('fill', self._color)
-        file.close()
-        self._icon_widget.load(self._svgdoc.toByteArray())
+        file = QFile(f'icons:{icon}', self)
+        try:
+            file.open(QFile.ReadOnly)
+            self._svgdoc.setContent(file.readAll())
+            self._svgdoc.documentElement().setAttribute('fill', self._color)
+            self._icon_widget.load(self._svgdoc.toByteArray())
+        finally:
+            file.close()
 
     def setEnabled(self, enabled):
         QWidget.setEnabled(self, enabled)
         self._svgdoc.documentElement().setAttribute('fill', self._color)
         self._svgdoc.documentElement().setAttribute('fill-opacity', '1' if self.isEnabled() else '0.4')
         self._icon_widget.load(self._svgdoc.toByteArray())
     
     def setColor(self, color=None):
-        color = format_color(color or self._theme_manager.get_color('button_foreground'), ColorFormat.rgb_string_256) or self._color
-        self._svgdoc.documentElement().setAttribute('fill', color)
+        self._color = format_color(color or self._theme_manager.get_color('button_foreground'), ColorFormat.rgb_string_256) or self._color
+        self._svgdoc.documentElement().setAttribute('fill', self._color)
         self._svgdoc.documentElement().setAttribute('fill-opacity', '1' if self.isEnabled() else '0.4')
         self._icon_widget.load(self._svgdoc.toByteArray())
 
 Icon = make_styleable(Icon)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/icon_button.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/icon_button.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QPushButton, QHBoxLayout, QSizePolicy, QPropertyAnimation, pyqtProperty, QEasingCurve, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QPropertyAnimation, QEasingCurve, pyqtSignal, pyqtProperty
+from PyQt5.QtWidgets import QPushButton, QHBoxLayout, QSizePolicy
 
 from pyqttoolkit.properties import AutoProperty
 from pyqttoolkit.colors import format_color, ColorFormat
 from pyqttoolkit.services.theme_manager import ThemeManager
 from .icon import Icon
 
 class IconButton(QPushButton):
@@ -36,15 +36,15 @@
         self._layout.setContentsMargins(0, 0, 0, 0)
         self.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
         self._size = size
         self.setFlat(True)
         self._background_opacity = 0.0
         self._background_opacity_stop = 0.0
         self._update_style_sheet()
-        self._animation = QPropertyAnimation(self, b'backgroundOpacity')
+        self._animation = QPropertyAnimation(self, b'backgroundOpacity', self)
         self.clicked.connect(self._update_background_opacity_stop)
     
     def setColor(self, color=None):
         self._icon.setColor(color)
     
     def setIcon(self, icon):
         self._icon.loadIcon(icon)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/json_edit.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/json_edit.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/labelled.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/labelled.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QWidget, QHBoxLayout, QLabel
+from PyQt5.QtWidgets import QWidget, QHBoxLayout, QLabel
 
 
 def make_labelled(parent, label: str, widget: QWidget):
     """Put a widget into a container with a label to the left of it. Like a single row of a `QFormLayout`"""
     container = QWidget(parent)
     label_widget = QLabel(label)
     layout = QHBoxLayout(container)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/line_edit.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/line_edit.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import pyqtSignal, Qt
+from PyQt5.QtCore import pyqtSignal, Qt
 from PyQt5.QtWidgets import QLineEdit
-#pylint: enable=no-name-in-module
 
 from pyqttoolkit.properties import AutoProperty
 from pyqttoolkit.views.styleable import make_styleable
 
 class LineEdit(QLineEdit):
     def __init__(self, parent):
         QLineEdit.__init__(self, parent)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/linkable.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/linkable.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QWidget
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget
 
 class LinkableWidget(QWidget):
     def __init__(self, parent, link_manager=None, link_type=None):
         QWidget.__init__(self, parent)
         self._link_display = None
         self._link_manager = link_manager
         self._link_type = link_type
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/list_view.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/list_view.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QListView, pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QListView
+from PyQt5.QtCore import pyqtSignal
 
 from pyqttoolkit.properties import AutoProperty
 
 class ListView(QListView):
     def __init__(self, parent):
         QListView.__init__(self, parent)
         self.selectedIndexChanged.connect(self._handle_selected_index_changed)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/main_window.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/main_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QMainWindow, QStyleOption, QPainter, QStyle
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QMainWindow, QStyleOption, QStyle
+from PyQt5.QtGui import QPainter
 
 from pyqttoolkit.colors import format_color
 
 class MainWindow(QMainWindow):
     def __init__(self, parent, theme_manager):
         QMainWindow.__init__(self, parent)
         self._theme_manager = theme_manager
         self.setStyleSheet(self._get_stylesheet())
+        self._painter = None
+        self._opt = QStyleOption()
     
     def paintEvent(self, _event):
-        opt = QStyleOption()
-        opt.initFrom(self)
-        painter = QPainter(self)
-        self.style().drawPrimitive(QStyle.PE_Widget, opt, painter, self)
-    
+        self._opt.initFrom(self)
+        self._painter = QPainter(self)
+        self.style().drawPrimitive(QStyle.PE_Widget, self._opt, self._painter, self)
+        self._painter.end()
+        return super().paintEvent(_event)
+
     @property
     def themeManager(self):
         return self._theme_manager
 
     def _get_stylesheet(self):
         color = lambda k: format_color(self._theme_manager.get_color(k))
         color_a = lambda k, a: format_color(self._theme_manager.get_color(k), opacity=a)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/metadata_selector.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/metadata_selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QWidget, pyqtSignal, QGridLayout, QSizePolicy, QHBoxLayout, QSize
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget, QGridLayout, QSizePolicy, QHBoxLayout
+from PyQt5.QtCore import pyqtSignal, QSize
 
 from pyqttoolkit.models.roles import DataRole
 from pyqttoolkit.views import ComboBox
 from pyqttoolkit.properties import AutoProperty, bind
 from .icon_button import IconButton
 
 class MetadataSelectorDropDown(QWidget):
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/modulewindow.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/modulewindow.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 """:mod:`modulewindow`
 Module window widget
 """
 from uuid import uuid4
 
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import pyqtSignal
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal
 
 from pyqttoolkit.modules.events import RejectableEvent
 
 from .main_window import MainWindow
 
 class ModuleWindow(MainWindow):
     """class::ModuleWindow
     Class for use with QWidget-based modules
     """
-    def __init__(self, theme_manager, title=None):
+    def __init__(self, theme_manager, title=None, singleton: bool = False):
         MainWindow.__init__(self, None, theme_manager)
         self._id = uuid4()
         self._theme_manager = theme_manager
+        self._singleton = singleton
+        self._force = not singleton
         if title:
             self.setWindowTitle(title)
 
     closing = pyqtSignal(str)
 
     def setModuleView(self, module_view):
         """function::setModuleView(self, module_view)
@@ -53,21 +53,29 @@
         """
         return str(self._id)
 
     def closeEvent(self, event):
         """function::closeEvent(self, event)
         Decorates the base class with a closing event
         """
+        if self._singleton and not self._force:
+            event.ignore()
+            self.hide()
+            return
         if hasattr(self.centralWidget(), 'prepareClose'):
             close_event = RejectableEvent()
             self.centralWidget().prepareClose(close_event)
             if not close_event.accepted:
                 event.ignore()
                 return
         MainWindow.closeEvent(self, event)
         if event.isAccepted():
             self.centralWidget().close()
             self.closing.emit(self.moduleId)
+    
+    def forceClose(self):
+        self._force = True
+        return self.close()
 
     @property
     def themeManager(self):
         return self._theme_manager
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/popout.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/popout.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QWidget, QVBoxLayout, Qt, QSizePolicy, QGridLayout
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QWidget, QSizePolicy, QGridLayout
+from PyQt5.QtCore import Qt
 
 from pyqttoolkit.views.styleable import make_styleable
 from pyqttoolkit.colors import format_color
 
 class PopoutWidget(QWidget):
     def __init__(self, parent, content, background_color, foreground_color, background_opacity=0.8):
         QWidget.__init__(self, parent)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/popup.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/popup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QFrame, QPoint, Qt, QGridLayout, QRect
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import QPoint, Qt, QRect
+from PyQt5.QtWidgets import QFrame, QGridLayout
 
 class Popup(QFrame):
     def __init__(self, parent, contents):
         super().__init__(parent, Qt.FramelessWindowHint | Qt.Popup)
         self.setFrameStyle(QFrame.WinPanel | QFrame.Raised)
         self._contents = contents
         self._layout = QGridLayout(self)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/property_tree.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/property_tree.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QTreeView
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QTreeView
 
 class PropertyTreeView(QTreeView):
     def __init__(self, parent):
         QTreeView.__init__(self, parent)
     
     def resizeEvent(self, event):
         width = event.size().width()
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/shrunk_push_button.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/shrunk_push_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QSize
+from PyQt5.QtCore import QSize
 from PyQt5.QtWidgets import QPushButton
-#pylint: enable=no-name-in-module
 
 from .styleable import make_styleable
 
 class ShrunkPushButton(QPushButton):
     def __init__(self, text, parent):
         QPushButton.__init__(self, text, parent)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/steppable_combo_box.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/steppable_combo_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QHBoxLayout, QWidget, pyqtSignal
-from PyQt5.QtWidgets import QToolButton
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import QToolButton, QHBoxLayout, QWidget
 
 from pyqttoolkit.properties import AutoProperty, bind
 from .combo_box import BindableComboBox
 
 
 class SteppableComboBox(QWidget):
     """ComboBox with left and right shift buttons to decrease and increase the current index"""
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/styleable.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/text_edit.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,27 +10,22 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QStyleOption, QStyle, QPainter
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import pyqtSignal
+from PyQt5.QtWidgets import QTextEdit
+from PyQt5.QtGui import QFont
 
-def _get_paintEvent(cls):
-    def _paintEvent(self, event):
-        opt = QStyleOption()
-        opt.initFrom(self)
-        painter = QPainter(self)
-        self.style().drawPrimitive(QStyle.PE_Widget, opt, painter, self)
-        return cls.paintEvent(self, event)
-    return _paintEvent
-
-def make_styleable(cls):
-    return type(
-        cls.__name__,
-        (cls,),
-        {
-            'paintEvent': _get_paintEvent(cls)
-        }
-    )
+class TextEdit(QTextEdit):
+    def __init__(self, parent):
+        QTextEdit.__init__(self, parent)
+        self.setAcceptRichText(False)
+        self.document().setDefaultFont(QFont('Courier', pointSize=7))
+    
+    editComplete = pyqtSignal(str)
+    
+    def focusOutEvent(self, event):
+        self.editComplete.emit(self.toPlainText())
+        QTextEdit.focusOutEvent(self, event)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/table.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
 """:mod:`synthesis`
 Defines the SynthesisView class
 """
-#pylint: disable=no-name-in-module
-from PyQt5.Qt import QTableView, QKeySequence, QApplication, QMenu, QAction, Qt, QModelIndex, QSortFilterProxyModel
-#pylint: enable=no-name-in-module
+from PyQt5.QtCore import Qt, QModelIndex, QSortFilterProxyModel
+from PyQt5.QtWidgets import QTableView, QApplication, QMenu, QAction
+from PyQt5.QtGui import QKeySequence
 
 from pyqttoolkit.models.roles import RowSpanRole, ColumnSpanRole
 
 class TableView(QTableView):
     def __init__(self, parent):
         QTableView.__init__(self, parent)
         self._menu = QMenu(self)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/views/text_edit.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/views/tool_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,21 +10,26 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301  USA
-from PyQt5.Qt import QTextEdit, pyqtSignal, QFont
-#pylint: enable=no-name-in-module
+from PyQt5.QtWidgets import QDialog, QDialogButtonBox, QGridLayout
 
-class TextEdit(QTextEdit):
-    def __init__(self, parent):
-        QTextEdit.__init__(self, parent)
-        self.setAcceptRichText(False)
-        self.document().setDefaultFont(QFont('Courier', pointSize=7))
-    
-    editComplete = pyqtSignal(str)
-    
-    def focusOutEvent(self, event):
-        self.editComplete.emit(self.toPlainText())
-        QTextEdit.focusOutEvent(self, event)
+class ToolWindow(QDialog):
+    def __init__(self, parent, view, name, show_buttons=True):
+        QDialog.__init__(self, parent)
+        self.setWindowTitle(name)
+
+        view.setParent(self)
+
+        self._layout = QGridLayout(self)
+        self._layout.addWidget(view, 0, 0)
+
+        if show_buttons:
+            self._buttons = QDialogButtonBox(QDialogButtonBox.Ok | QDialogButtonBox.Cancel, self)
+            self._buttons.accepted.connect(self.accept)
+            self._buttons.rejected.connect(self.reject)
+            self._layout.addWidget(self._buttons, 1, 0)
+        
+        self.setLayout(self._layout)
```

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit/__init__.py` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/pyqttoolkit.egg-info/SOURCES.txt` & `pyqttoolkit-0.8.0.dev1/pyqttoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/setup.py` & `pyqttoolkit-0.8.0.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `pyqttoolkit-0.8.0.dev0/versioneer.py` & `pyqttoolkit-0.8.0.dev1/versioneer.py`

 * *Files identical despite different names*

