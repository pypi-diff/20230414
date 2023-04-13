# Comparing `tmp/mosaicml_cli-0.3.6-py3-none-any.whl.zip` & `tmp/mosaicml_cli-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,46 +1,46 @@
-Zip file size: 288577 bytes, number of entries: 208
+Zip file size: 291298 bytes, number of entries: 208
 -rw-r--r--  2.0 unx       54 b- defN 22-Jun-27 19:47 mcli/__init__.py
 -rw-r--r--  2.0 unx    16462 b- defN 23-Apr-11 21:00 mcli/config.py
--rw-r--r--  2.0 unx     3884 b- defN 23-Apr-11 22:32 mcli/version.py
+-rw-r--r--  2.0 unx     3884 b- defN 23-Apr-13 22:08 mcli/version.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/api/__init__.py
 -rw-r--r--  2.0 unx    11677 b- defN 23-Apr-11 21:00 mcli/api/exceptions.py
 -rw-r--r--  2.0 unx      508 b- defN 23-Feb-02 19:35 mcli/api/types.py
 -rw-r--r--  2.0 unx     2354 b- defN 22-Jun-27 19:47 mcli/api/typing_future.py
 -rw-r--r--  2.0 unx      134 b- defN 22-Oct-27 18:49 mcli/api/cluster/__init__.py
--rw-r--r--  2.0 unx     4058 b- defN 23-Apr-11 21:00 mcli/api/cluster/api_get_clusters.py
+-rw-r--r--  2.0 unx     4141 b- defN 23-Apr-13 22:08 mcli/api/cluster/api_get_clusters.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/api/engine/__init__.py
 -rw-r--r--  2.0 unx    22935 b- defN 23-Apr-11 22:31 mcli/api/engine/engine.py
 -rw-r--r--  2.0 unx      787 b- defN 22-Sep-15 00:48 mcli/api/engine/utils.py
 -rw-r--r--  2.0 unx      879 b- defN 23-Apr-11 22:06 mcli/api/inference_deployments/__init__.py
--rw-r--r--  2.0 unx     3388 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--  2.0 unx     3278 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--  2.0 unx     6091 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--  2.0 unx     1156 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--  2.0 unx     1276 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--  2.0 unx     3402 b- defN 23-Apr-13 22:08 mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--  2.0 unx     3292 b- defN 23-Apr-13 22:08 mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--  2.0 unx     6105 b- defN 23-Apr-13 22:08 mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-Apr-13 22:08 mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--  2.0 unx     1126 b- defN 23-Apr-13 22:08 mcli/api/inference_deployments/api_predict_inference_deployment.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Aug-17 23:59 mcli/api/kube/__init__.py
 -rw-r--r--  2.0 unx      856 b- defN 22-Aug-17 23:59 mcli/api/kube/runs/__init__.py
 -rw-r--r--  2.0 unx     4900 b- defN 23-Apr-11 21:00 mcli/api/kube/runs/api_create_run.py
 -rw-r--r--  2.0 unx     5042 b- defN 23-Mar-06 23:35 mcli/api/kube/runs/api_delete_runs.py
 -rw-r--r--  2.0 unx    14458 b- defN 23-Mar-06 23:35 mcli/api/kube/runs/api_get_run_logs.py
--rw-r--r--  2.0 unx    16142 b- defN 23-Apr-11 22:31 mcli/api/kube/runs/api_get_runs.py
+-rw-r--r--  2.0 unx    16251 b- defN 23-Apr-13 22:08 mcli/api/kube/runs/api_get_runs.py
 -rw-r--r--  2.0 unx     6007 b- defN 23-Mar-06 23:35 mcli/api/kube/runs/api_stop_runs.py
 -rw-r--r--  2.0 unx     6210 b- defN 22-Oct-27 18:49 mcli/api/kube/runs/api_watch_run.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-06 23:35 mcli/api/mint/__init__.py
 -rw-r--r--  2.0 unx     4987 b- defN 23-Mar-06 23:35 mcli/api/mint/shell.py
 -rw-r--r--  2.0 unx     1530 b- defN 23-Mar-06 23:35 mcli/api/mint/tty.py
 -rw-r--r--  2.0 unx      209 b- defN 23-Apr-11 21:00 mcli/api/model/__init__.py
--rw-r--r--  2.0 unx     5655 b- defN 23-Apr-11 21:00 mcli/api/model/cluster_details.py
--rw-r--r--  2.0 unx     3015 b- defN 23-Apr-11 21:00 mcli/api/model/inference_deployment.py
--rw-r--r--  2.0 unx     7946 b- defN 23-Apr-11 22:06 mcli/api/model/run.py
+-rw-r--r--  2.0 unx     6186 b- defN 23-Apr-13 22:08 mcli/api/model/cluster_details.py
+-rw-r--r--  2.0 unx     2909 b- defN 23-Apr-13 22:08 mcli/api/model/inference_deployment.py
+-rw-r--r--  2.0 unx     8057 b- defN 23-Apr-13 22:08 mcli/api/model/run.py
 -rw-r--r--  2.0 unx     1102 b- defN 23-Apr-11 22:06 mcli/api/runs/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 23-Apr-11 22:06 mcli/api/runs/api_create_run.py
+-rw-r--r--  2.0 unx     2750 b- defN 23-Apr-13 22:08 mcli/api/runs/api_create_run.py
 -rw-r--r--  2.0 unx     3926 b- defN 23-Apr-11 22:06 mcli/api/runs/api_delete_runs.py
 -rw-r--r--  2.0 unx     9281 b- defN 23-Apr-11 21:00 mcli/api/runs/api_get_run_logs.py
--rw-r--r--  2.0 unx     8968 b- defN 23-Apr-11 22:31 mcli/api/runs/api_get_runs.py
+-rw-r--r--  2.0 unx     9008 b- defN 23-Apr-13 22:08 mcli/api/runs/api_get_runs.py
 -rw-r--r--  2.0 unx     5099 b- defN 23-Apr-11 22:06 mcli/api/runs/api_stop_runs.py
 -rw-r--r--  2.0 unx     3937 b- defN 23-Apr-11 22:06 mcli/api/runs/api_update_run_metadata.py
 -rw-r--r--  2.0 unx    10619 b- defN 23-Apr-11 21:00 mcli/api/runs/api_watch_run.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/api/schema/__init__.py
 -rw-r--r--  2.0 unx      636 b- defN 22-Aug-23 17:34 mcli/api/schema/generic_model.py
 -rw-r--r--  2.0 unx      309 b- defN 22-Sep-22 23:36 mcli/api/secrets/__init__.py
 -rw-r--r--  2.0 unx     2365 b- defN 23-Mar-06 23:35 mcli/api/secrets/api_create_secret.py
@@ -65,32 +65,32 @@
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_delete/__init__.py
 -rw-r--r--  2.0 unx    14072 b- defN 23-Apr-11 21:00 mcli/cli/m_delete/delete.py
 -rw-r--r--  2.0 unx     8417 b- defN 23-Apr-11 21:00 mcli/cli/m_delete/m_delete.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:00 mcli/cli/m_deploy/__init__.py
 -rw-r--r--  2.0 unx     3896 b- defN 23-Apr-11 21:00 mcli/cli/m_deploy/m_deploy.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-02 19:35 mcli/cli/m_describe/__init__.py
 -rw-r--r--  2.0 unx     4409 b- defN 23-Apr-11 21:00 mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--  2.0 unx     7818 b- defN 23-Apr-11 22:06 mcli/cli/m_describe/describe_runs.py
+-rw-r--r--  2.0 unx     9778 b- defN 23-Apr-13 22:08 mcli/cli/m_describe/describe_runs.py
 -rw-r--r--  2.0 unx     1860 b- defN 23-Apr-11 21:00 mcli/cli/m_describe/m_describe.py
 -rw-r--r--  2.0 unx      549 b- defN 23-Apr-11 21:00 mcli/cli/m_get/__init__.py
--rw-r--r--  2.0 unx     3909 b- defN 23-Apr-11 21:00 mcli/cli/m_get/clusters.py
+-rw-r--r--  2.0 unx     8477 b- defN 23-Apr-13 22:08 mcli/cli/m_get/clusters.py
 -rw-r--r--  2.0 unx     6452 b- defN 23-Apr-11 21:00 mcli/cli/m_get/display.py
 -rw-r--r--  2.0 unx     1315 b- defN 22-Sep-15 00:48 mcli/cli/m_get/envvars.py
 -rw-r--r--  2.0 unx     5361 b- defN 23-Apr-11 21:00 mcli/cli/m_get/inference_deployments.py
 -rw-r--r--  2.0 unx     4866 b- defN 23-Apr-11 21:00 mcli/cli/m_get/m_get.py
--rw-r--r--  2.0 unx     6346 b- defN 23-Apr-11 22:31 mcli/cli/m_get/runs.py
+-rw-r--r--  2.0 unx     8759 b- defN 23-Apr-13 22:08 mcli/cli/m_get/runs.py
 -rw-r--r--  2.0 unx     3567 b- defN 23-Apr-11 21:00 mcli/cli/m_get/secrets.py
 -rw-r--r--  2.0 unx     1580 b- defN 23-Feb-02 20:09 mcli/cli/m_get/users.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_init/__init__.py
 -rw-r--r--  2.0 unx     4113 b- defN 23-Apr-11 21:00 mcli/cli/m_init/m_init.py
 -rw-r--r--  2.0 unx     9374 b- defN 23-Apr-11 21:00 mcli/cli/m_init/m_init_kube.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_interactive/__init__.py
 -rw-r--r--  2.0 unx     9005 b- defN 23-Mar-06 23:35 mcli/cli/m_interactive/interactive.py
 -rw-r--r--  2.0 unx    16203 b- defN 23-Apr-11 21:00 mcli/cli/m_interactive/m_interactive.py
--rw-r--r--  2.0 unx     4571 b- defN 23-Apr-11 21:00 mcli/cli/m_interactive/temp_mcloud_interactive.py
+-rw-r--r--  2.0 unx     4601 b- defN 23-Apr-13 22:08 mcli/cli/m_interactive/temp_mcloud_interactive.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_log/__init__.py
 -rw-r--r--  2.0 unx     8633 b- defN 23-Apr-11 21:00 mcli/cli/m_log/m_log.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:00 mcli/cli/m_ping/__init__.py
 -rw-r--r--  2.0 unx     1742 b- defN 23-Apr-11 21:00 mcli/cli/m_ping/m_ping.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 21:00 mcli/cli/m_predict/__init__.py
 -rw-r--r--  2.0 unx     2160 b- defN 23-Apr-11 21:00 mcli/cli/m_predict/m_predict.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_root/__init__.py
@@ -107,20 +107,20 @@
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_use/__init__.py
 -rw-r--r--  2.0 unx     3234 b- defN 22-Dec-07 22:00 mcli/cli/m_use/m_use.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-14 21:04 mcli/cli/m_util/__init__.py
 -rw-r--r--  2.0 unx     9853 b- defN 23-Apr-11 21:00 mcli/cli/m_util/kube_util.py
 -rw-r--r--  2.0 unx     1147 b- defN 22-Oct-27 18:49 mcli/cli/m_util/m_util.py
 -rw-r--r--  2.0 unx     6515 b- defN 23-Apr-11 21:00 mcli/cli/m_util/util.py
 -rw-r--r--  2.0 unx     1199 b- defN 23-Apr-11 22:06 mcli/models/__init__.py
