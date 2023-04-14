# Comparing `tmp/apache-dolphinscheduler-4.0.2a8.tar.gz` & `tmp/apache-dolphinscheduler-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-dolphinscheduler-4.0.2a8.tar", last modified: Wed Mar 22 04:07:17 2023, max compression
+gzip compressed data, was "apache-dolphinscheduler-4.0.3.tar", last modified: Fri Apr 14 05:54:06 2023, max compression
```

## Comparing `apache-dolphinscheduler-4.0.2a8.tar` & `apache-dolphinscheduler-4.0.3.tar`

### file list

```diff
@@ -1,113 +1,119 @@
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.930171 apache-dolphinscheduler-4.0.2a8/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     7853 2023-03-22 04:07:17.930271 apache-dolphinscheduler-4.0.2a8/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6015 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/README.md
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2618 2023-03-22 04:07:17.930770 apache-dolphinscheduler-4.0.2a8/setup.cfg
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3027 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/setup.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.914184 apache-dolphinscheduler-4.0.2a8/src/
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.916091 apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     7853 2023-03-22 04:07:17.000000 apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4340 2023-03-22 04:07:17.000000 apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/SOURCES.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-03-22 04:07:17.000000 apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/dependency_links.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       75 2023-03-22 04:07:17.000000 apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/entry_points.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      561 2023-03-22 04:07:17.000000 apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/requires.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       19 2023-03-22 04:07:17.000000 apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/top_level.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-01-31 10:37:45.000000 apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/zip-safe
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.917463 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      851 2023-03-22 04:06:49.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.917851 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/cli/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      839 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/cli/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3023 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/cli/commands.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     7268 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/configuration.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3053 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/constants.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.919068 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1038 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3363 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/engine.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4557 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/parameter.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1168 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/process_definition.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2696 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/resource.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1997 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/resource_plugin.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    18112 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/task.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    18099 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/workflow.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    17251 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/yaml_workflow.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3100 2023-03-22 04:05:50.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/default_config.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.921888 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      869 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2217 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/bulk_create_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3841 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/local_parameter_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2923 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/multi_resources_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2341 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_condition_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3570 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_datax_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2510 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_dependent_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1755 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_dvc_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1326 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_flink_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1289 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_kubernetes_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1375 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_map_reduce_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3104 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_mlflow_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1415 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_openmldb_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2183 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_pytorch_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1645 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_sagemaker_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1320 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_spark_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2111 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_sql_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2084 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_switch_example.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2410 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/tutorial.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2763 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/tutorial_decorator.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2070 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/tutorial_resource_plugin.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1624 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/exceptions.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    10530 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/java_gateway.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.923767 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1379 2023-02-23 11:36:13.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2776 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/base.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1667 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/base_side.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1083 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/connection.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6401 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/datasource.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4779 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/meta.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2503 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/project.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1185 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/queue.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2802 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/tenant.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3948 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/user.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1146 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/worker_group.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.924819 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1171 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.925454 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/base/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      811 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/base/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2806 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/base/bucket.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3824 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/base/git.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3922 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/github.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4312 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/gitlab.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2019 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/local.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3038 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/oss.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2838 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/s3.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.928769 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2475 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6813 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/condition.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5209 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/datax.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     9737 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/dependent.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3605 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/dvc.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2883 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/flink.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2221 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/func_wrap.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3542 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/http.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1949 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/kubernetes.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1679 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/map_reduce.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     8634 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/mlflow.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1754 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/openmldb.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2637 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/procedure.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3763 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/python.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3527 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/pytorch.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1585 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/sagemaker.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1952 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/shell.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2636 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/spark.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5687 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/sql.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1627 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/sub_process.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2225 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/sub_workflow.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5980 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/switch.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.929708 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      812 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3364 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/date.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2193 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/file.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1490 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/string.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1790 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/versions.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5311 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/yaml_parser.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       23 2023-03-22 04:03:58.000000 apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/version_ext
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-03-22 04:07:17.930020 apache-dolphinscheduler-4.0.2a8/tests/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     9827 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/tests/test_configuration.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2398 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.2a8/tests/test_docs.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.792517 apache-dolphinscheduler-4.0.3/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    12843 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/CONTRIBUTING.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    12553 2022-12-14 07:25:00.000000 apache-dolphinscheduler-4.0.3/LICENSE
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      898 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/MANIFEST.in
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      177 2022-12-14 07:25:00.000000 apache-dolphinscheduler-4.0.3/NOTICE
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     7851 2023-04-14 05:54:06.792642 apache-dolphinscheduler-4.0.3/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6015 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/README.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9770 2023-04-14 05:50:48.000000 apache-dolphinscheduler-4.0.3/RELEASE.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2832 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/UPDATING.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4781 2023-04-14 05:54:06.793482 apache-dolphinscheduler-4.0.3/setup.cfg
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3027 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/setup.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.767804 apache-dolphinscheduler-4.0.3/src/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.771202 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     7851 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4406 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       75 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/entry_points.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      577 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/requires.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       19 2023-04-14 05:54:06.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/top_level.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-01-31 10:37:45.000000 apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/zip-safe
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.772986 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      848 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.773420 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      839 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3023 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/commands.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     7268 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/configuration.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2981 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/constants.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.775975 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1038 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3363 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/engine.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4557 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/parameter.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1168 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/process_definition.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2721 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/resource.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1997 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/resource_plugin.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    17725 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/task.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    18099 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/workflow.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    17251 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/yaml_workflow.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3093 2023-04-04 15:20:36.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/default_config.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.780672 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      869 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2217 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/bulk_create_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3841 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/local_parameter_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2923 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/multi_resources_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2341 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_condition_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3570 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_datax_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2510 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_dependent_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1755 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_dvc_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1326 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_flink_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1289 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_kubernetes_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1375 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_map_reduce_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3104 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_mlflow_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1415 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_openmldb_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2183 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_pytorch_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1645 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_sagemaker_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1320 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_spark_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2110 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_sql_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2084 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_switch_example.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1903 2023-04-11 03:29:16.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2763 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial_decorator.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2070 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial_resource_plugin.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1624 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/exceptions.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    11531 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/java_gateway.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.782996 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1379 2023-02-23 11:36:13.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2776 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/base.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1667 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/base_side.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1083 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/connection.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6290 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/datasource.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4779 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/meta.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2503 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/project.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1185 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/queue.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2802 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/tenant.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3948 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/user.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1146 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/worker_group.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.784232 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1171 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.784756 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      811 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2806 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/bucket.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3824 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/git.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3922 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/github.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4312 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/gitlab.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2019 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/local.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3038 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/oss.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2838 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/s3.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.790786 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2475 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6813 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/condition.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5209 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/datax.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9737 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/dependent.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3605 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/dvc.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2883 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/flink.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2221 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/func_wrap.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3542 2023-04-04 15:19:44.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/http.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1949 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/kubernetes.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1679 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/map_reduce.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     8634 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/mlflow.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1754 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/openmldb.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2637 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/procedure.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3763 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/python.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3527 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/pytorch.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1585 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sagemaker.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1952 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/shell.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2636 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/spark.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5687 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sql.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1627 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sub_process.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2225 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sub_workflow.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5980 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/switch.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.791866 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      812 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3364 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/date.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2193 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/file.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1490 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/string.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1790 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/versions.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5311 2023-02-01 06:51:22.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/yaml_parser.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       31 2023-04-14 05:53:48.000000 apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/version_ext
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-04-14 05:54:06.792182 apache-dolphinscheduler-4.0.3/tests/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9827 2023-04-04 15:19:49.000000 apache-dolphinscheduler-4.0.3/tests/test_configuration.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2398 2023-03-21 06:23:03.000000 apache-dolphinscheduler-4.0.3/tests/test_docs.py
```

### Comparing `apache-dolphinscheduler-4.0.2a8/PKG-INFO` & `apache-dolphinscheduler-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-dolphinscheduler
-Version: 4.0.2a8
+Version: 4.0.3
 Summary: pydolphinscheduler is Apache DolphinScheduler Python API.
 Home-page: https://dolphinscheduler.apache.org/python/main/index.html
 Author: Apache Software Foundation
 Author-email: dev@dolphinscheduler.apache.org
 License: Apache License 2.0
 Project-URL: Homepage, https://dolphinscheduler.apache.org/python/main/index.html
 Project-URL: Documentation, https://dolphinscheduler.apache.org/python/main/index.html
