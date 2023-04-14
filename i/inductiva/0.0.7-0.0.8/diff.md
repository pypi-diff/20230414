# Comparing `tmp/inductiva-0.0.7.tar.gz` & `tmp/inductiva-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductiva-0.0.7.tar", last modified: Thu Apr 13 17:01:24 2023, max compression
+gzip compressed data, was "inductiva-0.0.8.tar", last modified: Fri Apr 14 11:33:31 2023, max compression
```

## Comparing `inductiva-0.0.7.tar` & `inductiva-0.0.8.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.164712 inductiva-0.0.7/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       43 2023-03-29 15:57:40.000000 inductiva-0.0.7/MANIFEST.in
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3570 2023-04-13 17:01:24.164712 inductiva-0.0.7/PKG-INFO
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3196 2023-04-12 11:44:25.000000 inductiva-0.0.7/README.md
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      387 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/api/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-04-03 08:49:49.000000 inductiva-0.0.7/inductiva/api/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13042 2023-04-13 14:14:35.000000 inductiva-0.0.7/inductiva/api/methods.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60856 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/api_client.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/apis/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1421 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/path_to_api.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/apis/paths/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/admin_user.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/admin_user_username_tasks.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_submit.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_task_id_input.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_task_id_kill.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_task_id_output.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/paths/task_task_id_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      400 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/tag_to_api.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/apis/tags/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/tags/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      622 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/tags/admin_api.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      916 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/apis/tags/tasks_api.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16615 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/configuration.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/exceptions.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/model/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2759 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/body_upload_task_input.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3636 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/http_validation_error.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4386 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/new_user.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4682 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/queue_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3628 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/task_request.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6465 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/task_status.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7930 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/model/validation_error.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/models/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      843 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/models/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      617 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/admin_user/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/admin_user/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12303 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/admin_user/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/admin_user_username_tasks/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/admin_user_username_tasks/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10351 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/admin_user_username_tasks/get.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_submit/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_submit/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12455 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_submit/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_task_id_input/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_input/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15178 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_input/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_task_id_kill/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_kill/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10501 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_kill/post.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_task_id_output/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_output/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10463 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_output/get.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/client/paths/task_task_id_status/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_status/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10400 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/paths/task_task_id_status/get.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11962 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/rest.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103899 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/client/schemas.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/core/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/core/cupy/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/cupy/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/cupy/linalg.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/math.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/core/slepc/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/slepc/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/core/slepc/linalg.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-04-13 16:55:23.000000 inductiva-0.0.7/inductiva/core/test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/exceptions.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      432 2023-04-13 16:55:27.000000 inductiva-0.0.7/inductiva/fluids/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/fluid_types.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/post_processing/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/post_processing/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5247 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/post_processing/splishsplash.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/scenarios/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      250 2023-04-13 16:55:27.000000 inductiva-0.0.7/inductiva/fluids/scenarios/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1610 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/scenarios/_post_processing.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/scenarios/dam_break/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/dam_break/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2678 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/scenarios/dam_break/dam_break.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7087 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1350 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/unit_box.obj
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      182 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8165 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9161 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/fluids/shapes.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/fluids/simulators/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-04-03 08:49:49.000000 inductiva-0.0.7/inductiva/fluids/simulators/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1121 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/simulators/dualsphysics.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1288 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/fluids/simulators/openfoam.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1084 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/simulators/splishsplash.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1065 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/fluids/simulators/swash.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      995 2023-04-11 15:37:20.000000 inductiva-0.0.7/inductiva/fluids/simulators/xbeach.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/molecules/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/molecules/__init__.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/molecules/simulators/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       71 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/molecules/simulators/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1312 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/molecules/simulators/gromacs.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1760 2023-04-11 14:04:20.000000 inductiva-0.0.7/inductiva/scenarios.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva/simulation/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-04-03 08:49:49.000000 inductiva-0.0.7/inductiva/simulation/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1938 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/simulation/simulator.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/types.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.164712 inductiva-0.0.7/inductiva/utils/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/__init__.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8337 2023-04-03 08:49:49.000000 inductiva-0.0.7/inductiva/utils/data.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2167 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/utils/files.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/files_test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/flags.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/meta.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      272 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/utils/misc.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-04-10 14:10:51.000000 inductiva-0.0.7/inductiva/utils/misc_test.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      509 2023-03-29 15:57:40.000000 inductiva-0.0.7/inductiva/utils/templates.py
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14282 2023-04-13 15:38:04.000000 inductiva-0.0.7/inductiva/utils/visualization.py
-drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-13 17:01:24.160712 inductiva-0.0.7/inductiva.egg-info/
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3570 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/PKG-INFO
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4134 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/SOURCES.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/dependency_links.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      175 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/requires.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-04-13 17:01:24.000000 inductiva-0.0.7/inductiva.egg-info/top_level.txt
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-04-03 08:49:49.000000 inductiva-0.0.7/pyproject.toml
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      779 2023-04-13 17:01:24.164712 inductiva-0.0.7/setup.cfg
--rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-04-03 08:49:49.000000 inductiva-0.0.7/setup.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       43 2023-04-14 10:18:54.000000 inductiva-0.0.8/MANIFEST.in
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3570 2023-04-14 11:33:31.458069 inductiva-0.0.8/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3196 2023-04-14 10:18:54.000000 inductiva-0.0.8/README.md
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      387 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/api/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      122 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/api/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    13042 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/api/methods.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      805 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    60856 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/api_client.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/apis/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      214 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1421 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/path_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/apis/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      243 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      112 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/admin_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      137 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/admin_user_username_tasks.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      114 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_submit.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      126 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_task_id_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      124 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_task_id_kill.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_task_id_output.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      125 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/paths/task_task_id_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      400 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/tag_to_api.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/apis/tags/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/tags/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      622 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/tags/admin_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      916 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/apis/tags/tasks_api.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    16615 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/configuration.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4590 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/model/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      350 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2759 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/body_upload_task_input.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3636 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/http_validation_error.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4386 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/new_user.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4682 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/queue_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3628 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/task_request.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6465 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/task_status.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7930 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/model/validation_error.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/models/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      843 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/models/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      617 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/admin_user/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      311 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/admin_user/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12303 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/admin_user/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/admin_user_username_tasks/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      341 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/admin_user_username_tasks/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10351 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/admin_user_username_tasks/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_submit/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      313 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_submit/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    12455 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_submit/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_task_id_input/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      327 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_input/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    15178 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_input/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_task_id_kill/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      325 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_kill/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10501 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_kill/post.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_task_id_output/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_output/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10463 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_output/get.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/client/paths/task_task_id_status/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      329 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_status/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    10400 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/paths/task_task_id_status/get.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    11962 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/rest.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)   103899 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/client/schemas.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/core/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      120 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/core/cupy/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       85 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/cupy/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      379 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/cupy/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      586 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/math.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/core/slepc/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       64 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/slepc/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      491 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/slepc/linalg.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      333 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/core/test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      102 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/exceptions.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      571 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/fluids/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1002 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/fluid_types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/post_processing/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/post_processing/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     5247 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/post_processing/splishsplash.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/scenarios/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      250 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1610 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/_post_processing.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/scenarios/dam_break/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/dam_break/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2670 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/fluids/scenarios/dam_break/dam_break.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       78 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     7904 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4230 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1350 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      700 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/unit_box.obj
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      182 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8868 2023-04-14 11:29:18.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1914 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     9181 2023-04-14 11:29:18.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     6444 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2507 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/shapes.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/fluids/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      203 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1121 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/dualsphysics.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1288 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/openfoam.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1084 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/splishsplash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1065 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/swash.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      995 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/fluids/simulators/xbeach.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/molecules/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       74 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/molecules/__init__.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/molecules/simulators/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       71 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/molecules/simulators/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1312 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/molecules/simulators/gromacs.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1353 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/scenarios.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/simulation/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       76 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/simulation/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1938 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/simulation/simulator.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      142 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/types.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva/utils/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/__init__.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     8337 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/data.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     2159 2023-04-14 11:15:16.000000 inductiva-0.0.8/inductiva/utils/files.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      783 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/files_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1720 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/flags.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     1672 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/meta.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      272 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/misc.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      750 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/misc_test.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      509 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/templates.py
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)    14282 2023-04-14 10:18:54.000000 inductiva-0.0.8/inductiva/utils/visualization.py
+drwxrwxr-x   0 lpcunha   (1000) lpcunha   (1000)        0 2023-04-14 11:33:31.458069 inductiva-0.0.8/inductiva.egg-info/
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     3570 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/PKG-INFO
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)     4134 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)        1 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      175 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/requires.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       10 2023-04-14 11:33:31.000000 inductiva-0.0.8/inductiva.egg-info/top_level.txt
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       87 2023-04-14 10:18:54.000000 inductiva-0.0.8/pyproject.toml
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)      779 2023-04-14 11:33:31.458069 inductiva-0.0.8/setup.cfg
+-rw-rw-r--   0 lpcunha   (1000) lpcunha   (1000)       56 2023-04-14 10:18:54.000000 inductiva-0.0.8/setup.py
```

### Comparing `inductiva-0.0.7/PKG-INFO` & `inductiva-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inductiva
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python client for the Inductiva API
 Home-page: https://github.com/inductiva/inductiva
 Author: Inductiva Research Labs
 Author-email: contact@inductiva.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `inductiva-0.0.7/README.md` & `inductiva-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/api/methods.py` & `inductiva-0.0.8/inductiva/api/methods.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/__init__.py` & `inductiva-0.0.8/inductiva/client/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/api_client.py` & `inductiva-0.0.8/inductiva/client/api_client.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/apis/path_to_api.py` & `inductiva-0.0.8/inductiva/client/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/apis/tags/admin_api.py` & `inductiva-0.0.8/inductiva/client/apis/tags/admin_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/apis/tags/tasks_api.py` & `inductiva-0.0.8/inductiva/client/apis/tags/tasks_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/configuration.py` & `inductiva-0.0.8/inductiva/client/configuration.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/exceptions.py` & `inductiva-0.0.8/inductiva/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/model/body_upload_task_input.py` & `inductiva-0.0.8/inductiva/client/model/body_upload_task_input.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/model/http_validation_error.py` & `inductiva-0.0.8/inductiva/client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/model/new_user.py` & `inductiva-0.0.8/inductiva/client/model/new_user.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/model/queue_status.py` & `inductiva-0.0.8/inductiva/client/model/queue_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/model/task_request.py` & `inductiva-0.0.8/inductiva/client/model/task_request.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/model/task_status.py` & `inductiva-0.0.8/inductiva/client/model/task_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/model/validation_error.py` & `inductiva-0.0.8/inductiva/client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/models/__init__.py` & `inductiva-0.0.8/inductiva/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/paths/__init__.py` & `inductiva-0.0.8/inductiva/client/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/paths/admin_user/post.py` & `inductiva-0.0.8/inductiva/client/paths/admin_user/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/paths/admin_user_username_tasks/get.py` & `inductiva-0.0.8/inductiva/client/paths/admin_user_username_tasks/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/paths/task_submit/post.py` & `inductiva-0.0.8/inductiva/client/paths/task_submit/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/paths/task_task_id_input/post.py` & `inductiva-0.0.8/inductiva/client/paths/task_task_id_input/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/paths/task_task_id_kill/post.py` & `inductiva-0.0.8/inductiva/client/paths/task_task_id_kill/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/paths/task_task_id_output/get.py` & `inductiva-0.0.8/inductiva/client/paths/task_task_id_output/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/paths/task_task_id_status/get.py` & `inductiva-0.0.8/inductiva/client/paths/task_task_id_status/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/rest.py` & `inductiva-0.0.8/inductiva/client/rest.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/client/schemas.py` & `inductiva-0.0.8/inductiva/client/schemas.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/core/math.py` & `inductiva-0.0.8/inductiva/core/math.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/fluid_types.py` & `inductiva-0.0.8/inductiva/fluids/fluid_types.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/post_processing/splishsplash.py` & `inductiva-0.0.8/inductiva/fluids/post_processing/splishsplash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/_post_processing.py` & `inductiva-0.0.8/inductiva/fluids/scenarios/_post_processing.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/dam_break/dam_break.py` & `inductiva-0.0.8/inductiva/fluids/scenarios/dam_break/dam_break.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         simulator: Simulator = DualSPHysics(),
         output_dir: Optional[Path] = None,
         device: Literal["cpu", "gpu"] = "gpu",
         resolution: Literal["high", "medium", "low"] = "medium",
         simulation_time: float = 1,
     ):
         """Simulates the scenario.
-        
+
         Args:
             simulator: Simulator to use.
             output_dir: Directory to store the simulation output.
             device: Device in which to run the simulation.
             resolution: Resolution of the simulation.
             simulation_time: Simulation time, in seconds.
         """
```

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block.py` & `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Describes the physical scenarios and runs its simulation via API."""
+
+from functools import singledispatchmethod
 import os
 from typing import List, Literal, Optional
 import shutil
 
 from inductiva.types import Path
 from inductiva.scenarios import Scenario
 from inductiva.simulation import Simulator
@@ -71,15 +73,15 @@
         simulation_time: float = 1,
         adaptive_time_step: bool = True,
         particle_sorting: bool = True,
         time_step: float = 0.001,
         output_time_step: float = 1 / 60,
     ):
         """Simulates the scenario.
