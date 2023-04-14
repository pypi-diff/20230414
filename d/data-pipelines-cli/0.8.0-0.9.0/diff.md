# Comparing `tmp/data_pipelines_cli-0.8.0.tar.gz` & `tmp/data_pipelines_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/data_pipelines_cli-0.8.0.tar", last modified: Fri Dec 31 09:01:19 2021, max compression
+gzip compressed data, was "dist/data_pipelines_cli-0.9.0.tar", last modified: Mon Jan  3 09:06:15 2022, max compression
```

## Comparing `data_pipelines_cli-0.8.0.tar` & `data_pipelines_cli-0.9.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5854 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4490 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      627 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     5245 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/create.py
--rw-r--r--   0 runner    (1001) docker     (121)     5075 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/init.py
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/prepare_env.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/template.py
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5935 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/config_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2658 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2537 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/dbt_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/filesystem_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli/vcs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5854 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      447 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      584 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     8416 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (121)     3360 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     9908 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4351 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/test_init.py
--rw-r--r--   0 runner    (1001) docker     (121)     4906 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/test_prepare_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     3303 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/test_run_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-12-31 09:01:19.000000 data_pipelines_cli-0.8.0/tests/cli_commands/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5854 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4490 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5241 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/prepare_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/template.py
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1177 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5935 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/config_generation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3245 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2537 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/dbt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/filesystem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli/vcs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5854 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6400 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3360 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10813 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4906 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/test_prepare_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/test_run_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-01-03 09:06:15.000000 data_pipelines_cli-0.9.0/tests/cli_commands/test_template.py
```

### Comparing `data_pipelines_cli-0.8.0/LICENSE` & `data_pipelines_cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/PKG-INFO` & `data_pipelines_cli-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_pipelines_cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI for data platform
 Home-page: https://github.com/getindata/data-pipelines-cli/
 Author: Andrzej Swatowski
 Author-email: andrzej.swatowski@getindata.com
 License: Apache Software License (Apache 2.0)
 Description: # data-pipelines-cli
```

### Comparing `data_pipelines_cli-0.8.0/README.md` & `data_pipelines_cli-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/clean.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/clean.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/create.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/create.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/deploy.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/deploy.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,20 +30,21 @@
     """URI of the cloud storage to send build artifacts to"""
     provider_kwargs_dict: Dict[str, Any]
     """Dictionary of arguments required by a specific cloud storage provider,
     e.g. path to a token, username, password, etc."""
 
     def __init__(
         self,
-        docker_push: Optional[str],
+        env: str,
+        docker_push: bool,
         dags_path: Optional[str],
         provider_kwargs_dict: Optional[Dict[str, Any]],
         datahub_ingest: bool,
     ) -> None:
-        self.docker_args = DockerArgs(docker_push) if docker_push else None
+        self.docker_args = DockerArgs(env) if docker_push else None
         self.datahub_ingest = datahub_ingest
         self.provider_kwargs_dict = provider_kwargs_dict or {}
 
         try:
             self.blob_address_path = (
                 dags_path
                 or read_dictionary_from_config_directory(
@@ -120,43 +121,52 @@
         ).sync(delete=True)
 
 
 @click.command(
     name="deploy",
     help="Push and deploy the project to the remote machine",
 )
+@click.option("--env", default="base", type=str, help="Name of the environment")
 @click.option("--dags-path", required=False, help="Remote storage URI")
 @click.option(
     "--blob-args",
     required=False,
     type=click.File("r"),
     help="Path to JSON or YAML file with arguments that should be passed to "
     "your Bucket/blob provider",
 )
-@click.option("--docker-push", default=None, help="Path to the Docker repository")
+@click.option(
+    "--docker-push",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Whether to push image to the Docker repository",
+)
 @click.option(
     "--datahub-ingest",
     is_flag=True,
     default=False,
     help="Whether to ingest DataHub metadata",
 )
 def deploy_command(
+    env: str,
     dags_path: Optional[str],
     blob_args: Optional[io.TextIOWrapper],
-    docker_push: Optional[str],
+    docker_push: bool,
     datahub_ingest: bool,
 ) -> None:
     if blob_args:
         try:
             provider_kwargs_dict = json.load(blob_args)
         except json.JSONDecodeError:
             blob_args.seek(0)
             provider_kwargs_dict = yaml.safe_load(blob_args)
     else:
         provider_kwargs_dict = None
 
     DeployCommand(
+        env,
         docker_push,
         dags_path,
         provider_kwargs_dict,
         datahub_ingest,
     ).deploy()
```

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/init.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/init.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/prepare_env.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/prepare_env.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/run.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/run.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_commands/test.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_commands/test.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_constants.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 import pathlib
 
 from data_pipelines_cli.data_structures import DataPipelinesConfig
 
-#: DataHub URL environment variable to search for
-DATAHUB_URL_ENV: str = "DATAHUB_URL"
 #:
 IMAGE_TAG_TO_REPLACE: str = "<IMAGE_TAG>"
-#:
-DOCKER_REPOSITORY_URL_TO_REPLACE: str = "<DOCKER_REPOSITORY_URL>"
-#:
-INGEST_ENDPOINT_TO_REPLACE: str = "<INGEST_ENDPOINT>"
 #: Name of the environment and dbt target to use for a local machine
 PROFILE_NAME_LOCAL_ENVIRONMENT = "local"
 #: Name of the dbt target to use for a remote machine
 PROFILE_NAME_ENV_EXECUTION = "env_execution"
 AVAILABLE_ENVS = [PROFILE_NAME_LOCAL_ENVIRONMENT, PROFILE_NAME_ENV_EXECUTION]
 
 #: Content of the config file created by `dp init` command if no template path
```

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/cli_utils.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/config_generation.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/config_generation.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/data_structures.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/data_structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import sys
-from typing import Dict, Optional
+from typing import Dict
 
 import yaml
 
-from data_pipelines_cli.cli_utils import (
-    echo_warning,
-    get_argument_or_environment_variable,
-)
+from data_pipelines_cli.cli_utils import echo_warning
 from data_pipelines_cli.errors import DataPipelinesError, NoConfigFileError
 from data_pipelines_cli.io_utils import git_revision_hash
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict  # pylint: disable=no-name-in-module
 else:
     from typing_extensions import TypedDict
@@ -64,22 +61,38 @@
     """
 
     repository: str
     """URI of the Docker images repository"""
     commit_sha: str
     """Long hash of the current Git revision. Used as an image tag"""
 
-    def __init__(self, docker_repository_uri: Optional[str]) -> None:
-        self.repository = get_argument_or_environment_variable(
-            docker_repository_uri, "repository", "REPOSITORY_URL"
-        )
+    def __init__(self, env: str) -> None:
+        self.repository = self._get_docker_repository_uri_from_k8s_config(env)
         commit_sha = git_revision_hash()
         if not commit_sha:
             raise DataPipelinesError("Could not get git revision hash.")
         self.commit_sha = commit_sha
 
     def docker_build_tag(self) -> str:
         """
         :return: Tag for Docker Python API build command.
         :rtype: str
         """
         return f"{self.repository}:{self.commit_sha}"
+
+    @staticmethod
+    def _get_docker_repository_uri_from_k8s_config(env: str) -> str:
+        # Avoiding a dependency loop between `cli_constants` and `data_structures`
+        from data_pipelines_cli.cli_constants import BUILD_DIR
+        from data_pipelines_cli.config_generation import (
+            read_dictionary_from_config_directory,
+        )
+
+        k8s_config = read_dictionary_from_config_directory(
+            BUILD_DIR.joinpath("dag"), env, "k8s.yml"
+        )
+        try:
+            return k8s_config["image"]["repository"]
+        except KeyError as key_error:
+            raise DataPipelinesError(
+                f"Could not find 'repository' variable in build/config/{env}/k8s.yml."
+            ) from key_error
```

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/dbt_utils.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/errors.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/errors.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/filesystem_utils.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/filesystem_utils.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/io_utils.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/io_utils.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli/vcs_utils.py` & `data_pipelines_cli-0.9.0/data_pipelines_cli/vcs_utils.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/PKG-INFO` & `data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-pipelines-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI for data platform
 Home-page: https://github.com/getindata/data-pipelines-cli/
 Author: Andrzej Swatowski
 Author-email: andrzej.swatowski@getindata.com
 License: Apache Software License (Apache 2.0)
 Description: # data-pipelines-cli
```

### Comparing `data_pipelines_cli-0.8.0/data_pipelines_cli.egg-info/SOURCES.txt` & `data_pipelines_cli-0.9.0/data_pipelines_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/setup.cfg` & `data_pipelines_cli-0.9.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.0
+current_version = 0.9.0
 
 [bumpversion:file:setup.py]
 
 [bumpversion:file:data_pipelines_cli/__init__.py]
 
 [flake8]
 exclude = .git,__pycache__,build,dist,docs/source/conf.py
```

### Comparing `data_pipelines_cli-0.8.0/setup.py` & `data_pipelines_cli-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         "myst-parser>=0.16, <0.17",
     ],
     **EXTRA_FILESYSTEMS_REQUIRE,
 }
 
 setup(
     name="data_pipelines_cli",
-    version="0.8.0",
+    version="0.9.0",
     description="CLI for data platform",
     long_description=README,
     long_description_content_type="text/markdown",
     license="Apache Software License (Apache 2.0)",
     license_files=("LICENSE",),
     python_requires=">=3",
     classifiers=[
```

### Comparing `data_pipelines_cli-0.8.0/tests/cli_commands/test_clean.py` & `data_pipelines_cli-0.9.0/tests/cli_commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/tests/cli_commands/test_compile.py` & `data_pipelines_cli-0.9.0/tests/cli_commands/test_compile.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,21 +37,27 @@
     def setUp(self) -> None:
         self.all_subprocess_run_args = []
 
     def _mock_run(self, args: List[str]):
         self.all_subprocess_run_args += args
 
     @patch("pathlib.Path.cwd", lambda: goldens_dir_path)
-    def test_no_args(self):
+    @patch("data_pipelines_cli.data_structures.git_revision_hash")
+    def test_no_args(self, mock_git_revision_hash):
+        commit_sha = "aaa9876aaa"
+        mock_git_revision_hash.return_value = commit_sha
+
         runner = CliRunner()
         with tempfile.TemporaryDirectory() as tmp_dir, patch(
             "data_pipelines_cli.cli_commands.compile.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
             "data_pipelines_cli.config_generation.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
+            "data_pipelines_cli.cli_constants.BUILD_DIR", pathlib.Path(tmp_dir)
+        ), patch(
             "data_pipelines_cli.dbt_utils.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
             "data_pipelines_cli.dbt_utils.subprocess_run", self._mock_run
         ):
             result = runner.invoke(_cli, ["compile"])
             self.assertEqual(0, result.exit_code, msg=result.exception)
 
@@ -79,46 +85,18 @@
                 goldens_dir_path.joinpath("config", "base", "datahub.yml")
             ) as golden_datahub:
                 self.assertDictEqual(
                     yaml.safe_load(golden_datahub), yaml.safe_load(tmp_datahub)
                 )
             with open(
                 tmp_dir_path.joinpath("dag", "config", "base", "k8s.yml"), "r"
-            ) as tmp_k8s, open(
-                goldens_dir_path.joinpath("config", "base", "k8s.yml")
-            ) as golden_k8s:
-                self.assertDictEqual(
-                    yaml.safe_load(golden_k8s), yaml.safe_load(tmp_k8s)
-                )
-
-    @patch("pathlib.Path.cwd", lambda: goldens_dir_path)
-    @patch("data_pipelines_cli.data_structures.git_revision_hash")
-    def test_docker_uri_no_build(self, mock_git_revision_hash):
-        commit_sha = "aaa9876aaa"
-        mock_git_revision_hash.return_value = commit_sha
-
-        runner = CliRunner()
-        with tempfile.TemporaryDirectory() as tmp_dir, patch(
-            "data_pipelines_cli.cli_commands.compile.BUILD_DIR", pathlib.Path(tmp_dir)
-        ), patch(
-            "data_pipelines_cli.config_generation.BUILD_DIR", pathlib.Path(tmp_dir)
-        ), patch(
-            "data_pipelines_cli.dbt_utils.BUILD_DIR", pathlib.Path(tmp_dir)
-        ), patch(
-            "data_pipelines_cli.dbt_utils.subprocess_run", self._mock_run
-        ):
-            result = runner.invoke(_cli, ["compile", "--docker-repository-uri", "rep"])
-            self.assertEqual(0, result.exit_code, msg=result.exception)
-
-            tmp_dir_path = pathlib.Path(tmp_dir)
-            with open(
-                tmp_dir_path.joinpath("dag", "config", "base", "k8s.yml"), "r"
             ) as tmp_k8s:
                 self.assertDictEqual(
-                    self._k8s_content("rep", "aaa9876aaa"), yaml.safe_load(tmp_k8s)
+                    self._k8s_content("my_docker_repository_uri", "aaa9876aaa"),
+                    yaml.safe_load(tmp_k8s),
                 )
 
     @patch("pathlib.Path.cwd", lambda: goldens_dir_path)
     @patch("data_pipelines_cli.data_structures.git_revision_hash")
     def test_docker_not_installed(self, mock_git_revision_hash):
         commit_sha = "aaa9876aaa"
         mock_git_revision_hash.return_value = commit_sha
@@ -127,21 +105,23 @@
         with patch.dict(
             "sys.modules", docker=None
         ), tempfile.TemporaryDirectory() as tmp_dir, patch(
             "data_pipelines_cli.cli_commands.compile.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
             "data_pipelines_cli.config_generation.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
+            "data_pipelines_cli.cli_constants.BUILD_DIR", pathlib.Path(tmp_dir)
+        ), patch(
             "data_pipelines_cli.dbt_utils.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
             "data_pipelines_cli.dbt_utils.subprocess_run", self._mock_run
         ):
             result = runner.invoke(
                 _cli,
-                ["compile", "--docker-repository-uri", "rep", "--docker-build"],
+                ["compile", "--docker-build"],
             )
         self.assertEqual(1, result.exit_code)
         self.assertIsInstance(result.exception, DockerNotInstalledError)
 
     @patch("pathlib.Path.cwd", lambda: goldens_dir_path)
     @patch("data_pipelines_cli.data_structures.git_revision_hash")
     def test_docker_uri_build(self, mock_git_revision_hash):
@@ -164,44 +144,18 @@
 
         runner = CliRunner()
         with patch.dict(
             "sys.modules", docker=docker_mock
         ), tempfile.TemporaryDirectory() as tmp_dir, patch(
             "data_pipelines_cli.cli_commands.compile.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
-            "data_pipelines_cli.config_generation.BUILD_DIR", pathlib.Path(tmp_dir)
-        ), patch(
-            "data_pipelines_cli.dbt_utils.BUILD_DIR", pathlib.Path(tmp_dir)
-        ), patch(
-            "data_pipelines_cli.dbt_utils.subprocess_run", self._mock_run
-        ):
-            result = runner.invoke(
-                _cli, ["compile", "--docker-repository-uri", "rep", "--docker-build"]
-            )
-            self.assertEqual(0, result.exit_code, msg=result.exception)
-            self.assertEqual("rep:aaa9876aaa", docker_tag)
-
-    @patch("pathlib.Path.cwd", lambda: goldens_dir_path)
-    def test_datahub_uri(self):
-        runner = CliRunner()
-        with tempfile.TemporaryDirectory() as tmp_dir, patch(
-            "data_pipelines_cli.cli_commands.compile.BUILD_DIR", pathlib.Path(tmp_dir)
+            "data_pipelines_cli.cli_constants.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
             "data_pipelines_cli.config_generation.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
             "data_pipelines_cli.dbt_utils.BUILD_DIR", pathlib.Path(tmp_dir)
         ), patch(
             "data_pipelines_cli.dbt_utils.subprocess_run", self._mock_run
         ):
-            result = runner.invoke(
-                _cli, ["compile", "--datahub-gms-uri", "DaTaHuBuRi.example.io"]
-            )
+            result = runner.invoke(_cli, ["compile", "--docker-build"])
             self.assertEqual(0, result.exit_code, msg=result.exception)
-
-            tmp_dir_path = pathlib.Path(tmp_dir)
-            with open(
-                tmp_dir_path.joinpath("dag", "config", "base", "datahub.yml"), "r"
-            ) as tmp_datahub:
-                self.assertDictEqual(
-                    self._datahub_content("DaTaHuBuRi.example.io"),
-                    yaml.safe_load(tmp_datahub),
-                )
+            self.assertEqual("my_docker_repository_uri:aaa9876aaa", docker_tag)
```

### Comparing `data_pipelines_cli-0.8.0/tests/cli_commands/test_create.py` & `data_pipelines_cli-0.9.0/tests/cli_commands/test_create.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/tests/cli_commands/test_deploy.py` & `data_pipelines_cli-0.9.0/tests/cli_commands/test_deploy.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,23 +46,31 @@
         with open(blob_json_fd, "w") as f:
             yaml.dump(self.provider_args, f)
 
         self.dbt_project_config_dir = pathlib.Path(tempfile.mkdtemp())
         with open(self.dbt_project_config_dir.joinpath("dbt_project.yml"), "w") as f:
             yaml.dump(self.dbt_project_config, f)
 
+        self.build_temp_dir = pathlib.Path(tempfile.mkdtemp())
+        dags_path = pathlib.Path(self.build_temp_dir).joinpath("dag")
+        dags_path.mkdir(parents=True)
+        shutil.copytree(
+            self.goldens_dir_path.joinpath("config"), dags_path.joinpath("config")
+        )
+
         self.storage_uri = tempfile.mkdtemp()  # this way fsspec uses LocalFS
 
         self.subprocess_run_args = []
 
     def _mock_run(self, args: List[str]):
         self.subprocess_run_args = args
 
     def tearDown(self) -> None:
         shutil.rmtree(self.storage_uri)
+        shutil.rmtree(self.build_temp_dir)
         shutil.rmtree(self.dbt_project_config_dir)
         os.remove(self.blob_json_filename)
 
     def test_blob_args_types(self):
         for dump, format_name in [(json.dump, "json"), (yaml.dump, "yaml")]:
             with self.subTest(format=format_name):
                 runner = CliRunner()
@@ -70,14 +78,15 @@
                 with tempfile.NamedTemporaryFile(mode="w", delete=False) as tmp_file:
                     dump(self.provider_args, tmp_file)
 
                 result_provider_kwargs = {}
 
                 def mock_init(
                     _self,
+                    _env,
                     _docker_push,
                     _blob_address,
                     provider_kwargs_dict,
                     _datahub_ingest,
                 ):
                     nonlocal result_provider_kwargs
                     result_provider_kwargs = provider_kwargs_dict
@@ -117,20 +126,22 @@
             2,
             len(os.listdir(self.storage_uri)),
         )
 
     def test_no_module_cli(self):
         for module_name, cli_args in [
             ("datahub", ["--datahub-ingest"]),
-            ("docker", ["--docker-push", "rep"]),
+            ("docker", ["--docker-push"]),
         ]:
             with self.subTest(dep=module_name):
                 runner = CliRunner()
                 with patch.dict("sys.modules", **{module_name: None}), patch(
                     "pathlib.Path.cwd", lambda _: self.dbt_project_config_dir
+                ), patch(
+                    "data_pipelines_cli.cli_constants.BUILD_DIR", self.build_temp_dir
                 ):
                     result = runner.invoke(
                         _cli,
                         [
                             "deploy",
                             "--dags-path",
                             self.storage_uri,
@@ -143,63 +154,67 @@
                 self.assertIsInstance(result.exception, DependencyNotInstalledError)
 
     def test_no_datahub_method(self):
         with patch.dict("sys.modules", datahub=None), patch(
             "pathlib.Path.cwd", lambda _: self.dbt_project_config_dir
         ):
             with self.assertRaises(DependencyNotInstalledError):
-                DeployCommand(None, self.storage_uri, self.provider_args, True).deploy()
+                DeployCommand(
+                    "base", False, self.storage_uri, self.provider_args, True
+                ).deploy()
 
     @patch("data_pipelines_cli.cli_commands.deploy.BUILD_DIR", goldens_dir_path)
     def test_datahub_run(self):
         with patch("pathlib.Path.cwd", lambda _: self.dbt_project_config_dir), patch(
             "data_pipelines_cli.cli_commands.deploy.subprocess_run", self._mock_run
         ), patch.dict("sys.modules", datahub=MagicMock()):
-            DeployCommand(None, self.storage_uri, self.provider_args, True).deploy()
+            DeployCommand(
+                "base", False, self.storage_uri, self.provider_args, True
+            ).deploy()
             self.assertListEqual(
                 [
                     "datahub",
                     "ingest",
                     "-c",
                     f"{self.goldens_dir_path}/dag/config/base/datahub.yml",
                 ],
                 self.subprocess_run_args,
             )
 
     def test_no_docker_method(self):
         with patch.dict("sys.modules", docker=None), patch(
             "pathlib.Path.cwd", lambda _: self.dbt_project_config_dir
-        ):
+        ), patch("data_pipelines_cli.cli_constants.BUILD_DIR", self.build_temp_dir):
             with self.assertRaises(DependencyNotInstalledError):
                 DeployCommand(
-                    "rep", self.storage_uri, self.provider_args, False
+                    "base", True, self.storage_uri, self.provider_args, False
                 ).deploy()
 
     @patch(
         "data_pipelines_cli.cli_commands.deploy.BUILD_DIR",
         pathlib.Path("/tmp/some/non/ex/i/sting/path"),
     )
     def test_no_airflow_address(self):
         with self.assertRaises(AirflowDagsPathKeyError):
-            DeployCommand(None, None, None, False)
+            DeployCommand("base", False, None, None, False)
 
     def test_airflow_address(self):
         with tempfile.TemporaryDirectory() as tmp_dir, patch(
             "data_pipelines_cli.cli_commands.deploy.BUILD_DIR", pathlib.Path(tmp_dir)
         ):
             tmp_airflow_path = pathlib.Path(tmp_dir).joinpath(
                 "dag", "config", "base", "airflow.yml"
             )
             tmp_airflow_path.parent.mkdir(parents=True, exist_ok=True)
             shutil.copyfile(
                 self.goldens_dir_path.joinpath("config", "base", "airflow.yml"),
                 tmp_airflow_path,
             )
 
-            deploy_command = DeployCommand(None, None, None, False)
+            deploy_command = DeployCommand("base", False, None, None, False)
         self.assertEqual(
             "gcs://test-sync-project/sync-dir/dags/my-project-name",
             deploy_command.blob_address_path,
         )
 
     @patch("data_pipelines_cli.cli_commands.deploy.BUILD_DIR", goldens_dir_path)
     def test_docker_run(self):
@@ -217,18 +232,22 @@
         docker_mock = MagicMock()
         docker_mock.configure_mock(**{"from_env": lambda: docker_client_mock})
 
         with patch.dict("sys.modules", docker=docker_mock), patch(
             "pathlib.Path.cwd", lambda _: self.dbt_project_config_dir
         ), patch("docker.from_env", lambda: docker_client_mock), patch(
             "data_pipelines_cli.data_structures.git_revision_hash", lambda: "sha1234"
+        ), patch(
+            "data_pipelines_cli.cli_constants.BUILD_DIR", self.build_temp_dir
         ):
-            DeployCommand("rep", self.storage_uri, self.provider_args, False).deploy()
+            DeployCommand(
+                "base", True, self.storage_uri, self.provider_args, False
+            ).deploy()
 
-        self.assertEqual("rep", docker_kwargs.get("repository"))
+        self.assertEqual("my_docker_repository_uri", docker_kwargs.get("repository"))
         self.assertEqual("sha1234", docker_kwargs.get("tag"))
 
     @patch("data_pipelines_cli.cli_commands.deploy.BUILD_DIR", goldens_dir_path)
     def test_docker_error(self):
         def _mock_docker(**_kwargs):
             return [
                 '{"status":"The push refers to repository [docker.io/library/rep]"}',
@@ -244,13 +263,14 @@
         docker_mock = MagicMock()
         docker_mock.configure_mock(**{"from_env": lambda: docker_client_mock})
 
         with patch(
             "pathlib.Path.cwd", lambda _: self.dbt_project_config_dir
         ), patch.dict("sys.modules", docker=docker_mock), patch(
             "data_pipelines_cli.data_structures.git_revision_hash", lambda: "sha1234"
+        ), patch(
+            "data_pipelines_cli.cli_constants.BUILD_DIR", self.build_temp_dir
         ):
-
             with self.assertRaises(DataPipelinesError):
                 DeployCommand(
-                    "rep", self.storage_uri, self.provider_args, False
+                    "base", True, self.storage_uri, self.provider_args, False
                 ).deploy()
```

### Comparing `data_pipelines_cli-0.8.0/tests/cli_commands/test_init.py` & `data_pipelines_cli-0.9.0/tests/cli_commands/test_init.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/tests/cli_commands/test_prepare_env.py` & `data_pipelines_cli-0.9.0/tests/cli_commands/test_prepare_env.py`

 * *Files identical despite different names*

### Comparing `data_pipelines_cli-0.8.0/tests/cli_commands/test_run_test.py` & `data_pipelines_cli-0.9.0/tests/cli_commands/test_run_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,16 @@
                 "data_pipelines_cli.config_generation.BUILD_DIR", pathlib.Path(tmp_dir)
             ), patch(
                 "data_pipelines_cli.cli_commands.compile.BUILD_DIR",
                 pathlib.Path(tmp_dir),
             ), patch(
                 "data_pipelines_cli.dbt_utils.BUILD_DIR", pathlib.Path(tmp_dir)
             ), patch(
+                "data_pipelines_cli.cli_constants.BUILD_DIR", pathlib.Path(tmp_dir)
+            ), patch(
                 "data_pipelines_cli.dbt_utils.subprocess_run", self._mock_run
             ):
                 runner = CliRunner()
                 result = runner.invoke(_cli, [cmd])
                 self.assertEqual(0, result.exit_code, msg=result.exception)
 
                 self.assertEqual("dbt", self.subprocess_run_args[0])
@@ -61,14 +63,16 @@
                     pathlib.Path(tmp_dir),
                 ), patch(
                     "data_pipelines_cli.cli_commands.compile.BUILD_DIR",
                     pathlib.Path(tmp_dir),
                 ), patch(
                     "data_pipelines_cli.dbt_utils.BUILD_DIR", pathlib.Path(tmp_dir)
                 ), patch(
+                    "data_pipelines_cli.cli_constants.BUILD_DIR", pathlib.Path(tmp_dir)
+                ), patch(
                     "data_pipelines_cli.dbt_utils.subprocess_run", self._mock_run
                 ):
                     runner = CliRunner()
                     result = runner.invoke(_cli, [cmd, "--env", env])
                     self.assertEqual(0, result.exit_code, msg=result.exception)
 
                     self.assertEqual("dbt", self.subprocess_run_args[0])
```

### Comparing `data_pipelines_cli-0.8.0/tests/cli_commands/test_template.py` & `data_pipelines_cli-0.9.0/tests/cli_commands/test_template.py`

 * *Files identical despite different names*