```

### Comparing `apache-dolphinscheduler-4.0.2a8/README.md` & `apache-dolphinscheduler-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/setup.py` & `apache-dolphinscheduler-4.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/PKG-INFO` & `apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-dolphinscheduler
-Version: 4.0.2a8
+Version: 4.0.3
 Summary: pydolphinscheduler is Apache DolphinScheduler Python API.
 Home-page: https://dolphinscheduler.apache.org/python/main/index.html
 Author: Apache Software Foundation
 Author-email: dev@dolphinscheduler.apache.org
 License: Apache License 2.0
 Project-URL: Homepage, https://dolphinscheduler.apache.org/python/main/index.html
 Project-URL: Documentation, https://dolphinscheduler.apache.org/python/main/index.html
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/SOURCES.txt` & `apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,14 @@
+CONTRIBUTING.md
+LICENSE
+MANIFEST.in
+NOTICE
 README.md
+RELEASE.md
+UPDATING.md
 setup.cfg
 setup.py
 src/apache_dolphinscheduler.egg-info/PKG-INFO
 src/apache_dolphinscheduler.egg-info/SOURCES.txt
 src/apache_dolphinscheduler.egg-info/dependency_links.txt
 src/apache_dolphinscheduler.egg-info/entry_points.txt
 src/apache_dolphinscheduler.egg-info/requires.txt
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/apache_dolphinscheduler.egg-info/requires.txt` & `apache-dolphinscheduler-4.0.3/src/apache_dolphinscheduler.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 boto3>=1.23.10
 oss2>=2.16.0
 python-gitlab>=2.10.1
 click>=8.0.0
 py4j~=0.10
 ruamel.yaml
 stmdency>=0.0.2