-        
+
         Args:
             simulator: Simulator to use.
             output_dir: Directory to store the simulation output.
             device: Device in which to run the simulation.
             particle_radius: Radius of the fluid particles, in meters.
             simulation_time: Simulation time, in seconds.
             adaptive_time_step: Whether to use adaptive time step.
@@ -106,14 +108,32 @@
         # convert_vtk_data_dir_to_netcdf(
         #     data_dir=os.path.join(output_path, "vtk"),
         #     output_time_step=SPLISHSPLASH_OUTPUT_TIM_STEP,
         #     netcdf_data_dir=os.path.join(output_path, "netcdf"))
 
         return SPHSimulationOutput(output_path)
 
+    @singledispatchmethod
+    @classmethod
+    def get_config_filename(cls, simulator: Simulator):  # pylint: disable=unused-argument
+        raise ValueError(
+            f"Simulator not supported for `{cls.__name__}` scenario.")
+
+    @singledispatchmethod
+    def gen_aux_files(self, simulator: Simulator, input_dir: str):
+        raise ValueError(
+            f"Simulator not supported for `{self.__class__.__name__}` scenario."
+        )
+
+    @singledispatchmethod
+    def gen_config(self, simulator: Simulator, input_dir: str):
+        raise ValueError(
+            f"Simulator not supported for `{self.__class__.__name__}` scenario."
+        )
+
 
 @FluidBlock.get_config_filename.register
 def _(cls, simulator: SPlisHSPlasH):  # pylint: disable=unused-argument
     """Returns the configuration filename for SPlisHSPlasH."""
     return SPLISHSPLASH_CONFIG_FILENAME
 
 