--rw-r--r--  2.0 unx     8572 b- defN 23-Apr-11 21:00 mcli/models/inference_deployment_config.py
+-rw-r--r--  2.0 unx     8555 b- defN 23-Apr-13 22:08 mcli/models/inference_deployment_config.py
 -rw-r--r--  2.0 unx     3693 b- defN 23-Apr-11 21:00 mcli/models/mcli_cluster.py
 -rw-r--r--  2.0 unx      563 b- defN 22-Sep-15 00:48 mcli/models/mcli_envvar.py
 -rw-r--r--  2.0 unx     3386 b- defN 22-Sep-15 00:48 mcli/models/mcli_integration.py
 -rw-r--r--  2.0 unx     9400 b- defN 23-Feb-02 20:09 mcli/models/mcli_secret.py
--rw-r--r--  2.0 unx    17576 b- defN 23-Apr-11 22:06 mcli/models/run_config.py
+-rw-r--r--  2.0 unx    17234 b- defN 23-Apr-13 22:08 mcli/models/run_config.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/objects/__init__.py
 -rw-r--r--  2.0 unx      660 b- defN 22-Sep-15 00:48 mcli/objects/integrations/__init__.py
 -rw-r--r--  2.0 unx      671 b- defN 22-Jun-27 19:47 mcli/objects/integrations/apt_packages.py
 -rw-r--r--  2.0 unx     1287 b- defN 22-Sep-15 00:48 mcli/objects/integrations/comet.py
 -rw-r--r--  2.0 unx     2597 b- defN 23-Feb-02 19:35 mcli/objects/integrations/git_repo.py
 -rw-r--r--  2.0 unx     3491 b- defN 22-Sep-27 16:43 mcli/objects/integrations/local.py
 -rw-r--r--  2.0 unx     2126 b- defN 23-Jan-31 19:01 mcli/objects/integrations/mosaicml_agent.py
@@ -179,32 +179,32 @@
 -rw-r--r--  2.0 unx     8090 b- defN 22-Jun-27 19:47 mcli/serverside/job/mcli_k8s_job_typing.py
 -rw-r--r--  2.0 unx     7524 b- defN 22-Oct-11 22:54 mcli/serverside/job/mcli_k8s_resource_requirements_typing.py
 -rw-r--r--  2.0 unx      459 b- defN 22-Jun-27 19:47 mcli/serverside/job/mcli_k8s_service_typing.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/serverside/runners/__init__.py
 -rw-r--r--  2.0 unx     5770 b- defN 23-Feb-02 19:35 mcli/serverside/runners/runner.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/utils/__init__.py
 -rw-r--r--  2.0 unx     5306 b- defN 23-Apr-11 21:00 mcli/utils/utils_cli.py
--rw-r--r--  2.0 unx     6066 b- defN 23-Apr-11 21:00 mcli/utils/utils_config.py
+-rw-r--r--  2.0 unx     6073 b- defN 23-Apr-13 22:08 mcli/utils/utils_config.py
 -rw-r--r--  2.0 unx      740 b- defN 22-Sep-27 16:43 mcli/utils/utils_date.py
 -rw-r--r--  2.0 unx    10453 b- defN 23-Apr-11 21:00 mcli/utils/utils_docker.py
 -rw-r--r--  2.0 unx    12947 b- defN 23-Apr-11 21:00 mcli/utils/utils_epilog.py
 -rw-r--r--  2.0 unx      751 b- defN 22-Jun-27 19:47 mcli/utils/utils_file.py
 -rw-r--r--  2.0 unx    11769 b- defN 22-Dec-07 22:00 mcli/utils/utils_interactive.py
 -rw-r--r--  2.0 unx    49322 b- defN 22-Nov-23 06:32 mcli/utils/utils_kube.py
 -rw-r--r--  2.0 unx     6980 b- defN 23-Feb-02 19:35 mcli/utils/utils_kube_labels.py
--rw-r--r--  2.0 unx     4741 b- defN 23-Apr-11 21:00 mcli/utils/utils_logging.py
+-rw-r--r--  2.0 unx     4832 b- defN 23-Apr-13 22:08 mcli/utils/utils_logging.py
 -rw-r--r--  2.0 unx      359 b- defN 22-Jun-27 19:47 mcli/utils/utils_modules.py
 -rw-r--r--  2.0 unx     6614 b- defN 23-Apr-11 21:00 mcli/utils/utils_pypi.py
 -rw-r--r--  2.0 unx     6513 b- defN 23-Mar-06 23:35 mcli/utils/utils_rancher.py
 -rw-r--r--  2.0 unx     3115 b- defN 22-Aug-31 05:37 mcli/utils/utils_rich.py
 -rw-r--r--  2.0 unx     8533 b- defN 23-Mar-03 22:02 mcli/utils/utils_run_status.py
 -rw-r--r--  2.0 unx     4350 b- defN 22-Jun-27 19:47 mcli/utils/utils_serializable_dataclass.py
 -rw-r--r--  2.0 unx     1103 b- defN 23-Apr-11 21:00 mcli/utils/utils_spinner.py
 -rw-r--r--  2.0 unx    11437 b- defN 23-Mar-06 23:35 mcli/utils/utils_string_functions.py
 -rw-r--r--  2.0 unx     3954 b- defN 22-Nov-04 18:29 mcli/utils/utils_types.py
 -rw-r--r--  2.0 unx     1001 b- defN 22-Jun-27 19:47 mcli/utils/utils_yaml.py
--rw-r--r--  2.0 unx     4743 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       75 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    18462 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/RECORD
-208 files, 872390 bytes uncompressed, 259219 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx     4525 b- defN 23-Apr-13 22:08 mosaicml_cli-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 22:08 mosaicml_cli-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       75 b- defN 23-Apr-13 22:08 mosaicml_cli-0.3.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-13 22:08 mosaicml_cli-0.3.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    18462 b- defN 23-Apr-13 22:08 mosaicml_cli-0.3.7.dist-info/RECORD
+208 files, 881454 bytes uncompressed, 261940 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -603,23 +603,23 @@
 
 Filename: mcli/utils/utils_types.py
 Comment: 
 
 Filename: mcli/utils/utils_yaml.py
 Comment: 
 
-Filename: mosaicml_cli-0.3.6.dist-info/METADATA
+Filename: mosaicml_cli-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: mosaicml_cli-0.3.6.dist-info/WHEEL
+Filename: mosaicml_cli-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: mosaicml_cli-0.3.6.dist-info/entry_points.txt
+Filename: mosaicml_cli-0.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: mosaicml_cli-0.3.6.dist-info/top_level.txt
+Filename: mosaicml_cli-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mosaicml_cli-0.3.6.dist-info/RECORD
+Filename: mosaicml_cli-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mcli/version.py

```diff
@@ -111,13 +111,13 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

## mcli/api/cluster/api_get_clusters.py

```diff
@@ -17,17 +17,22 @@
 VARIABLE_DATA_NAME = 'getClustersData'
 QUERY = f"""
 query GetClusters(${VARIABLE_DATA_NAME}: GetClustersInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
     name
     provider
+    allowFractional
+    allowMultinode
     allowedInstances {{
+      name
       gpuType
+      gpusPerNode
       gpuNums
+      numNodes
     }}
   }}
 }}"""
 QUERY_UTILIZATION = f"""
 query GetClusters(${VARIABLE_DATA_NAME}: GetClustersInput!) {{
   {QUERY_FUNCTION}({VARIABLE_DATA_NAME}: ${VARIABLE_DATA_NAME}) {{
     id
```

## mcli/api/inference_deployments/api_create_inference_deployment.py

```diff
@@ -19,14 +19,15 @@
     name
     inferenceDeploymentInput
     originalInferenceDeploymentInput
     status
     createdAt
     updatedAt
     deletedAt
+    publicDNS
   }}
 }}"""
 
 
 @overload
 def create_inference_deployment(deployment: Union[InferenceDeploymentConfig, FinalInferenceDeploymentConfig],
                                 timeout: Optional[float] = 10,
```

## mcli/api/inference_deployments/api_delete_inference_deployments.py

```diff
@@ -19,14 +19,15 @@
     name
     inferenceDeploymentInput
     originalInferenceDeploymentInput
     status
     createdAt
     updatedAt
     deletedAt
+    publicDNS
   }}
 }}"""
 
 __all__ = ['delete_inference_deployments']
 
 
 @overload
```

## mcli/api/inference_deployments/api_get_inference_deployments.py

```diff
@@ -24,14 +24,15 @@
     name
     inferenceDeploymentInput
     originalInferenceDeploymentInput
     status
     createdAt
     updatedAt
     deletedAt
+    publicDNS
   }}
 }}"""
 
 
 @overload
 def get_inference_deployments(
     deployments: Optional[Union[List[str], List[InferenceDeployment]]] = None,
```

## mcli/api/inference_deployments/api_ping_inference_deployment.py

```diff
@@ -21,15 +21,13 @@
     Arguments:
         deployment: Inference deployment to ping for a status check
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised.
     Raises:
         HTTPError: If pinging the endpoint fails
     """
-    # Fallback needed for backward compatibility
-    url = deployment.public_dns or deployment.get_inference_deployment_address()
-    resp: Response = requests.get(url=url + '/ping', timeout=timeout)
+    resp: Response = requests.get(url=deployment.public_dns + '/ping', timeout=timeout)
     if resp.ok:
         return resp.json()
     else:
         resp.raise_for_status()
         return {}
```

## mcli/api/inference_deployments/api_predict_inference_deployment.py

```diff
@@ -22,15 +22,13 @@
         deployment: Inference deployment to send input to
         input: Input data to run prediction on in the form of dictionary
         timeout: Time, in seconds, in which the call should complete. If the call
             takes too long, a TimeoutError will be raised.
     Raises:
         HTTPError: If sending the request to the endpoint fails
     """
-    # Fallback needed for backward compatibility until public_dns is written to the DB
-    url = deployment.public_dns or deployment.get_inference_deployment_address()
-    resp: Response = requests.post(url=url + '/infer', timeout=timeout, json=inputs)
+    resp: Response = requests.post(url=deployment.public_dns + '/infer', timeout=timeout, json=inputs)
     if resp.ok:
         return resp.json()
     else:
         resp.raise_for_status()
         return {}
```

## mcli/api/kube/runs/api_get_runs.py

```diff
@@ -304,14 +304,15 @@
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     user_emails: Optional[List[str]] = None,
+    include_details: bool = False,
 ) -> List[Run]:
     ...
 
 
 @overload
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
@@ -321,14 +322,15 @@
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     user_emails: Optional[List[str]] = None,
+    include_details: bool = False,
 ) -> Future[List[Run]]:
     ...
 
 
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
     cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
