# Comparing `tmp/globus-compute-endpoint-2.0.0a1.tar.gz` & `tmp/globus-compute-endpoint-2.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.0.0a1.tar", last modified: Mon Apr  3 22:15:27 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.0.1a0.tar", last modified: Fri Apr 14 15:04:24 2023, max compression
```

## Comparing `globus-compute-endpoint-2.0.0a1.tar` & `globus-compute-endpoint-2.0.1a0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.226771 globus-compute-endpoint-2.0.0a1/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)      734 2023-04-03 22:15:27.226829 globus-compute-endpoint-2.0.0a1/PKG-INFO
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.221092 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/
--rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    19121 2023-04-03 22:11:17.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.222938 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/config.py
--rw-r--r--   0 lei        (501) staff       (20)      707 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/default_config.py
--rw-r--r--   0 lei        (501) staff       (20)    24947 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 lei        (501) staff       (20)    21117 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.223536 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.223773 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     4374 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/config.py
--rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.223900 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/
--rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.225294 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 lei        (501) staff       (20)    34995 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 lei        (501) staff       (20)     8427 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.225410 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/
--rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.225759 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.226333 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/
--rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     6989 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-03 22:13:08.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.221797 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)      734 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     2637 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-03 22:15:27.000000 globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-03 22:15:27.227104 globus-compute-endpoint-2.0.0a1/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3181 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/setup.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-03 22:15:27.226656 globus-compute-endpoint-2.0.0a1/tests/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/tests/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1937 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/tests/conftest.py
--rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-03 17:17:07.000000 globus-compute-endpoint-2.0.0a1/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.728863 globus-compute-endpoint-2.0.1a0/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)      734 2023-04-14 15:04:24.728943 globus-compute-endpoint-2.0.1a0/PKG-INFO
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.712566 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    18802 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.723125 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    24955 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.724002 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.724434 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/config.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.724593 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.726758 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    34995 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8427 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.726980 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.727456 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.728325 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-14 15:02:34.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.713578 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)      734 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     2637 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-14 15:04:24.000000 globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-14 15:04:24.729232 globus-compute-endpoint-2.0.1a0/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3179 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-14 15:04:24.728714 globus-compute-endpoint-2.0.1a0/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2693 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a0/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a0/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.0.0a1/LICENSE` & `globus-compute-endpoint-2.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/PKG-INFO` & `globus-compute-endpoint-2.0.1a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.0a1
+Version: 2.0.1a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,64 @@
 from __future__ import annotations
 
+import difflib
 import importlib.util
 import json
 import logging
-import os.path
 import pathlib
 import shutil
 import sys
 import uuid
 
 import click
 from click import ClickException
+from globus_compute_endpoint.endpoint.endpoint import Endpoint
+from globus_compute_endpoint.endpoint.endpoint_manager import EndpointManager
+from globus_compute_endpoint.endpoint.utils.config import Config
+from globus_compute_endpoint.logging_config import setup_logging
+from globus_compute_endpoint.version import DEPRECATION_FUNCX_ENDPOINT
 from globus_compute_sdk.sdk.login_manager import LoginManager
+from globus_compute_sdk.sdk.login_manager.tokenstore import ensure_compute_dir
 from globus_compute_sdk.sdk.login_manager.whoami import print_whoami_info
 
-from .endpoint.endpoint import Endpoint
-from .endpoint.endpoint_manager import EndpointManager
-from .endpoint.utils.config import Config
-from .logging_config import setup_logging
-from .version import DEPRECATION_FUNCX_ENDPOINT
-
 log = logging.getLogger(__name__)
 
 
 class CommandState:
     def __init__(self):
-        self.endpoint_config_dir: str = str(pathlib.Path.home() / ".funcx")
+        self.endpoint_config_dir: pathlib.Path = init_config_dir()
         self.debug = False
         self.no_color = False
         self.log_to_console = False
         self.endpoint_uuid = None
         self.die_with_parent = False
 
     @classmethod
     def ensure(cls) -> CommandState:
         return click.get_current_context().ensure_object(CommandState)
 
 