@@ -159,14 +179,19 @@
 
 @FluidBlock.get_config_filename.register
 def _(cls, simulator: DualSPHysics):  # pylint: disable=unused-argument
     """Returns the configuration filename for DualSPHysics."""
     return DUALSPHYSICS_CONFIG_FILENAME
 
 
+@FluidBlock.gen_aux_files.register
+def _(self, simulator: DualSPHysics, input_dir):  # pylint: disable=unused-argument
+    pass
+
+
 @FluidBlock.gen_config.register
 def _(self, simulator: DualSPHysics, input_dir: str):  # pylint: disable=unused-argument
     """Generates the configuration file for DualSPHysics."""
 
     replace_params_in_template(
         templates_dir=os.path.dirname(__file__),
         template_filename=DUALSPHYSICS_TEMPLATE_FILENAME,
```

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja` & `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block_template.dualsphysics.xml.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja` & `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/fluid_block_template.splishsplash.json.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_block/unit_box.obj` & `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_block/unit_box.obj`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py` & `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/fluid_tank.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Classes describing fluid tank scenarios."""
 
 from dataclasses import dataclass, field
 from enum import Enum
+from functools import singledispatchmethod
 import os
 from typing import List, Literal, Optional
 
 from inductiva.types import Path
 from inductiva.scenarios import Scenario
 from inductiva.simulation import Simulator
 from inductiva.fluids.shapes import BaseShape
@@ -141,24 +142,24 @@
         self.fluid = fluid
         self.fluid_level = fluid_level
         self.inlet = inlet
         self.outlet = outlet
 
     def simulate(
         self,
-        simulator: Simulator,
+        simulator: Simulator = SPlisHSPlasH(),
         output_dir: Optional[Path] = None,
         device: Literal["cpu", "gpu"] = "cpu",
         simulation_time: float = 5,
         resolution: Literal["low", "medium", "high"] = "low",
         output_time_step: float = 0.1,
         particle_sorting: bool = False,
     ):
         """Simulates the scenario.
-        
+
         Args:
             simulator: Simulator to use.
             output_dir: Directory to store the simulation output.
             device: Device in which to run the simulation.
             simulation_time: Simulation time, in seconds.
             output_time_step: Time step between output files, in seconds.
             resolution: Resolution of the simulation. Controls the particle
@@ -199,14 +200,32 @@
         # Extend the bounding box to include the outlet.
         if self.outlet is not None:
             outlet_bounding_box_min, _ = self.outlet.shape.get_bounding_box()
             bounding_box_min[2] = outlet_bounding_box_min[2]
 
         return bounding_box_min, bounding_box_max
 
+    @singledispatchmethod
+    @classmethod
+    def get_config_filename(cls, simulator: Simulator):  # pylint: disable=unused-argument
+        raise ValueError(
+            f"Simulator not supported for `{cls.__name__}` scenario.")
+
+    @singledispatchmethod
+    def gen_aux_files(self, simulator: Simulator, input_dir: str):
+        raise ValueError(
+            f"Simulator not supported for `{self.__class__.__name__}` scenario."
+        )
+
+    @singledispatchmethod
+    def gen_config(self, simulator: Simulator, input_dir: str):
+        raise ValueError(
+            f"Simulator not supported for `{self.__class__.__name__}` scenario."
+        )
+
 
 @FluidTank.get_config_filename.register
 def _(cls, simulator: SPlisHSPlasH) -> str:  # pylint: disable=unused-argument
     """Returns the config filename for SPlisHSPlasH."""
     return SPLISHSPLASH_CONFIG_FILENAME
```

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja` & `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/fluid_tank_template.splishsplash.json.jinja`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py` & `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/gmsh_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import contextlib
 import os
 
 import gmsh
 import meshio
 
-TMP_MSH_FILE_PATH = 'gmsh_generated.msh'
+TMP_MSH_FILE_PATH = "gmsh_generated.msh"
 MESH_SIZE = 0.05
 GMSH_LOG_LEVEL = 2
 
 
 class gmshAPIWrapper(contextlib.AbstractContextManager):  # pylint: disable=invalid-name
     """Wrapper to interact with the gmsh API.
 
@@ -34,18 +34,18 @@
     def __enter__(self):
         """Common operations applied before use case-specific primitives."""
 
         # Initialize the gmsh API.
         gmsh.initialize()
 
         # Set the log level.
-        gmsh.option.setNumber('General.Verbosity', self.log_level)
+        gmsh.option.setNumber("General.Verbosity", self.log_level)
 
         # Set the mesh size.
-        gmsh.option.setNumber('Mesh.MeshSizeMax', self.mesh_size)
+        gmsh.option.setNumber("Mesh.MeshSizeMax", self.mesh_size)
 
     def __exit__(self, *_):
         """Common operations applied after use case-specific primitives."""
 
         # Synchronize the representations (or kernels) available in gmsh:
         # - the built-in representation, used in a bottom-up manner (defining
         #   points first, then curves, surfaces and volumes).
@@ -278,17 +278,17 @@
 
 def convert_msh_to_obj_file(obj_file_path: str,
                             msh_file_path: str = TMP_MSH_FILE_PATH,
                             remove_msh_file: bool = True) -> None:
     """Converts msh to obj files using meshio."""
 
     # Read mesh using meshio.
-    mesh = meshio.read(msh_file_path)
+    mesh = meshio.read(msh_file_path, file_format="gmsh")
 
     # Filter cell blocks to keep only those representing surfaces.
-    cells = [block for block in mesh.cells if block.type == 'triangle']
+    cells = [block for block in mesh.cells if block.type == "triangle"]
 
     # Write mesh to obj file.
     meshio.write_points_cells(obj_file_path, mesh.points, cells)
 
     if remove_msh_file:
         os.remove(msh_file_path)
```

### Comparing `inductiva-0.0.7/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py` & `inductiva-0.0.8/inductiva/fluids/scenarios/fluid_tank/mesh_file_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/shapes.py` & `inductiva-0.0.8/inductiva/fluids/shapes.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/simulators/dualsphysics.py` & `inductiva-0.0.8/inductiva/fluids/simulators/dualsphysics.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/simulators/openfoam.py` & `inductiva-0.0.8/inductiva/fluids/simulators/openfoam.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/simulators/splishsplash.py` & `inductiva-0.0.8/inductiva/fluids/simulators/splishsplash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/simulators/swash.py` & `inductiva-0.0.8/inductiva/fluids/simulators/swash.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/fluids/simulators/xbeach.py` & `inductiva-0.0.8/inductiva/fluids/simulators/xbeach.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/molecules/simulators/gromacs.py` & `inductiva-0.0.8/inductiva/molecules/simulators/gromacs.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/scenarios.py` & `inductiva-0.0.8/inductiva/scenarios.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Base class for scenarios."""
 
 from abc import ABC
-from functools import singledispatchmethod
 import tempfile
 from typing import Optional
 
 from inductiva.types import Path
 from inductiva.simulation import Simulator
 from inductiva.utils.files import resolve_path, get_timestamped_path
 from inductiva.utils.misc import split_camel_case
@@ -42,20 +41,7 @@
                 input_dir,
                 *args,
                 output_dir=output_dir,
                 **kwargs,
             )
 
         return output_path
