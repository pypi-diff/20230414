# Comparing `tmp/orchid_python_api-2022.4.252.tar.gz` & `tmp/orchid_python_api-2023.1.220.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchid_python_api-2022.4.252.tar", max compression
+gzip compressed data, was "orchid_python_api-2023.1.220.tar", max compression
```

## Comparing `orchid_python_api-2022.4.252.tar` & `orchid_python_api-2023.1.220.tar`

### file list

```diff
@@ -1,83 +1,82 @@
--rw-r--r--   0        0        0     3386 2022-06-13 16:53:26.624155 orchid_python_api-2022.4.252/copy_orchid_examples.py
--rw-r--r--   0        0        0     3604 2022-08-31 14:36:22.386439 orchid_python_api-2022.4.252/copy_orchid_low_level_examples.py
--rw-r--r--   0        0        0     3586 2022-10-28 22:29:28.132961 orchid_python_api-2022.4.252/copy_orchid_manual_examples.py
--rw-r--r--   0        0        0     3410 2022-06-13 16:53:26.625155 orchid_python_api-2022.4.252/copy_orchid_tutorials.py
--rw-r--r--   0        0        0    10316 2020-08-10 18:06:53.776507 orchid_python_api-2022.4.252/LICENSE
--rw-r--r--   0        0        0     1555 2022-12-12 15:25:47.728652 orchid_python_api-2022.4.252/orchid/__init__.py
--rw-r--r--   0        0        0      724 2022-06-13 16:53:26.717215 orchid_python_api-2022.4.252/orchid/__version__.py
--rw-r--r--   0        0        0     1081 2022-09-20 16:13:56.982742 orchid_python_api-2022.4.252/orchid/base.py
--rw-r--r--   0        0        0     3772 2022-06-13 16:53:27.129402 orchid_python_api-2022.4.252/orchid/base_time_series_adapter.py
--rw-r--r--   0        0        0     6811 2022-09-20 16:13:56.983721 orchid_python_api-2022.4.252/orchid/configuration.py
--rw-r--r--   0        0        0     1831 2022-09-20 16:13:56.984722 orchid_python_api-2022.4.252/orchid/convert.py
--rw-r--r--   0        0        0     6530 2022-09-20 16:13:56.985721 orchid_python_api-2022.4.252/orchid/core.py
--rw-r--r--   0        0        0     1186 2022-06-13 16:53:34.853538 orchid_python_api-2022.4.252/orchid/dom_project_object.py
--rw-r--r--   0        0        0     2370 2022-09-20 16:13:56.986720 orchid_python_api-2022.4.252/orchid/dot_net.py
--rw-r--r--   0        0        0     2161 2022-06-13 16:53:33.898192 orchid_python_api-2022.4.252/orchid/dot_net_disposable.py
--rw-r--r--   0        0        0    10282 2022-11-29 00:18:40.805074 orchid_python_api-2022.4.252/orchid/dot_net_dom_access.py
--rw-r--r--   0        0        0     1421 2022-06-13 16:53:26.638490 orchid_python_api-2022.4.252/orchid/measurement.py
--rw-r--r--   0        0        0     8428 2022-10-28 22:29:28.140962 orchid_python_api-2022.4.252/orchid/native_data_frame_adapter.py
--rw-r--r--   0        0        0     2806 2022-06-13 16:53:28.174108 orchid_python_api-2022.4.252/orchid/native_monitor_adapter.py
--rw-r--r--   0        0        0     6212 2022-09-20 16:13:56.990126 orchid_python_api-2022.4.252/orchid/native_project_user_data_adapter.py
--rw-r--r--   0        0        0    30514 2022-12-12 15:25:47.729669 orchid_python_api-2022.4.252/orchid/native_stage_adapter.py
--rw-r--r--   0        0        0     2086 2022-08-31 15:42:07.697879 orchid_python_api-2022.4.252/orchid/native_stage_part_adapter.py
--rw-r--r--   0        0        0     2628 2022-09-20 16:13:56.992129 orchid_python_api-2022.4.252/orchid/native_subsurface_point.py
--rw-r--r--   0        0        0     2090 2022-06-13 16:53:26.719547 orchid_python_api-2022.4.252/orchid/native_time_series_adapter.py
--rw-r--r--   0        0        0    10606 2022-12-12 15:25:47.730663 orchid_python_api-2022.4.252/orchid/native_trajectory_adapter.py
--rw-r--r--   0        0        0     7470 2022-06-13 16:53:28.313621 orchid_python_api-2022.4.252/orchid/native_treatment_calculations.py
--rw-r--r--   0        0        0     2519 2022-06-13 16:53:26.997497 orchid_python_api-2022.4.252/orchid/native_treatment_curve_adapter.py
--rw-r--r--   0        0        0     5427 2022-12-12 15:25:47.731664 orchid_python_api-2022.4.252/orchid/native_well_adapter.py
--rw-r--r--   0        0        0    10800 2022-06-13 16:53:34.054171 orchid_python_api-2022.4.252/orchid/net_date_time.py
--rw-r--r--   0        0        0     2273 2022-12-12 15:25:47.732662 orchid_python_api-2022.4.252/orchid/net_enumerable.py
--rw-r--r--   0        0        0     2126 2022-12-12 15:25:47.732837 orchid_python_api-2022.4.252/orchid/net_fracture_diagnostics_factory.py
--rw-r--r--   0        0        0    27134 2022-11-23 06:38:51.792677 orchid_python_api-2022.4.252/orchid/net_quantity.py
--rw-r--r--   0        0        0     2433 2022-09-20 16:13:56.996125 orchid_python_api-2022.4.252/orchid/net_stage_qc.py
--rw-r--r--   0        0        0     1181 2022-06-13 16:53:26.642494 orchid_python_api-2022.4.252/orchid/physical_quantity.py
--rw-r--r--   0        0        0     7052 2022-10-28 22:29:28.141961 orchid_python_api-2022.4.252/orchid/project.py
--rw-r--r--   0        0        0    12481 2022-12-12 15:25:47.734267 orchid_python_api-2022.4.252/orchid/project_store.py
--rw-r--r--   0        0        0     1452 2022-12-12 15:25:47.735266 orchid_python_api-2022.4.252/orchid/reference_origins.py
--rw-r--r--   0        0        0     2919 2022-09-20 16:13:56.998125 orchid_python_api-2022.4.252/orchid/script_adapter_context.py
--rw-r--r--   0        0        0     1753 2022-10-28 22:29:28.141961 orchid_python_api-2022.4.252/orchid/searchable_data_frames.py
--rw-r--r--   0        0        0     7555 2022-11-04 14:05:16.585053 orchid_python_api-2022.4.252/orchid/searchable_project_objects.py
--rw-r--r--   0        0        0     2627 2022-06-13 16:53:32.847152 orchid_python_api-2022.4.252/orchid/searchable_stage_parts.py
--rw-r--r--   0        0        0     1226 2022-06-13 16:53:26.644979 orchid_python_api-2022.4.252/orchid/searchable_stages.py
--rw-r--r--   0        0        0     6549 2022-09-20 16:13:57.001224 orchid_python_api-2022.4.252/orchid/unit_system.py
--rw-r--r--   0        0        0     1792 2022-06-13 16:53:26.722402 orchid_python_api-2022.4.252/orchid/validation.py
--rw-r--r--   0        0        0       10 2023-01-30 21:54:40.668810 orchid_python_api-2022.4.252/orchid/VERSION
--rw-r--r--   0        0        0     1099 2022-06-13 16:53:26.722634 orchid_python_api-2022.4.252/orchid/version.py
--rw-r--r--   0        0        0      844 2022-06-13 16:53:26.645979 orchid_python_api-2022.4.252/orchid_python_api/__init__.py
--rw-r--r--   0        0        0     6475 2022-10-28 22:29:28.142961 orchid_python_api-2022.4.252/orchid_python_api/examples/add_stages.py
--rw-r--r--   0        0        0     4400 2022-10-28 22:29:28.143962 orchid_python_api-2022.4.252/orchid_python_api/examples/change_stage_times.py
--rw-r--r--   0        0        0    28155 2022-08-31 15:42:07.704749 orchid_python_api-2022.4.252/orchid_python_api/examples/completion_analysis.ipynb
--rw-r--r--   0        0        0    17039 2022-08-31 15:42:07.705778 orchid_python_api-2022.4.252/orchid_python_api/examples/completion_analysis.py
--rw-r--r--   0        0        0    11549 2022-10-28 22:29:28.144963 orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/add_stages_low.py
--rw-r--r--   0        0        0    23608 2022-12-12 15:25:47.736266 orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/auto_pick.ipynb
--rw-r--r--   0        0        0    15686 2022-12-12 15:25:47.737267 orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/auto_pick.py
--rw-r--r--   0        0        0    18318 2022-12-12 15:25:47.737267 orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py
--rw-r--r--   0        0        0    15900 2022-12-12 15:25:47.738267 orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/auto_pick_iterate_example.py
--rw-r--r--   0        0        0     2446 2022-06-13 16:53:26.650064 orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/monitor_time_series.py
--rw-r--r--   0        0        0    10418 2022-12-12 15:25:47.739267 orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/multi_picking_events.py
--rw-r--r--   0        0        0    21648 2022-10-28 22:29:28.149962 orchid_python_api-2022.4.252/orchid_python_api/examples/manual/data_frame_with_guid.ipynb
--rw-r--r--   0        0        0     1373 2022-10-28 22:29:28.149962 orchid_python_api-2022.4.252/orchid_python_api/examples/manual/data_frame_with_guid.py
--rw-r--r--   0        0        0     8260 2022-06-13 16:53:26.723708 orchid_python_api-2022.4.252/orchid_python_api/examples/plot_time_series.ipynb
--rw-r--r--   0        0        0     4425 2022-06-13 16:53:26.651064 orchid_python_api-2022.4.252/orchid_python_api/examples/plot_time_series.py
--rw-r--r--   0        0        0     7006 2022-06-13 16:53:26.724092 orchid_python_api-2022.4.252/orchid_python_api/examples/plot_trajectories.ipynb
--rw-r--r--   0        0        0     3121 2022-06-13 16:53:26.652064 orchid_python_api-2022.4.252/orchid_python_api/examples/plot_trajectories.py
--rw-r--r--   0        0        0     7256 2022-06-13 16:53:26.724462 orchid_python_api-2022.4.252/orchid_python_api/examples/plot_treatment.ipynb
--rw-r--r--   0        0        0     3822 2022-06-13 16:53:26.652728 orchid_python_api-2022.4.252/orchid_python_api/examples/plot_treatment.py
--rw-r--r--   0        0        0      561 2022-06-13 16:53:28.029648 orchid_python_api-2022.4.252/orchid_python_api/examples/python_api.yaml.example
--rw-r--r--   0        0        0    30806 2022-12-12 15:25:47.740274 orchid_python_api-2022.4.252/orchid_python_api/examples/pythonnet3/internal_tests.ipynb
--rw-r--r--   0        0        0    18688 2022-12-12 15:25:47.741270 orchid_python_api-2022.4.252/orchid_python_api/examples/pythonnet3/internal_tests.py
--rw-r--r--   0        0        0    19458 2022-12-12 15:25:47.741270 orchid_python_api-2022.4.252/orchid_python_api/examples/pythonnet3/low_level.ipynb
--rw-r--r--   0        0        0    14287 2022-12-12 15:25:47.742268 orchid_python_api-2022.4.252/orchid_python_api/examples/pythonnet3/low_level.py
--rw-r--r--   0        0        0    13245 2022-06-13 16:53:26.724633 orchid_python_api-2022.4.252/orchid_python_api/examples/search_data_frames.ipynb
--rw-r--r--   0        0        0     5985 2022-06-13 16:53:26.652964 orchid_python_api-2022.4.252/orchid_python_api/examples/search_data_frames.py
--rw-r--r--   0        0        0     8613 2022-10-28 22:29:28.150961 orchid_python_api-2022.4.252/orchid_python_api/examples/stage_qc_results.py
--rw-r--r--   0        0        0    12887 2022-06-13 16:53:26.725134 orchid_python_api-2022.4.252/orchid_python_api/examples/volume_2_first_response.ipynb
--rw-r--r--   0        0        0     8570 2022-06-13 16:53:26.654666 orchid_python_api-2022.4.252/orchid_python_api/examples/volume_2_first_response.py
--rw-r--r--   0        0        0    24090 2022-06-13 16:53:26.725641 orchid_python_api-2022.4.252/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb
--rw-r--r--   0        0        0    19171 2022-06-13 16:53:26.726574 orchid_python_api-2022.4.252/orchid_python_api/tutorials/dom_navigation_tutorial.py
--rw-r--r--   0        0        0     3721 2023-01-30 21:54:40.672810 orchid_python_api-2022.4.252/pyproject.toml
--rw-r--r--   0        0        0    32857 2022-12-12 16:52:27.199547 orchid_python_api-2022.4.252/README.md
--rw-r--r--   0        0        0    19299 2023-01-30 21:54:40.666810 orchid_python_api-2022.4.252/ReleaseNotes.md
--rw-r--r--   0        0        0    34848 1970-01-01 00:00:00.000000 orchid_python_api-2022.4.252/setup.py
--rw-r--r--   0        0        0    34602 1970-01-01 00:00:00.000000 orchid_python_api-2022.4.252/PKG-INFO
+-rw-r--r--   0        0        0     3386 2023-04-12 16:21:02.740314 orchid_python_api-2023.1.220/copy_orchid_examples.py
+-rw-r--r--   0        0        0     3604 2023-04-12 16:21:02.163735 orchid_python_api-2023.1.220/copy_orchid_low_level_examples.py
+-rw-r--r--   0        0        0     3586 2023-04-12 16:21:02.705105 orchid_python_api-2023.1.220/copy_orchid_manual_examples.py
+-rw-r--r--   0        0        0     3410 2023-04-12 16:21:02.938782 orchid_python_api-2023.1.220/copy_orchid_tutorials.py
+-rw-r--r--   0        0        0    10316 2023-03-30 13:38:52.087989 orchid_python_api-2023.1.220/LICENSE
+-rw-r--r--   0        0        0     1554 2023-04-12 16:21:02.762215 orchid_python_api-2023.1.220/orchid/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-12 16:21:02.525319 orchid_python_api-2023.1.220/orchid/__version__.py
+-rw-r--r--   0        0        0     1081 2023-04-12 16:21:02.775215 orchid_python_api-2023.1.220/orchid/base.py
+-rw-r--r--   0        0        0     3772 2023-04-12 16:21:02.808333 orchid_python_api-2023.1.220/orchid/base_time_series_adapter.py
+-rw-r--r--   0        0        0     6810 2023-04-12 16:21:02.884794 orchid_python_api-2023.1.220/orchid/configuration.py
+-rw-r--r--   0        0        0     1831 2023-04-12 16:21:02.159565 orchid_python_api-2023.1.220/orchid/convert.py
+-rw-r--r--   0        0        0     6529 2023-04-12 16:21:02.520319 orchid_python_api-2023.1.220/orchid/core.py
+-rw-r--r--   0        0        0     1186 2023-04-12 16:21:02.639055 orchid_python_api-2023.1.220/orchid/dom_project_object.py
+-rw-r--r--   0        0        0     2369 2023-04-12 16:21:02.996811 orchid_python_api-2023.1.220/orchid/dot_net.py
+-rw-r--r--   0        0        0     2161 2023-04-12 16:21:02.579975 orchid_python_api-2023.1.220/orchid/dot_net_disposable.py
+-rw-r--r--   0        0        0    10281 2023-04-12 16:21:02.874802 orchid_python_api-2023.1.220/orchid/dot_net_dom_access.py
+-rw-r--r--   0        0        0     1421 2023-04-12 16:21:02.558847 orchid_python_api-2023.1.220/orchid/measurement.py
+-rw-r--r--   0        0        0     8428 2023-04-12 16:21:02.917374 orchid_python_api-2023.1.220/orchid/native_data_frame_adapter.py
+-rw-r--r--   0        0        0     2806 2023-04-12 16:21:02.878801 orchid_python_api-2023.1.220/orchid/native_monitor_adapter.py
+-rw-r--r--   0        0        0     6212 2023-04-12 16:21:02.644044 orchid_python_api-2023.1.220/orchid/native_project_user_data_adapter.py
+-rw-r--r--   0        0        0    30513 2023-04-12 16:21:02.514320 orchid_python_api-2023.1.220/orchid/native_stage_adapter.py
+-rw-r--r--   0        0        0     2086 2023-04-12 16:21:02.135049 orchid_python_api-2023.1.220/orchid/native_stage_part_adapter.py
+-rw-r--r--   0        0        0     2628 2023-04-12 16:21:02.589125 orchid_python_api-2023.1.220/orchid/native_subsurface_point.py
+-rw-r--r--   0        0        0     2090 2023-04-12 16:21:02.288818 orchid_python_api-2023.1.220/orchid/native_time_series_adapter.py
+-rw-r--r--   0        0        0    10605 2023-04-12 16:21:02.144562 orchid_python_api-2023.1.220/orchid/native_trajectory_adapter.py
+-rw-r--r--   0        0        0     7470 2023-04-12 16:21:02.766214 orchid_python_api-2023.1.220/orchid/native_treatment_calculations.py
+-rw-r--r--   0        0        0     2518 2023-04-12 16:21:02.621140 orchid_python_api-2023.1.220/orchid/native_treatment_curve_adapter.py
+-rw-r--r--   0        0        0     5426 2023-04-12 16:21:02.233299 orchid_python_api-2023.1.220/orchid/native_well_adapter.py
+-rw-r--r--   0        0        0    10800 2023-04-12 16:21:02.263815 orchid_python_api-2023.1.220/orchid/net_date_time.py
+-rw-r--r--   0        0        0     2273 2023-04-12 16:23:05.743109 orchid_python_api-2023.1.220/orchid/net_enumerable.py
+-rw-r--r--   0        0        0     2126 2023-04-12 16:21:02.730340 orchid_python_api-2023.1.220/orchid/net_fracture_diagnostics_factory.py
+-rw-r--r--   0        0        0    27133 2023-04-12 16:21:02.701113 orchid_python_api-2023.1.220/orchid/net_quantity.py
+-rw-r--r--   0        0        0     2433 2023-04-12 16:21:02.574966 orchid_python_api-2023.1.220/orchid/net_stage_qc.py
+-rw-r--r--   0        0        0     1181 2023-04-12 16:21:03.150866 orchid_python_api-2023.1.220/orchid/physical_quantity.py
+-rw-r--r--   0        0        0     7051 2023-04-12 16:21:03.136869 orchid_python_api-2023.1.220/orchid/project.py
+-rw-r--r--   0        0        0    12480 2023-04-12 16:21:02.606576 orchid_python_api-2023.1.220/orchid/project_store.py
+-rw-r--r--   0        0        0     1452 2023-04-12 16:21:02.969782 orchid_python_api-2023.1.220/orchid/reference_origins.py
+-rw-r--r--   0        0        0     2919 2023-04-12 16:21:02.227787 orchid_python_api-2023.1.220/orchid/script_adapter_context.py
+-rw-r--r--   0        0        0     1753 2023-04-12 16:21:02.648060 orchid_python_api-2023.1.220/orchid/searchable_data_frames.py
+-rw-r--r--   0        0        0     7555 2023-04-12 16:21:02.617147 orchid_python_api-2023.1.220/orchid/searchable_project_objects.py
+-rw-r--r--   0        0        0     2627 2023-04-12 16:21:03.200893 orchid_python_api-2023.1.220/orchid/searchable_stage_parts.py
+-rw-r--r--   0        0        0     1226 2023-04-12 16:21:03.001811 orchid_python_api-2023.1.220/orchid/searchable_stages.py
+-rw-r--r--   0        0        0     6549 2023-04-12 16:21:02.173759 orchid_python_api-2023.1.220/orchid/unit_system.py
+-rw-r--r--   0        0        0     1791 2023-04-12 16:21:02.744321 orchid_python_api-2023.1.220/orchid/validation.py
+-rw-r--r--   0        0        0       10 2023-04-12 15:24:07.549281 orchid_python_api-2023.1.220/orchid/VERSION
+-rw-r--r--   0        0        0     1098 2023-04-12 16:21:02.353665 orchid_python_api-2023.1.220/orchid/version.py
+-rw-r--r--   0        0        0      844 2023-04-12 16:23:05.766656 orchid_python_api-2023.1.220/orchid_python_api/__init__.py
+-rw-r--r--   0        0        0     6474 2023-04-12 16:23:06.160412 orchid_python_api-2023.1.220/orchid_python_api/examples/add_stages.py
+-rw-r--r--   0        0        0     4400 2023-04-12 16:23:05.788673 orchid_python_api-2023.1.220/orchid_python_api/examples/change_stage_times.py
+-rw-r--r--   0        0        0    28071 2023-04-12 16:23:05.754130 orchid_python_api-2023.1.220/orchid_python_api/examples/completion_analysis.ipynb
+-rw-r--r--   0        0        0    17039 2023-04-12 16:23:05.682626 orchid_python_api-2023.1.220/orchid_python_api/examples/completion_analysis.py
+-rw-r--r--   0        0        0    11549 2023-04-12 16:23:05.703016 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/add_stages_low.py
+-rw-r--r--   0        0        0    23608 2023-04-12 16:23:05.794663 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick.ipynb
+-rw-r--r--   0        0        0    15686 2023-04-12 16:23:05.873178 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick.py
+-rw-r--r--   0        0        0    18318 2023-04-12 16:23:06.100791 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py
+-rw-r--r--   0        0        0    15900 2023-04-12 16:23:06.131875 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick_iterate_example.py
+-rw-r--r--   0        0        0     2446 2023-04-12 16:23:05.777657 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/monitor_time_series.py
+-rw-r--r--   0        0        0    10418 2023-04-12 16:23:05.841635 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/multi_picking_events.py
+-rw-r--r--   0        0        0    21648 2023-04-12 16:23:05.782679 orchid_python_api-2023.1.220/orchid_python_api/examples/manual/data_frame_with_guid.ipynb
+-rw-r--r--   0        0        0     1373 2023-04-12 16:23:05.771655 orchid_python_api-2023.1.220/orchid_python_api/examples/manual/data_frame_with_guid.py
+-rw-r--r--   0        0        0     8260 2023-04-12 16:23:06.066223 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_time_series.ipynb
+-rw-r--r--   0        0        0     4425 2023-04-12 16:23:05.738098 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_time_series.py
+-rw-r--r--   0        0        0     7006 2023-04-12 16:23:05.720577 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_trajectories.ipynb
+-rw-r--r--   0        0        0     3121 2023-04-12 16:23:05.708014 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_trajectories.py
+-rw-r--r--   0        0        0     7256 2023-04-12 16:23:05.820223 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_treatment.ipynb
+-rw-r--r--   0        0        0     3822 2023-04-12 16:23:05.696948 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_treatment.py
+-rw-r--r--   0        0        0      561 2023-03-30 13:38:52.090988 orchid_python_api-2023.1.220/orchid_python_api/examples/python_api.yaml.example
+-rw-r--r--   0        0        0    30806 2023-03-30 13:38:52.096506 orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/internal_tests.ipynb
+-rw-r--r--   0        0        0    18688 2023-04-12 16:23:06.218598 orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/internal_tests.py
+-rw-r--r--   0        0        0    19458 2023-03-30 13:38:52.096506 orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/low_level.ipynb
+-rw-r--r--   0        0        0    14287 2023-04-12 16:23:06.073222 orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/low_level.py
+-rw-r--r--   0        0        0    13245 2023-04-12 16:23:05.944772 orchid_python_api-2023.1.220/orchid_python_api/examples/search_data_frames.ipynb
+-rw-r--r--   0        0        0     5985 2023-04-12 16:23:06.153395 orchid_python_api-2023.1.220/orchid_python_api/examples/search_data_frames.py
+-rw-r--r--   0        0        0     8613 2023-04-12 16:23:05.965303 orchid_python_api-2023.1.220/orchid_python_api/examples/stage_qc_results.py
+-rw-r--r--   0        0        0    12887 2023-04-12 16:23:05.879194 orchid_python_api-2023.1.220/orchid_python_api/examples/volume_2_first_response.ipynb
+-rw-r--r--   0        0        0     8570 2023-04-12 16:23:06.247103 orchid_python_api-2023.1.220/orchid_python_api/examples/volume_2_first_response.py
+-rw-r--r--   0        0        0    24090 2023-04-12 16:23:05.934768 orchid_python_api-2023.1.220/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb
+-rw-r--r--   0        0        0    19171 2023-04-12 16:23:05.761122 orchid_python_api-2023.1.220/orchid_python_api/tutorials/dom_navigation_tutorial.py
+-rw-r--r--   0        0        0     3721 2023-04-12 15:26:48.304536 orchid_python_api-2023.1.220/pyproject.toml
+-rw-r--r--   0        0        0    32857 2023-03-30 13:38:52.098505 orchid_python_api-2023.1.220/README.md
+-rw-r--r--   0        0        0    19722 2023-04-12 15:13:05.860437 orchid_python_api-2023.1.220/ReleaseNotes.md
+-rw-r--r--   0        0        0    34602 1970-01-01 00:00:00.000000 orchid_python_api-2023.1.220/PKG-INFO
```

### Comparing `orchid_python_api-2022.4.252/copy_orchid_examples.py` & `orchid_python_api-2023.1.220/copy_orchid_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/copy_orchid_low_level_examples.py` & `orchid_python_api-2023.1.220/copy_orchid_low_level_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/copy_orchid_manual_examples.py` & `orchid_python_api-2023.1.220/copy_orchid_manual_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/copy_orchid_tutorials.py` & `orchid_python_api-2023.1.220/copy_orchid_tutorials.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! /usr/bin/env python
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/LICENSE` & `orchid_python_api-2023.1.220/LICENSE`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2022.4.252/orchid/__init__.py` & `orchid_python_api-2023.1.220/orchid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/__version__.py` & `orchid_python_api-2023.1.220/orchid/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/base.py` & `orchid_python_api-2023.1.220/orchid/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/base_time_series_adapter.py` & `orchid_python_api-2023.1.220/orchid/base_time_series_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/configuration.py` & `orchid_python_api-2023.1.220/orchid/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/convert.py` & `orchid_python_api-2023.1.220/orchid/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/core.py` & `orchid_python_api-2023.1.220/orchid/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/dom_project_object.py` & `orchid_python_api-2023.1.220/orchid/dom_project_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/dot_net.py` & `orchid_python_api-2023.1.220/orchid/dot_net.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/dot_net_disposable.py` & `orchid_python_api-2023.1.220/orchid/dot_net_disposable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/dot_net_dom_access.py` & `orchid_python_api-2023.1.220/orchid/dot_net_dom_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/measurement.py` & `orchid_python_api-2023.1.220/orchid/measurement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_data_frame_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_data_frame_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_monitor_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_monitor_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_project_user_data_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_project_user_data_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2017-2022 Reveal Energy Services, Inc
+#  Copyright 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_stage_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_stage_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_stage_part_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_stage_part_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2017-2022 Reveal Energy Services, Inc
+#  Copyright 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_subsurface_point.py` & `orchid_python_api-2023.1.220/orchid/native_subsurface_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_time_series_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_time_series_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_trajectory_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_trajectory_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_treatment_calculations.py` & `orchid_python_api-2023.1.220/orchid/native_treatment_calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_treatment_curve_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_treatment_curve_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/native_well_adapter.py` & `orchid_python_api-2023.1.220/orchid/native_well_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/net_date_time.py` & `orchid_python_api-2023.1.220/orchid/net_date_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/net_enumerable.py` & `orchid_python_api-2023.1.220/orchid/net_enumerable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/net_fracture_diagnostics_factory.py` & `orchid_python_api-2023.1.220/orchid/net_fracture_diagnostics_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/net_quantity.py` & `orchid_python_api-2023.1.220/orchid/net_quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/net_stage_qc.py` & `orchid_python_api-2023.1.220/orchid/net_stage_qc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2017-2022 Reveal Energy Services, Inc
+#  Copyright 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/physical_quantity.py` & `orchid_python_api-2023.1.220/orchid/physical_quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/project.py` & `orchid_python_api-2023.1.220/orchid/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/project_store.py` & `orchid_python_api-2023.1.220/orchid/project_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/reference_origins.py` & `orchid_python_api-2023.1.220/orchid/reference_origins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/script_adapter_context.py` & `orchid_python_api-2023.1.220/orchid/script_adapter_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/searchable_data_frames.py` & `orchid_python_api-2023.1.220/orchid/searchable_data_frames.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/searchable_project_objects.py` & `orchid_python_api-2023.1.220/orchid/searchable_project_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/searchable_stage_parts.py` & `orchid_python_api-2023.1.220/orchid/searchable_stage_parts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/searchable_stages.py` & `orchid_python_api-2023.1.220/orchid/searchable_stages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid/unit_system.py` & `orchid_python_api-2023.1.220/orchid/unit_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # This file is part of Orchid and related technologies.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
```