+packaging>=21.3
 
 [build]
 build
 setuptools>=42
 wheel
 
 [dev]
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Init root of pydolphinscheduler."""
 
-__version__ = "v4.0.2a8"
+__version__ = "4.0.3"
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/cli/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/cli/commands.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/cli/commands.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/configuration.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/configuration.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/constants.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,21 +31,14 @@
 class TaskFlag(str):
     """Constants for task flag."""
 
     YES = "YES"
     NO = "NO"
 
 
-class IsCache(str):
-    """Constants for Cache."""
-
-    YES = "YES"
-    NO = "NO"
-
-
 class TaskTimeoutFlag(str):
     """Constants for task timeout flag."""
 
     OFF = "CLOSE"
     ON = "OPEN"
 
 
@@ -115,15 +108,15 @@
     FMT_STD_TIME = "%H:%M:%S"
     FMT_NO_COLON_TIME = "%H%M%S"
 
 
 class ResourceKey(str):
     """Constants for key of resource."""
 
-    ID = "id"
+    NAME = "resourceName"
 
 
 class Symbol(str):
     """Constants for symbol."""
 
     SLASH = "/"
     POINT = "."
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/engine.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/engine.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/parameter.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/parameter.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/process_definition.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/process_definition.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/resource.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,23 +51,23 @@
         """Get resource info from java gateway, contains resource id, name."""
         if not self.user_name:
             raise PyDSParamException(
                 "`user_name` is required when querying resources from python gate."
             )
         return gateway.query_resources_file_info(self.user_name, self.name)
 
-    def get_id_from_database(self):
-        """Get resource id from java gateway."""
-        return self.get_info_from_database().getId()
+    def get_fullname_from_database(self):
+        """Get resource fullname from java gateway."""
+        return self.get_info_from_database().getFullName()
 
     def create_or_update_resource(self):
         """Create or update resource via java gateway."""
         if not self.content or not self.user_name:
             raise PyDSParamException(
                 "`user_name` and `content` are required when create or update resource from python gate."
             )
-        gateway.create_or_update_resource(
+        return gateway.create_or_update_resource(
             self.user_name,
             self.name,
-            self.content,
             self.description,
+            self.content,
         )
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/resource_plugin.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/resource_plugin.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/task.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from datetime import timedelta
 from logging import getLogger
 from typing import Dict, List, Optional, Sequence, Set, Tuple, Union
 
 from pydolphinscheduler import configuration
 from pydolphinscheduler.constants import (
     Delimiter,
-    IsCache,
     ResourceKey,
     Symbol,
     TaskFlag,
     TaskPriority,
     TaskTimeoutFlag,
 )
 from pydolphinscheduler.core.parameter import BaseDataType, Direction, ParameterHelper
@@ -97,15 +96,14 @@
     :param fail_retry_interval: default 1
     :param timeout_notify_strategy: default, None
     :param timeout: default None
     :param resource_list: default None
     :param wait_start_timeout: default None
     :param condition_result: default None,
     :param resource_plugin: default None
-    :param is_cache: default False
     :param input_params: default None, input parameters, {param_name: param_value}
     :param output_params: default None, input parameters, {param_name: param_value}
     """
 
     _DEFINE_ATTR = {
         "name",
         "code",
@@ -119,15 +117,14 @@
         "environment_code",
         "delay_time",
         "fail_retry_times",
         "fail_retry_interval",
         "timeout_flag",
         "timeout_notify_strategy",
         "timeout",
-        "is_cache",
     }
 
     # task default attribute will into `task_params` property
     _task_default_attr = {
         "local_params",
         "resource_list",
         "dependence",
@@ -160,24 +157,22 @@
         timeout: Optional[timedelta] = None,
         workflow: Optional[Workflow] = None,
         resource_list: Optional[List] = None,
         dependence: Optional[Dict] = None,
         wait_start_timeout: Optional[Dict] = None,
         condition_result: Optional[Dict] = None,
         resource_plugin: Optional[ResourcePlugin] = None,
-        is_cache: Optional[bool] = False,
         input_params: Optional[Dict] = None,
         output_params: Optional[Dict] = None,
         *args,
         **kwargs,
     ):
         super().__init__(name, description)
         self.task_type = task_type
         self.flag = flag