-
-    @singledispatchmethod
-    @classmethod
-    def get_config_filename(cls, simulator: Simulator):  # pylint: disable=unused-argument
-        return ""
-
-    @singledispatchmethod
-    def gen_aux_files(self, simulator: Simulator, input_dir: str):
-        pass
-
-    @singledispatchmethod
-    def gen_config(self, simulator: Simulator, input_dir: str):
-        pass
```

### Comparing `inductiva-0.0.7/inductiva/simulation/simulator.py` & `inductiva-0.0.8/inductiva/simulation/simulator.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/utils/data.py` & `inductiva-0.0.8/inductiva/utils/data.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/utils/files.py` & `inductiva-0.0.8/inductiva/utils/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     return pathlib.Path(root, path)
 
 
 def get_sorted_files(data_dir: str,
                      file_format: str = "name",
                      split_token: str = "_"):
     """Returns list of files sorted according to [file_key].
-    
+
     Order a set of .format files of the form
     ['name_1.format', 'name_2.format',...,'name_10.format',
     ...,'name_n.format'].
-    
+
     The default sorting methods for list, list.sort()
     or sorted(list), order 'name_10.format' before 'name_2.format',
     which is not representative of the time series.
 
     In this function we sort according to the number..
     """
```

### Comparing `inductiva-0.0.7/inductiva/utils/files_test.py` & `inductiva-0.0.8/inductiva/utils/files_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/utils/flags.py` & `inductiva-0.0.8/inductiva/utils/flags.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/utils/meta.py` & `inductiva-0.0.8/inductiva/utils/meta.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/utils/misc_test.py` & `inductiva-0.0.8/inductiva/utils/misc_test.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva/utils/visualization.py` & `inductiva-0.0.8/inductiva/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/inductiva.egg-info/PKG-INFO` & `inductiva-0.0.8/inductiva.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inductiva
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python client for the Inductiva API
 Home-page: https://github.com/inductiva/inductiva
 Author: Inductiva Research Labs
 Author-email: contact@inductiva.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `inductiva-0.0.7/inductiva.egg-info/SOURCES.txt` & `inductiva-0.0.8/inductiva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inductiva-0.0.7/setup.cfg` & `inductiva-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = inductiva
-version = 0.0.7
+version = 0.0.8
 description = Python client for the Inductiva API
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Inductiva Research Labs
 author_email = contact@inductiva.ai
 url = https://github.com/inductiva/inductiva
 classifiers =
```