@@ -337,14 +339,15 @@
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
     future: bool = False,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     user_emails: Optional[List[str]] = None,
+    include_details: bool = False,
 ):
     """Get a filtered list of runs
 
     List runs that have been launched in the MosaicML platform. The returned list will
     contain all of the details stored about the requested runs.
 
     Arguments:
@@ -382,16 +385,16 @@
 
     Returns:
         If future is False:
             A list of requested :class:`~mcli.api.model.run.Run` objects
         Otherwise:
             A :class:`~concurrent.futures.Future` for the list
     """
-    if before or after:
-        raise NotImplementedError('Before and after run filters not supported in legacy mcli')
+    if before or after or include_details:
+        raise NotImplementedError('This filter is not suported in legacy mcli')
 
     # Coerce arg types to strings
     run_names: Optional[List[str]] = None
     if runs is not None:
         run_names = [r.name if isinstance(r, Run) else r for r in runs]
 
     cluster_names = cluster_names or clusters
```

## mcli/api/model/cluster_details.py

```diff
@@ -96,28 +96,36 @@
 
 
 @dataclass
 @functools.total_ordering
 class Instance:
     """Instance of a cluster
     """
-
+    name: str
     gpu_type: str
+    gpus: int
+    nodes: int
     gpu_nums: List[int] = field(default_factory=list)
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> Instance:
-        check_response(response, {'gpuType', 'gpuNums'})
-        return cls(gpu_type=response['gpuType'], gpu_nums=response['gpuNums'])
+        check_response(response, {'name', 'gpusPerNode', 'numNodes', 'gpuType', 'gpuNums'})
+        return cls(name=response['name'],
+                   gpu_type=response['gpuType'],
+                   gpus=response['gpusPerNode'],
+                   nodes=response['numNodes'],
+                   gpu_nums=response['gpuNums'])
 
     @classmethod
     def from_available_instances(cls, available_instances: Dict[GPUType, List[int]]) -> List[Instance]:
-        return [Instance(gpu_type.value, gpu_nums) for gpu_type, gpu_nums in available_instances.items()]
+        return [Instance('', gpu_type.value, 0, 0, gpu_nums) for gpu_type, gpu_nums in available_instances.items()]
 
     def __lt__(self, other: Instance):
+        if self.gpu_type.lower() == 'none':
+            return True
         return self.gpu_type < other.gpu_type
 
 
 def get_provider_name(raw_provider: str):
     raw_provider = raw_provider.upper()
 
     overrides = {
@@ -133,14 +141,16 @@
 @functools.total_ordering
 class ClusterDetails(SerializableDataclass, DeserializableModel):
     """Details of a cluster, including instances and utilization
     """
 
     name: str
     provider: str = 'MosaicML'
+    allow_fractional: bool = False
+    allow_multinode: bool = False
     cluster_instances: List[Instance] = field(default_factory=list)
     utilization: Optional[ClusterUtilization] = None
 
     kubernetes_context: str = ''
     namespace: str = ''
 
     id: Optional[str] = None
@@ -148,14 +158,16 @@
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> ClusterDetails:
         check_response(response, {'name'})
         utilization = None if 'utilization' not in response else ClusterUtilization.from_mapi_response(
             response['utilization'])
         return cls(name=response['name'],
                    provider=get_provider_name(response.get('provider', '')),
+                   allow_fractional=response.get('allowFractional', False),
+                   allow_multinode=response.get('allowMultinode', False),
                    cluster_instances=[Instance.from_mapi_response(i) for i in response.get('allowedInstances', [])],
                    utilization=utilization,
                    id=response.get('id'))
 
     def __lt__(self, other: ClusterDetails):
         return self.name < other.name
```

## mcli/api/model/inference_deployment.py

```diff
@@ -32,18 +32,15 @@
     config: FinalInferenceDeploymentConfig
     public_dns: str = ""
 
     deleted_at: Optional[datetime] = None
     submitted_config: Optional[InferenceDeploymentConfig] = None
 
     _required_properties: Tuple[str] = tuple(
-        ['id', 'name', 'status', 'createdAt', 'updatedAt', 'inferenceDeploymentInput'])
-
-    def get_inference_deployment_address(self) -> str:
-        return f"https://{self.name}.inf.hosted-on.mosaicml.hosting"
+        ['id', 'name', 'status', 'createdAt', 'updatedAt', 'inferenceDeploymentInput', 'publicDNS'])
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]):
         missing = set(cls._required_properties) - set(response)
         if missing:
             raise MAPIException(
                 status=HTTPStatus.BAD_REQUEST,
@@ -60,10 +57,10 @@
 
         return cls(deployment_uid=response['id'],
                    name=response['name'],
                    created_at=convert_datetime(response['createdAt']),
                    updated_at=convert_datetime(response['updatedAt']),
                    deleted_at=deleted_at,
                    status=response['status'],
+                   public_dns=response['publicDNS'],
                    config=FinalInferenceDeploymentConfig.from_mapi_response(response['inferenceDeploymentInput']),
                    submitted_config=submit_config)
-        #    public_dns=response['publicDNS'])
```

## mcli/api/model/run.py

```diff
@@ -58,14 +58,15 @@
 
     started_at: Optional[datetime] = None
     completed_at: Optional[datetime] = None
     reason: Optional[str] = None
     nodes: List[Node] = field(default_factory=list)
     submitted_config: Optional[RunConfig] = None
     metadata: Optional[Dict[str, Any]] = None
+    last_attempt_id: Optional[str] = None
 
     _required_properties: Tuple[str] = tuple([
         'id',
         'name',
         'status',
         'createdAt',
         'updatedAt',
@@ -222,9 +223,10 @@
         details = response.get('details', {})
         if details:
             submitted_run_input = details.get('originalRunInput')
             args['submitted_config'] = RunConfig.from_mapi_response(
                 submitted_run_input) if submitted_run_input is not None else None
 
             args['metadata'] = details.get('metadata')
+            args['last_attempt_id'] = details.get('lastExecutionId')
 
         return cls(**args)
```

## mcli/api/runs/api_create_run.py

```diff
@@ -26,14 +26,15 @@
     startedAt
     completedAt
     updatedAt
     reason
     details {{
         originalRunInput
         metadata
+        lastExecutionId
     }}
   }}
 }}"""
 
 
 @overload
 def create_run(run: Union[RunConfig, FinalRunConfig],
```

## mcli/api/runs/api_get_runs.py

```diff
@@ -52,14 +52,15 @@
         name
     }}
     createdByEmail
     runInput
     details {{
         originalRunInput
         metadata
+        lastExecutionId
     }}
   }}
 }}
 """
 
 
 @overload
@@ -207,15 +208,15 @@
         date_filters = {}
         if before:
             date_filters['lt'] = before.astimezone().isoformat() if isinstance(before, datetime) else before
         if after:
             date_filters['gte'] = after.astimezone().isoformat() if isinstance(after, datetime) else after
         filters['createdAt'] = date_filters
     if statuses:
-        filters['status'] = {'in': [s.value if isinstance(s, RunStatus) else s for s in statuses]}
+        filters['status'] = {'in': [s.value.upper() if isinstance(s, RunStatus) else s.upper() for s in statuses]}
 
     cluster_names = cluster_names or clusters  # for backwards compatibility, clusters is supported as cluster_names
     if cluster_names:
         filters['clusterName'] = {'in': [c.name if isinstance(c, Cluster) else c for c in cluster_names]}
     if gpu_types:
         filters['gpuType'] = {'in': [gt.value if isinstance(gt, GPUType) else gt for gt in gpu_types]}
     if gpu_nums:
```

## mcli/cli/m_describe/describe_runs.py

```diff
@@ -1,23 +1,24 @@
 """Implementation of mcli describe run"""
 from __future__ import annotations
 
 import logging
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from enum import Enum
-from typing import Any, Dict, Generator, List, Optional, Tuple
+from typing import Any, Dict, Generator, List, Optional, Tuple, TypeVar
 
 from rich.table import Table
 
 from mcli.api.exceptions import cli_error_handler
 from mcli.api.model.run import Node, Run
 from mcli.cli.m_get.display import (MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_vertical_display_table,
                                     format_timestamp)
+from mcli.models.run_config import DEFAULT_PRIORITY_NAME, ComputeConfig
 from mcli.sdk import get_run
-from mcli.utils.utils_logging import FormatString, format_string, print_timedelta
+from mcli.utils.utils_logging import FormatString, console, format_string, print_timedelta
 
 logger = logging.getLogger(__name__)
 
 DISPLAY_RUN_STATUSES = ['PENDING', 'RUNNING', 'COMPLETED']
 
 
 class DisplayRunStatus(Enum):
@@ -25,60 +26,57 @@
     RUNNING = 'RUNNING'
     COMPLETED = 'COMPLETED'
 
 
 class DescribeRunDetailColumns(Enum):
     NAME = 'name'
     RUN_ID = 'run_uid'
-    CLUSTER = 'cluster'
-    GPU_TYPE = 'gpu_type'
-    GPU_NUM = 'gpu_num'
-    CPUS = 'cpus'
     IMAGE = 'image'
+    PRIORITY = 'priority'
 
 
 class DescribeRunLifecycleColumns(Enum):
     STATUS = 'status'
     START_TIME = 'start_time'
     END_TIME = 'end_time'
     DURATION = 'duration'
 
 
 class DescribeRunOriginalInputColumns(Enum):
     SUBMITTED_CONFIG = 'submitted_config'
 
 
-RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Cluster', 'Image', 'GPU Type', 'GPU Num']
+RUN_DETAIL_DISPLAY_NAMES = ['Run Name', 'Image', 'Priority']
 
 RUN_LIFECYCLE_DISPLAY_NAMES = [
     'Start Time',
     'End Time',
     'Duration',
 ]
 RUN_NODES_DISPLAY_NAMES = ['Node Name']
 SUBMITTED_CONFIG = ['Run Config']
 
 
 @dataclass
 class DescribeRunDetailDisplayItem(MCLIDisplayItem):
     """Tuple that extracts detailed run data for display purposes"""
     name: str
-    cluster: str
     image: str
-    gpu_type: Optional[str] = None
-    gpu_num: Optional[str] = None
+    priority: str
 
     @classmethod
     def from_run(cls, run: Run) -> DescribeRunDetailDisplayItem:
+        priority = run.config.scheduling.get('priority', None) or DEFAULT_PRIORITY_NAME
+        if priority and priority.lower() == 'default':
+            priority = DEFAULT_PRIORITY_NAME
+
         extracted: Dict[str, Any] = {
             DescribeRunDetailColumns.NAME.value: run.config.name,
-            DescribeRunDetailColumns.CLUSTER.value: run.config.cluster,
             DescribeRunDetailColumns.IMAGE.value: run.config.image,
-            DescribeRunDetailColumns.GPU_TYPE.value: run.config.gpu_type,
-            DescribeRunDetailColumns.GPU_NUM.value: run.config.gpu_num,
+            DescribeRunDetailColumns.PRIORITY.value: priority.lower(),
         }
 
         return DescribeRunDetailDisplayItem(**extracted)
 
 
 @dataclass
 class DescribeRunLifecycleDisplayItem(MCLIDisplayItem):