### Comparing `orchid_python_api-2022.4.252/orchid/validation.py` & `orchid_python_api-2023.1.220/orchid/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid/version.py` & `orchid_python_api-2023.1.220/orchid/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc 
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/__init__.py` & `orchid_python_api-2023.1.220/orchid_python_api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/add_stages.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/add_stages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright 2017-2022 Reveal Energy Services, Inc 
+#  Copyright 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License"); 
 #  you may not use this file except in compliance with the License. 
 #  You may obtain a copy of the License at 
 #
 #      http://www.apache.org/licenses/LICENSE-2.0 
 #
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/change_stage_times.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/change_stage_times.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/completion_analysis.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/completion_analysis.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999485948225444%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#  Copyright (c) 2017-2023 Reveal Energy Services, "*

 * *            "Inc\\n')], delete: [0]}}, 30: {'metadata': {delete: ['pycharm']}, 'source': {insert: "*

 * *            '[(0, \'def show_proppant_loading_plot(data_frame):\\n\'), (12, "                   '*

 * *            'colors[i], marker=\'o\', linestyle=\'\', ms=6, label=name)\\n"), (22, '*

 * *            '"show_proppant_loading_plot(bakken_summaries[bakken_summaries[bakken_columns[\'stage\']] '*

 * *            '> 5])")], delete […]*