-        self._is_cache = is_cache
         self.task_priority = task_priority
         self.worker_group = worker_group
         self._environment_name = environment_name
         self.fail_retry_times = fail_retry_times
         self.fail_retry_interval = fail_retry_interval
         self.delay_time = delay_time
         self.timeout_notify_strategy = timeout_notify_strategy
@@ -248,40 +243,34 @@
 
     @property
     def timeout_flag(self) -> str:
         """Whether the timeout attribute is being set or not."""
         return TaskTimeoutFlag.ON if self._timeout else TaskTimeoutFlag.OFF
 
     @property
-    def is_cache(self) -> str:
-        """Whether the cache is being set or not."""
-        if isinstance(self._is_cache, bool):
-            return IsCache.YES if self._is_cache else IsCache.NO
-        else:
-            raise PyDSParamException("is_cache must be a bool")
-
-    @property
     def resource_list(self) -> List[Dict[str, Resource]]:
         """Get task define attribute `resource_list`."""
         resources = set()
         for res in self._resource_list:
             if type(res) == str:
                 resources.add(
-                    Resource(name=res, user_name=self.user_name).get_id_from_database()
+                    Resource(
+                        name=res, user_name=self.user_name
+                    ).get_fullname_from_database()
                 )
-            elif type(res) == dict and res.get(ResourceKey.ID) is not None:
+            elif type(res) == dict and ResourceKey.NAME in res:
                 warnings.warn(
                     """`resource_list` should be defined using List[str] with resource paths,
                        the use of ids to define resources will be remove in version 3.2.0.
                     """,
                     DeprecationWarning,
                     stacklevel=2,
                 )