@@ -176,17 +174,65 @@
             yield MCLIDescribeRunNodeDisplayItem(n.rank, n.name)
 
     @property
     def index_label(self) -> str:
         return 'rank'
 
 
-# Run lifecycle
+T = TypeVar('T')
+
+
+def compute_or_deprecated(compute: ComputeConfig, key: str, deprecated: T) -> Optional[T]:
+    from_compute = compute.get(key, None)
+    if from_compute is not None:
+        return from_compute
+    return deprecated
 
 
+@dataclass
+class DescribeComputeRequests():
+    """Describer for compute requests"""
+    cluster: Optional[str] = None
+    gpu_type: Optional[str] = None
+    gpus: Optional[int] = None
+    cpus: Optional[int] = None
+    instance: Optional[str] = None
+    nodes: Optional[int] = None
+
+    @property
+    def display_names(self) -> Dict[str, str]:
+        # Return display name mapping for table
+        return {
+            'cluster': 'Cluster',
+            'gpu_type': 'GPU Type',
+            'gpus': 'GPUs',
+            'cpus': 'CPUs',
+            'instance': 'Instance',
+            'nodes': 'Nodes',
+        }
+
+    @classmethod
+    def from_run(cls, run: Run) -> DescribeComputeRequests:
+        return DescribeComputeRequests(
+            cluster=compute_or_deprecated(run.config.compute, 'cluster', run.config.cluster),
+            gpu_type=compute_or_deprecated(run.config.compute, 'gpu_type', run.config.gpu_type),
+            gpus=compute_or_deprecated(run.config.compute, 'gpus', run.config.gpu_num),
+            cpus=compute_or_deprecated(run.config.compute, 'cpus', run.config.cpus),
+            instance=run.config.compute.get('instance', None),
+            nodes=run.config.compute.get('nodes', None),
+        )
+
+    def to_table(self) -> Table:
+        data = {self.display_names.get(k, k.capitalize()): str(v) for k, v in asdict(self).items() if v is not None}
+        columns = list(data.keys())
+        values = [tuple(data.values())]
+        return create_vertical_display_table(data=values, columns=columns)
+
+
+# Run lifecycle
 def format_run_status(status: str, run: Run) -> DescribeRunLifecycleDisplayItem:
     if status == DisplayRunStatus.PENDING.value:
         duration = print_timedelta(run.started_at - run.created_at) if run.started_at and run.created_at else '-'
         return DescribeRunLifecycleDisplayItem(status=status,
                                                start_time=format_timestamp(run.created_at),
                                                end_time=format_timestamp(run.started_at),
                                                duration=duration)
@@ -208,20 +254,26 @@
     """
     Fetches more details of a Run
     """
     del kwargs
 
     run = get_run(run_name)
 
-    # Run metadata section
+    # Run details section
     print(format_string('Run Details', FormatString.BOLD))
     metadata_display = MCLIDescribeRunDetailsDisplay([run])
     metadata_display.print(output)
     print()
 
+    # Compute requests section
+    print(format_string('Compute Requests', FormatString.BOLD))
+    compute_display = DescribeComputeRequests.from_run(run)
+    console.print(compute_display.to_table())
+    print()
+
     # Run lifecycle section
     print(format_string('Run Lifecycle', FormatString.BOLD))
     lifecycle_display = MCLIDescribeRunLifecycleDisplay([run])
     lifecycle_display.print(output)
     print()
 
     if run.metadata:
```

## mcli/cli/m_get/clusters.py

```diff
@@ -1,70 +1,213 @@
 """CLI getter for clusters"""
 import logging
 from dataclasses import dataclass
 from http import HTTPStatus
-from typing import Dict, Generator, List, Optional
+from typing import Any, Dict, Generator, List, Optional
+
+from rich.table import Table
 
 from mcli.api.cluster import get_clusters as api_get_cluster
 from mcli.api.exceptions import MAPIErrorMessages, MAPIException, cli_error_handler
 from mcli.api.model.cluster_details import ClusterDetails
-from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay
+from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, create_display_table
 from mcli.config import FeatureFlag, MCLIConfig
-from mcli.models import Cluster
+from mcli.models.mcli_cluster import Cluster
 from mcli.serverside.clusters.cluster_instances import UserInstanceRegistry
 from mcli.serverside.clusters.gpu_type import GPUType
 from mcli.utils.utils_logging import WARN
 
 logger = logging.getLogger(__name__)
 
 
+def get_gpu_description(gpus: int, nodes: int, allow_fractional: bool, allow_multinode: bool) -> str:
+    """Get a string showing possible `gpus` values for the instance
+
+    Args:
+        gpus (int): Number of GPUs per node for the instance
+        nodes (int): Number of nodes of the instance type that are available
+        allow_fractional (bool): Whether fractional nodes can be allocated
+        allow_multinode (bool): Whether multinode runs are allowed
+
+    Returns:
+        str: Useful string of gpu values
+
+    Examples:
+    For only single node runs with fractional enabled:
+    >>> get_gpu_description(8, 1, True, False)
+    "≤8"
+
+    For multinode runs with 10 nodes available:
+    >>> get_gpu_description(8, 10, False, True)
+    "8,16,...,80"
+    """
+    if nodes < 1:
+        return '-'
+
+    if gpus == 0:
+        return '0'
+
+    options: List[str] = []
+    if allow_fractional:
+        options.append(f'≤{gpus}')
+    else:
+        options.append(f'{gpus}')
+
+    if not allow_multinode or nodes == 1:
+        return options[0]
+
+    options.append(f'{2 * gpus}')
+    if nodes > 3:
+        options.extend(['...', f'{nodes * gpus}'])
+    elif nodes == 3:
+        options.append(f'{3 * gpus}')
+
+    return ','.join(options)
+
+
+def get_nodes_description(nodes: int, allow_multinode: bool) -> str:
+    """Get a string showing possible `nodes` values for the instance
+    """
+    if nodes == 0:
+        return '-'
+    if not allow_multinode or nodes == 1:
+        return '1'
+    else:
+        return f'≤{nodes}'
+
+
 @dataclass
 class ClusterDisplayItem(MCLIDisplayItem):
+    # Cluster columns
     id: Optional[str]
     name: str
     provider: str
-    context: str
-    namespace: str
-    gpu_types_and_nums: Dict[str, List[int]]
+
+    # GPU columns
+    gpu_type: str
+    gpus: str
+
+    # Instance columns
+    instance: str
+    nodes: str
+
+
+GPU_COLUMNS = ['gpu_type', 'gpus']
+INSTANCE_COLUMNS = ['instance', 'nodes']
+SEP_HEADER = ['']
+SEP = ['│']
 
 
 class ClusterDisplay(MCLIGetDisplay):
     """`mcli get cluster` display class
     """
 
     def __init__(self, cluster: List[ClusterDetails], include_ids: bool = False):
         self.cluster = sorted(cluster)
         self.include_ids = include_ids
 
     def __iter__(self) -> Generator[ClusterDisplayItem, None, None]:
         for c in self.cluster:
-            yield ClusterDisplayItem(id=c.id if self.include_ids else None,
-                                     name=c.name,
-                                     provider=c.provider,
-                                     context=c.kubernetes_context,
-                                     namespace=c.namespace,
-                                     gpu_types_and_nums={i.gpu_type: i.gpu_nums for i in c.cluster_instances})
+            for instance in sorted(c.cluster_instances, reverse=True):
+
+                # cpu instance sometimes captures non-worker nodes, so we'll just set
+                # the value to 1 (unless it was 0)
+                nodes = get_nodes_description(instance.nodes, c.allow_multinode)
+                if instance.name == 'cpu' and nodes != '-':
+                    nodes = '1'
+
+                yield ClusterDisplayItem(
+                    id=c.id if self.include_ids else None,
+                    name=c.name,
+                    provider=c.provider,
+                    instance=instance.name,
+                    nodes=nodes,
+                    gpu_type=instance.gpu_type.lower(),
+                    gpus=get_gpu_description(
+                        instance.gpus,
+                        instance.nodes,
+                        c.allow_fractional,
+                        c.allow_multinode,
+                    ),
+                )
+
+    def to_name(self, items: List[Dict[str, Any]]) -> List[str]:
+        """Customized name output for clusters that removes duplicates
+        """
+        return list({item['name']: None for item in items}.keys())
+
+    def to_table(self, items: List[Dict[str, Any]]) -> Table:
+        """Customized table output for clusters that includes a separator between
+        gpu details and instance details
+        """
+
+        # Get cluster columns and instance columns
+        # Cluster columns will be suppressed if repeated
+        cluster_columns, gpu_columns, instance_columns = [], [], []
+        reference = items[0]
+        for k in reference:
+            if k == 'name':
+                continue
+            if k == 'id' and not self.include_ids:
+                continue
+            if k in GPU_COLUMNS:
+                gpu_columns.append(k)
+            elif k in INSTANCE_COLUMNS:
+                instance_columns.append(k)
+            else:
+                cluster_columns.append(k)
+
+        def apply_dim(value: str, nodes: str) -> str:
+            return f'[dim]{value}[/]' if nodes == '-' else value
+
+        columns, names = [], []
+        last_cluster = None
+        for item in items:
+            name = f'[bold bright_blue]{item["name"]}[/]'
+            cluster_values = [item[k] for k in cluster_columns]
+            gpu_values = [apply_dim(item[k], item['nodes']) for k in gpu_columns]
+            instance_values = [apply_dim(item[k], item['nodes']) for k in instance_columns]
+            all_instance_values = SEP + gpu_values + SEP + instance_values
+            if name != last_cluster:
+                names.append(name)
+                columns.append(tuple(cluster_values + all_instance_values))
+                last_cluster = name
+            else:
+                names.append('')
+                columns.append(tuple([''] * len(cluster_columns) + all_instance_values))
+        column_names = cluster_columns + SEP_HEADER + gpu_columns + SEP_HEADER + instance_columns
+        return create_display_table(names, columns, column_names, 'NAME')
+
+
+@dataclass
+class KubeClusterDisplayItem(MCLIDisplayItem):
+    id: Optional[str]
+    name: str
+    provider: str
+    context: str
+    namespace: str
+    gpu_types_and_nums: Dict[str, List[int]]
 
 
 class KubeClusterDisplay(MCLIGetDisplay):
     """`mcli get cluster` display class that talks to kubernetes
     """
 
     def __init__(self, cluster: List[Cluster]):
         self.cluster = cluster
 
-    def __iter__(self) -> Generator[ClusterDisplayItem, None, None]:
+    def __iter__(self) -> Generator[KubeClusterDisplayItem, None, None]:
         gpu_registry = _get_gpu_registry(self.cluster)
         for cluster in self.cluster:
-            yield ClusterDisplayItem(id=None,
-                                     name=cluster.name,
-                                     provider='MosaicML',
-                                     context=cluster.kubernetes_context,
-                                     namespace=cluster.namespace,
-                                     gpu_types_and_nums=gpu_registry[cluster.name])
+            yield KubeClusterDisplayItem(id=None,
+                                         name=cluster.name,
+                                         provider='MosaicML',
+                                         context=cluster.kubernetes_context,
+                                         namespace=cluster.namespace,
+                                         gpu_types_and_nums=gpu_registry[cluster.name])
 
 
 def _get_gpu_registry(clusters: List[Cluster]) -> Dict[str, Dict[str, List[int]]]:
     user_registry = UserInstanceRegistry(clusters=clusters)
     gpu_info: Dict[str, Dict[str, List[int]]] = {}
     for cluster, gpu_dict in user_registry.registry.items():
         gpu_info[cluster] = {}
@@ -100,8 +243,9 @@
     else:
         del include_ids
         if conf.clusters:
             display = KubeClusterDisplay(conf.clusters)
             display.print(output)
         else:
             logger.warning(f'{WARN} No clusters found.\n\nTo create a cluster, run:\n\n[bold]mcli create cluster[/]')
+
     return 0
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## mcli/cli/m_get/runs.py

```diff
@@ -1,78 +1,81 @@
 """Implementation of mcli get runs"""
 from __future__ import annotations
 
 import argparse
 import logging
+import math
 from dataclasses import dataclass
 from enum import Enum
-from typing import Dict, Generator, List, Optional
+from typing import Dict, Generator, List, Optional, Tuple
 
 from mcli import config
 from mcli.api.exceptions import cli_error_handler
 from mcli.cli.common.run_filters import configure_submission_filter_argparser, get_runs_with_filters
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, format_timestamp
 from mcli.sdk import Run
 from mcli.utils.utils_cli import comma_separated
 from mcli.utils.utils_run_status import RunStatus
 
 logger = logging.getLogger(__name__)
 
+GPUS_PER_NODE = 8
+
 
 class RunColumns(Enum):
     ID = 'id'
     NAME = 'name'
+    USER = 'user'
     CLUSTER = 'cluster'
-    GPU_TYPE = 'gpu_type'
-    GPU_NUM = 'gpu_num'
+    INSTANCE = 'instance'
+    NODES = 'nodes'
     CREATED_TIME = 'created_time'
     START_TIME = 'start_time'
     END_TIME = 'end_time'
-    USER = 'user'
     STATUS = 'status'
 
 
 @dataclass
 class RunDisplayItem(MCLIDisplayItem):
     """Tuple that extracts run data for display purposes.
     """
     name: str
-    gpu_num: str
+    nodes: str
     created_time: str
     start_time: str
     end_time: str
     status: str
     user: str
+    instance: str
     cluster: Optional[str] = None
-    gpu_type: Optional[str] = None
     id: Optional[str] = None
 
     @classmethod
     def from_run(cls, run: Run, include_ids: bool = False) -> RunDisplayItem:
         display_status = run.status.display_name
         if run.reason:
             display_status = f"{display_status} ({run.reason})"
+        instance, nodes = get_instance_name_and_nodes(run)
         extracted: Dict[str, str] = {
             RunColumns.NAME.value: run.name,
+            RunColumns.USER.value: run.created_by,
             RunColumns.CLUSTER.value: run.config.cluster,
-            RunColumns.GPU_TYPE.value: run.config.gpu_type or run.config.compute.get('gpu_type', None) or 'Unknown',
-            RunColumns.GPU_NUM.value: str(run.config.gpu_num),
+            RunColumns.INSTANCE.value: instance,
+            RunColumns.NODES.value: str(nodes),
             RunColumns.CREATED_TIME.value: format_timestamp(run.created_at),
             RunColumns.START_TIME.value: format_timestamp(run.started_at),
             RunColumns.END_TIME.value: format_timestamp(run.completed_at),
-            RunColumns.USER.value: run.created_by,
-            RunColumns.STATUS.value: display_status
+            RunColumns.STATUS.value: display_status,
         }
         if include_ids:
             extracted[RunColumns.ID.value] = run.run_uid
 
         return RunDisplayItem(**extracted)
 
 
-# TODO: add column for USER
 class MCLIRunDisplay(MCLIGetDisplay):
     """Display manager for runs
     """
 
     def __init__(self, models: List[Run], include_ids: bool = False):
         self.models = sorted(models, key=lambda x: x.created_at, reverse=True)
         self.include_ids = include_ids
@@ -90,14 +93,84 @@
 
     def __iter__(self) -> Generator[RunDisplayItem, None, None]:
         for model in self.models:
             item = RunDisplayItem.from_run(model, include_ids=self.include_ids)
             yield item
 
 
+def get_instance_name_and_nodes(run: Run) -> Tuple[str, int]:
+    """Get the run's instance name and number of nodes
+
+    We'll try to create a human-readable name based on the gpu number and type (ie 8x v100),
+    if possible.
+
+    With the addition of `compute` to the run config, all values should be filled in, so much
+    of the logic here is for older runs. These have a limited set of possible values, so we
+    make some assumptions which should largely be correct.
+
+    Args:
+        run (Run): a Run
+
+    Returns:
+        Tuple[str, int]: The instance name and number of nodes
+    """
+
+    # Extract GPU Type
+    # Default to 'cpu' type
+    gpu_type = 'cpu'
+    if run.config.compute.get('gpu_type', None):
+        assert 'gpu_type' in run.config.compute  # for the linter
+        gpu_type = run.config.compute['gpu_type']
+        assert gpu_type is not None  # Also for the linter...
+    elif run.config.gpu_type:
+        gpu_type = run.config.gpu_type
+
+    # Convert 'None' to 'cpu'
+    if gpu_type.lower() == 'none':
+        gpu_type = 'cpu'
+
+    # Extract GPU Number
+    # Default to 0 because some older runs may only set gpu type, which was probably "None"
+    total_gpus = 0
+    if 'gpus' in run.config.compute and run.config.compute['gpus'] is not None:
+        total_gpus = run.config.compute['gpus']
+    elif run.config.gpu_num is not None:
+        total_gpus = run.config.gpu_num
+
+    # Get the instance type as a fallback
+    instance = run.config.compute.get('instance', None)
+
+    # Get the number of nodes
+    nodes = run.config.compute.get('nodes', None)
+    if nodes is not None:
+        # Trim to gpus per node
+        gpus = int(total_gpus / nodes)
+    elif total_gpus > GPUS_PER_NODE:
+        # If we have more than 8 gpus, we can reasonably assume we're on multinode
+        # This assumes 8 gpus per node, which should be valid for all old runs
+        nodes = math.ceil(total_gpus / GPUS_PER_NODE)
+        gpus = GPUS_PER_NODE
+    else:
+        nodes = 1
+        gpus = total_gpus
+
+    if gpu_type != 'cpu':
+        # Prefer the gpu type as a description, if available
+        return f"{gpus}x {gpu_type.lower()}", nodes
+    elif instance:
+        # Fall back on instance type (especially for cpu instances)
+        return instance, nodes
+    elif gpu_type == 'cpu':
+        # Otherwise just use "cpu"
+        return gpu_type, nodes
+    else:
+        # Last resort, go with unknown
+        return 'unknown', nodes
+
+
 @cli_error_handler('mcli get runs')
 def cli_get_runs(
     name_filter: Optional[List[str]] = None,
     cluster_filter: Optional[List[str]] = None,
     before_filter: Optional[str] = None,
     after_filter: Optional[str] = None,
     gpu_type_filter: Optional[List[str]] = None,
```

## mcli/cli/m_interactive/temp_mcloud_interactive.py

```diff
@@ -31,15 +31,15 @@
     connect: bool = True,
     reconnect: Optional[str] = None,
 ) -> int:
 
     run: Optional[Run] = None
 
     if reconnect:
-        all_runs = get_runs([reconnect])
+        all_runs = get_runs([reconnect], include_details=True)
         if not all_runs:
             raise RuntimeError(f'Could not find an interactive session named {reconnect}')
 
         run = all_runs[0]
         if run.status >= RunStatus.TERMINATING:
             raise RuntimeError(f'Run {run.name} is {run.status.value}. Please select a running run')
         cluster = run.config.cluster
@@ -96,15 +96,15 @@
 
         namespace = simple_prompt(
             f'Which kube namespace should be used to connect to the interactive run? [{default_namespace}]',
             default=default_namespace,
             mandatory=False,
         )
 
-        pod_id = f"{run.run_uid}-{rank}"
+        pod_id = f"{run.last_attempt_id}-{rank}"
         logger.info(f'{INFO} Waiting for session to start with pod [blue]{pod_id}[/]...')
         logger.info(f'{INFO} Press Ctrl+C to quit and interact with your session manually.')
         run = wait_for_run_status(run, status=RunStatus.RUNNING, timeout=300)
 
         rank_str = f"node rank [cyan]{rank}[/] of " if rank > 0 else ""
         logger.info(f'{OK} Connecting to {rank_str}interactive session [cyan]{run.name}[/]')
```

## mcli/models/inference_deployment_config.py

```diff
@@ -199,15 +199,15 @@
         'command': 'command',
         'replicas': 'replicas',
         'metadata': 'metadata',
         'envVariables': 'env_variables',
         'integrations': 'integrations',
     }
 
-    _optional_display_properties = {'gpu_type', 'metadata', 'env_variables', 'integrations'}
+    _required_display_properties = {'name', 'image', 'command', 'replicas'}
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> InferenceDeploymentConfig:
         data = {}
         for k, v in cls._property_translations.items():
             if k not in response:
                 # This must be an optional property, so skip
```

## mcli/models/run_config.py