```diff
@@ -10,15 +10,15 @@
                 },
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "#  Copyright (c) 2017-2022 Reveal Energy Services, Inc\n",
+                "#  Copyright (c) 2017-2023 Reveal Energy Services, Inc\n",
                 "#\n",
                 "#  Licensed under the Apache License, Version 2.0 (the \"License\");\n",
                 "#  you may not use this file except in compliance with the License.\n",
                 "#  You may obtain a copy of the License at\n",
                 "#\n",
                 "#      http://www.apache.org/licenses/LICENSE-2.0\n",
                 "#\n",
@@ -528,44 +528,41 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
-                },
-                "pycharm": {
-                    "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "def build_proppant_loading_plot(data_frame):\n",
+                "def show_proppant_loading_plot(data_frame):\n",
                 "    groups = data_frame.groupby(bakken_columns['well'])\n",
                 "\n",
                 "    fig, ax = plt.subplots(len(groups), sharex=True, sharey=True)\n",
                 "    fig.suptitle(f'{bakken_columns[\"proppant_loading\"]} by Stage')\n",
                 "    i=0\n",
                 "    colors=['tab:blue', 'tab:orange', 'tab:green', 'tab:red', 'tab:purple',\n",
                 "            'tab:brown', 'tab:pink', 'tab:gray', 'tab:olive', 'tab:cyan']\n",
                 "    for name, group in groups:\n",
                 "        ax[i].margins(0.05)\n",
                 "        ax[i].plot(group[bakken_columns['stage']],\n",
                 "                   group[bakken_columns['proppant_loading']],\n",
-                "                   marker='o', linestyle='', ms=6, label=name)\n",
+                "                   colors[i], marker='o', linestyle='', ms=6, label=name)\n",
                 "        ax[i].legend()\n",
                 "        ax[i].set_xlabel('Stage Number')\n",
                 "        i = i+1\n",
                 "        # Hide x labels and tick labels for all but bottom plot.\n",
                 "    for a in ax:\n",
                 "        a.label_outer()\n",
                 "    plt.rcParams['figure.dpi'] = 150\n",
                 "    plt.show()\n",
                 "\n",
-                "build_proppant_loading_plot(bakken_summaries[bakken_summaries[bakken_columns['stage']]>5])"
+                "show_proppant_loading_plot(bakken_summaries[bakken_summaries[bakken_columns['stage']] > 5])"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "pycharm": {
                     "name": "#%% md\n"
@@ -948,22 +945,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
-                },
-                "pycharm": {
-                    "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "build_proppant_loading_plot(combined)"
+                "show_proppant_loading_plot(combined)"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/completion_analysis.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/completion_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/add_stages_low.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/add_stages_low.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/auto_pick.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999362244897959%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, '# Copyright (c) 2017-2023 Reveal Energy Services.  All "*

 * *            "Rights Reserved.\\n')], delete: [3]}}}"}*

```diff
@@ -5,15 +5,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#\n",
                 "# This file is part of Orchid and related technologies.\n",
                 "#\n",
-                "# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.\n",
+                "# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.\n",
                 "#\n",
                 "# LEGAL NOTICE:\n",
                 "# Orchid contains trade secrets and otherwise confidential information\n",
                 "# owned by Reveal Energy Services. Access to and use of this information is\n",
                 "# strictly limited and controlled by the Company. This file may not be copied,\n",
                 "# distributed, or otherwise disclosed outside of the Company's facilities\n",
                 "# except under appropriate precautions to maintain the confidentiality hereof,\n",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/auto_pick.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/auto_pick_iterate_example.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick_iterate_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/monitor_time_series.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/monitor_time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/low_level/multi_picking_events.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/multi_picking_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/manual/data_frame_with_guid.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/manual/data_frame_with_guid.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999134948096886%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#  Copyright (c) 2017-2023 Reveal Energy Services, "*

 * *            "Inc\\n')], delete: [0]}}}"}*

```diff
@@ -4,15 +4,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "#  Copyright (c) 2017-2022 Reveal Energy Services, Inc\n",
+                "#  Copyright (c) 2017-2023 Reveal Energy Services, Inc\n",
                 "#\n",
                 "#  Licensed under the Apache License, Version 2.0 (the \"License\");\n",
                 "#  you may not use this file except in compliance with the License.\n",
                 "#  You may obtain a copy of the License at\n",
                 "#\n",
                 "#      https://www.apache.org/licenses/LICENSE-2.0\n",
                 "#\n",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/manual/data_frame_with_guid.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/manual/data_frame_with_guid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/plot_time_series.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_time_series.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999183006535948%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#  Copyright (c) 2017-2023 Reveal Energy Services, "*

 * *            "Inc\\n')], delete: [0]}}}"}*

```diff
@@ -10,15 +10,15 @@
                 },
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "#  Copyright (c) 2017-2022 Reveal Energy Services, Inc\n",
+                "#  Copyright (c) 2017-2023 Reveal Energy Services, Inc\n",
                 "#\n",
                 "#  Licensed under the Apache License, Version 2.0 (the \"License\");\n",
                 "#  you may not use this file except in compliance with the License.\n",
                 "#  You may obtain a copy of the License at\n",
                 "#\n",
                 "#      http://www.apache.org/licenses/LICENSE-2.0\n",
                 "#\n",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/plot_time_series.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/plot_trajectories.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_trajectories.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999922600619195%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#  Copyright (c) 2017-2023 Reveal Energy Services, "*

 * *            "Inc\\n')], delete: [0]}}}"}*

```diff
@@ -10,15 +10,15 @@
                 },
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "#  Copyright (c) 2017-2022 Reveal Energy Services, Inc\n",
+                "#  Copyright (c) 2017-2023 Reveal Energy Services, Inc\n",
                 "#\n",
                 "#  Licensed under the Apache License, Version 2.0 (the \"License\");\n",
                 "#  you may not use this file except in compliance with the License.\n",
                 "#  You may obtain a copy of the License at\n",
                 "#\n",
                 "#      http://www.apache.org/licenses/LICENSE-2.0\n",
                 "#\n",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/plot_trajectories.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_trajectories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/plot_treatment.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_treatment.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999134948096886%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#  Copyright (c) 2017-2023 Reveal Energy Services, "*

 * *            "Inc\\n')], delete: [0]}}}"}*

```diff
@@ -10,15 +10,15 @@
                 },
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "#  Copyright (c) 2017-2022 Reveal Energy Services, Inc\n",
+                "#  Copyright (c) 2017-2023 Reveal Energy Services, Inc\n",
                 "#\n",
                 "#  Licensed under the Apache License, Version 2.0 (the \"License\");\n",
                 "#  you may not use this file except in compliance with the License.\n",
                 "#  You may obtain a copy of the License at\n",
                 "#\n",
                 "#      http://www.apache.org/licenses/LICENSE-2.0\n",
                 "#\n",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/plot_treatment.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_treatment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/python_api.yaml.example` & `orchid_python_api-2023.1.220/orchid_python_api/examples/python_api.yaml.example`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/pythonnet3/internal_tests.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/internal_tests.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/pythonnet3/internal_tests.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/internal_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/pythonnet3/low_level.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/low_level.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/pythonnet3/low_level.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/low_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/search_data_frames.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/search_data_frames.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999591503267974%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#  Copyright (c) 2017-2023 Reveal Energy Services, "*

 * *            "Inc\\n')], delete: [0]}}}"}*

```diff
@@ -10,15 +10,15 @@
                 },
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "#  Copyright (c) 2017-2022 Reveal Energy Services, Inc\n",
+                "#  Copyright (c) 2017-2023 Reveal Energy Services, Inc\n",
                 "#\n",
                 "#  Licensed under the Apache License, Version 2.0 (the \"License\");\n",
                 "#  you may not use this file except in compliance with the License.\n",
                 "#  You may obtain a copy of the License at\n",
                 "#\n",
                 "#      http://www.apache.org/licenses/LICENSE-2.0\n",
                 "#\n",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/search_data_frames.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/search_data_frames.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/stage_qc_results.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/stage_qc_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/volume_2_first_response.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/examples/volume_2_first_response.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999455337690633%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#  Copyright (c) 2017-2023 Reveal Energy Services, "*

 * *            "Inc\\n')], delete: [0]}}}"}*