-                resources.add(res.get(ResourceKey.ID))
-        return [{ResourceKey.ID: r} for r in resources]
+                resources.add(res.get(ResourceKey.NAME))
+        return [{ResourceKey.NAME: r} for r in resources]
 
     @property
     def user_name(self) -> Optional[str]:
         """Return username of workflow."""
         if self.workflow:
             return self.workflow.user.name
         else:
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/workflow.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/workflow.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/core/yaml_workflow.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/core/yaml_workflow.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/default_config.yaml` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/default_config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 # including ``user``, ``workflow`` 
 default:
   # Default value for dolphinscheduler's user object
   user:
     name: admin
     password: dolphinscheduler123
     email: userPythonGateway@dolphinscheduler.com
-    tenant: whalescheduler
+    tenant: default
     phone: 11111111111
     state: 1
   # Default value for dolphinscheduler's workflow object
   workflow:
     project: project-pydolphin
     user: admin
     queue: queuePythonGateway
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/bulk_create_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/bulk_create_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/local_parameter_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/local_parameter_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/multi_resources_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/multi_resources_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_condition_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_condition_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_datax_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_datax_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_dependent_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_dependent_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_dvc_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_dvc_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_flink_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_flink_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_kubernetes_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_kubernetes_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_map_reduce_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_map_reduce_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_mlflow_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_mlflow_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_openmldb_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_openmldb_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_pytorch_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_pytorch_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_sagemaker_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_sagemaker_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_spark_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_spark_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_sql_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_sql_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,38 +26,41 @@
 
 with Workflow(
     name="task_sql_example",
 ) as workflow:
     # [start bare_sql_desc]
     bare_sql = Sql(
         name="bare_sql",
-        datasource_name="whalescheduler",
+        datasource_name="metadata",
         sql="select * from t_ds_version",
     )
     # [end bare_sql_desc]
     # [start sql_file_desc]
     sql_file = Sql(
         name="sql_file",
-        datasource_name="whalescheduler",
+        datasource_name="metadata",
         sql="ext/example.sql",
         sql_type=SqlType.SELECT,
         resource_plugin=Local(prefix=str(Path(__file__).parent)),
     )
     # [end sql_file_desc]
     # [start sql_with_pre_post_desc]
     sql_with_pre_post = Sql(
         name="sql_with_pre_post",
-        datasource_name="whalescheduler",
+        datasource_name="metadata",
         sql="select * from t_ds_version",
         pre_statements=[
-            "update test.table_one set name = '1.3.6'",
-            "delete from test.table_two where name = '1.3.6'",
+            "update table_one set version = '1.3.6'",
+            "delete from table_two where version = '1.3.6'",
         ],
-        post_statements="update test.table_one set name = '3.0.0'",
+        post_statements="update table_one set version = '3.0.0'",
     )
     # [end sql_with_pre_post_desc]
 
-    bare_sql >> sql_file >> sql_with_pre_post
+    bare_sql >> [
+        sql_file,
+        sql_with_pre_post,
+    ]
 
     workflow.submit()
 
 # [end workflow_declare]
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/task_switch_example.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/task_switch_example.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/tutorial_decorator.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial_decorator.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/examples/tutorial_resource_plugin.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/examples/tutorial_resource_plugin.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/exceptions.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/java_gateway.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/java_gateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,27 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """Module java gateway, contain gateway behavior."""
 
+import contextlib
+import warnings
 from logging import getLogger
 from typing import Any, Optional
 
 from py4j.java_collections import JavaMap
 from py4j.java_gateway import GatewayParameters, JavaGateway
+from py4j.protocol import Py4JError
 
-from pydolphinscheduler import configuration
-from pydolphinscheduler.constants import JavaGatewayDefault
+from pydolphinscheduler import __version__, configuration
+from pydolphinscheduler.constants import JavaGatewayDefault, Version
 from pydolphinscheduler.exceptions import PyDSJavaGatewayException
+from pydolphinscheduler.utils.versions import version_match
 
 logger = getLogger(__name__)
 
 
 def gateway_result_checker(
     result: JavaMap,
     msg_check: Optional[str] = JavaGatewayDefault.RESULT_MESSAGE_SUCCESS,
@@ -59,14 +63,32 @@
         auth_token: Optional[str] = None,
     ):
         self._gateway = None
         self.address = address or configuration.JAVA_GATEWAY_ADDRESS
         self.port = port or configuration.JAVA_GATEWAY_PORT
         self.auto_convert = auto_convert or configuration.JAVA_GATEWAY_AUTO_CONVERT
         self.auth_token = auth_token or configuration.JAVA_GATEWAY_AUTH_TOKEN
+        gateway_version = "unknown"
+        with contextlib.suppress(Py4JError):
+            # 1. Java gateway version is too old: doesn't have method 'getGatewayVersion()'
+            # 2. Error connecting to Java gateway
+            gateway_version = self.get_gateway_version()
+        if (
+            not __version__.endswith("dev")
+            and gateway_version
+            and not version_match(Version.DS, gateway_version)
+        ):
+            warnings.warn(
+                f"Using unmatched version of pydolphinscheduler (version {__version__}) "
+                f"and Java gateway (version {gateway_version}) may cause errors. "
+                "We strongly recommend you to find the matched version "
+                "(check: https://pypi.org/project/apache-dolphinscheduler)",
+                UserWarning,
+                stacklevel=2,
+            )
 
     @property
     def gateway(self) -> JavaGateway:
         """Launch java gateway to pydolphinscheduler.
 
         TODO Note that automatic conversion makes calling Java methods slightly less efficient because
         in the worst case, Py4J needs to go through all registered converters for all parameters.
@@ -99,15 +121,15 @@
         return self.gateway.entry_point.getDatasource(name, type)
 
     def get_resources_file_info(self, program_type: str, main_package: str):
         """Get resources file info through java gateway."""
         return self.gateway.entry_point.getResourcesFileInfo(program_type, main_package)
 
     def create_or_update_resource(
-        self, user_name: str, name: str, content: str, description: Optional[str] = None
+        self, user_name: str, name: str, description: str, content: str
     ):
         """Create or update resource through java gateway."""
         return self.gateway.entry_point.createOrUpdateResource(
             user_name, name, description, content
         )
 
     def query_resources_file_info(self, user_name: str, name: str):
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/base.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/base.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/base_side.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/base_side.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/connection.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/connection.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/datasource.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from pydolphinscheduler.models.connection import Connection
 from pydolphinscheduler.models.meta import ModelMeta
 
 
 class TaskUsage(NamedTuple):
     """Class for task usage just like datasource in web ui."""
 
-    id: str
+    id: int
     type: str
 
 
 class Datasource(metaclass=ModelMeta):
     """Model datasource, communicate with DolphinScheduler API server and convert Java Object into Python.
 
     We use metaclass :class:`pydolphinscheduler.models.meta.ModelMeta` to convert Java Object into Python.
@@ -65,17 +65,15 @@
                 "jdbcUrl": "jdbc:mysql://127.0.0.1:3306/test",
                 "driverClassName": "com.mysql.cj.jdbc.Driver",
                 "validationQuery": "select 1"
             }
 
     """
 
-    _PATTERN = re.compile(
-        "jdbc:.*://(?P<host>[\\w\\W]+):(?P<port>\\d+)/(?P<database>[\\w\\W]+)\\?"
-    )
+    _PATTERN = re.compile("jdbc:.*://(?P<host>[\\w\\W]+):(?P<port>\\d+)")
 
     _DATABASE_TYPE_MAP = dict(
         mysql=0,
         postgresql=1,
         hive=2,
         spark=3,
         clickhouse=4,
@@ -87,26 +85,26 @@
         redshift=10,
         dameng=11,
         starrocks=12,
     )
 
     def __init__(
         self,
-        st_db_type: str,
+        type_: str,
         name: str,
         connection_params: str,
         user_id: Optional[int] = None,
         id_: Optional[int] = None,
         note: Optional[str] = None,
     ):
         self.id = id_
         self.name = name
         self.note = note
         # TODO try to handle type_ in metaclass
-        self.st_db_type: JavaObject = st_db_type
+        self.type_: JavaObject = type_
         self.user_id = user_id
         self.connection_params = connection_params
 
     @classmethod
     def get(
         cls, datasource_name: str, datasource_type: Optional[str] = None
     ) -> "Datasource":
@@ -125,44 +123,42 @@
     @classmethod
     def get_task_usage_4j(
         cls, datasource_name: str, datasource_type: Optional[str] = None
     ) -> TaskUsage:
         """Get the necessary information of datasource for task usage in web UI."""
         datasource: "Datasource" = cls.get(datasource_name, datasource_type)
         return TaskUsage(
-            id=str(datasource.id),
-            type=datasource.type,
+            id=datasource.id,
+            type=datasource.type.upper(),
         )
 
     @property
     def connection(self) -> Connection:
         """Parse dolphinscheduler connection_params to Connection."""
         data = json.loads(self.connection_params)
 
-        pattern_match = self._PATTERN.match(
-            data.get("jdbcUrl", data.get("url", None))
-        ).groupdict()
+        address_match = self._PATTERN.match(data.get("jdbcUrl", None)).groupdict()
 
         return Connection(
-            host=pattern_match.get("host", None),
-            port=int(pattern_match.get("port", None)),
-            schema=pattern_match.get("database", None),
+            host=address_match.get("host", None),
+            port=int(address_match.get("port", None)),
+            schema=data.get("database", None),
             username=data.get("user", None),
             password=data.get("password", None),
         )
 
     @property
     def type(self) -> str:
         """Property datasource type."""
-        return self.st_db_type.getDescp()
+        return self.type_.getDescp()
 
     @property
     def type_code(self) -> str:
         """Property datasource type."""
-        return self.st_db_type.getCode()
+        return self.type_.getCode()
 
     @property
     def host(self) -> str:
         """Property datasource host, such as ``127.0.0.1`` or ``localhosts``."""
         return self.connection.host
 
     @property
```

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/meta.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/meta.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/project.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/project.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/queue.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/queue.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/tenant.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/tenant.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/user.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/user.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/models/worker_group.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/models/worker_group.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/base/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/base/bucket.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/bucket.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/base/git.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/base/git.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/github.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/github.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/gitlab.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/gitlab.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/local.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/local.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/oss.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/oss.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/resources_plugin/s3.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/resources_plugin/s3.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/condition.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/condition.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/datax.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/datax.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/dependent.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/dependent.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/dvc.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/dvc.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/flink.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/flink.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/func_wrap.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/func_wrap.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/http.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/http.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/kubernetes.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/map_reduce.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/map_reduce.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/mlflow.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/mlflow.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/openmldb.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/openmldb.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/procedure.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/procedure.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/python.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/python.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/pytorch.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/pytorch.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/sagemaker.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/shell.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/spark.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/spark.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/sql.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sql.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/sub_process.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sub_process.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/sub_workflow.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/sub_workflow.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/tasks/switch.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/tasks/switch.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/__init__.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/date.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/date.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/file.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/file.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/string.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/string.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/versions.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/versions.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/src/pydolphinscheduler/utils/yaml_parser.py` & `apache-dolphinscheduler-4.0.3/src/pydolphinscheduler/utils/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/tests/test_configuration.py` & `apache-dolphinscheduler-4.0.3/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `apache-dolphinscheduler-4.0.2a8/tests/test_docs.py` & `apache-dolphinscheduler-4.0.3/tests/test_docs.py`

 * *Files identical despite different names*