```diff
@@ -17,22 +17,23 @@
 from mcli.utils.utils_string_functions import (MAX_KUBERNETES_LENGTH, ensure_rfc1123_compatibility, validate_image,
                                                validate_rfc1123_name)
 
 logger = logging.getLogger(__name__)
 RUN_CONFIG_UID_LENGTH = 6
 VALID_OPTIMIZATION_LEVELS = frozenset([0, 1, 2, 3])
 MAX_RUN_NAME_LENGTH = MAX_KUBERNETES_LENGTH - RUN_CONFIG_UID_LENGTH - 1  # -1 for the dash
+DEFAULT_PRIORITY_NAME = 'medium'
 
 
-class SchedulingConfig(TypedDict):
+class SchedulingConfig(TypedDict, total=False):
     """Typed dictionary for nested scheduling configurations"""
     priority: Optional[str]
 
 
-class ComputeConfig(TypedDict):
+class ComputeConfig(TypedDict, total=False):
     """Typed dictionary for nested compute requests"""
     cluster: Optional[str]
     instance: Optional[str]
     nodes: Optional[int]
     gpu_type: Optional[str]
     gpus: Optional[int]
     cpus: Optional[int]
@@ -73,20 +74,18 @@
     cluster: str = ''
     platform: str = ''
 
     # Partition is an optional new keyword
     partitions: Optional[List[str]] = None
 
     # Scheduling parameters - optional for backwards-compatibility
-    # pylint: disable-next=unnecessary-lambda
-    scheduling: SchedulingConfig = field(default_factory=lambda: SchedulingConfig(**{}))
+    scheduling: SchedulingConfig = field(default_factory=SchedulingConfig)
 
     # Compute parameters - optional for backwards-compatibility
-    # pylint: disable-next=unnecessary-lambda
-    compute: ComputeConfig = field(default_factory=lambda: ComputeConfig(**{}))
+    compute: ComputeConfig = field(default_factory=ComputeConfig)
 
     # User defined metadata
     metadata: Dict[str, Any] = field(default_factory=dict)
 
     _property_translations = {
         'run_id': 'run_id',
         'runName': 'name',
@@ -383,18 +382,16 @@
     platform: Optional[str] = None
     cluster: Optional[str] = None
     image: Optional[str] = None
     partitions: Optional[List[str]] = None
     optimization_level: Optional[int] = None
     integrations: List[Dict[str, Any]] = field(default_factory=list)
     env_variables: List[Dict[str, str]] = field(default_factory=list)
-    # pylint: disable-next=unnecessary-lambda
-    scheduling: SchedulingConfig = field(default_factory=lambda: SchedulingConfig(**{}))
-    # pylint: disable-next=unnecessary-lambda
-    compute: ComputeConfig = field(default_factory=lambda: ComputeConfig(**{}))
+    scheduling: SchedulingConfig = field(default_factory=SchedulingConfig)
+    compute: ComputeConfig = field(default_factory=ComputeConfig)
     metadata: Dict[str, Any] = field(default_factory=dict)
 
     command: str = ''
     parameters: Dict[str, Any] = field(default_factory=dict)
     entrypoint: str = ''
 
     _property_translations = {
@@ -410,18 +407,15 @@
         'command': 'command',
         'entrypoint': 'entrypoint',
         'scheduling': 'scheduling',
         'metadata': 'metadata',
         'compute': 'compute',
     }
 
-    _optional_display_properties = {
-        'cpus', 'env_variables', 'entrypoint', 'gpu_type', 'integrations', 'optimization_level', 'parameters',
-        'partitions', 'platform', 'run_name', 'scheduling', 'metadata'
-    }
+    _required_display_properties = {'name', 'image', 'command'}
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> RunConfig:
         data = {}
         for k, v in cls._property_translations.items():
             if k not in response:
                 # This must be an optional property, so skip
```

## mcli/utils/utils_config.py

```diff
@@ -24,15 +24,15 @@
     return ''.join(items)
 
 
 @dataclass
 class BaseSubmissionConfig():
     """ Base class for config objects"""
 
-    _optional_display_properties = []
+    _required_display_properties = set()
 
     @classmethod
     def empty(cls):
         return cls()
 
     @classmethod
     def from_file(cls, path: Union[str, Path]):
@@ -68,15 +68,15 @@
 
         return cls(**constructor)
 
     def __str__(self) -> str:
         filtered_dict = {}
         for k, v in asdict(self).items():
             # skip nested and direct empty values for optional properties
-            if k in self._optional_display_properties:
+            if k not in self._required_display_properties:
                 if isinstance(v, dict) and not any(v.values()):
                     continue
                 if not v:
                     continue
             filtered_dict[k] = v
         # to use with safe_dump:
         yaml.representer.SafeRepresenter.add_representer(str, str_presenter)
```

## mcli/utils/utils_logging.py

```diff
@@ -6,14 +6,15 @@
 from typing import List
 
 from rich import print as rprint
 from rich.console import Console
 from rich.highlighter import NullHighlighter
 from rich.logging import RichHandler
 from rich.tree import Tree
+from yaml.representer import SafeRepresenter
 
 console = Console()
 err_console = Console(stderr=True)
 
 FAIL = '[red]✗[/] '
 OK = '[green]✔[/] '
 INFO = '[blue]i[/] '
@@ -139,14 +140,15 @@
         return f'{int(seconds/60)}min'
     elif seconds < 24 * 3600:
         return f'{int(seconds/3600)}hr'
     else:
         return f'{int(seconds/3600/24)}d'
 
 
-def str_presenter(dumper, data):
+def str_presenter(dumper: SafeRepresenter, data: str):
     """Converts multiline data into |\n<data>
     This is useful for displaying Run.command.
     """
+    data = data.strip()
     if len(data.splitlines()) > 1:  # check for multiline string
         return dumper.represent_scalar('tag:yaml.org,2002:str', data, style='|')
     return dumper.represent_scalar('tag:yaml.org,2002:str', data)
```

## Comparing `mosaicml_cli-0.3.6.dist-info/METADATA` & `mosaicml_cli-0.3.7.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,62 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.3.6
+Version: 0.3.7
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: argcomplete (>=2.0.0)
 Requires-Dist: backoff (>=2.2.1)
-Requires-Dist: coolname (>=1.1.0)
-Requires-Dist: fire (>=0.4.0)
 Requires-Dist: kubernetes (>=21.7.0)
-Requires-Dist: parse (>=1.19.0)
 Requires-Dist: prompt-toolkit (>=3.0.29)
 Requires-Dist: pyyaml (>=5.4.1)
 Requires-Dist: questionary (>=1.10.0)
 Requires-Dist: rich (>=10.16.2)
 Requires-Dist: ruamel.yaml (>=0.17.21)
 Requires-Dist: toml (>=0.10.2)
 Requires-Dist: typing-extensions (>=4.0.1)
-Requires-Dist: wandb (>=0.12.2)
-Requires-Dist: yaspin (>=2.1.0)
-Requires-Dist: jinja2
 Requires-Dist: arrow (>=1.2.2)
-Requires-Dist: slack-sdk (>=3.17.1)
 Requires-Dist: docker (>=5.0.3)
 Requires-Dist: gql[websockets] (>=3.4.0)
 Provides-Extra: all
 Requires-Dist: sphinxcontrib-serializinghtml (>=1.1.5) ; extra == 'all'
-Requires-Dist: sphinxcontrib-images (>=0.9.4) ; extra == 'all'
-Requires-Dist: pytest-mock (>=3.7.0) ; extra == 'all'
-Requires-Dist: sphinx-panels (>=0.6.0) ; extra == 'all'
-Requires-Dist: sphinxcontrib-htmlhelp (>=2.0.0) ; extra == 'all'
+Requires-Dist: sphinx-design ; extra == 'all'
 Requires-Dist: myst-parser (>=0.16.1) ; extra == 'all'
-Requires-Dist: pylint (>=2.12.2) ; extra == 'all'
-Requires-Dist: furo (>=2022.3.4) ; extra == 'all'
+Requires-Dist: sphinxcontrib-devhelp (>=1.0.2) ; extra == 'all'
+Requires-Dist: pytest-cov (>=4.0.0) ; extra == 'all'
 Requires-Dist: pre-commit (>=2.17.0) ; extra == 'all'
-Requires-Dist: pytest (>=6.2.5) ; extra == 'all'
+Requires-Dist: sphinxext-opengraph (>=0.6.1) ; extra == 'all'
+Requires-Dist: sphinxcontrib-htmlhelp (>=2.0.0) ; extra == 'all'
 Requires-Dist: sphinxcontrib-katex (>=0.8.6) ; extra == 'all'
-Requires-Dist: isort (>=5.9.3) ; extra == 'all'
+Requires-Dist: sphinx-external-toc (>=0.3.0) ; extra == 'all'
+Requires-Dist: pytest-mock (>=3.7.0) ; extra == 'all'
+Requires-Dist: yapf (>=0.32.0) ; extra == 'all'
 Requires-Dist: sphinxemoji (>=0.2.0) ; extra == 'all'
-Requires-Dist: sphinx-rtd-theme (>=1.0.0) ; extra == 'all'
+Requires-Dist: sphinx-panels (>=0.6.0) ; extra == 'all'
+Requires-Dist: pyright (>=1.1.256) ; extra == 'all'
+Requires-Dist: pytest (>=6.2.5) ; extra == 'all'
+Requires-Dist: sphinxcontrib-qthelp (>=1.0.3) ; extra == 'all'
 Requires-Dist: radon (>=5.1.0) ; extra == 'all'
-Requires-Dist: sphinx-design ; extra == 'all'
-Requires-Dist: sphinx-external-toc (>=0.3.0) ; extra == 'all'
-Requires-Dist: sphinxext-opengraph (>=0.6.1) ; extra == 'all'
-Requires-Dist: sphinx-markdown-tables (>=0.0.15) ; extra == 'all'
+Requires-Dist: sphinxcontrib-images (>=0.9.4) ; extra == 'all'
+Requires-Dist: sphinx-copybutton (>=0.5.0) ; extra == 'all'
 Requires-Dist: sphinxcontrib-applehelp (>=1.0.2) ; extra == 'all'
+Requires-Dist: pylint (>=2.12.2) ; extra == 'all'
+Requires-Dist: sphinx-markdown-tables (>=0.0.15) ; extra == 'all'
+Requires-Dist: sphinx-rtd-theme (>=1.0.0) ; extra == 'all'
+Requires-Dist: sphinxcontrib-jsmath (>=1.0.1) ; extra == 'all'
 Requires-Dist: sphinx (>=4.4.0) ; extra == 'all'
-Requires-Dist: sphinxcontrib-qthelp (>=1.0.3) ; extra == 'all'
-Requires-Dist: yapf (>=0.32.0) ; extra == 'all'
+Requires-Dist: isort (>=5.9.3) ; extra == 'all'
+Requires-Dist: furo (>=2022.3.4) ; extra == 'all'
 Requires-Dist: sphinx-argparse (>=0.3.1) ; extra == 'all'
-Requires-Dist: sphinxcontrib-jsmath (>=1.0.1) ; extra == 'all'
-Requires-Dist: sphinx-copybutton (>=0.5.0) ; extra == 'all'
-Requires-Dist: sphinxcontrib-devhelp (>=1.0.2) ; extra == 'all'
-Requires-Dist: pytest-cov (>=4.0.0) ; extra == 'all'
-Requires-Dist: pyright (>=1.1.256) ; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: isort (>=5.9.3) ; extra == 'dev'
 Requires-Dist: pre-commit (>=2.17.0) ; extra == 'dev'
 Requires-Dist: pylint (>=2.12.2) ; extra == 'dev'
 Requires-Dist: pyright (>=1.1.256) ; extra == 'dev'
 Requires-Dist: pytest (>=6.2.5) ; extra == 'dev'
 Requires-Dist: pytest-mock (>=3.7.0) ; extra == 'dev'
```

## Comparing `mosaicml_cli-0.3.6.dist-info/RECORD` & `mosaicml_cli-0.3.7.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 mcli/__init__.py,sha256=rjbBF2gbyBq8Hf3mMT7B1S_Chir9b2m6O7N95xthTPE,54
 mcli/config.py,sha256=wFms9BQwrR6YPu9kcRUs5Txgr0lig7pyMW122NgWuUw,16462