-def init_endpoint_configuration_dir(conf_dir: pathlib.Path):
-    if not conf_dir.exists():
-        log.info("No existing configuration found at %s. Initializing...", conf_dir)
-        try:
-            conf_dir.mkdir(mode=0o700, exist_ok=True)
-        except Exception as exc:
-            e = click.ClickException(
-                f"{exc}\n\nUnable to create configuration directory"
-            )
-            raise e from exc
-
-    elif not conf_dir.is_dir():
-        raise click.ClickException(
-            f"File already exists: {conf_dir}\n\n"
-            "Refusing to initialize Globus Compute configuration directory: "
-            "path already exists"
-        )
+def init_config_dir() -> pathlib.Path:
+    try:
+        return ensure_compute_dir()
+    except FileExistsError as e:
+        raise ClickException(str(e))
 
 
 def get_config_dir() -> pathlib.Path:
     state = CommandState.ensure()
-    return pathlib.Path(state.endpoint_config_dir)
+    return state.endpoint_config_dir
 
 
 def get_cli_endpoint() -> Endpoint:
     # this getter creates an Endpoint object from the CommandState
     # it takes its various configurable values from the current CommandState
     # as a result, any number of CLI options may be used to tweak the CommandState
     # via callbacks, and the Endpoint will only be constructed within commands which
     # access the Endpoint via this getter
-    conf_dir = get_config_dir()
-    init_endpoint_configuration_dir(conf_dir)
-
     state = CommandState.ensure()
     endpoint = Endpoint(debug=state.debug)
 
     return endpoint
 
 
 def set_param_to_config(ctx, param, value):
@@ -141,15 +126,15 @@
     return click.argument("name", required=False, default="default")(f)
 
 
 def config_dir_callback(ctx, param, value):
     if value is None or ctx.resilient_parsing:
         return
     state = CommandState.ensure()
