# Comparing `tmp/create_docker_compose-0.1.tar.gz` & `tmp/create_docker_compose-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create_docker_compose-0.1.tar", last modified: Fri Apr 14 10:50:49 2023, max compression
+gzip compressed data, was "create_docker_compose-0.2.tar", last modified: Fri Apr 14 12:48:55 2023, max compression
```

## Comparing `create_docker_compose-0.1.tar` & `create_docker_compose-0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:50:49.388026 create_docker_compose-0.1/
--rw-rw-rw-   0        0        0       66 2023-04-14 10:50:49.388026 create_docker_compose-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-14 10:50:49.378024 create_docker_compose-0.1/create_docker_compose/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:39:37.000000 create_docker_compose-0.1/create_docker_compose/__init__.py
--rw-rw-rw-   0        0        0     1427 2023-04-14 10:38:15.000000 create_docker_compose-0.1/create_docker_compose/create_docker_compose.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:50:49.385025 create_docker_compose-0.1/create_docker_compose.egg-info/
--rw-rw-rw-   0        0        0       66 2023-04-14 10:50:49.000000 create_docker_compose-0.1/create_docker_compose.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-14 10:50:49.000000 create_docker_compose-0.1/create_docker_compose.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 10:50:49.000000 create_docker_compose-0.1/create_docker_compose.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-04-14 10:50:49.000000 create_docker_compose-0.1/create_docker_compose.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-14 10:50:49.000000 create_docker_compose-0.1/create_docker_compose.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-14 10:50:49.000000 create_docker_compose-0.1/create_docker_compose.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 10:50:49.387025 create_docker_compose-0.1/create_env_file/
--rw-rw-rw-   0        0        0        0 2023-04-14 10:39:37.000000 create_docker_compose-0.1/create_env_file/__init__.py
--rw-rw-rw-   0        0        0     1361 2023-04-14 10:38:23.000000 create_docker_compose-0.1/create_env_file/create_env_file.py
--rw-rw-rw-   0        0        0       42 2023-04-14 10:50:49.389025 create_docker_compose-0.1/setup.cfg
--rw-rw-rw-   0        0        0      420 2023-04-14 10:42:29.000000 create_docker_compose-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:48:55.228325 create_docker_compose-0.2/
+-rw-rw-rw-   0        0        0     4094 2023-04-14 12:48:55.227323 create_docker_compose-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3879 2023-04-14 12:42:11.000000 create_docker_compose-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 12:48:55.193324 create_docker_compose-0.2/create_docker_compose/
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:39:37.000000 create_docker_compose-0.2/create_docker_compose/__init__.py
+-rw-rw-rw-   0        0        0     1427 2023-04-14 10:38:15.000000 create_docker_compose-0.2/create_docker_compose/create_docker_compose.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:48:55.224324 create_docker_compose-0.2/create_docker_compose.egg-info/
+-rw-rw-rw-   0        0        0     4094 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2023-04-14 12:48:55.000000 create_docker_compose-0.2/create_docker_compose.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 12:48:55.226324 create_docker_compose-0.2/create_env_file/
+-rw-rw-rw-   0        0        0        0 2023-04-14 10:39:37.000000 create_docker_compose-0.2/create_env_file/__init__.py
+-rw-rw-rw-   0        0        0     1361 2023-04-14 10:38:23.000000 create_docker_compose-0.2/create_env_file/create_env_file.py
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:48:55.229324 create_docker_compose-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-04-14 12:48:35.000000 create_docker_compose-0.2/setup.py
```

### Comparing `create_docker_compose-0.1/create_docker_compose/create_docker_compose.py` & `create_docker_compose-0.2/create_docker_compose/create_docker_compose.py`

 * *Files identical despite different names*

### Comparing `create_docker_compose-0.1/create_env_file/create_env_file.py` & `create_docker_compose-0.2/create_env_file/create_env_file.py`

 * *Files identical despite different names*