-mcli/version.py,sha256=8nI9AsLSPDx7mQR7JRjGn-jF0zOjfcAW9c0ubi8WncM,3884
+mcli/version.py,sha256=fPQwK4156pMiNH29Za9Z3IjWMvUyky4AQCacgyC-UBs,3884
 mcli/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/exceptions.py,sha256=DTs9XbfuNvXYyy4tiFVpw4kx5eWchVYyd_56HkalmjU,11677
 mcli/api/types.py,sha256=5ZDeWvycwdF70hqfNfmiBJdHY4-wVoeDh-IkBLqLQRQ,508
 mcli/api/typing_future.py,sha256=dtcpSyHS0g3gvgZ_ACrSnTAYFEuh9UjNshcfPJaXkd4,2354
 mcli/api/cluster/__init__.py,sha256=NXNkGsa4lOdwfP8oVjLjakgJxfh8u76u2I_gd3qGSho,134
-mcli/api/cluster/api_get_clusters.py,sha256=TPLdeGqCJMhxe9_jr2kFuNlnzUfJXQhcwV1xeq0fFHs,4058
+mcli/api/cluster/api_get_clusters.py,sha256=VZab5zVJkeiOgUopBOTmS6VJXttP5wXJOXbrSLJ5nFg,4141
 mcli/api/engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/engine/engine.py,sha256=nv5sL_iI-u90zi1c9Ij7mXNy7gWrT_tYn1QmKZuIHmY,22935
 mcli/api/engine/utils.py,sha256=_SVWfxUR1tfNRiKZR454oq06xw7O9qvmHT7JpdCa5BU,787
 mcli/api/inference_deployments/__init__.py,sha256=WAL54R3PjKUWRUbnOz-IaemRCa_8yAKYtuyo6zcp9OY,879
-mcli/api/inference_deployments/api_create_inference_deployment.py,sha256=PV5rURaNgWOKTHZ0ZjN1-O6XJpg-62SqlNMXdt_5yK8,3388
-mcli/api/inference_deployments/api_delete_inference_deployments.py,sha256=_HyVvxvs3SpbMsY9S86d1cyhBsoPAG98TMIByJE-ekc,3278
-mcli/api/inference_deployments/api_get_inference_deployments.py,sha256=V2liHBIT5rwGPVcbmPSKqooMxzwdRmsIVWw5a6vpxSA,6091
-mcli/api/inference_deployments/api_ping_inference_deployment.py,sha256=CgewB6lmHAqOHHQNHUNaZoukNoGPmzS1wir6g61aaAk,1156
-mcli/api/inference_deployments/api_predict_inference_deployment.py,sha256=bIKcmh1L25jVrjkx8QKqOm2BUtH6slqYXsCsu8ymMt0,1276
+mcli/api/inference_deployments/api_create_inference_deployment.py,sha256=lvAuoYiTOeCmt1mG7ONwgn9F7-bHKjnzaKFrtxTaJvY,3402
+mcli/api/inference_deployments/api_delete_inference_deployments.py,sha256=PGAKhVNPFSI_ngcqhmQvqrlyl-BHdFs39YSoj_3kusY,3292
+mcli/api/inference_deployments/api_get_inference_deployments.py,sha256=49el9cs6oIhLq_NyPufn-rZPr9nFeJAe3ki31vcqq30,6105
+mcli/api/inference_deployments/api_ping_inference_deployment.py,sha256=jKfa9IGNB8TggUAw7bQHFvL6ZoYnDl-DnRkqJvfbZFw,1044
+mcli/api/inference_deployments/api_predict_inference_deployment.py,sha256=cYb8rzflztnZowXxcgUIN4VE_QeuuPMHCfgbl1f6jzo,1126
 mcli/api/kube/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/kube/runs/__init__.py,sha256=ZNMoJSzTUF8S5o1E0JgIXGmFycUiKA2ei1SsMR7dCd0,856
 mcli/api/kube/runs/api_create_run.py,sha256=zl8ZJxccRGONih02NSweT0cGRT92VlOE1WJfnGN1GA0,4900
 mcli/api/kube/runs/api_delete_runs.py,sha256=NrnhEZ2bYnsvXl2fbMZzDqiuGMy0l0Nc2Yd_BDhZitM,5042
 mcli/api/kube/runs/api_get_run_logs.py,sha256=L5pM-MAF82bOwFHOMVw2J6TSgFi_uNiQ79i282AsbWU,14458
-mcli/api/kube/runs/api_get_runs.py,sha256=iCJFa5Uhb7c73fU8Gzappx-y7RVaA4K6jIU0C_3VqVE,16142
+mcli/api/kube/runs/api_get_runs.py,sha256=5xFIWwZoJWKOx5O72qe7anQBcrrnF2Hfqet4dX5r6I4,16251
 mcli/api/kube/runs/api_stop_runs.py,sha256=fShzT4zQ1HmHKVwE777QpI9T8S6s37DwsgdaeE_rxUI,6007
 mcli/api/kube/runs/api_watch_run.py,sha256=y2U8hsT1FtlDhh6ui_HojqBRMTWtX8gvwEAaQ-Xr_T8,6210
 mcli/api/mint/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/mint/shell.py,sha256=taYNm5G4JNrTBij9r9YLaCIWCm_OHMxPVees7Ee7NjA,4987
 mcli/api/mint/tty.py,sha256=xUNMaK7f0kVO-9YJ5Ze6YjCCEOfHs2qMi9OJVMxNfJw,1530
 mcli/api/model/__init__.py,sha256=RE0PFDKAL5nAwQk30tk9ShXeUwBS9Tu0Bg2qWppsPVE,209
-mcli/api/model/cluster_details.py,sha256=bAcIVF6kgjZ53o2vJswi8tPJfLSRihOZ7slja6OXfr4,5655
-mcli/api/model/inference_deployment.py,sha256=pUa7ya1m8tKVodF22qZTX_QOQnG6QPOGsw2_7WUTW9A,3015
-mcli/api/model/run.py,sha256=nqNbltSh34H7osgpNNeYu-WNOaLyeW5f94Y770IW95Q,7946
+mcli/api/model/cluster_details.py,sha256=KlaZeEoE2htotJE6A8n7BhMNQHBfIL9CFtFR6oP9pF4,6186
+mcli/api/model/inference_deployment.py,sha256=70wDG-fBofBs-NujKjaIEEWIzceFMqYlp1I1JFXbqyA,2909
+mcli/api/model/run.py,sha256=OkorF5jH165W3G17kVLnU25pq64ggjDVW3xRikxdzBw,8057
 mcli/api/runs/__init__.py,sha256=Lx2k8QidFOo2dJarOwP4hAxrLpIKB_bJwJ7XJKZi0zI,1102
-mcli/api/runs/api_create_run.py,sha256=4OHsrS1eXsBn52RCjEfHPnQF11J8RNF9NHhut97gLgI,2726
+mcli/api/runs/api_create_run.py,sha256=uzyqUhE19Vg-HowXvQBblEVXztOL0MduGeSsJgutu5I,2750
 mcli/api/runs/api_delete_runs.py,sha256=2sED0FIKpTrJjrkqpPTedk4E6Lo8ZBpT7Ev3WvlPDOM,3926
 mcli/api/runs/api_get_run_logs.py,sha256=YHZt3j9ffpjhf-Wsumkn4h4az92OGMach9ZXZ0bGcXw,9281
-mcli/api/runs/api_get_runs.py,sha256=o4TIHHWDnppWSJirdREHi--hCjbIh9DEEm2gT1oq9hE,8968
+mcli/api/runs/api_get_runs.py,sha256=YcvGUwv1nhr8zq3zAqZV43t8LmAlj2EvSvGG7fUBZ0A,9008
 mcli/api/runs/api_stop_runs.py,sha256=sJHr2iadiGk0SaeGne_EajvC71kQ90TY4hYrmwOJVLE,5099
 mcli/api/runs/api_update_run_metadata.py,sha256=bbJ4sjPiRXS-97kKAvWJTIwzcc2A4BZjFx7FlbGEuPQ,3937
 mcli/api/runs/api_watch_run.py,sha256=i502PYIuTY1eYxfnVYlN0Gx1MAEMoO2cLCdJIsICalQ,10619
 mcli/api/schema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/schema/generic_model.py,sha256=UrDz_zxAxulD9HFV2h-j0Bmgi8Jo0JFRJzqEkTioJLM,636
 mcli/api/secrets/__init__.py,sha256=bAZh1wEkxpZN18pOc-NrGPdzT7W1lJsOa_u2Rr1F2Vk,309
 mcli/api/secrets/api_create_secret.py,sha256=zjHsMCfmLBWfQ-gYOnklkSusSXGY7eXJcW_FAaq2eTw,2365
@@ -64,32 +64,32 @@
 mcli/cli/m_delete/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_delete/delete.py,sha256=POMhTa4pOIxGtUPx5rpyEiOdu_Sab5eWxann4pwdEOQ,14072
 mcli/cli/m_delete/m_delete.py,sha256=fW0xC5sh6z2og3o21o7Elt5wsiQjvfwbjGqezxsyQE4,8417
 mcli/cli/m_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_deploy/m_deploy.py,sha256=lmlbm1EXo2o7LJ5DEiMjFBhFQv8FrWyjAu42-Nw2ECc,3896
 mcli/cli/m_describe/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_describe/describe_inference_deployments.py,sha256=YJzxwfJIfcyzz4zMhew1h-ea_S1_90NlX1d-SGEnTnU,4409
-mcli/cli/m_describe/describe_runs.py,sha256=KM4giCNFRXcbtMXSrUZPuK4ZF459e4dl2I9aINO2b8w,7818
+mcli/cli/m_describe/describe_runs.py,sha256=v1XBdQoqZ9siWtH2vM4NHhqdDHNcDB62K_iPgOXZWkM,9778
 mcli/cli/m_describe/m_describe.py,sha256=L_-rKu8p1MhmC-bpEFzR5Io1E4Bk09wZ-SlhyRCnQek,1860
 mcli/cli/m_get/__init__.py,sha256=nS0qdgx4DwqtFUbnNREWSfSHY17K6xT2fr7i15nN0jc,549
-mcli/cli/m_get/clusters.py,sha256=7eV157RasxpoBIaQcG6D7k11VY3hSM15rUEcz1emJrQ,3909
+mcli/cli/m_get/clusters.py,sha256=sWqDi-9_cbyh9K9-EcKkVbGFALZJqCWszhW-8wvo-qM,8477
 mcli/cli/m_get/display.py,sha256=IFoYOBDieSpok94Ey_q4tl3sUsbOK6ac2SexIGe0HgY,6452
 mcli/cli/m_get/envvars.py,sha256=Jqy3tnK9g3EO1xePREMhRzWo45G_ZDjbLjOszQ1Nl9Q,1315
 mcli/cli/m_get/inference_deployments.py,sha256=BRu6pojlonNjyJSDivpgvYddtUEYpeBjW9vzIYEiWv0,5361
 mcli/cli/m_get/m_get.py,sha256=goLhmY5n0_Xqr3RRgHZtfi2DiSCIwr25HnuFm_N6uwg,4866