-    state.endpoint_config_dir = value
+    state.endpoint_config_dir = pathlib.Path(value)
 
 
 @click.group("globus-compute-endpoint")
 @click.option(
     "-c",
     "--config-dir",
     default=None,
@@ -177,30 +162,35 @@
 @click.option(
     "--multi-tenant",
     is_flag=True,
     default=False,
     hidden=True,
     help="Configure endpoint as multi-tenant capable",
 )
+@click.option(
+    "--display-name",
+    help="A human readable display name for the endpoint, if desired",
+)
 @name_arg
 @common_options
 def configure_endpoint(
     *,
     name: str,
     endpoint_config: str | None,
     multi_tenant: bool,
+    display_name: str | None,
 ):
     """Configure an endpoint
 
-    Drops a config.py template into the funcx configs directory.
-    The template usually goes to ~/.funcx/<ENDPOINT_NAME>/config.py
+    Drops a config.py template into the Globus Compute configs directory.
+    The template usually goes to ~/.globus_compute/<ENDPOINT_NAME>/config.py
     """
     compute_dir = get_config_dir()
     ep_dir = compute_dir / name
-    Endpoint.configure_endpoint(ep_dir, endpoint_config, multi_tenant)
+    Endpoint.configure_endpoint(ep_dir, endpoint_config, multi_tenant, display_name)
 
 
 @app.command(name="start", help="Start an endpoint by name")
 @name_arg
 @start_options
 @common_options
 def start_endpoint(*, name: str, **_kwargs):
@@ -309,81 +299,73 @@
 
     The force flag will overwrite an existing (non-directory) config.py.bak
 
     This method uses a randomly generated intermediate output file in case
     there are any permission or unforeseen file system issues
     """
     ep_dir = get_config_dir() / name
-    old_config = ep_dir / "config.py"
+    config_path = ep_dir / "config.py"
     config_backup = ep_dir / "config.py.bak"
 
     try:
-        # Scan config.py first in case it's a no-op
-        with open(old_config) as f:
-            lines = f.readlines()
-        reformatted_count = 0
-        output_lines = []
-        if lines:
-            for line in lines:
-                modified_line = False
-                for k, v in FUNCX_COMPUTE_IMPORT_UPDATES.items():
-                    if line.startswith(k):
-                        modified_line = True
-                        output_lines.append(line.replace(k, v, 1))
-                        break
-                if not modified_line:
-                    output_lines.append(line)
-                else:
-                    reformatted_count += 1
-        format_msg = f"No funcX import statements found in config.py for {name}"
-        if reformatted_count == 0:
-            return format_msg
-
-        remove_backup = False
-        if os.path.exists(config_backup):
-            if not force:
-                msg = (
-                    f"{config_backup} already exists.\n"
-                    "Rename it or use the --force flag to update config."
-                )
-                raise ClickException(msg)
-            if os.path.isdir(config_backup):
-                msg = (
-                    f"{config_backup} is a directory.\n"
-                    "Rename it before proceeding with config update."
-                )
-                raise ClickException(msg)
-            remove_backup = True
+        config_text = config_path.read_text()
+        upd_config_text = config_text
+
+        for original, repl in FUNCX_COMPUTE_IMPORT_UPDATES.items():
+            upd_config_text = upd_config_text.replace(original, repl)
+
+        if upd_config_text == config_text:
+            return f"No funcX import statements found in config.py for {name}"
 
-        # Write to temporary file in case of unexpected file errors
+        change_diff = "".join(
+            difflib.unified_diff(
+                config_text.splitlines(keepends=True),
+                upd_config_text.splitlines(keepends=True),
+                n=3,  # Typical 3 lines of context
+            )
+        )
+
+        if config_backup.exists() and not force:
+            msg = (
+                f"{config_backup} already exists.\n"
+                "Rename it or use the --force flag to update config."
+            )
+            raise ClickException(msg)
+        elif config_backup.is_dir():
+            msg = (
+                f"{config_backup} is a directory.\n"
+                "Rename it before proceeding with config update."
+            )
+            raise ClickException(msg)
+
+        # Write to temporary file in case of issues
         tmp_output_path = ep_dir / ("config.py." + uuid.uuid4().hex)
-        with open(tmp_output_path.name, "w") as f:
-            for line in output_lines:
-                f.write(line)
-        if remove_backup:
-            os.remove(config_backup)
-        shutil.move(old_config, config_backup)  # Preserve file timestamp
-        os.rename(tmp_output_path.name, old_config)
-        format_msg = (
-            f"{reformatted_count} lines were modified for endpoint {name}\n"
+        tmp_output_path.write_text(upd_config_text)
+
+        # Rename files last, as it's the least likely to err
+        config_backup.unlink(missing_ok=True)
+        shutil.move(config_path, config_backup)  # Preserve file timestamp
+        shutil.move(tmp_output_path, config_path)
+
+        return (
+            f"Applied following diff for endpoint {name}:\n{change_diff}\n\n"
             f"  The previous config has been renamed to {config_backup}"
         )
-        return format_msg
 
     except FileNotFoundError as err:
         msg = f"No config.py was found for endpoint ({name}) in {ep_dir}"
         raise ClickException(msg) from err
     except ClickException:
         raise
     except Exception as err:
         msg = f"Unknown Exception {err} attempting to reformat config.py in {ep_dir}"
         raise ClickException(msg) from err
 
 
-def read_config(endpoint_dir: pathlib.Path, warn_funcx_imports: bool = True) -> Config:
+def read_config(endpoint_dir: pathlib.Path) -> Config:
     endpoint_name = endpoint_dir.name
 
     try:
         conf_path = endpoint_dir / "config.py"
         spec = importlib.util.spec_from_file_location("config", conf_path)
         if not (spec and spec.loader):
             raise Exception(f"Unable to import configuration (no spec): {conf_path}")
@@ -420,15 +402,15 @@
             "\n\nFailed to find expected data structure in configuration file."
             "\nHas the configuration file been corrupted or modified incorrectly?\n"
         )
         raise ClickException(msg) from err
 
     except ModuleNotFoundError as err:
         # Catch specific error when old config.py references funcx_endpoint
-        if warn_funcx_imports and "No module named 'funcx_endpoint." in err.msg:
+        if "No module named 'funcx_endpoint'" in err.msg:
             msg = (
                 f"{conf_path} contains import statements from a previously "
                 "configured endpoint that uses the (deprecated) "
                 "funcx-endpoint library. Please update the imports to reference "
                 "globus_compute_endpoint.\n\ni.e.\n"
                 "    from funcx_endpoint.endpoint.utils.config -> "
                 "from globus_compute_endpoint.endpoint.utils.config\n"
@@ -585,13 +567,23 @@
 def cli_run():
     """Entry point for setuptools to point to"""
     app()
 
 
 def cli_run_funcx():
     """Entry point that prints a custom message. i.e. deprecation warnings"""
-    print(DEPRECATION_FUNCX_ENDPOINT)
+    fmt = DEPRECATION_FUNCX_ENDPOINT
+
+    # Colorized notice to be a bit more visible
+    fmt = "{title}DEPRECATION NOTICE{rs}\n{body}" + fmt + "{rs}"
+    title = frs = body = rs = ""
+    if sys.stderr.isatty():
+        title = "\033[37;41m"  # White FG, Red BG
+        body = "\033[33m"  # Yellow FG
+        rs = "\033[0m"  # Reset colors
+
+    print(fmt.format(title=title, body=body, frs=frs, rs=rs), file=sys.stderr)
     app()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/default_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from globus_compute_endpoint.endpoint.utils.config import Config
 from globus_compute_endpoint.executors import HighThroughputExecutor
 from parsl.providers import LocalProvider
 
 config = Config(
+    display_name=None,  # If None, defaults to the endpoint name
     executors=[
         HighThroughputExecutor(
             provider=LocalProvider(
                 init_blocks=1,
                 min_blocks=0,
                 max_blocks=1,
             ),
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,17 +54,41 @@
 
     @staticmethod
     def update_config_file(
         ep_name: str,
         original_path: pathlib.Path,
         target_path: pathlib.Path,
         multi_tenant: bool,
+        display_name: str | None,
     ):
         endpoint_config = Template(original_path.read_text()).substitute(name=ep_name)
 
+        # Note that this logic does NOT support replacing arbitrary
+        # display_name="abc xyz" entries, as str quote parsing is beyond the
+        # current use case of calling this method only at endpoint creation
+        display_str = "None" if display_name is None else f'"{display_name}"'
+        display_text = f"display_name={display_str},"
+
+        d_index = endpoint_config.find("display_name")
+        if d_index != -1:
+            if endpoint_config[d_index + 13 : d_index + 18] == "None,":
+                if display_name is not None:
+                    endpoint_config = endpoint_config.replace(
+                        "display_name=None,", display_text
+                    )
+            else:
+                raise Exception(
+                    "Modifying existing display_name not supported "
+                    f"at this time. Please edit {original_path} manually."
+                )
+        else:
+            endpoint_config = endpoint_config.replace(
+                "\nconfig = Config(\n", f"\nconfig = Config(\n    {display_text}\n"
+            )
+
         if endpoint_config.find("multi_tenant=") != -1:
             # If the option is already in the config, merely update the value
             endpoint_config = re.sub(
                 "multi_tenant=(True|False)",
                 f"multi_tenant={multi_tenant is True}",
                 endpoint_config,
             )
@@ -77,68 +101,75 @@
         target_path.write_text(endpoint_config)
 
     @staticmethod
     def init_endpoint_dir(
         endpoint_dir: pathlib.Path,
         endpoint_config: pathlib.Path | None = None,
         multi_tenant=False,
+        display_name: str | None = None,
     ):
         """Initialize a clean endpoint dir
 
         :param endpoint_dir pathlib.Path Path to the endpoint configuration dir
         :param endpoint_config str Path to a config file to be used instead
          of the Globus Compute default config file
         :param multi_tenant bool Whether the endpoint is a multi-user endpoint
+        :param display_name str A display name to use, if desired
         """
         log.debug(f"Creating endpoint dir {endpoint_dir}")
         user_umask = os.umask(0o0077)
         os.umask(0o0077 | (user_umask & 0o0400))  # honor only the UR bit for dirs
         try:
             # pathlib.Path does not handle unusual umasks (e.g., 0o0111) so well
             # in the parents=True case, so temporarily change it.  This is nominally
-            # only an issue for totally new users (no .funcx/!), but that is also
-            # precisely the interaction -- the first one -- that should go smoothly
+            # only an issue for totally new users (no .globus_compute/!), but that is
+            # also precisely the interaction -- the first one -- that should go smoothly
             endpoint_dir.mkdir(parents=True, exist_ok=True)
 
             config_target_path = Endpoint._config_file_path(endpoint_dir)
 
             if endpoint_config is None:
                 endpoint_config = pathlib.Path(endpoint_default_config.__file__)
 
             Endpoint.update_config_file(
                 endpoint_dir.name,
                 endpoint_config,
                 config_target_path,
                 multi_tenant,
+                display_name,
             )
         finally:
             os.umask(user_umask)
 
     @staticmethod
     def configure_endpoint(
-        conf_dir: pathlib.Path, endpoint_config: str | None, multi_tenant: bool = False
+        conf_dir: pathlib.Path,
+        endpoint_config: str | None,
+        multi_tenant: bool = False,
+        display_name: str | None = None,
     ):
         ep_name = conf_dir.name
         if conf_dir.exists():
+            print(conf_dir)
             print(f"config dir <{ep_name}> already exists")
             raise Exception("ConfigExists")
 
         templ_conf_path = pathlib.Path(endpoint_config) if endpoint_config else None
-        Endpoint.init_endpoint_dir(conf_dir, templ_conf_path, multi_tenant)
+        Endpoint.init_endpoint_dir(
+            conf_dir, templ_conf_path, multi_tenant, display_name
+        )
         config_path = Endpoint._config_file_path(conf_dir)
         if multi_tenant:
             print(f"Created multi-tenant profile for <{ep_name}>")
         else:
             print(f"Created profile for <{ep_name}>")
         print(
             f"\n    Configuration file: {config_path}\n"
             "\nUse the `start` subcommand to run it:\n"
             f"\n    $ globus-compute-endpoint start {ep_name}"
-            # If we want to show 'funcx-endpoint start' when using the wrapper
-            # f"\n    $ {sys.argv[0]} start {ep_name}"
         )
 
     @staticmethod
     def get_endpoint_id(endpoint_dir: pathlib.Path) -> str | None:
         info_file_path = endpoint_dir / "endpoint.json"
         try:
             return json.loads(info_file_path.read_bytes())["endpoint_id"]
@@ -197,19 +228,14 @@
                     "A prior Endpoint instance appears to have been terminated without "
                     "proper cleanup. Cleaning up now."
                 )
                 Endpoint.pidfile_cleanup(endpoint_dir)
 
         result_store = ResultStore(endpoint_dir=endpoint_dir)
 
-        # From this point on, we don't read from stdin;
-        with open(os.devnull) as stdin:
-            if os.dup2(stdin.fileno(), 0) != 0:
-                raise Exception("Unable to close stdin")
-
         # Create a daemon context
         # If we are running a full detached daemon then we will send the output to
         # log files, otherwise we can piggy back on our stdout
         if endpoint_config.detach_endpoint:
             stdout: typing.TextIO = open(
                 os.path.join(endpoint_dir, endpoint_config.stdout), "a+"
             )
@@ -247,14 +273,15 @@
             try:
                 fx_client = Endpoint.get_funcx_client(endpoint_config)
                 reg_info = fx_client.register_endpoint(
                     endpoint_dir.name,
                     endpoint_uuid,
                     metadata=Endpoint.get_metadata(endpoint_config),
                     multi_tenant=False,
+                    display_name=endpoint_config.display_name,
                 )
 
             except GlobusAPIError as e:
                 if e.http_status in (409, 410, 423):
                     # CONFLICT, GONE or LOCKED
                     log.warning(f"Endpoint registration blocked.  [{e.message}]")
                     exit(os.EX_UNAVAILABLE)
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/interchange.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 # multiprocessing.Event is a method, not a class
 # to annotate, we need the "real" class
 # see: https://github.com/python/typeshed/issues/4266
 from multiprocessing.synchronize import Event as EventType
 
 import globus_compute_endpoint.endpoint.utils.config
 import pika.exceptions
+import setproctitle
 from globus_compute_common.messagepack import InvalidMessageError, pack, unpack
 from globus_compute_common.messagepack.message_types import (
+    EPStatusReport,
     Result,
     ResultErrorDetails,
     Task,
 )
 from globus_compute_endpoint import __version__ as funcx_endpoint_version
 from globus_compute_endpoint.endpoint.messages_compat import (
     convert_to_internaltask,
@@ -140,22 +142,20 @@
             raise
 
         self._test_start = False
 
     def load_config(self):
         """Load the config"""
         log.info("Loading endpoint local config")
-
         self.results_passthrough = mpQueue()
         self.executors: dict[
             str, globus_compute_endpoint.executors.HighThroughputExecutor
         ] = {}
         for executor in self.config.executors:
             log.info(f"Initializing executor: {executor.label}")
-            executor.funcx_service_address = self.config.funcx_service_address
             if not executor.endpoint_id:
                 executor.endpoint_id = self.endpoint_id
             else:
                 if not executor.endpoint_id == self.endpoint_id:
                     eep_id = f"Executor({executor.endpoint_id})"
                     sep_id = f"Interchange({self.endpoint_id})"
                     raise Exception(f"InconsistentEndpointId: {eep_id} != {sep_id}")
@@ -303,14 +303,15 @@
             except pika.exceptions.ConnectionClosedByBroker as e:
                 log.warning(f"AMQP service closed connection: {e}")
             except pika.exceptions.ProbableAuthenticationError as e:
                 log.error(f"Unable to connect to AMQP service: {e}")
                 self._kill_event.set()
             except Exception:
                 log.error("Unhandled exception in main kernel.")
+                log.debug("Unhandled exception in main kernel.", exc_info=True)
             finally:
                 if not self._kill_event.is_set():
                     self._reconnect_fail_counter += 1
                     log.info(
                         "Reconnection count: %s (of %s)",
                         self._reconnect_fail_counter,
                         self.reconnect_attempt_limit,
@@ -345,17 +346,15 @@
         non-happy path.  If an error occurs that is too "unhappy" (e.g., communication
         with RMQ fails), the catch-all solution is to "reboot" and try again.  That is,
         this method exits, communication is shutdown, started again, and we restart
         this method.
         """
         log.debug("_main_loop begins")
 
-        results_publisher = ResultQueuePublisher(
-            queue_info=self.result_q_info,
-        )
+        results_publisher = ResultQueuePublisher(queue_info=self.result_q_info)
 
         with results_publisher:
             executor = list(self.executors.values())[0]
 
             num_tasks_forwarded = 0
             num_results_forwarded = 0
 
@@ -439,15 +438,15 @@
                         log.warning(
                             f"Invalid message received: no task_id.  Ignoring. {exc}"
                         )
                         continue
 
                     try:
                         # This either works or it doesn't; if it doesn't, then
-                        # serialize an execption and send _that_
+                        # serialize an exception and send _that_
                         # will be a packed EPStatusReport or Result
                         message = try_convert_to_messagepack(packed_result)
 
                     except Exception as exc:
                         log.exception(
                             f"Unable to parse result message for task {task_id}."
                             "   Marking task as failed."
@@ -467,15 +466,16 @@
                         message = pack(Result(**kwargs))
 
                     if task_id:
                         log.debug(f"Forwarding result for task {task_id}")
 
                     try:
                         results_publisher.publish(message)
-                        num_results_forwarded += 1  # Safe given GIL
+                        if task_id:
+                            num_results_forwarded += 1  # Safe given GIL
 
                     except Exception:
                         # Publishing didn't work -- quiesce and see if a simple restart
                         # fixes the issue.
                         self._quiesce_event.set()
 
                         log.exception("Something broke while forwarding results")
@@ -495,30 +495,109 @@
             result_processor_thread = threading.Thread(
                 target=process_pending_results, name="Pending Result Handler"
             )
             stored_processor_thread.start()
             task_processor_thread.start()
             result_processor_thread.start()
 
-            log.debug("_main_loop entered running state")
             last_t, last_r = 0, 0
+
+            soft_idle_limit = max(0, self.config.idle_heartbeats_soft)
+            hard_idle_limit = max(soft_idle_limit + 1, self.config.idle_heartbeats_hard)
+            soft_idle_heartbeats = 0  # "happy path" idle timeout
+            hard_idle_heartbeats = 0  # catch-all idle timeout
+
+            live_proc_title = setproctitle.getproctitle()
+            log.debug("_main_loop entered running state")
             while not self._quiesce_event.wait(self.heartbeat_period):
                 # Possibly TOCTOU here, but we don't need to be super precise.  The
                 # point here is to mention "still alive" and that we're still working
                 num_t, num_r = num_tasks_forwarded, num_results_forwarded
+                diff_t, diff_r = num_t - last_t, num_r - last_r
                 log.debug(
                     "Heartbeat.  Approximate Tasks and Results forwarded since last "
                     "heartbeat: %s (T), %s (R)",
-                    num_t - last_t,
-                    num_r - last_r,
+                    diff_t,
+                    diff_r,
                 )
                 last_t, last_r = num_t, num_r
 
                 # only reset come heartbeat and still alive
                 self._reconnect_fail_counter = 0
 
+                if not soft_idle_limit:
+                    # idle timeout not enabled; "always on"
+                    continue
+
+                if diff_t or diff_r:
+                    # a task moved; reset idle heartbeat counter
+                    if soft_idle_heartbeats or hard_idle_heartbeats:
+                        log.info(
+                            "Moved to active state (due to tasks processed since"
+                            " last heartbeat)."
+                        )
+                    setproctitle.setproctitle(live_proc_title)
+                    soft_idle_heartbeats = 0
+                    hard_idle_heartbeats = 0
+                    continue
+
+                # only start "timer" if we've at least done *some* work
+                hard_idle_heartbeats += 1
+                if (num_t or num_r) and num_r >= num_t:
+                    # similar to above, only start "timer" if *idle* ... but
+                    # note that given self.result_store, it's possible to
+                    # have forwarded more results than tasks received.
+                    soft_idle_heartbeats += 1
+                    shutdown_s = soft_idle_limit - soft_idle_heartbeats
+                    shutdown_s *= self.heartbeat_period
+
+                    if soft_idle_heartbeats == 1:
+                        log.info(
+                            "In idle state (due to no task or result movement);"
+                            f" shut down in {shutdown_s:,}s.  (idle_heartbeats_soft)"
+                        )
+                    idle_proc_title = "[idle; shut down in {:,}s] {}"
+                    setproctitle.setproctitle(
+                        idle_proc_title.format(shutdown_s, live_proc_title)
+                    )
+
+                    if soft_idle_heartbeats >= soft_idle_limit:
+                        log.info("Idle heartbeats reached.  Shutting down.")
+                        self.time_to_quit = True
+                        self.stop()
+
+                elif hard_idle_heartbeats > hard_idle_limit:
+                    log.warning("Shutting down due to idle heartbeats HARD limit.")
+                    self.time_to_quit = True
+                    self.stop()
+
+                elif hard_idle_heartbeats > soft_idle_limit:
+                    shutdown_s = hard_idle_limit - hard_idle_heartbeats
+                    shutdown_s *= self.heartbeat_period
+                    if hard_idle_heartbeats == soft_idle_limit + 1:
+                        # only log the first time; no sense in filling logs
+                        log.info(
+                            "Possibly idle -- no task or result movement.  Will"
+                            f" shut down in {shutdown_s:,}s.  (idle_heartbeats_hard)"
+                        )
+                    idle_proc_title = "[possibly idle; shut down in {:,}s] {}"
+                    setproctitle.setproctitle(
+                        idle_proc_title.format(shutdown_s, live_proc_title)
+                    )
+
             # The timeouts aren't nominally necessary because if the above loop has
             # quit, then the _quiesce_event is set, and both threads check that event
             # every internal iteration.  But "for kicks."
             stored_processor_thread.join(timeout=5)
             task_processor_thread.join(timeout=5)
             result_processor_thread.join(timeout=5)
+
+            # let higher-level error handling take over if the following excepts
+            message = EPStatusReport(
+                endpoint_id=self.endpoint_id,
+                # 0 == "no more heartbeats coming"
+                global_state={"heartbeat_period": 0},
+                task_statuses={},
+            )
+            results_publisher.publish(pack(message))
+
+            log.debug("_main_loop exits")
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,14 +47,34 @@
         Default: 30s
 
     heartbeat_threshold: int (seconds)
         Seconds since the last hearbeat message from the Globus Compute web service
         after which the connection is assumed to be disconnected.
         Default: 120s
 
+    idle_heartbeats_soft: int (count)
+        Number of heartbeats after an endpoint is idle (no outstanding tasks or
+        results, and at least 1 task or result has been forwarded) before the
+        endpoint shuts down.  If 0, then the endpoint must be manually triggered
+        to shut down (e.g., SIGINT or SIGTERM).
+        Default: 0
+
+    idle_heartbeats_hard: int (count)
+        Number of heartbeats after no task or result has moved before the endpoint
+        shuts down.  Unlike `idle_heartbeats_soft`, this idle timer does not require
+        that there are no outstanding tasks or results.  If no task or result has
+        moved in this many heartbeats, then the endpoint will shut down.  In
+        particular, this is intended to catch the error condition that a worker
+        has gone missing, and will thus _never_ return the task it was sent.
+        Note that this setting is only enabled if the `idle_heartbeats_soft` is a
+        value greater than 0.  Suggested value: a multiplier of heartbeat_period
+        equivalent to two days.  For example, if `heartbeat_period` is 30s, then
+        suggest 5760.
+        Default: 5760
+
     stdout : str
         Path where the endpoint's stdout should be written
         Default: ./interchange.stdout
 
     stderr : str
         Path where the endpoint's stderr should be written
         Default: ./interchange.stderr
@@ -67,28 +87,36 @@
     log_dir : str
         Optional path string to the top-level directory where logs should be written to.
         Default: None
 
     multi_tenant : bool | None
         Designates the endpoint as a multi-tenant endpoint
         Default: None
+
+    display_name : str | None
+        The display name for the endpoint.  If None, defaults to name
+        Default: None
     """
 
     def __init__(
         self,
         # Execution backed
         executors: list = _DEFAULT_EXECUTORS,
         # Connection info
         environment: str | None = None,
         funcx_service_address=None,
         multi_tenant: bool | None = None,
         # Tuning info
         heartbeat_period=30,
         heartbeat_threshold=120,
+        idle_heartbeats_soft=0,
+        idle_heartbeats_hard=5760,  # Two days, divided by `heartbeat_period`
         detach_endpoint=True,
+        # Misc info
+        display_name: str | None = None,
         # Logging info
         log_dir=None,
         stdout="./endpoint.log",
         stderr="./endpoint.log",
         **kwargs,
     ):
         for deprecated_name in ("results_ws_uri", "warn_about_url_mismatch"):
@@ -120,13 +148,18 @@
         self.funcx_service_address = funcx_service_address
 
         self.multi_tenant = multi_tenant is True
 
         # Tuning info
         self.heartbeat_period = heartbeat_period
         self.heartbeat_threshold = heartbeat_threshold
+        self.idle_heartbeats_soft = int(max(0, idle_heartbeats_soft))
+        self.idle_heartbeats_hard = int(max(0, idle_heartbeats_hard))
         self.detach_endpoint = detach_endpoint
 
         # Logging info
         self.log_dir = log_dir
         self.stdout = stdout
         self.stderr = stderr
+
+        # Misc info
+        self.display_name = display_name
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,16 @@
         )
         self._thread.daemon = True
 
     def start(self, interchange):
         """Actually start the strategy
         Parameters
         ----------
-        interchange: gce.executors.high_throughput.interchange.Interchange
+        interchange:
+         globus_compute_endpoint.executors.high_throughput.interchange.Interchange
             Interchange to bind the strategy to
         """
         self.interchange = interchange
         if hasattr(interchange, "provider"):
             log.debug(
                 "Strategy bounds-> init:{}, min:{}, max:{}".format(
                     interchange.provider.init_blocks,
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.0a1"
+__version__ = "2.0.1a0"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.0a1
+Version: 2.0.1a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `globus-compute-endpoint-2.0.0a1/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.0.1a0/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.0a1/setup.py` & `globus-compute-endpoint-2.0.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk>=2.0.0a0",
+    "globus-compute-sdk>=2.0.0",
     "globus-compute-common==0.1.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
```

### Comparing `globus-compute-endpoint-2.0.0a1/tests/conftest.py` & `globus-compute-endpoint-2.0.1a0/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,50 @@
 from __future__ import annotations
 
 import random
+import signal
 import string
 import time
 import uuid
 
 import globus_compute_sdk as gc
 import globus_sdk
 import pytest
 import responses
 from globus_compute_sdk.sdk.web_client import WebClient
 
 
+@pytest.fixture(autouse=True)
+def verify_all_tests_reset_signals():
+    orig_sig_handlers = [
+        (sig, signal.getsignal(sig))
+        for sig in range(1, 21)
+        if sig not in (signal.SIGKILL, signal.SIGSTOP)  # the uncatchables
+    ]
+    yield
+    handlers = [(sig, sigh, signal.getsignal(sig)) for sig, sigh in orig_sig_handlers]
+    for sig, bef, aft in handlers:
+        assert bef == aft, f"Signal {sig} not reset"
+
+
+@pytest.fixture
+def reset_signals():
+    # As identified by an interaction with Parsl during our UTs, ensure that we
+    # return the signals after each test.  Interprocess play is fun ...
+    orig_sig_handlers = [
+        (sig, signal.getsignal(sig))
+        for sig in range(1, 21)
+        if sig not in (signal.SIGKILL, signal.SIGSTOP)  # the uncatchables
+    ]
+
+    yield
+    for sig, sigh in orig_sig_handlers:
+        signal.signal(sig, sigh)
+
+
 @pytest.fixture(scope="session")
 def endpoint_uuid():
     return str(uuid.UUID(int=0))
 
 
 @pytest.fixture(scope="session")
 def default_endpoint_id():
@@ -38,17 +67,14 @@
 
     def logout(self) -> bool:
         ...
 
     def get_auth_client(self) -> globus_sdk.AuthClient:
         return globus_sdk.AuthClient(authorizer=globus_sdk.NullAuthorizer())
 
-    def get_search_client(self) -> globus_sdk.SearchClient:
-        return globus_sdk.SearchClient(authorizer=globus_sdk.NullAuthorizer())
-
     def get_web_client(self, *, base_url: str | None = None) -> WebClient:
         return WebClient(
             base_url="https://api2.funcx.org/v2/",
             authorizer=globus_sdk.NullAuthorizer(),
         )
```

### Comparing `globus-compute-endpoint-2.0.0a1/tests/utils.py` & `globus-compute-endpoint-2.0.1a0/tests/utils.py`

 * *Files identical despite different names*