```diff
@@ -6,15 +6,15 @@
             "metadata": {
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "#  Copyright (c) 2017-2022 Reveal Energy Services, Inc\n",
+                "#  Copyright (c) 2017-2023 Reveal Energy Services, Inc\n",
                 "#\n",
                 "#  Licensed under the Apache License, Version 2.0 (the \"License\");\n",
                 "#  you may not use this file except in compliance with the License.\n",
                 "#  You may obtain a copy of the License at\n",
                 "#\n",
                 "#      http://www.apache.org/licenses/LICENSE-2.0\n",
                 "#\n",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/examples/volume_2_first_response.py` & `orchid_python_api-2023.1.220/orchid_python_api/examples/volume_2_first_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of Orchid and related technologies.
 #
-# Copyright (c) 2017-2022 Reveal Energy Services.  All Rights Reserved.
+# Copyright (c) 2017-2023 Reveal Energy Services.  All Rights Reserved.
 #
 # LEGAL NOTICE:
 # Orchid contains trade secrets and otherwise confidential information
 # owned by Reveal Energy Services. Access to and use of this information is 
 # strictly limited and controlled by the Company. This file may not be copied,
 # distributed, or otherwise disclosed outside of the Company's facilities 
 # except under appropriate precautions to maintain the confidentiality hereof,
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb` & `orchid_python_api-2023.1.220/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999687108886107%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '#  Copyright (c) 2017-2023 Reveal Energy Services, "*

 * *            "Inc\\n')], delete: [0]}}}"}*

```diff
@@ -10,15 +10,15 @@
                 },
                 "pycharm": {
                     "name": "#%%\n"
                 }
             },
             "outputs": [],
             "source": [
-                "#  Copyright (c) 2017-2022 Reveal Energy Services, Inc\n",
+                "#  Copyright (c) 2017-2023 Reveal Energy Services, Inc\n",
                 "#\n",
                 "#  Licensed under the Apache License, Version 2.0 (the \"License\");\n",
                 "#  you may not use this file except in compliance with the License.\n",
                 "#  You may obtain a copy of the License at\n",
                 "#\n",
                 "#      http://www.apache.org/licenses/LICENSE-2.0\n",
                 "#\n",
```

### Comparing `orchid_python_api-2022.4.252/orchid_python_api/tutorials/dom_navigation_tutorial.py` & `orchid_python_api-2023.1.220/orchid_python_api/tutorials/dom_navigation_tutorial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2017-2022 Reveal Energy Services, Inc
+#  Copyright (c) 2017-2023 Reveal Energy Services, Inc
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `orchid_python_api-2022.4.252/pyproject.toml` & `orchid_python_api-2023.1.220/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "orchid-python-api"
-version = "2022.4.252"
+version = "2023.1.220"
 description = "Defines and implements the Python API for Orchid*. (*Orchid is a mark of Reveal Energy Services, Inc.)"
 authors = [ "Reveal Energy Services, Inc. <support@reveal-energy.com>",]
 maintainers = [ "Reveal Energy Services, Inc. <support@reveal-energy.com>",]
 license = "Apache-2.0"
 readme = "README.md"
 homepage="https://github.com/Reveal-Energy-Services/orchid-python-api"
 repository="https://github.com/Reveal-Energy-Services/orchid-python-api"
```

### Comparing `orchid_python_api-2022.4.252/README.md` & `orchid_python_api-2023.1.220/README.md`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2022.4.252/ReleaseNotes.md` & `orchid_python_api-2023.1.220/ReleaseNotes.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,35 @@
 - [ReleaseNotes.md](./ReleaseNotes.md) - The release notes for this project.
 
 Although one can read this document in any text editor since it is simply a text file, consider installing
 the [Python grip utility](https://pypi.org/project/grip/). This application allows one to "render local readme
 files before sending off to GitHub". Although you need not send any of these file to `GitHub`, by using `grip` 
 to render the file, you can much more easily navigate the document links.
 
+### Release notes for 2023.1.220
+
+This release is the production release of the Orchid Python API corresponding to Orchid 2023.1.220. A very basic example of how
+to get to a project's well horizon markers was added. Additionally, a fix to an integration test is included.
+
+#### Possible breaking .NET API changes
+
+- None
+
+#### Resolved Issues
+
+- None
+
+#### Features
+
+- None
+
+#### Known Issues
+
+- None
+
 ### Release notes for 2022.4.252
 
 This release is the production release of the Orchid Python API corresponding to Orchid 2022.4.252. The main
 features in this release are the upgrade of the internal package, `pythonnet`, to version `3.x`, and the change 
 requiring Python 3.10 for the runtime environment.
 
 #### Possible breaking .NET API changes
```

### Comparing `orchid_python_api-2022.4.252/setup.py` & `orchid_python_api-2023.1.220/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,628 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: orchid-python-api
+Version: 2023.1.220
+Summary: Defines and implements the Python API for Orchid*. (*Orchid is a mark of Reveal Energy Services, Inc.)
+Home-page: https://github.com/Reveal-Energy-Services/orchid-python-api
+License: Apache-2.0
+Keywords: Orchid Integration,Fracture Diagnostics
+Author: Reveal Energy Services, Inc.
+Author-email: support@reveal-energy.com
+Maintainer: Reveal Energy Services, Inc.
+Maintainer-email: support@reveal-energy.com
+Requires-Python: >=3.10,<3.11
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: deal (>=4.23.4,<5.0.0)
+Requires-Dist: ipython (>=8.7.0,<9.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: jupyterlab (>=3.5.1,<4.0.0)
+Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: option (>=2.1.0,<3.0.0)
+Requires-Dist: packaging (>=22.0,<23.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pendulum (>=2.1.2,<3.0.0)
+Requires-Dist: pint (>=0.20.1,<0.21.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: pythonnet (==3.0.0-post1)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: seaborn (>=0.12.1,<0.13.0)
+Requires-Dist: toolz (>=0.12.0,<0.13.0)
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Documentation, https://github.com/Reveal-Energy-Services/orchid-python-api/wiki
+Project-URL: Issues, https://github.com/Reveal-Energy-Services/orchid-python-api/issues
+Project-URL: Repository, https://github.com/Reveal-Energy-Services/orchid-python-api
+Description-Content-Type: text/markdown
 
-packages = \
-['orchid_python_api',
- 'orchid_python_api.examples',
- 'orchid_python_api.examples.low_level',
- 'orchid_python_api.examples.manual',
- 'orchid_python_api.examples.pythonnet3',
- 'orchid_python_api.tutorials']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['deal>=4.23.4,<5.0.0',
- 'ipython>=8.7.0,<9.0.0',
- 'jupyter>=1.0.0,<2.0.0',
- 'jupyterlab>=3.5.1,<4.0.0',
- 'matplotlib>=3.6.2,<4.0.0',
- 'numpy>=1.23.5,<2.0.0',
- 'option>=2.1.0,<3.0.0',
- 'packaging>=22.0,<23.0',
- 'pandas>=1.5.2,<2.0.0',
- 'pendulum>=2.1.2,<3.0.0',
- 'pint>=0.20.1,<0.21.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'pythonnet==3.0.0-post1',
- 'pyyaml>=6.0,<7.0',
- 'scipy>=1.9.3,<2.0.0',
- 'seaborn>=0.12.1,<0.13.0',
- 'toolz>=0.12.0,<0.13.0',
- 'typing-extensions>=4.4.0,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['copy_orchid_examples = copy_orchid_examples:main',
-                     'copy_orchid_low_level_examples = '
-                     'copy_orchid_low_level_examples:main',
-                     'copy_orchid_manual_examples = '
-                     'copy_orchid_manual_examples:main',
-                     'copy_orchid_tutorials = copy_orchid_tutorials:main']}
-
-setup_kwargs = {
-    'name': 'orchid-python-api',
-    'version': '2022.4.252',
-    'description': 'Defines and implements the Python API for Orchid*. (*Orchid is a mark of Reveal Energy Services, Inc.)',
-    'long_description': '## Introduction \n\nThis project defines the implementation of the Python API for Orchid*.\n\nSpecifically, the `orchid` package makes Orchid features available to Python applications and to the\nPython REPL.\n\n(* Orchid is a mark of Reveal Energy Services, Inc.)\n\n### A Reading Suggestion\n\nThis document is one of several documents you may want to read:\n\n- [README](./README.md) - This file.\n- [README-dev.md](./README-dev.md) - A similar file targeting for package developers.\n- [ReleaseNotes.md](./ReleaseNotes.md) - The release notes for this project.\n\nAdditionally, as part of the 2022.4 release, we upgraded `pythonnet`, the package we use to expose .NET to the Python\nruntime, from version 2.5.2 to version 3.0.0.post1. This upgrade is a breaking upgrade. The document, \n[README-pythonnet3.md](./README-pythonnet3.md), describes the changes that we needed to make to the Orchid Python API to\nrepair failing internal tests. The document, [README-pythonnet3-low.md](./README-pythonnet3-low.md), describes the \nchanges that we needed to make to the Orchid Python API to repair failing low-level examples.\n\nAlthough one can read this document in any text editor since it is simply a text file, consider installing\nthe [Python grip utility](https://pypi.org/project/grip/). This application allows one to "render local readme\nfiles before sending off to GitHub". Although you need not send any of these file to `GitHub`, by using `grip` \nto render the file, you can much more easily navigate the document links.\n\n## Examples\n\n### High-level examples\n\nThis project includes eight scripts and six notebooks in the `examples` directory of the `orchid-python-api` package:\n\n| Name                            | Demonstrates...                                                                     |\n|---------------------------------|-------------------------------------------------------------------------------------|\n| `completion_analysis.ipynb`     | A detailed analysis of the completion performed on two different wells in a project |\n| `plot_trajectories.ipynb`       | Plotting the well trajectories for a project                                        |\n| `plot_time_series.ipynb`        | Plotting the monitor curves for a project                                           |\n| `plot_treatment.ipynb`          | Plotting the treatment curves for a specific stage of a well in a project           | \n| `search_data_frames.ipynb`      | Searching object collections and our data frame access                              | \n| `volume_2_first_response.ipynb` | Using derivatives to calculate the fluid volume pumped before the first response    | \n\nSix of the eight scripts contain the same code as the notebooks but run either at the command line or in a REPL. The\nlast three scripts:\n\n| Name                            | Demonstrates using the high-level Python API to...                               |\n|---------------------------------|----------------------------------------------------------------------------------|\n| `stage_qc_results.py`           | Read and write QC results for a stage. (Replaces low-level `stage_qc_status.py`) |\n| `change_stage_times.py`         | Change the start and stop times (the time range) of a stage                      |\n| `add_stages.py`                 | Add one or more stages to a well. (Improvement over `add_stages_low.py`)         |\n\n### Low-level examples\n\nIn addition, this project includes five scripts and a notebook in the `examples/low_level` directory of the\n`orchid-python-api` package:\n\n| Name                                      | Demonstrates...                                                  |\n|-------------------------------------------|------------------------------------------------------------------|\n| `auto_pick.py`                            | Automatically pick observations and save them to an .ifrac file  |\n| `auto_pick_and_create_stage_attribute.py` | Create and save stage attributes                                 |\n| `auto_pick_iterate_example.py`            | Use iteration to find visible stages instead of .NET method      |\n| `monitor_time_series.py`                  | Find high-level time series from a low-level monitor time series | \n| `add_stages_low.py`                       | Adds newly created stages to a well of a project                 | \n| `multi_picking_events.py`                 | Creates and adds a number of multi-picking events                |\n\nThe notebook, `auto_pick.ipynb` contain the same code as the script, `auto_pick.py`, but runs in a Jupyter\nnotebook.\n \nTo use these examples: \n\n- You may need to \n  [configure the Orchid Python API to find the Orchid installation](#configure-the-orchid-python-api)\n- You **must** \n  [configure the Orchid Python API to find the Orchid training data](#configure-the-orchid-training-data)\n- You may need to [view the Orchid API configuration details](#view-orchid-configuration-details)\n- You may want to invoke the command, `copy_orchid_examples`\n\n    This command copies the example files into an optionally specified (virtual environment) directory. (The \n    default destination is your current working directory.) Note that this command is a command-line script \n    that runs in a console or terminal. Additionally, this command supports a help flag, `-h` or `--help`, to \n    provide you with help on running this command.\n\nMore detailed instructions for running the examples can be found at:\n\n- [Run Orchid high-level examples](#run-orchid-high-level-examples).\n\n## Tutorials\n\nAdditionally, this project includes one notebook and one script in the `tutorials` directory of the\n`orchid-python-api` package:\n\n- `dom_navigation_tutorial.ipynb`\n- `dom_navigation_tutorial.py`\n\nThe notebook, `dom_navigation_tutorial.ipynb`, demonstrates using the Orchid Python API class,\n`SearchableProjectObjects`, to navigate a project. The `SearchableProjectObjects` provides:\n\n- Three query methods:\n    - `all_names()`\n    - `all_display_names()`\n    - `all_object_ids()`\n- Three specific search methods:\n    - `find_by_name()`\n    - `find_by_display_name()`\n    - `find_by_object_id()`\n- A general search method:\n    - `find()` - This method expects a predicate to identify project objects of interest\n- Two general iteration methods:\n  - `all_objects()`\n  - `SearchableProjectObjects` is an _iterator_\n\nThe script contains code similar to the notebook but runs either at the command line or in a REPL.\n\nTo use these tutorials:\n\n- You may need to\n  [configure the Orchid Python API to find the Orchid installation](#configure-the-orchid-python-api)\n- You **must**\n  [configure the Orchid Python API to find the Orchid training data](#configure-the-orchid-training-data)\n- You may need to [view the Orchid API configuration details](#view-orchid-configuration-details)\n- You may want to invoke the command, `copy_orchid_tutorials`\n\n  This command copies the tutorial files into an optionally specified (virtual environment) directory. (The\n  default destination is your current working directory.) Note that this command is a command-line script\n  that runs in a console or terminal. Additionally, this command supports a help flag, `-h` or `--help`, to\n  provide you with help on running this command.\n\nMore detailed instructions for running the tutorials can be found at:\n\n- [Run Orchid tutorials](#run-orchid-tutorials).\n\n## Getting Started\n\n### Virtual environments\n\nWe recommend the use of virtual environments to use the Orchid Python API. This choice avoids putting \nOrchid-specific packages in your system Python environment.\n\nYou have several options to create and manage virtual environments: `venv`, `pipenv`, `poetry`, and `conda`.\nThe `venv ` is available as a standard Python package and is a spartan tool to manage environments. `poetry`\nis a tool targeting developers but can be used by end-users. Our recommended tool is `pipenv`. It provides a \ngood balance between `venv ` and `poetry`. Remember, both `pipenv` and `poetry` must be installed in your \nPython environment separately from Python itself, but can be installed using `pip`. Finally, \n[conda](https://docs.conda.io/en/latest/)\n\n> is an open source package management system and environment management system that runs on Windows, macOS\n> and Linux. Conda quickly installs, runs and updates packages and their dependencies. Conda easily creates,\n> saves, loads and switches between environments on your local computer. It was created for Python programs,\n> but it can package and distribute software for any language.\n\nWe recommend the use of `pipenv`. This environment hides a number of details involved in managing a virtual\nenvironment and yet provides a fairly simple interface. We will assume in this document that you are using\n`pipenv`.\n\nAlthough we recommend `pipenv`, because we understand many of our users use `conda` (either Anaconda or\nMiniconda), we have a [section](#step-by-step-conda-install) for installing the `orchid-python-api` in a\n`conda` virtual environment.\n\nUsing any of `pipenv`, `venv` or `poetry`, your first step is to create a directory for **your** project.\nThen, change into that project directory.\n\n### Step-by-step pipenv install\n\n- Install python 3.10 by following [these installation instructions](https://docs.python.org/3/using/windows.html). To \n  ensure access from the command line, be sure to select the "Add Python 3.x to PATH" option on the\n  [installer start page](https://docs.python.org/3/_images/win_installer.png). \n- Open a console using either `powershell` or the Windows console.\n- Create a directory for the virtual environment. We will symbolically call it `/path/to/orchid-virtualenv`.\n- Change the current working directory by executing, `chdir /path/to/orchid-virtualenv`.\n- Create an empty virtual environment by running `pipenv install`.\n- Activate the virtual environment by running `pipenv shell`\n- Install Orchid by running `pip install orchid-python-api`.\n\n### Step-by-step conda install\n\n- Install [Anaconda](https://docs.anaconda.com/anaconda/install/) or\n  [Miniconda](https://docs.conda.io/en/latest/miniconda.html) following the corresponding instructions for\n  your operating system. \n- If installing on Windows, the installer will present \n  [this screen](https://docs.anaconda.com/_images/win-install-options.png). We have seen no need to install \n  Anaconda / Miniconda on your [PATH](https://en.wikipedia.org/wiki/PATH_(variable)). Although we do not\n  disagree with option to register the Anaconda / Miniconda version of Python as your default Python\n  executable, in some situations, accepting this choice can cause problems. \n- Since we will be using **both** `conda install` and `pip install` to install packages, read the article, \n  [Using Pip in a Conda Environment](https://www.anaconda.com/blog/using-pip-in-a-conda-environment). Our \n  subsequent instructions assume you have read this article and have chosen how you wish to manage these\n  two package installers together. \n  \nThe following instructions assume that you will use the simple (put perhaps not scalable) process of creating\nthe `conda` virtual environment with all packages you want to use available in the Anaconda/Miniconda\necosystem and, within that virtual environment, use `pip` to install `orchid-python-api`.\n\n- Open an Anaconda Powershell console.\n- Optionally create a directory for your work.\n    - We symbolically call it `/path/to/orchid-virtualenv`.\n    - Change to the current working directory by executing `chdir /path/to/orchid-virtualenv`.\n- Create an empty virtual environment by running `conda create --name <your-virtualenv-name> python=3.10`.\n- Activate the virtual environment by running `conda activate <your-virtualenv_name>`\n- Install Orchid by running `pip install orchid-python-api`.\n\n### Using a requirements file\n\nAn alternative method used by customers uses a requirements file, `requirements.txt`, that we create as part of our\nrelease process but **do not** include in our distribution. \n[This file](https://github.com/Reveal-Energy-Services/orchid-python-api/blob/master/requirements.txt) is available\nfrom our GitHub repository. For `pipenv`, use \n[these import instructions](https://pipenv-fork.readthedocs.io/en/latest/basics.html#importing-from-requirements-txt). For\n`conda`, read the accepted answer to this \n[Stack Overflow post](https://stackoverflow.com/questions/63379968/using-requirements-txt-to-automatically-install-packages-from-conda-channels-and)\nfor the correct command and additional options you may need to consider.\n\n### Configure the Orchid Python API\n\nThe Orchid Python API requires a licensed Orchid installation on your workstation. Depending on the details of\nthe installation, you may need to configure the Orchid Python API to refer to different locations.\n\n#### Using the fallback configuration\n\nIf you installed the latest version Orchid using the installation defaults, and you installed the\n`orchid-python-api` using the [pipenv installation instructions](#step-by-step-pipenv-install) or \nthe [conda installation instructions](#step-by-step-conda-install), you need to take **no** additional\nsteps to configure the Orchid Python API to find this installation. For your information, the default\ninstallation location is, `%ProgramFiles%\\Reveal Energy Services\\Orchid`. The Orchid Python API uses the API\nversion to find and use the corresponding version of Orchid.\n\n#### Using an environment variable\n\nThis mechanism is perhaps the easiest procedure to create an Orchid Python API configuration that changes \nrarely and is available to all your tools. It works best with a system restart. (Environment variables can be \nmade available for a narrow set of tools on your system or available to all your tools depending on arcane\ntechnical rules that you need not understand.) \n\nTo use environment variables to configure the Orchid Python API, you will need to create the environment\nvariable `ORCHID_ROOT` and set its value to the path of the `PythonApiLibs` directory beneath the Orchid\ninstallation directory. (For your information, the `PythonApiLibs` directory containing the version-specific\nOrchid binary and configuration files should be in a subdirectory like \n`ORCHID_ROOT/Orchid-2020.4.232/PythonApiLibs` when you accept the installation defaults.) \n\nThis section assumes you want to create a long-term configuration that survives a system restart and is\navailable to all your tools. Symbolically, this document will refer to the directory containing the binaries\nrequired by the Orchid Python API as `/path-to/orchid/version/python-api-libs`.\n\nTo create the required environment variable, enter the search term "environment variables" in the Windows-10 \nsearch box and select the item named, "Edit environment variables for your account." The system will then \npresent you with the "Environment Variables" dialog. Under the section named "User variables for \n<your.username>", click the "New" button. In the "Variable name" text box, enter "ORCHID_ROOT". (These two \nwords are separated by the underscore symbol.)\n\nNavigate to the "Variable Value" text box. Click the "Browse Directory" button to select the directory into\nwhich Orchid is installed, `/path-to/orchid/version/python-api-libs`. This action pastes the directory\nname into the "Variable Value" text box. Verify that the directory is correct, and then click "OK". Verify\nthat you see the name `ORCHID_ROOT` with the correct value in the "User variables for <your.username>" list.\nFinally, click "OK" to dismiss the "Environment Variables" dialog.\n\nAlthough you have created the `ORCHID_ROOT` environment variable with the appropriate value, only "new" opened\ntools can use that variable. However, the details of "new" is technical and may not correspond to what you\nexpect. If you understand these details, you can jump to \n[Verify Installation](#verify-installation). If you are not confident of these details, restart\nyour system before proceeding to [Verify Installation](#verify-installation).\n\n#### Using a configuration file\n\nAnother option to configure the Orchid Python API is by creating a configuration file. A configuration file is\neasier to change than an environment variable and does not require a system restart to work best. However, it\nrequires more knowledge and work on your part. In general, a configuration file is better if your requirements\nchange "often". For example, if you are working with multiple, side-by-side Orchid versions and Orchid Python \nAPI versions, you may find it faster and easier to create a configuration file once and change it as you \nchange Orchid / Orchid Python API versions.\n\nTo use a file to configure the Orchid Python API, you will need to create a configuration file named\n`python_api.yaml` and set the value of the `orchid` > `root` key to the path of the `PythonApiLibs` directory\nbeneath the Orchid installation directory. (For your information, the `PythonApiLibs` directory containing the\nversion-specific Orchid binary and configuration files should be in a subdirectory like\n`ORCHID_ROOT/Orchid-2020.4.232/PythonApiLibs` when you accept the installation defaults.)\n\nSymbolically, this document will refer to the directory containing the binaries required by the\nOrchid Python API as `/path-to/orchid/version/python-api-libs`.\n\nTo create a configuration file used by the Orchid Python API, you must:\n\n- Create the directory, `/path/to/home-directory/.orchid`, where `/path/to/home-directory` is a symbolic\n  reference to your home directory.\n- Create the file, `python_api.yaml` in `/path/to/home-directory/.orchid`.\n\nTechnically, the format of the file is `YAML` ("YAML Ain\'t Markup Language"), a "human friendly data\nserialization standard". (For technical details, visit [the website](https://yaml.org/). For a gentler\nintroduction, visit [the Wikipedia entry](https://en.wikipedia.org/wiki/YAML) or read / watch one of the many\n`YAML` introductions / tutorials.)\n\nBecause these articles describe `YAML` generally, they **do not** describe the details of the `YAML` document\nexpected by the Orchid Python API. We, however, distribute an example file name `python_api.yaml.example` in\neach installed `orchid-python-api` package. Assuming you created a virtual environment as described in\nthe step-by-step [pipenv installation instructions](#step-by-step-pipenv-install) or\nthe [conda installation instructions](#step-by-step-conda-install) section, you can find this example file,\n`python_api.yaml.example`, in the directory,\n`/path/to/orchid-virtualenv/Lib/site-packages/orchid_python_api/examples`. \n\nTo use this configuration file as an example:\n\n- Copy the file to the expected location. For example, assuming the symbolic names referenced above, execute:\n  ```\n  copy /path/to/orchid-virtualenv/Lib/site-packages/orchid_python_api/examples/python_api.yaml.example /path/to/home-directory/.orchid/python_api.yaml\n  ```\n- Edit the copied file, `/path/to/home-directory/.orchid/python_api.yaml`, using your favorite **text** editor.\n\nThe example file, contains comments, introduced by a leading octothorpe character (#, number sign, or hash),\nthat describe the information expected by the Orchid Python API. In summary, you\'ll need to provide a value\nfor the `orchid` > `root` key that contains (symbolically), `/path-to/orchid/version/python-api-libs`.\n\nIf you want to ensure your configuration is correct,\n[view the Orchid API configuration details](#view-orchid-configuration-details).\n\n### Configure the Orchid training data\n\nUsing the Orchid Python API **requires** a licensed Orchid installation on your workstation. However,\nto use the example Jupyter notebooks or scripts, you **must** configure the Orchid Python API to find the\nOrchid training data.\n\n#### Using an environment variable\n\nThis mechanism is perhaps the easiest procedure to create an Orchid Python API configuration that changes \nrarely and is available to all your tools. It works best with a system restart. (Environment variables can be \nmade available for a narrow set of tools on your system or available to all your tools depending on arcane\ntechnical rules that you need not understand.) \n\nTo use environment variables to configure the Orchid Python API to find the Orchid training data, you will \nneed to create the environment variable `ORCHID_TRAINING_DATA` and set its value to the location of the Orchid \ntraining data.\n\nThis document assumes you want to create a long-term configuration that survives a system restart and is \navailable to all your tools. Symbolically, this document will refer to the Orchid training data location as\n`/path-to/orchid/training-data`. \n\nTo create the required environment variable, enter the search term "environment variables" in the Windows-10 \nsearch box and select the item named, "Edit environment variables for your account." The system will then \npresent your with the "Environment Variables" dialog. Under the section named "User variables for \n<your.username>", click the "New" button. In the "Variable name" text box, enter "ORCHID_TRAINING_DATA".\n(These three words are separated by the underscore symbol.)\n\nNavigate to the "Variable Value" text box. Click the "Browse Directory" button to select the directory \ncontaining the Orchid training data, `/path-to/orchid/training-data`. This action pastes the directory name\ninto the "Variable Value" text box. Verify that the directory is correct, and then click "OK". Verify that\nyou see the name `ORCHID_TRAINING_DATA` with the correct value in the "User variables for <your.username>"\nlist. Finally, click "OK" to dismiss the "Environment Variables" dialog.\n\nAlthough you have now created the `ORCHID_TRAINING_DATA` environment variable with the appropriate value,\nonly "new" tools can now use that variable. However, the details of "new" is technical and may not correspond\nto your what you expect. If you understand these details, you can jump to\n[Verify Installation](#verify-installation). If you are not confident of these details, restart\nyour system before proceeding to [Verify Installation](#verify-installation).\n\n#### Using a configuration file\n\nAnother option to configure the Orchid Python API to find the Orchid training data is by creating a \nconfiguration file. A configuration file is easier to change than an environment variable and does not require \na system restart to work best. However, it requires more knowledge and work on your part. In general, a \nconfiguration file is better if your requirements change "often". For example, if you are working with \nmultiple, side-by-side Orchid versions and Orchid Python API versions, you may find it faster and easier to\ncreate a configuration file once and change it as you change Orchid / Orchid Python API versions or training\ndata locations.\n\nTo create a configuration file used by the Orchid Python API, you create a file named `python_api.yaml`\nand put it in the directory, `/path/to/home-directory/.orchid`, where `/path/to/home-directory` is a \nsymbolic reference to your home directory. Technically, the format of the file is `YAML` ("YAML Ain\'t Markup\nLanguage"), a "human friendly data serialization standard". (For technical details, visit\n[the website](https://yaml.org/). For a gentler introduction, visit \n[the Wikipedia entry](https://en.wikipedia.org/wiki/YAML) or read / watch on of the many `YAML` \nintroductions / tutorials.)\n\nBecause these articles describe `YAML` generally, they **do not** describe the details of the `YAML` document\nexpected by the Orchid Python API. We, however, distribute an example file name `python_api.yaml.example` in\neach installed `orchid-python-api` package. Assuming you created a virtual environment as described in\nthe step-by-step [pipenv installation instructions](#step-by-step-pipenv-install) or the \n[conda installation instructions](#step-by-step-conda-install), you can find this example file,\n`python_api.yaml.example`, in the directory,\n`/path/to/orchid-virtualenv/Lib/site-packages/orchid_python_api/examples`.\n\nTo use this configuration file as an example:\n\n- Copy the file to the expected location. For example, assuming the symbolic names referenced above, execute\n  the command\n  \n  ```\n  copy /path/to/orchid-virtualenv/Lib/site-packages/orchid_python_api/examples/python_api.yaml.example /path/to/home-directory/.orchid/python_api.yaml\n  ```  \n  \n- Edit the copied file, `/path/to/home-directory/.orchid/python_api.yaml`, using your favorite **text** editor.\n\nThe example file, contains comments, introduced by a leading octothorpe character (#, number sign, or hash),\nthat describe the information expected by the Orchid Python API. In summary, you\'ll need to provide a value\nfor the \'orchid\' > \'training_data\' key that contains the pathname of the directory containing the Orchid\ntraining data files.\n\nIf you want to ensure your configuration is correct,\n[view the Orchid API configuration details](#view-orchid-configuration-details).\n\n## Verify installation\n\n### Jupyter lab\n\n- In your activated virtual environment, run `jupyter lab` to open a browser tab.\n- In the first cell, enter `import orchid`.\n- Run the cell.\n- Wait patiently.\n\nThe import should complete with no errors.\n\n### Python REPL\n\n- In your activated virtual environment, run either `python` or `ipython` to open a REPL.\n- Enter `import orchid`.\n- Wait patiently.\n\nThe import should complete with no errors.\n\n## Run Orchid high-level examples\n\n- If you have not already done so, \n[configure the Orchid Python API to find the Orchid installation](#configure-the-orchid-python-api)\n- You **must** \n[configure the Orchid Python API to find the Orchid training data](#configure-the-orchid-training-data)\n- Navigate to the directory associated with the virtual environment\n- If necessary, activate the virtual environment by executing either \n    - `pipenv shell` or \n    - `conda activate <your-virtualenv_name>`.\n- Run `copy_orchid_examples`\n- If the script reports that it skipped notebooks or scripts, repeat the command with an additional argument:  \n  `copy_orchid_examples --overwrite`\n- Verify that the current directory has six example notebooks:\n    - `completion_analysis.ipynb`\n    - `plot_time_series.ipynb`\n    - `plot_trajectories.ipynb`\n    - `plot_treatment.ipynb`\n    - `search_data_frames.ipynb`\n    - `volume_2_first_response.ipynb`\n- Verify that the current directory has nine example scripts:\n    - `completion_analysis.py`\n    - `plot_time_series.py`\n    - `plot_trajectories.py`\n    - `plot_treatment.py`\n    - `search_data_frames.py`\n    - `volume_2_first_response.py`\n    - `stage_qc_results.py`\n    - `change_stage_times.py`\n    - `add_stages.py`\n\n### Run high-level example scripts\n\n- Run the first script\n    - Execute the command `python plot_trajectories.py`\n    - Wait patiently for the `matplotlib` plot window to appear.\n    - Ensure the plot is correct.\n    - Dismiss the `matplotlib` window.\n- Repeat for these scripts:\n    - `plot_treatment.py`\n    - `plot_time_series.py` \n    - `completion_analysis.py` (This script prints multiple messages and presents **multiple** plots.\n       You must dismiss each plot to continue.)\n    - `volume_2_first_response.py`\n    - `search_data_frames.py`\n- Run the `stage_qc_results.py` script.\n- Run the `change_stage_times.py` script.\n- Run the `add_stages.py` script.\n\nThe scripts, `stage_qc_results.py`, `change_stage_times.py`, and `add_stages.py`, differ from the other scripts. These\nscripts require a number of command line arguments to run correctly.\n\nFor example, to see an explanation of these arguments, execute any of this scripts with the `--help` option.\nThe most typical arguments are described in the following paragraphs.\n\nTo both read and write stage QC results, run the command:\n```\npython stage_qc_results.py -v2 /path/to/orchid-traing-data/frankNstein_Bakken_UTM13_FEET.v11.ifrac \n```\n\nTo only read the existing stage QC data, run the command\n```\npython stage_qc_results.py -v2 --read-only /path/to/orchid-traing-data/frankNstein_Bakken_UTM13_FEET.ifrac\n```\n\nTo change the stage start and stop times (the time range), run the command\n```\npython change_stage_times.py -v2 /path/to/orchid-traing-data/frankNstein_Bakken_UTM13_FEET.ifrac \n```\n\nTo add stages to a well, run the command\n```\npython add_stages.py -v2 /path/to/orchid-traing-data/frankNstein_Bakken_UTM13_FEET.v11.ifrac \n```\n\n### Run high-level example notebooks\n\n- Open Jupyter by running `jupyter lab` in the shell\n- Within Jupyter,\n    - Successfully run notebook, `plot_trajectories.ipynb`\n        1. Open notebook\n        2. Run all cells of notebook\n        3. Wait patiently\n        4. Verify that no exceptions occurred\n    - Repeat for remaining notebooks:\n        - `plot_time_series.ipynb`\n        - `plot_treatment.ipynb`\n        - `completion_analysis.ipynb`\n        - `volume_2_first_response.ipynb`\n        - `search_data_frames.ipynb`\n\n## Run Orchid tutorials\n\n- If you have not already done so,\n  [configure the Orchid Python API to find the Orchid installation](#configure-the-orchid-python-api)\n- You **must**\n  [configure the Orchid Python API to find the Orchid training data](#configure-the-orchid-training-data)\n- Navigate to the directory associated with the virtual environment\n- If necessary, activate the virtual environment by executing either\n    - `pipenv shell` or\n    - `conda activate <your-virtualenv_name>`.\n- Run `copy_orchid_tutorials.exe`\n- If the script reports that it skipped notebooks or scripts, repeat the command with an additional argument:  \n  `python </path/to/virtualenv/Lib/site-packages/copy_orchid_tutorials.py --overwrite`\n- Verify that the current directory has one tutorial notebooks:\n    - `dom_navigation_tutorial.ipynb`\n- Verify that the current directory has five example scripts:\n    - `dom_navigation_tutorial.py`\n\n### Run tutorial script\n\n- Run the `dom_navigation_tutorial.py` script\n    - Execute the command `python dom_navigation_tutorial.py`\n    - Follow the on-screen messages to advance through the tutorial\n\n### Run tutorial notebook\n\n- Open Jupyter by running `jupyter lab` in the shell\n- Within Jupyter,\n    - Run the notebook, `dom_navigation_tutorial.ipynb`\n        1. Open the notebook in `jupyter`\n        2. Run each cell of the notebook. Typically, this process involves\n            - Read the instructions or comments preceding the code cell(s)\n            - Observe the result of executing the code\n\n## View Orchid Configuration Details\n\nTo "debug" the Orchid Python API configuration, perform the following steps:\n\n- Change to the directory associated with your Python virtual environment.\n- If necessary, activate the virtual environment.\n- Within that virtual environment, invoke Python. It is important to create a new REPL so that you start with\n  a "clean" environment.\n- Within the Python REPL, execute the following commands.\n\n  ```\n  import logging\n  logging.basicConfig(level=logging.DEBUG)\n  import orchid\n  ```\n  \nEnabling logging **before** importing is critical. If you have already imported `orchid`, the simplest\nsolution is to close this REPL and create another, "clean" REPL.\n\nYou should see output like the following:\n\n```\nDEBUG:orchid.configuration:fallback configuration={\'orchid\': {\'root\': \'C:\\\\Program Files\\\\Reveal Energy Services\\\\Orchid\\\\Orchid-2020.4.361\'}}\nDEBUG:orchid.configuration:file configuration={\'orchid\': {\'root\': \'c:\\\\path-to\\\\bin\\\\x64\\\\Debug\\\\net48\', \'training_data \': \'c:\\\\path-to\\\\installed-training-data\'}}\nDEBUG:orchid.configuration:environment configuration = {\'orchid\': {\'root\': \'c:\\\\another\\\\path-to\\bin\\\\x64\\\\Debug\\\\net48\'}}\nDEBUG:orchid.configuration:result configuration={\'orchid\': {\'root\': \'c:\\\\another\\\\path-to\\bin\\\\x64\\\\Debug\\\\net48\'}}\n```\n\nThis output describes four details of the configuration.\n\n| Configuration | Explanation                                                            |\n|---------------|------------------------------------------------------------------------|\n| fallback      | The always available configuration (may be empty)                      |\n| file          | The configuration specified in your configuration file (may be empty)  |\n| environment   | The configuration specified using environment variables (may be empty) | \n| result        | The configuration used by the Orchid Python API (should not be empty)  |\n\n',
-    'author': 'Reveal Energy Services, Inc.',
-    'author_email': 'support@reveal-energy.com',
-    'maintainer': 'Reveal Energy Services, Inc.',
-    'maintainer_email': 'support@reveal-energy.com',
-    'url': 'https://github.com/Reveal-Energy-Services/orchid-python-api',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<3.11',
-}
+## Introduction 
+
+This project defines the implementation of the Python API for Orchid*.
+
+Specifically, the `orchid` package makes Orchid features available to Python applications and to the
+Python REPL.
+
+(* Orchid is a mark of Reveal Energy Services, Inc.)
+
+### A Reading Suggestion
+
+This document is one of several documents you may want to read:
+
+- [README](./README.md) - This file.
+- [README-dev.md](./README-dev.md) - A similar file targeting for package developers.
+- [ReleaseNotes.md](./ReleaseNotes.md) - The release notes for this project.
+
+Additionally, as part of the 2022.4 release, we upgraded `pythonnet`, the package we use to expose .NET to the Python
+runtime, from version 2.5.2 to version 3.0.0.post1. This upgrade is a breaking upgrade. The document, 
+[README-pythonnet3.md](./README-pythonnet3.md), describes the changes that we needed to make to the Orchid Python API to
+repair failing internal tests. The document, [README-pythonnet3-low.md](./README-pythonnet3-low.md), describes the 
+changes that we needed to make to the Orchid Python API to repair failing low-level examples.
+
+Although one can read this document in any text editor since it is simply a text file, consider installing
+the [Python grip utility](https://pypi.org/project/grip/). This application allows one to "render local readme
+files before sending off to GitHub". Although you need not send any of these file to `GitHub`, by using `grip` 
+to render the file, you can much more easily navigate the document links.
+
+## Examples
+
+### High-level examples
+
+This project includes eight scripts and six notebooks in the `examples` directory of the `orchid-python-api` package:
+
+| Name                            | Demonstrates...                                                                     |
+|---------------------------------|-------------------------------------------------------------------------------------|
+| `completion_analysis.ipynb`     | A detailed analysis of the completion performed on two different wells in a project |
+| `plot_trajectories.ipynb`       | Plotting the well trajectories for a project                                        |
+| `plot_time_series.ipynb`        | Plotting the monitor curves for a project                                           |
+| `plot_treatment.ipynb`          | Plotting the treatment curves for a specific stage of a well in a project           | 
+| `search_data_frames.ipynb`      | Searching object collections and our data frame access                              | 
+| `volume_2_first_response.ipynb` | Using derivatives to calculate the fluid volume pumped before the first response    | 
+
+Six of the eight scripts contain the same code as the notebooks but run either at the command line or in a REPL. The
+last three scripts:
+
+| Name                            | Demonstrates using the high-level Python API to...                               |
+|---------------------------------|----------------------------------------------------------------------------------|
+| `stage_qc_results.py`           | Read and write QC results for a stage. (Replaces low-level `stage_qc_status.py`) |
+| `change_stage_times.py`         | Change the start and stop times (the time range) of a stage                      |
+| `add_stages.py`                 | Add one or more stages to a well. (Improvement over `add_stages_low.py`)         |
+
+### Low-level examples
+
+In addition, this project includes five scripts and a notebook in the `examples/low_level` directory of the
+`orchid-python-api` package:
+
+| Name                                      | Demonstrates...                                                  |
+|-------------------------------------------|------------------------------------------------------------------|
+| `auto_pick.py`                            | Automatically pick observations and save them to an .ifrac file  |
+| `auto_pick_and_create_stage_attribute.py` | Create and save stage attributes                                 |
+| `auto_pick_iterate_example.py`            | Use iteration to find visible stages instead of .NET method      |
+| `monitor_time_series.py`                  | Find high-level time series from a low-level monitor time series | 
+| `add_stages_low.py`                       | Adds newly created stages to a well of a project                 | 
+| `multi_picking_events.py`                 | Creates and adds a number of multi-picking events                |
+
+The notebook, `auto_pick.ipynb` contain the same code as the script, `auto_pick.py`, but runs in a Jupyter
+notebook.
+ 
+To use these examples: 
+
+- You may need to 
+  [configure the Orchid Python API to find the Orchid installation](#configure-the-orchid-python-api)
+- You **must** 
+  [configure the Orchid Python API to find the Orchid training data](#configure-the-orchid-training-data)
+- You may need to [view the Orchid API configuration details](#view-orchid-configuration-details)
+- You may want to invoke the command, `copy_orchid_examples`
+
+    This command copies the example files into an optionally specified (virtual environment) directory. (The 
+    default destination is your current working directory.) Note that this command is a command-line script 
+    that runs in a console or terminal. Additionally, this command supports a help flag, `-h` or `--help`, to 
+    provide you with help on running this command.
+
+More detailed instructions for running the examples can be found at:
+
+- [Run Orchid high-level examples](#run-orchid-high-level-examples).
+
+## Tutorials
+
+Additionally, this project includes one notebook and one script in the `tutorials` directory of the
+`orchid-python-api` package:
+
+- `dom_navigation_tutorial.ipynb`
+- `dom_navigation_tutorial.py`
+
+The notebook, `dom_navigation_tutorial.ipynb`, demonstrates using the Orchid Python API class,
+`SearchableProjectObjects`, to navigate a project. The `SearchableProjectObjects` provides:
+
+- Three query methods:
+    - `all_names()`
+    - `all_display_names()`
+    - `all_object_ids()`
+- Three specific search methods:
+    - `find_by_name()`
+    - `find_by_display_name()`
+    - `find_by_object_id()`
+- A general search method:
+    - `find()` - This method expects a predicate to identify project objects of interest
+- Two general iteration methods:
+  - `all_objects()`
+  - `SearchableProjectObjects` is an _iterator_
+
+The script contains code similar to the notebook but runs either at the command line or in a REPL.
+
+To use these tutorials:
+
+- You may need to
+  [configure the Orchid Python API to find the Orchid installation](#configure-the-orchid-python-api)
+- You **must**
+  [configure the Orchid Python API to find the Orchid training data](#configure-the-orchid-training-data)
+- You may need to [view the Orchid API configuration details](#view-orchid-configuration-details)
+- You may want to invoke the command, `copy_orchid_tutorials`
+
+  This command copies the tutorial files into an optionally specified (virtual environment) directory. (The
+  default destination is your current working directory.) Note that this command is a command-line script
+  that runs in a console or terminal. Additionally, this command supports a help flag, `-h` or `--help`, to
+  provide you with help on running this command.
+
+More detailed instructions for running the tutorials can be found at:
+
+- [Run Orchid tutorials](#run-orchid-tutorials).
+
+## Getting Started
+
+### Virtual environments
+
+We recommend the use of virtual environments to use the Orchid Python API. This choice avoids putting 
+Orchid-specific packages in your system Python environment.
+
+You have several options to create and manage virtual environments: `venv`, `pipenv`, `poetry`, and `conda`.
+The `venv ` is available as a standard Python package and is a spartan tool to manage environments. `poetry`
+is a tool targeting developers but can be used by end-users. Our recommended tool is `pipenv`. It provides a 
+good balance between `venv ` and `poetry`. Remember, both `pipenv` and `poetry` must be installed in your 
+Python environment separately from Python itself, but can be installed using `pip`. Finally, 
+[conda](https://docs.conda.io/en/latest/)
+
+> is an open source package management system and environment management system that runs on Windows, macOS
+> and Linux. Conda quickly installs, runs and updates packages and their dependencies. Conda easily creates,
+> saves, loads and switches between environments on your local computer. It was created for Python programs,
+> but it can package and distribute software for any language.
+
+We recommend the use of `pipenv`. This environment hides a number of details involved in managing a virtual
+environment and yet provides a fairly simple interface. We will assume in this document that you are using
+`pipenv`.
+
+Although we recommend `pipenv`, because we understand many of our users use `conda` (either Anaconda or
+Miniconda), we have a [section](#step-by-step-conda-install) for installing the `orchid-python-api` in a
+`conda` virtual environment.
+
+Using any of `pipenv`, `venv` or `poetry`, your first step is to create a directory for **your** project.
+Then, change into that project directory.
+
+### Step-by-step pipenv install
+
+- Install python 3.10 by following [these installation instructions](https://docs.python.org/3/using/windows.html). To 
+  ensure access from the command line, be sure to select the "Add Python 3.x to PATH" option on the
+  [installer start page](https://docs.python.org/3/_images/win_installer.png). 
+- Open a console using either `powershell` or the Windows console.
+- Create a directory for the virtual environment. We will symbolically call it `/path/to/orchid-virtualenv`.
+- Change the current working directory by executing, `chdir /path/to/orchid-virtualenv`.
+- Create an empty virtual environment by running `pipenv install`.
+- Activate the virtual environment by running `pipenv shell`
+- Install Orchid by running `pip install orchid-python-api`.
+
+### Step-by-step conda install
+
+- Install [Anaconda](https://docs.anaconda.com/anaconda/install/) or
+  [Miniconda](https://docs.conda.io/en/latest/miniconda.html) following the corresponding instructions for
+  your operating system. 
+- If installing on Windows, the installer will present 
+  [this screen](https://docs.anaconda.com/_images/win-install-options.png). We have seen no need to install 
+  Anaconda / Miniconda on your [PATH](https://en.wikipedia.org/wiki/PATH_(variable)). Although we do not
+  disagree with option to register the Anaconda / Miniconda version of Python as your default Python
+  executable, in some situations, accepting this choice can cause problems. 
+- Since we will be using **both** `conda install` and `pip install` to install packages, read the article, 
+  [Using Pip in a Conda Environment](https://www.anaconda.com/blog/using-pip-in-a-conda-environment). Our 
+  subsequent instructions assume you have read this article and have chosen how you wish to manage these
+  two package installers together. 
+  
+The following instructions assume that you will use the simple (put perhaps not scalable) process of creating
+the `conda` virtual environment with all packages you want to use available in the Anaconda/Miniconda
+ecosystem and, within that virtual environment, use `pip` to install `orchid-python-api`.
+
+- Open an Anaconda Powershell console.
+- Optionally create a directory for your work.
+    - We symbolically call it `/path/to/orchid-virtualenv`.
+    - Change to the current working directory by executing `chdir /path/to/orchid-virtualenv`.
+- Create an empty virtual environment by running `conda create --name <your-virtualenv-name> python=3.10`.
+- Activate the virtual environment by running `conda activate <your-virtualenv_name>`
+- Install Orchid by running `pip install orchid-python-api`.
+
+### Using a requirements file
+
+An alternative method used by customers uses a requirements file, `requirements.txt`, that we create as part of our
+release process but **do not** include in our distribution. 
+[This file](https://github.com/Reveal-Energy-Services/orchid-python-api/blob/master/requirements.txt) is available
+from our GitHub repository. For `pipenv`, use 
+[these import instructions](https://pipenv-fork.readthedocs.io/en/latest/basics.html#importing-from-requirements-txt). For
+`conda`, read the accepted answer to this 
+[Stack Overflow post](https://stackoverflow.com/questions/63379968/using-requirements-txt-to-automatically-install-packages-from-conda-channels-and)
+for the correct command and additional options you may need to consider.
+
+### Configure the Orchid Python API
+
+The Orchid Python API requires a licensed Orchid installation on your workstation. Depending on the details of
+the installation, you may need to configure the Orchid Python API to refer to different locations.
+
+#### Using the fallback configuration
+
+If you installed the latest version Orchid using the installation defaults, and you installed the
+`orchid-python-api` using the [pipenv installation instructions](#step-by-step-pipenv-install) or 
+the [conda installation instructions](#step-by-step-conda-install), you need to take **no** additional
+steps to configure the Orchid Python API to find this installation. For your information, the default
+installation location is, `%ProgramFiles%\Reveal Energy Services\Orchid`. The Orchid Python API uses the API
+version to find and use the corresponding version of Orchid.
+
+#### Using an environment variable
+
+This mechanism is perhaps the easiest procedure to create an Orchid Python API configuration that changes 
+rarely and is available to all your tools. It works best with a system restart. (Environment variables can be 
+made available for a narrow set of tools on your system or available to all your tools depending on arcane
+technical rules that you need not understand.) 
+
+To use environment variables to configure the Orchid Python API, you will need to create the environment
+variable `ORCHID_ROOT` and set its value to the path of the `PythonApiLibs` directory beneath the Orchid
+installation directory. (For your information, the `PythonApiLibs` directory containing the version-specific
+Orchid binary and configuration files should be in a subdirectory like 
+`ORCHID_ROOT/Orchid-2020.4.232/PythonApiLibs` when you accept the installation defaults.) 
+
+This section assumes you want to create a long-term configuration that survives a system restart and is
+available to all your tools. Symbolically, this document will refer to the directory containing the binaries
+required by the Orchid Python API as `/path-to/orchid/version/python-api-libs`.
+
+To create the required environment variable, enter the search term "environment variables" in the Windows-10 
+search box and select the item named, "Edit environment variables for your account." The system will then 
+present you with the "Environment Variables" dialog. Under the section named "User variables for 
+<your.username>", click the "New" button. In the "Variable name" text box, enter "ORCHID_ROOT". (These two 
+words are separated by the underscore symbol.)
+
+Navigate to the "Variable Value" text box. Click the "Browse Directory" button to select the directory into
+which Orchid is installed, `/path-to/orchid/version/python-api-libs`. This action pastes the directory
+name into the "Variable Value" text box. Verify that the directory is correct, and then click "OK". Verify
+that you see the name `ORCHID_ROOT` with the correct value in the "User variables for <your.username>" list.
+Finally, click "OK" to dismiss the "Environment Variables" dialog.
+
+Although you have created the `ORCHID_ROOT` environment variable with the appropriate value, only "new" opened
+tools can use that variable. However, the details of "new" is technical and may not correspond to what you
+expect. If you understand these details, you can jump to 
+[Verify Installation](#verify-installation). If you are not confident of these details, restart
+your system before proceeding to [Verify Installation](#verify-installation).
+
+#### Using a configuration file
+
+Another option to configure the Orchid Python API is by creating a configuration file. A configuration file is
+easier to change than an environment variable and does not require a system restart to work best. However, it
+requires more knowledge and work on your part. In general, a configuration file is better if your requirements
+change "often". For example, if you are working with multiple, side-by-side Orchid versions and Orchid Python 
+API versions, you may find it faster and easier to create a configuration file once and change it as you 
+change Orchid / Orchid Python API versions.
+
+To use a file to configure the Orchid Python API, you will need to create a configuration file named
+`python_api.yaml` and set the value of the `orchid` > `root` key to the path of the `PythonApiLibs` directory
+beneath the Orchid installation directory. (For your information, the `PythonApiLibs` directory containing the
+version-specific Orchid binary and configuration files should be in a subdirectory like
+`ORCHID_ROOT/Orchid-2020.4.232/PythonApiLibs` when you accept the installation defaults.)
+
+Symbolically, this document will refer to the directory containing the binaries required by the
+Orchid Python API as `/path-to/orchid/version/python-api-libs`.
+
+To create a configuration file used by the Orchid Python API, you must:
+
+- Create the directory, `/path/to/home-directory/.orchid`, where `/path/to/home-directory` is a symbolic
+  reference to your home directory.
+- Create the file, `python_api.yaml` in `/path/to/home-directory/.orchid`.
+
+Technically, the format of the file is `YAML` ("YAML Ain't Markup Language"), a "human friendly data
+serialization standard". (For technical details, visit [the website](https://yaml.org/). For a gentler
+introduction, visit [the Wikipedia entry](https://en.wikipedia.org/wiki/YAML) or read / watch one of the many
+`YAML` introductions / tutorials.)
+
+Because these articles describe `YAML` generally, they **do not** describe the details of the `YAML` document
+expected by the Orchid Python API. We, however, distribute an example file name `python_api.yaml.example` in
+each installed `orchid-python-api` package. Assuming you created a virtual environment as described in
+the step-by-step [pipenv installation instructions](#step-by-step-pipenv-install) or
+the [conda installation instructions](#step-by-step-conda-install) section, you can find this example file,
+`python_api.yaml.example`, in the directory,
+`/path/to/orchid-virtualenv/Lib/site-packages/orchid_python_api/examples`. 
+
+To use this configuration file as an example:
+
+- Copy the file to the expected location. For example, assuming the symbolic names referenced above, execute:
+  ```
+  copy /path/to/orchid-virtualenv/Lib/site-packages/orchid_python_api/examples/python_api.yaml.example /path/to/home-directory/.orchid/python_api.yaml
+  ```
+- Edit the copied file, `/path/to/home-directory/.orchid/python_api.yaml`, using your favorite **text** editor.
+
+The example file, contains comments, introduced by a leading octothorpe character (#, number sign, or hash),
+that describe the information expected by the Orchid Python API. In summary, you'll need to provide a value
+for the `orchid` > `root` key that contains (symbolically), `/path-to/orchid/version/python-api-libs`.
+
+If you want to ensure your configuration is correct,
+[view the Orchid API configuration details](#view-orchid-configuration-details).
+
+### Configure the Orchid training data
+
+Using the Orchid Python API **requires** a licensed Orchid installation on your workstation. However,
+to use the example Jupyter notebooks or scripts, you **must** configure the Orchid Python API to find the
+Orchid training data.
+
+#### Using an environment variable
+
+This mechanism is perhaps the easiest procedure to create an Orchid Python API configuration that changes 
+rarely and is available to all your tools. It works best with a system restart. (Environment variables can be 
+made available for a narrow set of tools on your system or available to all your tools depending on arcane
+technical rules that you need not understand.) 
+
+To use environment variables to configure the Orchid Python API to find the Orchid training data, you will 
+need to create the environment variable `ORCHID_TRAINING_DATA` and set its value to the location of the Orchid 
+training data.
+
+This document assumes you want to create a long-term configuration that survives a system restart and is 
+available to all your tools. Symbolically, this document will refer to the Orchid training data location as
+`/path-to/orchid/training-data`. 
+
+To create the required environment variable, enter the search term "environment variables" in the Windows-10 
+search box and select the item named, "Edit environment variables for your account." The system will then 
+present your with the "Environment Variables" dialog. Under the section named "User variables for 
+<your.username>", click the "New" button. In the "Variable name" text box, enter "ORCHID_TRAINING_DATA".
+(These three words are separated by the underscore symbol.)
+
+Navigate to the "Variable Value" text box. Click the "Browse Directory" button to select the directory 
+containing the Orchid training data, `/path-to/orchid/training-data`. This action pastes the directory name
+into the "Variable Value" text box. Verify that the directory is correct, and then click "OK". Verify that
+you see the name `ORCHID_TRAINING_DATA` with the correct value in the "User variables for <your.username>"
+list. Finally, click "OK" to dismiss the "Environment Variables" dialog.
+
+Although you have now created the `ORCHID_TRAINING_DATA` environment variable with the appropriate value,
+only "new" tools can now use that variable. However, the details of "new" is technical and may not correspond
+to your what you expect. If you understand these details, you can jump to
+[Verify Installation](#verify-installation). If you are not confident of these details, restart
+your system before proceeding to [Verify Installation](#verify-installation).
+
+#### Using a configuration file
+
+Another option to configure the Orchid Python API to find the Orchid training data is by creating a 
+configuration file. A configuration file is easier to change than an environment variable and does not require 
+a system restart to work best. However, it requires more knowledge and work on your part. In general, a 
+configuration file is better if your requirements change "often". For example, if you are working with 
+multiple, side-by-side Orchid versions and Orchid Python API versions, you may find it faster and easier to
+create a configuration file once and change it as you change Orchid / Orchid Python API versions or training
+data locations.
+
+To create a configuration file used by the Orchid Python API, you create a file named `python_api.yaml`
+and put it in the directory, `/path/to/home-directory/.orchid`, where `/path/to/home-directory` is a 
+symbolic reference to your home directory. Technically, the format of the file is `YAML` ("YAML Ain't Markup
+Language"), a "human friendly data serialization standard". (For technical details, visit
+[the website](https://yaml.org/). For a gentler introduction, visit 
+[the Wikipedia entry](https://en.wikipedia.org/wiki/YAML) or read / watch on of the many `YAML` 
+introductions / tutorials.)
+
+Because these articles describe `YAML` generally, they **do not** describe the details of the `YAML` document
+expected by the Orchid Python API. We, however, distribute an example file name `python_api.yaml.example` in
+each installed `orchid-python-api` package. Assuming you created a virtual environment as described in
+the step-by-step [pipenv installation instructions](#step-by-step-pipenv-install) or the 
+[conda installation instructions](#step-by-step-conda-install), you can find this example file,
+`python_api.yaml.example`, in the directory,
+`/path/to/orchid-virtualenv/Lib/site-packages/orchid_python_api/examples`.
+
+To use this configuration file as an example:
+
+- Copy the file to the expected location. For example, assuming the symbolic names referenced above, execute
+  the command
+  
+  ```
+  copy /path/to/orchid-virtualenv/Lib/site-packages/orchid_python_api/examples/python_api.yaml.example /path/to/home-directory/.orchid/python_api.yaml
+  ```  
+  
+- Edit the copied file, `/path/to/home-directory/.orchid/python_api.yaml`, using your favorite **text** editor.
+
+The example file, contains comments, introduced by a leading octothorpe character (#, number sign, or hash),
+that describe the information expected by the Orchid Python API. In summary, you'll need to provide a value
+for the 'orchid' > 'training_data' key that contains the pathname of the directory containing the Orchid
+training data files.
+
+If you want to ensure your configuration is correct,
+[view the Orchid API configuration details](#view-orchid-configuration-details).
+
+## Verify installation
+
+### Jupyter lab
+
+- In your activated virtual environment, run `jupyter lab` to open a browser tab.
+- In the first cell, enter `import orchid`.
+- Run the cell.
+- Wait patiently.
+
+The import should complete with no errors.
+
+### Python REPL
+
+- In your activated virtual environment, run either `python` or `ipython` to open a REPL.
+- Enter `import orchid`.
+- Wait patiently.
+
+The import should complete with no errors.
+
+## Run Orchid high-level examples
+
+- If you have not already done so, 
+[configure the Orchid Python API to find the Orchid installation](#configure-the-orchid-python-api)
+- You **must** 
+[configure the Orchid Python API to find the Orchid training data](#configure-the-orchid-training-data)
+- Navigate to the directory associated with the virtual environment
+- If necessary, activate the virtual environment by executing either 
+    - `pipenv shell` or 
+    - `conda activate <your-virtualenv_name>`.
+- Run `copy_orchid_examples`
+- If the script reports that it skipped notebooks or scripts, repeat the command with an additional argument:  
+  `copy_orchid_examples --overwrite`
+- Verify that the current directory has six example notebooks:
+    - `completion_analysis.ipynb`
+    - `plot_time_series.ipynb`
+    - `plot_trajectories.ipynb`
+    - `plot_treatment.ipynb`
+    - `search_data_frames.ipynb`
+    - `volume_2_first_response.ipynb`
+- Verify that the current directory has nine example scripts:
+    - `completion_analysis.py`
+    - `plot_time_series.py`
+    - `plot_trajectories.py`
+    - `plot_treatment.py`
+    - `search_data_frames.py`
+    - `volume_2_first_response.py`
+    - `stage_qc_results.py`
+    - `change_stage_times.py`
+    - `add_stages.py`
+
+### Run high-level example scripts
+
+- Run the first script
+    - Execute the command `python plot_trajectories.py`
+    - Wait patiently for the `matplotlib` plot window to appear.
+    - Ensure the plot is correct.
+    - Dismiss the `matplotlib` window.
+- Repeat for these scripts:
+    - `plot_treatment.py`
+    - `plot_time_series.py` 
+    - `completion_analysis.py` (This script prints multiple messages and presents **multiple** plots.
+       You must dismiss each plot to continue.)
+    - `volume_2_first_response.py`
+    - `search_data_frames.py`
+- Run the `stage_qc_results.py` script.
+- Run the `change_stage_times.py` script.
+- Run the `add_stages.py` script.
+
+The scripts, `stage_qc_results.py`, `change_stage_times.py`, and `add_stages.py`, differ from the other scripts. These
+scripts require a number of command line arguments to run correctly.
+
+For example, to see an explanation of these arguments, execute any of this scripts with the `--help` option.
+The most typical arguments are described in the following paragraphs.
+
+To both read and write stage QC results, run the command:
+```
+python stage_qc_results.py -v2 /path/to/orchid-traing-data/frankNstein_Bakken_UTM13_FEET.v11.ifrac 
+```
+
+To only read the existing stage QC data, run the command
+```
+python stage_qc_results.py -v2 --read-only /path/to/orchid-traing-data/frankNstein_Bakken_UTM13_FEET.ifrac
+```
+
+To change the stage start and stop times (the time range), run the command
+```
+python change_stage_times.py -v2 /path/to/orchid-traing-data/frankNstein_Bakken_UTM13_FEET.ifrac 
+```
+
+To add stages to a well, run the command
+```
+python add_stages.py -v2 /path/to/orchid-traing-data/frankNstein_Bakken_UTM13_FEET.v11.ifrac 
+```
+
+### Run high-level example notebooks
+
+- Open Jupyter by running `jupyter lab` in the shell
+- Within Jupyter,
+    - Successfully run notebook, `plot_trajectories.ipynb`
+        1. Open notebook
+        2. Run all cells of notebook
+        3. Wait patiently
+        4. Verify that no exceptions occurred
+    - Repeat for remaining notebooks:
+        - `plot_time_series.ipynb`
+        - `plot_treatment.ipynb`
+        - `completion_analysis.ipynb`
+        - `volume_2_first_response.ipynb`
+        - `search_data_frames.ipynb`
+
+## Run Orchid tutorials
+
+- If you have not already done so,
+  [configure the Orchid Python API to find the Orchid installation](#configure-the-orchid-python-api)
+- You **must**
+  [configure the Orchid Python API to find the Orchid training data](#configure-the-orchid-training-data)
+- Navigate to the directory associated with the virtual environment
+- If necessary, activate the virtual environment by executing either
+    - `pipenv shell` or
+    - `conda activate <your-virtualenv_name>`.
+- Run `copy_orchid_tutorials.exe`
+- If the script reports that it skipped notebooks or scripts, repeat the command with an additional argument:  
+  `python </path/to/virtualenv/Lib/site-packages/copy_orchid_tutorials.py --overwrite`
+- Verify that the current directory has one tutorial notebooks:
+    - `dom_navigation_tutorial.ipynb`
+- Verify that the current directory has five example scripts:
+    - `dom_navigation_tutorial.py`
+
+### Run tutorial script
+
+- Run the `dom_navigation_tutorial.py` script
+    - Execute the command `python dom_navigation_tutorial.py`
+    - Follow the on-screen messages to advance through the tutorial
+
+### Run tutorial notebook
+
+- Open Jupyter by running `jupyter lab` in the shell
+- Within Jupyter,
+    - Run the notebook, `dom_navigation_tutorial.ipynb`
+        1. Open the notebook in `jupyter`
+        2. Run each cell of the notebook. Typically, this process involves
+            - Read the instructions or comments preceding the code cell(s)
+            - Observe the result of executing the code
+
+## View Orchid Configuration Details
+
+To "debug" the Orchid Python API configuration, perform the following steps:
+
+- Change to the directory associated with your Python virtual environment.
+- If necessary, activate the virtual environment.
+- Within that virtual environment, invoke Python. It is important to create a new REPL so that you start with
+  a "clean" environment.
+- Within the Python REPL, execute the following commands.
+
+  ```
+  import logging
+  logging.basicConfig(level=logging.DEBUG)
+  import orchid
+  ```
+  
+Enabling logging **before** importing is critical. If you have already imported `orchid`, the simplest
+solution is to close this REPL and create another, "clean" REPL.
+
+You should see output like the following:
+
+```
+DEBUG:orchid.configuration:fallback configuration={'orchid': {'root': 'C:\\Program Files\\Reveal Energy Services\\Orchid\\Orchid-2020.4.361'}}
+DEBUG:orchid.configuration:file configuration={'orchid': {'root': 'c:\\path-to\\bin\\x64\\Debug\\net48', 'training_data ': 'c:\\path-to\\installed-training-data'}}
+DEBUG:orchid.configuration:environment configuration = {'orchid': {'root': 'c:\\another\\path-to\bin\\x64\\Debug\\net48'}}
+DEBUG:orchid.configuration:result configuration={'orchid': {'root': 'c:\\another\\path-to\bin\\x64\\Debug\\net48'}}
+```
+
+This output describes four details of the configuration.
+
+| Configuration | Explanation                                                            |
+|---------------|------------------------------------------------------------------------|
+| fallback      | The always available configuration (may be empty)                      |
+| file          | The configuration specified in your configuration file (may be empty)  |
+| environment   | The configuration specified using environment variables (may be empty) | 
+| result        | The configuration used by the Orchid Python API (should not be empty)  |
 
 
-setup(**setup_kwargs)
```