-mcli/cli/m_get/runs.py,sha256=EKvA70QVMEvClQBqVQ37f87-GgpgdC8NpmcTh0WJQKs,6346
+mcli/cli/m_get/runs.py,sha256=a71Bpdr_9_UiZYldwpS_AC0tEDN6PFBDztKmiQoF7WE,8759
 mcli/cli/m_get/secrets.py,sha256=6HvbxJVOOsK6fYderHCHNlAHxVtUaNW4O5kses0tvP8,3567
 mcli/cli/m_get/users.py,sha256=kSYAJDRUeEGqXi2-escvzOM2_sw671crBDsqaZQDi_I,1580
 mcli/cli/m_init/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_init/m_init.py,sha256=xMOxNjQnscFuvK0wnF2UIzUYOCXl3eTabLqShtHDgWo,4113
 mcli/cli/m_init/m_init_kube.py,sha256=Vd7M1qAJG2oDKSCj3FC7m7NFiQ_jwnaT3wMlcri-YXE,9374
 mcli/cli/m_interactive/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_interactive/interactive.py,sha256=IWTsgO-VaqazPcJuA6M-NgcMgFf2Me3Q0vwYom2RKTg,9005
 mcli/cli/m_interactive/m_interactive.py,sha256=a4ee2jtmzTaz7BIUEGPPAsXDC8riW2JTNd5xzP1WjtY,16203
-mcli/cli/m_interactive/temp_mcloud_interactive.py,sha256=Uq4nwPEgMZjCpPYn6fE9fJXpIvgH8aGUDCii1DmeS78,4571
+mcli/cli/m_interactive/temp_mcloud_interactive.py,sha256=D7LPkBlWuEY0HSgvqQHVjql-N-GOCVY_8Ld4tvcyiqs,4601
 mcli/cli/m_log/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_log/m_log.py,sha256=9nwlWjBjE5zSVaxwKqdAGLTnwY5wl16HKIbZL67RuII,8633
 mcli/cli/m_ping/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_ping/m_ping.py,sha256=xG2ju-T4GUlPbwA8bwiaZTcVnNE_6QPlktB23I4aJ5w,1742
 mcli/cli/m_predict/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_predict/m_predict.py,sha256=Bc3SLCOw15P0RoJeq9EY98UOKc7Lk2rbGRTlFCwCr5k,2160
 mcli/cli/m_root/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -106,20 +106,20 @@
 mcli/cli/m_use/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_use/m_use.py,sha256=fo2ug4xuyXzzvq-CrDmVjSHLCu5h7QJ0QAS3kUK502A,3234
 mcli/cli/m_util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_util/kube_util.py,sha256=yn0a5xPaCz72nDN3uMYn8YkgbIzr_iTeeSeNu6mkp2I,9853
 mcli/cli/m_util/m_util.py,sha256=TcH9xHnIxMgp9V0iI2Gsd7G2Vs44Zh2_X49-zw95ClM,1147
 mcli/cli/m_util/util.py,sha256=fN1XiUBkmSa9_DZvlVE0MT6tRlEcvMLssFzO4qdkKXM,6515
 mcli/models/__init__.py,sha256=RBw_yR7hcJOjvLrRP5NMj3lTGqWiPVL5IpWWdS_v_18,1199
-mcli/models/inference_deployment_config.py,sha256=hu430hjwGGzr2Y8lwPEl5Wu_VbWlLqc4G3Pc272bK64,8572
+mcli/models/inference_deployment_config.py,sha256=3tUig6bltBNqV9xocAA6KAed6vsC16_4OvCN8WSuGvo,8555
 mcli/models/mcli_cluster.py,sha256=V6UfCAGepIC8gk7Uen0TsHRqWcoeXTRrjOEkGNTHcRI,3693
 mcli/models/mcli_envvar.py,sha256=v9XMY3UNRgF_silwD68LkB2nvrqbV-cyjvR1VUO4_GA,563
 mcli/models/mcli_integration.py,sha256=yeHkttw5xLKrvWQwp8Cosy0kLz_rxiTGIZVQsrXpT7g,3386
 mcli/models/mcli_secret.py,sha256=VNtBhie1cIda7zqFQylidUcj1Y9rB7ba-7f-N183kVY,9400
-mcli/models/run_config.py,sha256=SdZngL1rKZDZEr-YAXfD7AehqNRvlkYFvay3-9RAHtE,17576
+mcli/models/run_config.py,sha256=mWCbSXEvAD7XPIbyx1h5OanTGwnRpA2vvnqNs0qJgrE,17234
 mcli/objects/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/objects/integrations/__init__.py,sha256=qf-u-HNHr7b2_VqhGwjX7Yqy7J_i_yVP7Rp2d3r5azw,660
 mcli/objects/integrations/apt_packages.py,sha256=iFuGUcJ2uR9M3powX_DgbYq-ZQ0J0CBlQ3N0eJi_o1w,671
 mcli/objects/integrations/comet.py,sha256=fa_AGggx1OcBbkRu1O6BqloU2KDsDyi585K6VesbFQk,1287
 mcli/objects/integrations/git_repo.py,sha256=HrVwQBSX3CZfMRl4tO_9axlcsQIYkl9ooDIr_niJ5Pw,2597
 mcli/objects/integrations/local.py,sha256=wawQl7-rdJ7bukjZB30W4AOXjNE4ZC7CRy4Aw3S9yfw,3491
 mcli/objects/integrations/mosaicml_agent.py,sha256=Zgpjvvu9MGwiO_ReKkcxJCIsk9DE7IsPXE7OtxdgaZo,2126
@@ -178,31 +178,31 @@
 mcli/serverside/job/mcli_k8s_job_typing.py,sha256=4wewc33SCD9WGhlsQwwhxdJcHyNUGwIfhfnD42qdonw,8090
 mcli/serverside/job/mcli_k8s_resource_requirements_typing.py,sha256=lX5t5u-uO2e6qsAiNjkizKtUQWLU9YOzHMw3lY94saw,7524
 mcli/serverside/job/mcli_k8s_service_typing.py,sha256=y2Ef7Uy1AExuvfrRa399utVCKfu7CicfGsmx1gjuuiw,459
 mcli/serverside/runners/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/serverside/runners/runner.py,sha256=XdT4OQtPdD8LZULAUKj7rSN9AhHbFe4FM1oAuxRswBs,5770
 mcli/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/utils/utils_cli.py,sha256=I6JT9W5HQLQFi6XpgZ5m83hY8zIN3_k0eMDOOWWEaaw,5306
-mcli/utils/utils_config.py,sha256=8GW1P3Wl5z0bHXC1GLiXwTdrsKqRM5zNeJerG8_3lpA,6066
+mcli/utils/utils_config.py,sha256=HLn0ZW96mdSeBtPz_knGvizZWZFxR8_3erEN-RT-We4,6073
 mcli/utils/utils_date.py,sha256=KP4zrYLT9df3zpd9bzOJsqiEHEkj9AIat0GPCksZJHE,740
 mcli/utils/utils_docker.py,sha256=VTA-kWf7TfYQejJABkh8qLA6tPi_9iv1FEUZ6HHLicA,10453
 mcli/utils/utils_epilog.py,sha256=rmROmAF1EMDTr2PoZ1yYby_9-bPR0O9ifJopSJnxDH0,12947
 mcli/utils/utils_file.py,sha256=GLfXPLC4H4R2pmRgPSXYjE5RZ1_d24aTvWZCnIgStCE,751
 mcli/utils/utils_interactive.py,sha256=98gqwb7SUq3Ssj8hPNU59y1KdEwEhxgTtpajQf9IBXc,11769
 mcli/utils/utils_kube.py,sha256=LHbdcBlaLJvZ2TC3tJyNVcCY-JzHFXUuyJg-q5az0a0,49322
 mcli/utils/utils_kube_labels.py,sha256=DzNjpvMeV_qBn4LOKZuB_Hzx0NzU_X5bE-RWmjrFfpI,6980
-mcli/utils/utils_logging.py,sha256=YWCVyusLuuh8BGkNoGzHvvLvTDbTEDZ2tGX3Hb6V_Dw,4741
+mcli/utils/utils_logging.py,sha256=pMf5z_e-ewpbXAvp0rkGqFwqmw3_rL53sbEaGUTuaWo,4832
 mcli/utils/utils_modules.py,sha256=6pdHzloArxVE6eD6xDzwmLkkVrvVMvra6s60pHofwyY,359
 mcli/utils/utils_pypi.py,sha256=oI7_LYZ01lG6OwldsFz-nOv-_lu71LHWfAgHQDPixjk,6614
 mcli/utils/utils_rancher.py,sha256=4EYHA2FMqHgvcAaT9S50HVYNToePQF-HbQL8Wm9Hllc,6513
 mcli/utils/utils_rich.py,sha256=CbQiVIzXgf6yQzIrUj2d8JZWOF2L05gHV2Fry4tHxM4,3115
 mcli/utils/utils_run_status.py,sha256=Iv5AWtF1tDsC0VK-n3W6vynNzDtvX918krhO_oFA4MQ,8533
 mcli/utils/utils_serializable_dataclass.py,sha256=m0rhTI60NpN1ET2T7VChnjZID1JpDDRuBI4A3LMRacI,4350
 mcli/utils/utils_spinner.py,sha256=NZZ0l0OJyEs-fFZSt1S3h_LiSGP4oT67HMPXATUPZtY,1103
 mcli/utils/utils_string_functions.py,sha256=Z5ouIGOf02pxxTlE_ZijZxhsSaj9p499TA7fP65Ik-0,11437
 mcli/utils/utils_types.py,sha256=EVfUa5HG0SoOo3w7A6Wh4Vqi7ojTeiEPjudFok1u-hs,3954
 mcli/utils/utils_yaml.py,sha256=O-ucRDZr5zYlALUtngFQ1E5bf-cj6Zu7OyaiUR2SgEs,1001
-mosaicml_cli-0.3.6.dist-info/METADATA,sha256=w6GgLzBAdv3H_CXsxEHw7DdWD2gdZLSBJWfIc63jYXg,4743
-mosaicml_cli-0.3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mosaicml_cli-0.3.6.dist-info/entry_points.txt,sha256=YgBbHmB6YftDcyJhavLU_Tpcn8gyZN9M1i11AGD9HPI,75
-mosaicml_cli-0.3.6.dist-info/top_level.txt,sha256=_bnO8J2EUkliWivey_1le0UrnocFKmyVMQjbQ8iVXjc,5
-mosaicml_cli-0.3.6.dist-info/RECORD,,
+mosaicml_cli-0.3.7.dist-info/METADATA,sha256=yf5VbL5y0fxPs7JwbUidWYNc80iqzn0Eo2dL8yHfoMA,4525
+mosaicml_cli-0.3.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mosaicml_cli-0.3.7.dist-info/entry_points.txt,sha256=YgBbHmB6YftDcyJhavLU_Tpcn8gyZN9M1i11AGD9HPI,75
+mosaicml_cli-0.3.7.dist-info/top_level.txt,sha256=_bnO8J2EUkliWivey_1le0UrnocFKmyVMQjbQ8iVXjc,5
+mosaicml_cli-0.3.7.dist-info/RECORD,,
```

