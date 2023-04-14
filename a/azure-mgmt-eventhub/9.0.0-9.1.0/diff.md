# Comparing `tmp/azure-mgmt-eventhub-9.0.0.zip` & `tmp/azure-mgmt-eventhub-9.1.0.zip`

## zipinfo {}

```diff
@@ -1,158 +1,198 @@
-Zip file size: 318031 bytes, number of entries: 156
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/tests/
--rw-rw-r--  2.0 unx      126 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/MANIFEST.in
--rw-rw-r--  2.0 unx    10951 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/CHANGELOG.md
--rw-rw-r--  2.0 unx      576 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/_meta.json
--rw-rw-r--  2.0 unx     3045 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/setup.py
--rw-rw-r--  2.0 unx      772 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/README.md
--rw-rw-r--  2.0 unx       67 b- defN 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/setup.cfg
--rw-rw-r--  2.0 unx    15023 b- defN 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/PKG-INFO
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/
--rw-rw-r--  2.0 unx       64 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/
--rw-rw-r--  2.0 unx       64 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/
--rw-rw-r--  2.0 unx      345 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/_version.py
--rw-rw-r--  2.0 unx     3355 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/_configuration.py
--rw-rw-r--  2.0 unx    16992 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      675 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/__init__.py
--rw-rw-r--  2.0 unx      360 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/models.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/
--rw-rw-r--  2.0 unx     3374 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/_configuration.py
--rw-rw-r--  2.0 unx     5556 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      675 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/__init__.py
--rw-rw-r--  2.0 unx     3810 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_event_hub_management_client_enums.py
--rw-rw-r--  2.0 unx    42302 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_models.py
--rw-rw-r--  2.0 unx     5297 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/__init__.py
--rw-rw-r--  2.0 unx    44792 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     4858 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_operations.py
--rw-rw-r--  2.0 unx    18074 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_consumer_groups_operations.py
--rw-rw-r--  2.0 unx     1005 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/__init__.py
--rw-rw-r--  2.0 unx    39996 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_event_hubs_operations.py
--rw-rw-r--  2.0 unx    66715 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx     5395 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_regions_operations.py
--rw-rw-r--  2.0 unx    37241 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_disaster_recovery_configs_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/
--rw-rw-r--  2.0 unx     3317 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/_configuration.py
--rw-rw-r--  2.0 unx     5531 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      574 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/__init__.py
--rw-rw-r--  2.0 unx     4798 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    17820 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_consumer_groups_operations.py
--rw-rw-r--  2.0 unx     1005 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    39498 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_event_hubs_operations.py
--rw-rw-r--  2.0 unx    66193 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx     5327 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_regions_operations.py
--rw-rw-r--  2.0 unx    36795 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_disaster_recovery_configs_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/
--rw-rw-r--  2.0 unx     3382 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/_configuration.py
--rw-rw-r--  2.0 unx     6163 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      675 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/__init__.py
--rw-rw-r--  2.0 unx     4954 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_event_hub_management_client_enums.py
--rw-rw-r--  2.0 unx    54785 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models.py
--rw-rw-r--  2.0 unx     6674 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/__init__.py
--rw-rw-r--  2.0 unx    58424 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models_py3.py
--rw-rw-r--  2.0 unx     5020 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx     4882 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_operations.py
--rw-rw-r--  2.0 unx    18146 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_consumer_groups_operations.py
--rw-rw-r--  2.0 unx    20232 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     1181 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/__init__.py
--rw-rw-r--  2.0 unx    40172 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_event_hubs_operations.py
--rw-rw-r--  2.0 unx    59957 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx    37401 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_disaster_recovery_configs_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/
--rw-rw-r--  2.0 unx     3325 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_configuration.py
--rw-rw-r--  2.0 unx     6142 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      574 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/__init__.py
--rw-rw-r--  2.0 unx     4885 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx     4822 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    17892 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_consumer_groups_operations.py
--rw-rw-r--  2.0 unx    20056 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     1181 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    39674 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_event_hubs_operations.py
--rw-rw-r--  2.0 unx    59471 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx    36955 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/
--rw-rw-r--  2.0 unx     3374 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/_configuration.py
--rw-rw-r--  2.0 unx     4856 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      675 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/__init__.py
--rw-rw-r--  2.0 unx     3099 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_event_hub_management_client_enums.py
--rw-rw-r--  2.0 unx    32411 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_models.py
--rw-rw-r--  2.0 unx     4278 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/__init__.py
--rw-rw-r--  2.0 unx    34639 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     4749 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_operations.py
--rw-rw-r--  2.0 unx    16834 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_consumer_groups_operations.py
--rw-rw-r--  2.0 unx      803 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/__init__.py
--rw-rw-r--  2.0 unx    42020 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_event_hubs_operations.py
--rw-rw-r--  2.0 unx    52377 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_namespaces_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/
--rw-rw-r--  2.0 unx     3317 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/_configuration.py
--rw-rw-r--  2.0 unx     4823 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      574 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/__init__.py
--rw-rw-r--  2.0 unx     4689 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    16592 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_consumer_groups_operations.py
--rw-rw-r--  2.0 unx      803 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    41484 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_event_hubs_operations.py
--rw-rw-r--  2.0 unx    51967 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx     3307 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/_configuration.py
--rw-rw-r--  2.0 unx    17270 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      574 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/
--rw-rw-r--  2.0 unx     3382 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/_configuration.py
--rw-rw-r--  2.0 unx     7167 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      675 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/__init__.py
--rw-rw-r--  2.0 unx     4652 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_event_hub_management_client_enums.py
--rw-rw-r--  2.0 unx    60954 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models.py
--rw-rw-r--  2.0 unx     8128 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/__init__.py
--rw-rw-r--  2.0 unx    64963 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models_py3.py
--rw-rw-r--  2.0 unx     5020 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx     4882 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_operations.py
--rw-rw-r--  2.0 unx    18146 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_consumer_groups_operations.py
--rw-rw-r--  2.0 unx     9266 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_configuration_operations.py
--rw-rw-r--  2.0 unx    20232 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     1430 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/__init__.py
--rw-rw-r--  2.0 unx    40172 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_event_hubs_operations.py
--rw-rw-r--  2.0 unx    88771 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx     5419 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_regions_operations.py
--rw-rw-r--  2.0 unx    37401 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_disaster_recovery_configs_operations.py
--rw-rw-r--  2.0 unx    33530 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_clusters_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/
--rw-rw-r--  2.0 unx     3325 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_configuration.py
--rw-rw-r--  2.0 unx     7158 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_event_hub_management_client.py
--rw-rw-r--  2.0 unx      574 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/__init__.py
--rw-rw-r--  2.0 unx     4885 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_link_resources_operations.py
--rw-rw-r--  2.0 unx     4822 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_operations.py
--rw-rw-r--  2.0 unx    17892 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_consumer_groups_operations.py
--rw-rw-r--  2.0 unx     9089 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_configuration_operations.py
--rw-rw-r--  2.0 unx    20056 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_endpoint_connections_operations.py
--rw-rw-r--  2.0 unx     1430 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    39674 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_event_hubs_operations.py
--rw-rw-r--  2.0 unx    88013 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_namespaces_operations.py
--rw-rw-r--  2.0 unx     5351 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_regions_operations.py
--rw-rw-r--  2.0 unx    36955 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
--rw-rw-r--  2.0 unx    33316 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_clusters_operations.py
--rw-rw-r--  2.0 unx        1 b- defN 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx      105 b- defN 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx     7936 b- defN 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        6 b- defN 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/top_level.txt
--rw-rw-r--  2.0 unx    15023 b- defN 21-May-26 04:44 azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     1515 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/tests/conftest.py
--rw-rw-r--  2.0 unx     1017 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/tests/_aio_testcase.py
--rw-rw-r--  2.0 unx    13903 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/tests/test_cli_mgmt_eventhub_async.py
--rw-rw-r--  2.0 unx    16485 b- defN 21-May-26 04:42 azure-mgmt-eventhub-9.0.0/tests/test_cli_mgmt_eventhub.py
-156 files, 2117625 bytes uncompressed, 280479 bytes compressed:  86.8%
+Zip file size: 412174 bytes, number of entries: 196
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/tests/
+-rw-rw-r--  2.0 unx     3045 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/setup.py
+-rw-rw-r--  2.0 unx    15422 b- defN 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/PKG-INFO
+-rw-rw-r--  2.0 unx    11270 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/CHANGELOG.md
+-rw-rw-r--  2.0 unx      772 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/README.md
+-rw-rw-r--  2.0 unx       67 b- defN 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/setup.cfg
+-rw-rw-r--  2.0 unx      576 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/_meta.json
+-rw-rw-r--  2.0 unx      126 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/MANIFEST.in
+-rw-rw-r--  2.0 unx        1 b- defN 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx    15422 b- defN 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx    10452 b- defN 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx        6 b- defN 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx      105 b- defN 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/dependency_links.txt
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/
+-rw-rw-r--  2.0 unx       64 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/
+-rw-rw-r--  2.0 unx       64 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/
+-rw-rw-r--  2.0 unx    19863 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx      360 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/models.py
+-rw-rw-r--  2.0 unx     3355 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/_configuration.py
+-rw-rw-r--  2.0 unx      675 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/__init__.py
+-rw-rw-r--  2.0 unx      345 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/_version.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/
+-rw-rw-r--  2.0 unx     6868 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3393 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/_configuration.py
+-rw-rw-r--  2.0 unx      728 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/__init__.py
+-rw-rw-r--  2.0 unx      486 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/_version.py
+-rw-rw-r--  2.0 unx    20232 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     4882 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_operations.py
+-rw-rw-r--  2.0 unx    36779 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_clusters_operations.py
+-rw-rw-r--  2.0 unx     9266 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_configuration_operations.py
+-rw-rw-r--  2.0 unx    18146 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    37401 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_disaster_recovery_configs_operations.py
+-rw-rw-r--  2.0 unx     5020 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    59957 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    40172 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx     1354 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/
+-rw-rw-r--  2.0 unx     6855 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3337 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/_configuration.py
+-rw-rw-r--  2.0 unx      574 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/__init__.py
+-rw-rw-r--  2.0 unx    20056 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     4822 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    36579 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_clusters_operations.py
+-rw-rw-r--  2.0 unx     9089 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_configuration_operations.py
+-rw-rw-r--  2.0 unx    17892 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    36955 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_disaster_recovery_configs_operations.py
+-rw-rw-r--  2.0 unx     4885 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    59471 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    39674 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx     1354 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    62054 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/_models.py
+-rw-rw-r--  2.0 unx    66230 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/_models_py3.py
+-rw-rw-r--  2.0 unx     5328 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/_event_hub_management_client_enums.py
+-rw-rw-r--  2.0 unx     7680 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/
+-rw-rw-r--  2.0 unx     6163 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3393 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/_configuration.py
+-rw-rw-r--  2.0 unx      728 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/__init__.py
+-rw-rw-r--  2.0 unx      486 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/_version.py
+-rw-rw-r--  2.0 unx    20232 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     4882 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_operations.py
+-rw-rw-r--  2.0 unx    18146 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    37401 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_disaster_recovery_configs_operations.py
+-rw-rw-r--  2.0 unx     5020 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    59957 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    40172 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx     1181 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/
+-rw-rw-r--  2.0 unx     6142 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3337 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_configuration.py
+-rw-rw-r--  2.0 unx      574 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/__init__.py
+-rw-rw-r--  2.0 unx    20056 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     4822 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    17892 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    36955 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
+-rw-rw-r--  2.0 unx     4885 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    59471 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    39674 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx     1181 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    54920 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models.py
+-rw-rw-r--  2.0 unx    58581 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models_py3.py
+-rw-rw-r--  2.0 unx     4954 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_event_hub_management_client_enums.py
+-rw-rw-r--  2.0 unx     6674 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/
+-rw-rw-r--  2.0 unx     4856 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3385 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/_configuration.py
+-rw-rw-r--  2.0 unx      728 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/__init__.py
+-rw-rw-r--  2.0 unx      486 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/_version.py
+-rw-rw-r--  2.0 unx     4749 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_operations.py
+-rw-rw-r--  2.0 unx    16834 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    52377 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    42020 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx      803 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/
+-rw-rw-r--  2.0 unx     4823 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3329 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx      574 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/__init__.py
+-rw-rw-r--  2.0 unx     4689 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    16592 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    51967 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    41484 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx      803 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    32411 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_models.py
+-rw-rw-r--  2.0 unx    34639 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3099 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_event_hub_management_client_enums.py
+-rw-rw-r--  2.0 unx     4278 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/__init__.py
+-rw-rw-r--  2.0 unx    20223 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3307 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/_configuration.py
+-rw-rw-r--  2.0 unx      574 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/
+-rw-rw-r--  2.0 unx     7167 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3393 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/_configuration.py
+-rw-rw-r--  2.0 unx      728 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/__init__.py
+-rw-rw-r--  2.0 unx      486 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/_version.py
+-rw-rw-r--  2.0 unx    20232 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     5419 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_regions_operations.py
+-rw-rw-r--  2.0 unx     4882 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_operations.py
+-rw-rw-r--  2.0 unx    33530 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_clusters_operations.py
+-rw-rw-r--  2.0 unx     9266 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_configuration_operations.py
+-rw-rw-r--  2.0 unx    18146 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    37401 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_disaster_recovery_configs_operations.py
+-rw-rw-r--  2.0 unx     5020 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    88771 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    40172 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx     1430 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/
+-rw-rw-r--  2.0 unx     7158 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3337 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_configuration.py
+-rw-rw-r--  2.0 unx      574 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/__init__.py
+-rw-rw-r--  2.0 unx    20056 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_endpoint_connections_operations.py
+-rw-rw-r--  2.0 unx     5351 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_regions_operations.py
+-rw-rw-r--  2.0 unx     4822 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    33316 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_clusters_operations.py
+-rw-rw-r--  2.0 unx     9089 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_configuration_operations.py
+-rw-rw-r--  2.0 unx    17892 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    36955 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
+-rw-rw-r--  2.0 unx     4885 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_link_resources_operations.py
+-rw-rw-r--  2.0 unx    88013 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    39674 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx     1430 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    61024 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models.py
+-rw-rw-r--  2.0 unx    65071 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models_py3.py
+-rw-rw-r--  2.0 unx     4652 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_event_hub_management_client_enums.py
+-rw-rw-r--  2.0 unx     8128 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/
+-rw-rw-r--  2.0 unx     5556 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3385 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/_configuration.py
+-rw-rw-r--  2.0 unx      728 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/__init__.py
+-rw-rw-r--  2.0 unx      486 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/_version.py
+-rw-rw-r--  2.0 unx     5395 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_regions_operations.py
+-rw-rw-r--  2.0 unx     4858 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_operations.py
+-rw-rw-r--  2.0 unx    18074 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    37241 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_disaster_recovery_configs_operations.py
+-rw-rw-r--  2.0 unx    66715 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    39996 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx     1005 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 21-Sep-18 01:37 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/
+-rw-rw-r--  2.0 unx     5531 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/_event_hub_management_client.py
+-rw-rw-r--  2.0 unx     3329 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx      574 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/__init__.py
+-rw-rw-r--  2.0 unx     5327 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_regions_operations.py
+-rw-rw-r--  2.0 unx     4798 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx    17820 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_consumer_groups_operations.py
+-rw-rw-r--  2.0 unx    36795 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_disaster_recovery_configs_operations.py
+-rw-rw-r--  2.0 unx    66193 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_namespaces_operations.py
+-rw-rw-r--  2.0 unx    39498 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_event_hubs_operations.py
+-rw-rw-r--  2.0 unx     1005 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    42302 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_models.py
+-rw-rw-r--  2.0 unx    44792 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3810 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_event_hub_management_client_enums.py
+-rw-rw-r--  2.0 unx     5297 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/__init__.py
+-rw-rw-r--  2.0 unx    13903 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/tests/test_cli_mgmt_eventhub_async.py
+-rw-rw-r--  2.0 unx     1515 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/tests/conftest.py
+-rw-rw-r--  2.0 unx     1017 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/tests/_aio_testcase.py
+-rw-rw-r--  2.0 unx    16485 b- defN 21-Sep-18 01:36 azure-mgmt-eventhub-9.1.0/tests/test_cli_mgmt_eventhub.py
+196 files, 2757319 bytes uncompressed, 364066 bytes compressed:  86.8%
```

## zipnote {}

```diff
@@ -1,469 +1,589 @@
-Filename: azure-mgmt-eventhub-9.0.0/
+Filename: azure-mgmt-eventhub-9.1.0/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/
+Filename: azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/
+Filename: azure-mgmt-eventhub-9.1.0/azure/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/tests/
+Filename: azure-mgmt-eventhub-9.1.0/tests/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/MANIFEST.in
+Filename: azure-mgmt-eventhub-9.1.0/setup.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/CHANGELOG.md
+Filename: azure-mgmt-eventhub-9.1.0/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/_meta.json
+Filename: azure-mgmt-eventhub-9.1.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/setup.py
+Filename: azure-mgmt-eventhub-9.1.0/README.md
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/README.md
+Filename: azure-mgmt-eventhub-9.1.0/setup.cfg
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/setup.cfg
+Filename: azure-mgmt-eventhub-9.1.0/_meta.json
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/PKG-INFO
+Filename: azure-mgmt-eventhub-9.1.0/MANIFEST.in
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/
+Filename: azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/
+Filename: azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/
+Filename: azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/requires.txt
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/
+Filename: azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/
+Filename: azure-mgmt-eventhub-9.1.0/azure/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/_version.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/models.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/models.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_event_hub_management_client_enums.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/_version.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_models.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_models_py3.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_consumer_groups_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_event_hubs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/_version.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_namespaces_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_regions_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_disaster_recovery_configs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_configuration_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_consumer_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_disaster_recovery_configs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_consumer_groups_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/_event_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_event_hubs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_namespaces_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_regions_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_disaster_recovery_configs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_configuration_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_consumer_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_disaster_recovery_configs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_event_hub_management_client_enums.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_event_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models_py3.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_consumer_groups_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/_event_hub_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_event_hubs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_namespaces_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_disaster_recovery_configs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/_version.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_consumer_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_consumer_groups_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_disaster_recovery_configs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_event_hubs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_event_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_namespaces_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_consumer_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_event_hub_management_client_enums.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_models.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_models_py3.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_event_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_consumer_groups_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_event_hubs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_event_hub_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_namespaces_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_consumer_groups_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/_version.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_event_hubs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_namespaces_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_consumer_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_event_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_consumer_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_event_hub_management_client_enums.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_event_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models_py3.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_models.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_event_hub_management_client_enums.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_consumer_groups_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_configuration_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_event_hubs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_namespaces_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_regions_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_disaster_recovery_configs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_clusters_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_configuration.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/_version.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_event_hub_management_client.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_regions_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_link_resources_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_consumer_groups_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_configuration_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_configuration_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_consumer_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_endpoint_connections_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_disaster_recovery_configs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/__init__.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_link_resources_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_event_hubs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_namespaces_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_namespaces_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_event_hubs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_regions_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_clusters_operations.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_event_hub_management_client.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/dependency_links.txt
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_configuration.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/requires.txt
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/__init__.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/not-zip-safe
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_endpoint_connections_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/SOURCES.txt
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_regions_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/top_level.txt
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/PKG-INFO
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_clusters_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/tests/conftest.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_configuration_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/tests/_aio_testcase.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_consumer_groups_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/tests/test_cli_mgmt_eventhub_async.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
 Comment: 
 
-Filename: azure-mgmt-eventhub-9.0.0/tests/test_cli_mgmt_eventhub.py
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_link_resources_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_namespaces_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_event_hubs_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models_py3.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_event_hub_management_client_enums.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/_event_hub_management_client.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/_configuration.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/_version.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_regions_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_consumer_groups_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_disaster_recovery_configs_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_namespaces_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_event_hubs_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/_event_hub_management_client.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/_configuration.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_regions_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_consumer_groups_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_disaster_recovery_configs_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_namespaces_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_event_hubs_operations.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_models.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_models_py3.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_event_hub_management_client_enums.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/__init__.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/tests/test_cli_mgmt_eventhub_async.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/tests/conftest.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/tests/_aio_testcase.py
+Comment: 
+
+Filename: azure-mgmt-eventhub-9.1.0/tests/test_cli_mgmt_eventhub.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-mgmt-eventhub-9.0.0/CHANGELOG.md` & `azure-mgmt-eventhub-9.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Release History
 
+## 9.1.0 (2021-09-17)
+
+**Features**
+
+  - Model Cluster has a new parameter system_data
+  - Model EHNamespace has a new parameter disable_local_auth
+  - Model EHNamespace has a new parameter status
+  - Model NetworkRuleSet has a new parameter public_network_access
+  - Added operation ClustersOperations.list_by_subscription
+
 ## 9.0.0 (2021-05-25)
 
 **Features**
 
   - Model NetworkRuleSet has a new parameter system_data
   - Model ConsumerGroup has a new parameter system_data
   - Model PrivateEndpointConnection has a new parameter system_data
@@ -45,29 +55,29 @@
 
 - Credential system has been completly revamped:
 
   - `azure.common.credentials` or `msrestazure.azure_active_directory` instances are no longer supported, use the `azure-identity` classes instead: https://pypi.org/project/azure-identity/
   - `credentials` parameter has been renamed `credential`
 
 - The `config` attribute no longer exists on a client, configuration should be passed as kwarg. Example: `MyClient(credential, subscription_id, enable_logging=True)`. For a complete set of
-  supported options, see the [parameters accept in init documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
+  supported options, see the [parameters accept in init documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
 - You can't import a `version` module anymore, use `__version__` instead
 - Operations that used to return a `msrest.polling.LROPoller` now returns a `azure.core.polling.LROPoller` and are prefixed with `begin_`.
 - Exceptions tree have been simplified and most exceptions are now `azure.core.exceptions.HttpResponseError` (`CloudError` has been removed).
 - Most of the operation kwarg have changed. Some of the most noticeable:
 
   - `raw` has been removed. Equivalent feature can be found using `cls`, a callback that will give access to internal HTTP response for advanced user
   - For a complete set of
-  supported options, see the [parameters accept in Request documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
+  supported options, see the [parameters accept in Request documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
 
 **General new features**
 
 - Type annotations support using `typing`. SDKs are mypy ready.
 - This client has now stable and official support for async. Check the `aio` namespace of your package to find the async client.
-- This client now support natively tracing library like OpenCensus or OpenTelemetry. See this [tracing quickstart](https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/core/azure-core-tracing-opentelemetry) for an overview.
+- This client now support natively tracing library like OpenCensus or OpenTelemetry. See this [tracing quickstart](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-tracing-opentelemetry) for an overview.
 
 ## 4.0.0 (2020-06-12)
 
 **Features**
 
   - Model Cluster has a new parameter updated_at
   - Model Cluster has a new parameter created_at
```

## Comparing `azure-mgmt-eventhub-9.0.0/_meta.json` & `azure-mgmt-eventhub-9.1.0/_meta.json`

 * *Files 25% similar despite different names*

### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'autorest'": "'3.4.5'",*

 * * "'autorest_command'": "'autorest specification/eventhub/resource-manager/readme.md --multiapi "*

 * *                       '--python --python-mode=update '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/s/azure-sdk-for-python/sdk --track2 '*

 * *                       '--use=@autorest/python@5.8.4 --use=@autorest/modelerfour@4.19.2 '*

 * *                       "--version=3.4.5'",*

 * * "'commit'": "'c9992af7235a6550087d4fed8f081ed35019f605'",*

 * * "'use'": "['@autorest/python@5.8.4', '@ […]*

```diff
@@ -1,11 +1,11 @@
 {
-    "autorest": "3.4.2",
-    "autorest_command": "autorest specification/eventhub/resource-manager/readme.md --multiapi --python --python-mode=update --python-sdks-folder=/home/vsts/work/1/s/azure-sdk-for-python/sdk --track2 --use=@autorest/python@5.8.0 --use=@autorest/modelerfour@4.19.1 --version=3.4.2",
-    "commit": "243dc16d38ca0f0d251efa2d216468a670cd8beb",
+    "autorest": "3.4.5",
+    "autorest_command": "autorest specification/eventhub/resource-manager/readme.md --multiapi --python --python-mode=update --python-sdks-folder=/home/vsts/work/1/s/azure-sdk-for-python/sdk --track2 --use=@autorest/python@5.8.4 --use=@autorest/modelerfour@4.19.2 --version=3.4.5",
+    "commit": "c9992af7235a6550087d4fed8f081ed35019f605",
     "readme": "specification/eventhub/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@5.8.0",
-        "@autorest/modelerfour@4.19.1"
+        "@autorest/python@5.8.4",
+        "@autorest/modelerfour@4.19.2"
     ]
 }
```

## Comparing `azure-mgmt-eventhub-9.0.0/setup.py` & `azure-mgmt-eventhub-9.1.0/setup.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/README.md` & `azure-mgmt-eventhub-9.1.0/README.md`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/PKG-INFO` & `azure-mgmt-eventhub-9.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-eventhub
-Version: 9.0.0
+Version: 9.1.0
 Summary: Microsoft Azure EventHub Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Microsoft Azure SDK for Python
         
@@ -27,14 +27,24 @@
         
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-eventhub%2FREADME.png)
         
         
         # Release History
         
+        ## 9.1.0 (2021-09-17)
+        
+        **Features**
+        
+          - Model Cluster has a new parameter system_data
+          - Model EHNamespace has a new parameter disable_local_auth
+          - Model EHNamespace has a new parameter status
+          - Model NetworkRuleSet has a new parameter public_network_access
+          - Added operation ClustersOperations.list_by_subscription
+        
         ## 9.0.0 (2021-05-25)
         
         **Features**
         
           - Model NetworkRuleSet has a new parameter system_data
           - Model ConsumerGroup has a new parameter system_data
           - Model PrivateEndpointConnection has a new parameter system_data
@@ -76,29 +86,29 @@
         
         - Credential system has been completly revamped:
         
           - `azure.common.credentials` or `msrestazure.azure_active_directory` instances are no longer supported, use the `azure-identity` classes instead: https://pypi.org/project/azure-identity/
           - `credentials` parameter has been renamed `credential`
         
         - The `config` attribute no longer exists on a client, configuration should be passed as kwarg. Example: `MyClient(credential, subscription_id, enable_logging=True)`. For a complete set of
-          supported options, see the [parameters accept in init documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
+          supported options, see the [parameters accept in init documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
         - You can't import a `version` module anymore, use `__version__` instead
         - Operations that used to return a `msrest.polling.LROPoller` now returns a `azure.core.polling.LROPoller` and are prefixed with `begin_`.
         - Exceptions tree have been simplified and most exceptions are now `azure.core.exceptions.HttpResponseError` (`CloudError` has been removed).
         - Most of the operation kwarg have changed. Some of the most noticeable:
         
           - `raw` has been removed. Equivalent feature can be found using `cls`, a callback that will give access to internal HTTP response for advanced user
           - For a complete set of
-          supported options, see the [parameters accept in Request documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
+          supported options, see the [parameters accept in Request documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
         
         **General new features**
         
         - Type annotations support using `typing`. SDKs are mypy ready.
         - This client has now stable and official support for async. Check the `aio` namespace of your package to find the async client.
-        - This client now support natively tracing library like OpenCensus or OpenTelemetry. See this [tracing quickstart](https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/core/azure-core-tracing-opentelemetry) for an overview.
+        - This client now support natively tracing library like OpenCensus or OpenTelemetry. See this [tracing quickstart](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-tracing-opentelemetry) for an overview.
         
         ## 4.0.0 (2020-06-12)
         
         **Features**
         
           - Model Cluster has a new parameter updated_at
           - Model Cluster has a new parameter created_at
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/_event_hub_management_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -91,190 +91,221 @@
     def models(cls, api_version=DEFAULT_API_VERSION):
         """Module depends on the API version:
 
            * 2015-08-01: :mod:`v2015_08_01.models<azure.mgmt.eventhub.v2015_08_01.models>`
            * 2017-04-01: :mod:`v2017_04_01.models<azure.mgmt.eventhub.v2017_04_01.models>`
            * 2018-01-01-preview: :mod:`v2018_01_01_preview.models<azure.mgmt.eventhub.v2018_01_01_preview.models>`
            * 2021-01-01-preview: :mod:`v2021_01_01_preview.models<azure.mgmt.eventhub.v2021_01_01_preview.models>`
+           * 2021-06-01-preview: :mod:`v2021_06_01_preview.models<azure.mgmt.eventhub.v2021_06_01_preview.models>`
         """
         if api_version == '2015-08-01':
             from .v2015_08_01 import models
             return models
         elif api_version == '2017-04-01':
             from .v2017_04_01 import models
             return models
         elif api_version == '2018-01-01-preview':
             from .v2018_01_01_preview import models
             return models
         elif api_version == '2021-01-01-preview':
             from .v2021_01_01_preview import models
             return models
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview import models
+            return models
         raise ValueError("API version {} is not available".format(api_version))
 
     @property
     def clusters(self):
         """Instance depends on the API version:
 
            * 2018-01-01-preview: :class:`ClustersOperations<azure.mgmt.eventhub.v2018_01_01_preview.operations.ClustersOperations>`
+           * 2021-06-01-preview: :class:`ClustersOperations<azure.mgmt.eventhub.v2021_06_01_preview.operations.ClustersOperations>`
         """
         api_version = self._get_api_version('clusters')
         if api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import ClustersOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import ClustersOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'clusters'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def configuration(self):
         """Instance depends on the API version:
 
            * 2018-01-01-preview: :class:`ConfigurationOperations<azure.mgmt.eventhub.v2018_01_01_preview.operations.ConfigurationOperations>`
+           * 2021-06-01-preview: :class:`ConfigurationOperations<azure.mgmt.eventhub.v2021_06_01_preview.operations.ConfigurationOperations>`
         """
         api_version = self._get_api_version('configuration')
         if api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import ConfigurationOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import ConfigurationOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'configuration'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def consumer_groups(self):
         """Instance depends on the API version:
 
            * 2015-08-01: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2015_08_01.operations.ConsumerGroupsOperations>`
            * 2017-04-01: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2017_04_01.operations.ConsumerGroupsOperations>`
            * 2018-01-01-preview: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2018_01_01_preview.operations.ConsumerGroupsOperations>`
            * 2021-01-01-preview: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2021_01_01_preview.operations.ConsumerGroupsOperations>`
+           * 2021-06-01-preview: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2021_06_01_preview.operations.ConsumerGroupsOperations>`
         """
         api_version = self._get_api_version('consumer_groups')
         if api_version == '2015-08-01':
             from .v2015_08_01.operations import ConsumerGroupsOperations as OperationClass
         elif api_version == '2017-04-01':
             from .v2017_04_01.operations import ConsumerGroupsOperations as OperationClass
         elif api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import ConsumerGroupsOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from .v2021_01_01_preview.operations import ConsumerGroupsOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import ConsumerGroupsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'consumer_groups'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def disaster_recovery_configs(self):
         """Instance depends on the API version:
 
            * 2017-04-01: :class:`DisasterRecoveryConfigsOperations<azure.mgmt.eventhub.v2017_04_01.operations.DisasterRecoveryConfigsOperations>`
            * 2018-01-01-preview: :class:`DisasterRecoveryConfigsOperations<azure.mgmt.eventhub.v2018_01_01_preview.operations.DisasterRecoveryConfigsOperations>`
            * 2021-01-01-preview: :class:`DisasterRecoveryConfigsOperations<azure.mgmt.eventhub.v2021_01_01_preview.operations.DisasterRecoveryConfigsOperations>`
+           * 2021-06-01-preview: :class:`DisasterRecoveryConfigsOperations<azure.mgmt.eventhub.v2021_06_01_preview.operations.DisasterRecoveryConfigsOperations>`
         """
         api_version = self._get_api_version('disaster_recovery_configs')
         if api_version == '2017-04-01':
             from .v2017_04_01.operations import DisasterRecoveryConfigsOperations as OperationClass
         elif api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import DisasterRecoveryConfigsOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from .v2021_01_01_preview.operations import DisasterRecoveryConfigsOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import DisasterRecoveryConfigsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'disaster_recovery_configs'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def event_hubs(self):
         """Instance depends on the API version:
 
            * 2015-08-01: :class:`EventHubsOperations<azure.mgmt.eventhub.v2015_08_01.operations.EventHubsOperations>`
            * 2017-04-01: :class:`EventHubsOperations<azure.mgmt.eventhub.v2017_04_01.operations.EventHubsOperations>`
            * 2018-01-01-preview: :class:`EventHubsOperations<azure.mgmt.eventhub.v2018_01_01_preview.operations.EventHubsOperations>`
            * 2021-01-01-preview: :class:`EventHubsOperations<azure.mgmt.eventhub.v2021_01_01_preview.operations.EventHubsOperations>`
+           * 2021-06-01-preview: :class:`EventHubsOperations<azure.mgmt.eventhub.v2021_06_01_preview.operations.EventHubsOperations>`
         """
         api_version = self._get_api_version('event_hubs')
         if api_version == '2015-08-01':
             from .v2015_08_01.operations import EventHubsOperations as OperationClass
         elif api_version == '2017-04-01':
             from .v2017_04_01.operations import EventHubsOperations as OperationClass
         elif api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import EventHubsOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from .v2021_01_01_preview.operations import EventHubsOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import EventHubsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'event_hubs'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def namespaces(self):
         """Instance depends on the API version:
 
            * 2015-08-01: :class:`NamespacesOperations<azure.mgmt.eventhub.v2015_08_01.operations.NamespacesOperations>`
            * 2017-04-01: :class:`NamespacesOperations<azure.mgmt.eventhub.v2017_04_01.operations.NamespacesOperations>`
            * 2018-01-01-preview: :class:`NamespacesOperations<azure.mgmt.eventhub.v2018_01_01_preview.operations.NamespacesOperations>`
            * 2021-01-01-preview: :class:`NamespacesOperations<azure.mgmt.eventhub.v2021_01_01_preview.operations.NamespacesOperations>`
+           * 2021-06-01-preview: :class:`NamespacesOperations<azure.mgmt.eventhub.v2021_06_01_preview.operations.NamespacesOperations>`
         """
         api_version = self._get_api_version('namespaces')
         if api_version == '2015-08-01':
             from .v2015_08_01.operations import NamespacesOperations as OperationClass
         elif api_version == '2017-04-01':
             from .v2017_04_01.operations import NamespacesOperations as OperationClass
         elif api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import NamespacesOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from .v2021_01_01_preview.operations import NamespacesOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import NamespacesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'namespaces'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def operations(self):
         """Instance depends on the API version:
 
            * 2015-08-01: :class:`Operations<azure.mgmt.eventhub.v2015_08_01.operations.Operations>`
            * 2017-04-01: :class:`Operations<azure.mgmt.eventhub.v2017_04_01.operations.Operations>`
            * 2018-01-01-preview: :class:`Operations<azure.mgmt.eventhub.v2018_01_01_preview.operations.Operations>`
            * 2021-01-01-preview: :class:`Operations<azure.mgmt.eventhub.v2021_01_01_preview.operations.Operations>`
+           * 2021-06-01-preview: :class:`Operations<azure.mgmt.eventhub.v2021_06_01_preview.operations.Operations>`
         """
         api_version = self._get_api_version('operations')
         if api_version == '2015-08-01':
             from .v2015_08_01.operations import Operations as OperationClass
         elif api_version == '2017-04-01':
             from .v2017_04_01.operations import Operations as OperationClass
         elif api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import Operations as OperationClass
         elif api_version == '2021-01-01-preview':
             from .v2021_01_01_preview.operations import Operations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import Operations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'operations'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def private_endpoint_connections(self):
         """Instance depends on the API version:
 
            * 2018-01-01-preview: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.eventhub.v2018_01_01_preview.operations.PrivateEndpointConnectionsOperations>`
            * 2021-01-01-preview: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.eventhub.v2021_01_01_preview.operations.PrivateEndpointConnectionsOperations>`
+           * 2021-06-01-preview: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.eventhub.v2021_06_01_preview.operations.PrivateEndpointConnectionsOperations>`
         """
         api_version = self._get_api_version('private_endpoint_connections')
         if api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import PrivateEndpointConnectionsOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from .v2021_01_01_preview.operations import PrivateEndpointConnectionsOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import PrivateEndpointConnectionsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'private_endpoint_connections'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def private_link_resources(self):
         """Instance depends on the API version:
 
            * 2018-01-01-preview: :class:`PrivateLinkResourcesOperations<azure.mgmt.eventhub.v2018_01_01_preview.operations.PrivateLinkResourcesOperations>`
            * 2021-01-01-preview: :class:`PrivateLinkResourcesOperations<azure.mgmt.eventhub.v2021_01_01_preview.operations.PrivateLinkResourcesOperations>`
+           * 2021-06-01-preview: :class:`PrivateLinkResourcesOperations<azure.mgmt.eventhub.v2021_06_01_preview.operations.PrivateLinkResourcesOperations>`
         """
         api_version = self._get_api_version('private_link_resources')
         if api_version == '2018-01-01-preview':
             from .v2018_01_01_preview.operations import PrivateLinkResourcesOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from .v2021_01_01_preview.operations import PrivateLinkResourcesOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from .v2021_06_01_preview.operations import PrivateLinkResourcesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'private_link_resources'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def regions(self):
         """Instance depends on the API version:
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 from typing import TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy
 
+from ._version import VERSION
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any
 
     from azure.core.credentials import TokenCredential
 
-VERSION = "unknown"
 
 class EventHubManagementClientConfiguration(Configuration):
     """Configuration for EventHubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
@@ -43,15 +44,15 @@
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
         super(EventHubManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2017-04-01"
+        self.api_version = "2021-06-01-preview"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-eventhub/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs  # type: Any
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/_event_hub_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._event_hub_management_client import EventHubManagementClient
+from ._version import VERSION
+
+__version__ = VERSION
 __all__ = ['EventHubManagementClient']
 
 try:
     from ._patch import patch_sdk  # type: ignore
     patch_sdk()
 except ImportError:
     pass
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_event_hub_management_client_enums.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_event_hub_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_models.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/models/_models_py3.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_consumer_groups_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_consumer_groups_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_event_hubs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_event_hubs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_namespaces_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_namespaces_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_regions_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_regions_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/operations/_disaster_recovery_configs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/operations/_disaster_recovery_configs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy
 
+from .._version import VERSION
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
-VERSION = "unknown"
 
 class EventHubManagementClientConfiguration(Configuration):
     """Configuration for EventHubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/_event_hub_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_consumer_groups_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_consumer_groups_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_event_hubs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_event_hubs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_namespaces_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_namespaces_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_regions_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_regions_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_disaster_recovery_configs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2017_04_01/aio/operations/_disaster_recovery_configs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 from typing import TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy
 
+from ._version import VERSION
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any
 
     from azure.core.credentials import TokenCredential
 
-VERSION = "unknown"
 
 class EventHubManagementClientConfiguration(Configuration):
     """Configuration for EventHubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/_event_hub_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._event_hub_management_client import EventHubManagementClient
+from ._version import VERSION
+
+__version__ = VERSION
 __all__ = ['EventHubManagementClient']
 
 try:
     from ._patch import patch_sdk  # type: ignore
     patch_sdk()
 except ImportError:
     pass
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_event_hub_management_client_enums.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_event_hub_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -602,14 +602,16 @@
     :type sku: ~azure.mgmt.eventhub.v2021_01_01_preview.models.Sku
     :param identity: Properties of BYOK Identity description.
     :type identity: ~azure.mgmt.eventhub.v2021_01_01_preview.models.Identity
     :ivar system_data: The system meta data relating to this resource.
     :vartype system_data: ~azure.mgmt.eventhub.v2021_01_01_preview.models.SystemData
     :ivar provisioning_state: Provisioning state of the Namespace.
     :vartype provisioning_state: str
+    :ivar status: Status of the Namespace.
+    :vartype status: str
     :ivar created_at: The time the Namespace was created.
     :vartype created_at: ~datetime.datetime
     :ivar updated_at: The time the Namespace was updated.
     :vartype updated_at: ~datetime.datetime
     :ivar service_bus_endpoint: Endpoint you can use to perform Service Bus operations.
     :vartype service_bus_endpoint: str
     :param cluster_arm_id: Cluster ARM ID of the Namespace.
@@ -636,14 +638,15 @@
 
     _validation = {
         'id': {'readonly': True},
         'name': {'readonly': True},
         'type': {'readonly': True},
         'system_data': {'readonly': True},
         'provisioning_state': {'readonly': True},
+        'status': {'readonly': True},
         'created_at': {'readonly': True},
         'updated_at': {'readonly': True},
         'service_bus_endpoint': {'readonly': True},
         'metric_id': {'readonly': True},
         'maximum_throughput_units': {'maximum': 20, 'minimum': 0},
     }
 
@@ -653,14 +656,15 @@
         'type': {'key': 'type', 'type': 'str'},
         'location': {'key': 'location', 'type': 'str'},
         'tags': {'key': 'tags', 'type': '{str}'},
         'sku': {'key': 'sku', 'type': 'Sku'},
         'identity': {'key': 'identity', 'type': 'Identity'},
         'system_data': {'key': 'systemData', 'type': 'SystemData'},
         'provisioning_state': {'key': 'properties.provisioningState', 'type': 'str'},
+        'status': {'key': 'properties.status', 'type': 'str'},
         'created_at': {'key': 'properties.createdAt', 'type': 'iso-8601'},
         'updated_at': {'key': 'properties.updatedAt', 'type': 'iso-8601'},
         'service_bus_endpoint': {'key': 'properties.serviceBusEndpoint', 'type': 'str'},
         'cluster_arm_id': {'key': 'properties.clusterArmId', 'type': 'str'},
         'metric_id': {'key': 'properties.metricId', 'type': 'str'},
         'is_auto_inflate_enabled': {'key': 'properties.isAutoInflateEnabled', 'type': 'bool'},
         'maximum_throughput_units': {'key': 'properties.maximumThroughputUnits', 'type': 'int'},
@@ -675,14 +679,15 @@
         **kwargs
     ):
         super(EHNamespace, self).__init__(**kwargs)
         self.sku = kwargs.get('sku', None)
         self.identity = kwargs.get('identity', None)
         self.system_data = None
         self.provisioning_state = None
+        self.status = None
         self.created_at = None
         self.updated_at = None
         self.service_bus_endpoint = None
         self.cluster_arm_id = kwargs.get('cluster_arm_id', None)
         self.metric_id = None
         self.is_auto_inflate_enabled = kwargs.get('is_auto_inflate_enabled', None)
         self.maximum_throughput_units = kwargs.get('maximum_throughput_units', None)
@@ -715,44 +720,38 @@
         self.value = kwargs.get('value', None)
         self.next_link = kwargs.get('next_link', None)
 
 
 class Encryption(msrest.serialization.Model):
     """Properties to configure Encryption.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     :param key_vault_properties: Properties of KeyVault.
     :type key_vault_properties:
      list[~azure.mgmt.eventhub.v2021_01_01_preview.models.KeyVaultProperties]
-    :ivar key_source: Enumerates the possible value of keySource for Encryption. Default value:
+    :param key_source: Enumerates the possible value of keySource for Encryption. The only
+     acceptable values to pass in are None and "Microsoft.KeyVault". The default value is
      "Microsoft.KeyVault".
-    :vartype key_source: str
+    :type key_source: str
     :param require_infrastructure_encryption: Enable Infrastructure Encryption (Double Encryption).
     :type require_infrastructure_encryption: bool
     """
 
-    _validation = {
-        'key_source': {'constant': True},
-    }
-
     _attribute_map = {
         'key_vault_properties': {'key': 'keyVaultProperties', 'type': '[KeyVaultProperties]'},
         'key_source': {'key': 'keySource', 'type': 'str'},
         'require_infrastructure_encryption': {'key': 'requireInfrastructureEncryption', 'type': 'bool'},
     }
 
-    key_source = "Microsoft.KeyVault"
-
     def __init__(
         self,
         **kwargs
     ):
         super(Encryption, self).__init__(**kwargs)
         self.key_vault_properties = kwargs.get('key_vault_properties', None)
+        self.key_source = kwargs.get('key_source', "Microsoft.KeyVault")
         self.require_infrastructure_encryption = kwargs.get('require_infrastructure_encryption', None)
 
 
 class ErrorResponse(msrest.serialization.Model):
     """Error response indicates Event Hub service is not able to process the incoming request. The reason is provided in the error message.
 
     :param code: Error code.
@@ -1344,15 +1343,15 @@
      should be 0 to 20 throughput units. The Event Hubs premium units for Premium tier, where value
      should be 0 to 10 premium units.
     :type capacity: int
     """
 
     _validation = {
         'name': {'required': True},
-        'capacity': {'maximum': 20, 'minimum': 0},
+        'capacity': {'minimum': 0},
     }
 
     _attribute_map = {
         'name': {'key': 'name', 'type': 'str'},
         'tier': {'key': 'tier', 'type': 'str'},
         'capacity': {'key': 'capacity', 'type': 'int'},
     }
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models_py3.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/models/_models_py3.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,14 +645,16 @@
     :type sku: ~azure.mgmt.eventhub.v2021_01_01_preview.models.Sku
     :param identity: Properties of BYOK Identity description.
     :type identity: ~azure.mgmt.eventhub.v2021_01_01_preview.models.Identity
     :ivar system_data: The system meta data relating to this resource.
     :vartype system_data: ~azure.mgmt.eventhub.v2021_01_01_preview.models.SystemData
     :ivar provisioning_state: Provisioning state of the Namespace.
     :vartype provisioning_state: str
+    :ivar status: Status of the Namespace.
+    :vartype status: str
     :ivar created_at: The time the Namespace was created.
     :vartype created_at: ~datetime.datetime
     :ivar updated_at: The time the Namespace was updated.
     :vartype updated_at: ~datetime.datetime
     :ivar service_bus_endpoint: Endpoint you can use to perform Service Bus operations.
     :vartype service_bus_endpoint: str
     :param cluster_arm_id: Cluster ARM ID of the Namespace.
@@ -679,14 +681,15 @@
 
     _validation = {
         'id': {'readonly': True},
         'name': {'readonly': True},
         'type': {'readonly': True},
         'system_data': {'readonly': True},
         'provisioning_state': {'readonly': True},
+        'status': {'readonly': True},
         'created_at': {'readonly': True},
         'updated_at': {'readonly': True},
         'service_bus_endpoint': {'readonly': True},
         'metric_id': {'readonly': True},
         'maximum_throughput_units': {'maximum': 20, 'minimum': 0},
     }
 
@@ -696,14 +699,15 @@
         'type': {'key': 'type', 'type': 'str'},
         'location': {'key': 'location', 'type': 'str'},
         'tags': {'key': 'tags', 'type': '{str}'},
         'sku': {'key': 'sku', 'type': 'Sku'},
         'identity': {'key': 'identity', 'type': 'Identity'},
         'system_data': {'key': 'systemData', 'type': 'SystemData'},
         'provisioning_state': {'key': 'properties.provisioningState', 'type': 'str'},
+        'status': {'key': 'properties.status', 'type': 'str'},
         'created_at': {'key': 'properties.createdAt', 'type': 'iso-8601'},
         'updated_at': {'key': 'properties.updatedAt', 'type': 'iso-8601'},
         'service_bus_endpoint': {'key': 'properties.serviceBusEndpoint', 'type': 'str'},
         'cluster_arm_id': {'key': 'properties.clusterArmId', 'type': 'str'},
         'metric_id': {'key': 'properties.metricId', 'type': 'str'},
         'is_auto_inflate_enabled': {'key': 'properties.isAutoInflateEnabled', 'type': 'bool'},
         'maximum_throughput_units': {'key': 'properties.maximumThroughputUnits', 'type': 'int'},
@@ -730,14 +734,15 @@
         **kwargs
     ):
         super(EHNamespace, self).__init__(location=location, tags=tags, **kwargs)
         self.sku = sku
         self.identity = identity
         self.system_data = None
         self.provisioning_state = None
+        self.status = None
         self.created_at = None
         self.updated_at = None
         self.service_bus_endpoint = None
         self.cluster_arm_id = cluster_arm_id
         self.metric_id = None
         self.is_auto_inflate_enabled = is_auto_inflate_enabled
         self.maximum_throughput_units = maximum_throughput_units
@@ -773,47 +778,42 @@
         self.value = value
         self.next_link = next_link
 
 
 class Encryption(msrest.serialization.Model):
     """Properties to configure Encryption.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     :param key_vault_properties: Properties of KeyVault.
     :type key_vault_properties:
      list[~azure.mgmt.eventhub.v2021_01_01_preview.models.KeyVaultProperties]
-    :ivar key_source: Enumerates the possible value of keySource for Encryption. Default value:
+    :param key_source: Enumerates the possible value of keySource for Encryption. The only
+     acceptable values to pass in are None and "Microsoft.KeyVault". The default value is
      "Microsoft.KeyVault".
-    :vartype key_source: str
+    :type key_source: str
     :param require_infrastructure_encryption: Enable Infrastructure Encryption (Double Encryption).
     :type require_infrastructure_encryption: bool
     """
 
-    _validation = {
-        'key_source': {'constant': True},
-    }
-
     _attribute_map = {
         'key_vault_properties': {'key': 'keyVaultProperties', 'type': '[KeyVaultProperties]'},
         'key_source': {'key': 'keySource', 'type': 'str'},
         'require_infrastructure_encryption': {'key': 'requireInfrastructureEncryption', 'type': 'bool'},
     }
 
-    key_source = "Microsoft.KeyVault"
-
     def __init__(
         self,
         *,
         key_vault_properties: Optional[List["KeyVaultProperties"]] = None,
+        key_source: Optional[str] = "Microsoft.KeyVault",
         require_infrastructure_encryption: Optional[bool] = None,
         **kwargs
     ):
         super(Encryption, self).__init__(**kwargs)
         self.key_vault_properties = key_vault_properties
+        self.key_source = key_source
         self.require_infrastructure_encryption = require_infrastructure_encryption
 
 
 class ErrorResponse(msrest.serialization.Model):
     """Error response indicates Event Hub service is not able to process the incoming request. The reason is provided in the error message.
 
     :param code: Error code.
@@ -1459,15 +1459,15 @@
      should be 0 to 20 throughput units. The Event Hubs premium units for Premium tier, where value
      should be 0 to 10 premium units.
     :type capacity: int
     """
 
     _validation = {
         'name': {'required': True},
-        'capacity': {'maximum': 20, 'minimum': 0},
+        'capacity': {'minimum': 0},
     }
 
     _attribute_map = {
         'name': {'key': 'name', 'type': 'str'},
         'tier': {'key': 'tier', 'type': 'str'},
         'capacity': {'key': 'capacity', 'type': 'int'},
     }
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_link_resources_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_consumer_groups_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_consumer_groups_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_event_hubs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_event_hubs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_namespaces_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_namespaces_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_disaster_recovery_configs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/operations/_disaster_recovery_configs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_06_01_preview/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy
 
+from .._version import VERSION
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
-VERSION = "unknown"
 
 class EventHubManagementClientConfiguration(Configuration):
     """Configuration for EventHubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
@@ -40,15 +41,15 @@
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
         super(EventHubManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2021-01-01-preview"
+        self.api_version = "2021-06-01-preview"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-eventhub/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs: Any
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/_event_hub_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_consumer_groups_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_consumer_groups_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_event_hubs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_event_hubs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_namespaces_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_namespaces_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 from typing import TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy
 
+from ._version import VERSION
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any
 
     from azure.core.credentials import TokenCredential
 
-VERSION = "unknown"
 
 class EventHubManagementClientConfiguration(Configuration):
     """Configuration for EventHubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
@@ -43,15 +44,15 @@
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
         super(EventHubManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2015-08-01"
+        self.api_version = "2018-01-01-preview"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-eventhub/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs  # type: Any
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/_event_hub_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._event_hub_management_client import EventHubManagementClient
+from ._version import VERSION
+
+__version__ = VERSION
 __all__ = ['EventHubManagementClient']
 
 try:
     from ._patch import patch_sdk  # type: ignore
     patch_sdk()
 except ImportError:
     pass
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_event_hub_management_client_enums.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_event_hub_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_models.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/models/_models_py3.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_consumer_groups_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_consumer_groups_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_event_hubs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_event_hubs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/operations/_namespaces_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/operations/_namespaces_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy
 
+from .._version import VERSION
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
-VERSION = "unknown"
 
 class EventHubManagementClientConfiguration(Configuration):
     """Configuration for EventHubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/_event_hub_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_consumer_groups_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_consumer_groups_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_event_hubs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_event_hubs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_namespaces_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/aio/operations/_namespaces_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/_event_hub_management_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,190 +89,221 @@
     def models(cls, api_version=DEFAULT_API_VERSION):
         """Module depends on the API version:
 
            * 2015-08-01: :mod:`v2015_08_01.models<azure.mgmt.eventhub.v2015_08_01.models>`
            * 2017-04-01: :mod:`v2017_04_01.models<azure.mgmt.eventhub.v2017_04_01.models>`
            * 2018-01-01-preview: :mod:`v2018_01_01_preview.models<azure.mgmt.eventhub.v2018_01_01_preview.models>`
            * 2021-01-01-preview: :mod:`v2021_01_01_preview.models<azure.mgmt.eventhub.v2021_01_01_preview.models>`
+           * 2021-06-01-preview: :mod:`v2021_06_01_preview.models<azure.mgmt.eventhub.v2021_06_01_preview.models>`
         """
         if api_version == '2015-08-01':
             from ..v2015_08_01 import models
             return models
         elif api_version == '2017-04-01':
             from ..v2017_04_01 import models
             return models
         elif api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview import models
             return models
         elif api_version == '2021-01-01-preview':
             from ..v2021_01_01_preview import models
             return models
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview import models
+            return models
         raise ValueError("API version {} is not available".format(api_version))
 
     @property
     def clusters(self):
         """Instance depends on the API version:
 
            * 2018-01-01-preview: :class:`ClustersOperations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.ClustersOperations>`
+           * 2021-06-01-preview: :class:`ClustersOperations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.ClustersOperations>`
         """
         api_version = self._get_api_version('clusters')
         if api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import ClustersOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import ClustersOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'clusters'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def configuration(self):
         """Instance depends on the API version:
 
            * 2018-01-01-preview: :class:`ConfigurationOperations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.ConfigurationOperations>`
+           * 2021-06-01-preview: :class:`ConfigurationOperations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.ConfigurationOperations>`
         """
         api_version = self._get_api_version('configuration')
         if api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import ConfigurationOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import ConfigurationOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'configuration'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def consumer_groups(self):
         """Instance depends on the API version:
 
            * 2015-08-01: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2015_08_01.aio.operations.ConsumerGroupsOperations>`
            * 2017-04-01: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2017_04_01.aio.operations.ConsumerGroupsOperations>`
            * 2018-01-01-preview: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.ConsumerGroupsOperations>`
            * 2021-01-01-preview: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2021_01_01_preview.aio.operations.ConsumerGroupsOperations>`
+           * 2021-06-01-preview: :class:`ConsumerGroupsOperations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.ConsumerGroupsOperations>`
         """
         api_version = self._get_api_version('consumer_groups')
         if api_version == '2015-08-01':
             from ..v2015_08_01.aio.operations import ConsumerGroupsOperations as OperationClass
         elif api_version == '2017-04-01':
             from ..v2017_04_01.aio.operations import ConsumerGroupsOperations as OperationClass
         elif api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import ConsumerGroupsOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from ..v2021_01_01_preview.aio.operations import ConsumerGroupsOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import ConsumerGroupsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'consumer_groups'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def disaster_recovery_configs(self):
         """Instance depends on the API version:
 
            * 2017-04-01: :class:`DisasterRecoveryConfigsOperations<azure.mgmt.eventhub.v2017_04_01.aio.operations.DisasterRecoveryConfigsOperations>`
            * 2018-01-01-preview: :class:`DisasterRecoveryConfigsOperations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.DisasterRecoveryConfigsOperations>`
            * 2021-01-01-preview: :class:`DisasterRecoveryConfigsOperations<azure.mgmt.eventhub.v2021_01_01_preview.aio.operations.DisasterRecoveryConfigsOperations>`
+           * 2021-06-01-preview: :class:`DisasterRecoveryConfigsOperations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.DisasterRecoveryConfigsOperations>`
         """
         api_version = self._get_api_version('disaster_recovery_configs')
         if api_version == '2017-04-01':
             from ..v2017_04_01.aio.operations import DisasterRecoveryConfigsOperations as OperationClass
         elif api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import DisasterRecoveryConfigsOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from ..v2021_01_01_preview.aio.operations import DisasterRecoveryConfigsOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import DisasterRecoveryConfigsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'disaster_recovery_configs'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def event_hubs(self):
         """Instance depends on the API version:
 
            * 2015-08-01: :class:`EventHubsOperations<azure.mgmt.eventhub.v2015_08_01.aio.operations.EventHubsOperations>`
            * 2017-04-01: :class:`EventHubsOperations<azure.mgmt.eventhub.v2017_04_01.aio.operations.EventHubsOperations>`
            * 2018-01-01-preview: :class:`EventHubsOperations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.EventHubsOperations>`
            * 2021-01-01-preview: :class:`EventHubsOperations<azure.mgmt.eventhub.v2021_01_01_preview.aio.operations.EventHubsOperations>`
+           * 2021-06-01-preview: :class:`EventHubsOperations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.EventHubsOperations>`
         """
         api_version = self._get_api_version('event_hubs')
         if api_version == '2015-08-01':
             from ..v2015_08_01.aio.operations import EventHubsOperations as OperationClass
         elif api_version == '2017-04-01':
             from ..v2017_04_01.aio.operations import EventHubsOperations as OperationClass
         elif api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import EventHubsOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from ..v2021_01_01_preview.aio.operations import EventHubsOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import EventHubsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'event_hubs'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def namespaces(self):
         """Instance depends on the API version:
 
            * 2015-08-01: :class:`NamespacesOperations<azure.mgmt.eventhub.v2015_08_01.aio.operations.NamespacesOperations>`
            * 2017-04-01: :class:`NamespacesOperations<azure.mgmt.eventhub.v2017_04_01.aio.operations.NamespacesOperations>`
            * 2018-01-01-preview: :class:`NamespacesOperations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.NamespacesOperations>`
            * 2021-01-01-preview: :class:`NamespacesOperations<azure.mgmt.eventhub.v2021_01_01_preview.aio.operations.NamespacesOperations>`
+           * 2021-06-01-preview: :class:`NamespacesOperations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.NamespacesOperations>`
         """
         api_version = self._get_api_version('namespaces')
         if api_version == '2015-08-01':
             from ..v2015_08_01.aio.operations import NamespacesOperations as OperationClass
         elif api_version == '2017-04-01':
             from ..v2017_04_01.aio.operations import NamespacesOperations as OperationClass
         elif api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import NamespacesOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from ..v2021_01_01_preview.aio.operations import NamespacesOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import NamespacesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'namespaces'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def operations(self):
         """Instance depends on the API version:
 
            * 2015-08-01: :class:`Operations<azure.mgmt.eventhub.v2015_08_01.aio.operations.Operations>`
            * 2017-04-01: :class:`Operations<azure.mgmt.eventhub.v2017_04_01.aio.operations.Operations>`
            * 2018-01-01-preview: :class:`Operations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.Operations>`
            * 2021-01-01-preview: :class:`Operations<azure.mgmt.eventhub.v2021_01_01_preview.aio.operations.Operations>`
+           * 2021-06-01-preview: :class:`Operations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.Operations>`
         """
         api_version = self._get_api_version('operations')
         if api_version == '2015-08-01':
             from ..v2015_08_01.aio.operations import Operations as OperationClass
         elif api_version == '2017-04-01':
             from ..v2017_04_01.aio.operations import Operations as OperationClass
         elif api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import Operations as OperationClass
         elif api_version == '2021-01-01-preview':
             from ..v2021_01_01_preview.aio.operations import Operations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import Operations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'operations'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def private_endpoint_connections(self):
         """Instance depends on the API version:
 
            * 2018-01-01-preview: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.PrivateEndpointConnectionsOperations>`
            * 2021-01-01-preview: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.eventhub.v2021_01_01_preview.aio.operations.PrivateEndpointConnectionsOperations>`
+           * 2021-06-01-preview: :class:`PrivateEndpointConnectionsOperations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.PrivateEndpointConnectionsOperations>`
         """
         api_version = self._get_api_version('private_endpoint_connections')
         if api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import PrivateEndpointConnectionsOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from ..v2021_01_01_preview.aio.operations import PrivateEndpointConnectionsOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import PrivateEndpointConnectionsOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'private_endpoint_connections'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def private_link_resources(self):
         """Instance depends on the API version:
 
            * 2018-01-01-preview: :class:`PrivateLinkResourcesOperations<azure.mgmt.eventhub.v2018_01_01_preview.aio.operations.PrivateLinkResourcesOperations>`
            * 2021-01-01-preview: :class:`PrivateLinkResourcesOperations<azure.mgmt.eventhub.v2021_01_01_preview.aio.operations.PrivateLinkResourcesOperations>`
+           * 2021-06-01-preview: :class:`PrivateLinkResourcesOperations<azure.mgmt.eventhub.v2021_06_01_preview.aio.operations.PrivateLinkResourcesOperations>`
         """
         api_version = self._get_api_version('private_link_resources')
         if api_version == '2018-01-01-preview':
             from ..v2018_01_01_preview.aio.operations import PrivateLinkResourcesOperations as OperationClass
         elif api_version == '2021-01-01-preview':
             from ..v2021_01_01_preview.aio.operations import PrivateLinkResourcesOperations as OperationClass
+        elif api_version == '2021-06-01-preview':
+            from ..v2021_06_01_preview.aio.operations import PrivateLinkResourcesOperations as OperationClass
         else:
             raise ValueError("API version {} does not have operation group 'private_link_resources'".format(api_version))
         return OperationClass(self._client, self._config, Serializer(self._models_dict(api_version)), Deserializer(self._models_dict(api_version)))
 
     @property
     def regions(self):
         """Instance depends on the API version:
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/aio/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2015_08_01/_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 from typing import TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy
 
+from ._version import VERSION
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from typing import Any
 
     from azure.core.credentials import TokenCredential
 
-VERSION = "unknown"
 
 class EventHubManagementClientConfiguration(Configuration):
     """Configuration for EventHubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
@@ -43,15 +44,15 @@
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
         super(EventHubManagementClientConfiguration, self).__init__(**kwargs)
 
         self.credential = credential
         self.subscription_id = subscription_id
-        self.api_version = "2018-01-01-preview"
+        self.api_version = "2015-08-01"
         self.credential_scopes = kwargs.pop('credential_scopes', ['https://management.azure.com/.default'])
         kwargs.setdefault('sdk_moniker', 'mgmt-eventhub/{}'.format(VERSION))
         self._configure(**kwargs)
 
     def _configure(
         self,
         **kwargs  # type: Any
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/_event_hub_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._event_hub_management_client import EventHubManagementClient
+from ._version import VERSION
+
+__version__ = VERSION
 __all__ = ['EventHubManagementClient']
 
 try:
     from ._patch import patch_sdk  # type: ignore
     patch_sdk()
 except ImportError:
     pass
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_event_hub_management_client_enums.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_event_hub_management_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,15 +562,15 @@
     :type name: str or ~azure.mgmt.eventhub.v2018_01_01_preview.models.ClusterSkuName
     :param capacity: The quantity of Event Hubs Cluster Capacity Units contained in this cluster.
     :type capacity: int
     """
 
     _validation = {
         'name': {'required': True},
-        'capacity': {'maximum': 32, 'minimum': 1},
+        'capacity': {'minimum': 1},
     }
 
     _attribute_map = {
         'name': {'key': 'name', 'type': 'str'},
         'capacity': {'key': 'capacity', 'type': 'int'},
     }
 
@@ -731,14 +731,16 @@
     :type tags: dict[str, str]
     :param sku: Properties of sku resource.
     :type sku: ~azure.mgmt.eventhub.v2018_01_01_preview.models.Sku
     :param identity: Properties of BYOK Identity description.
     :type identity: ~azure.mgmt.eventhub.v2018_01_01_preview.models.Identity
     :ivar provisioning_state: Provisioning state of the Namespace.
     :vartype provisioning_state: str
+    :ivar status: Status of the Namespace.
+    :vartype status: str
     :ivar created_at: The time the Namespace was created.
     :vartype created_at: ~datetime.datetime
     :ivar updated_at: The time the Namespace was updated.
     :vartype updated_at: ~datetime.datetime
     :ivar service_bus_endpoint: Endpoint you can use to perform Service Bus operations.
     :vartype service_bus_endpoint: str
     :param cluster_arm_id: Cluster ARM ID of the Namespace.
@@ -761,14 +763,15 @@
     """
 
     _validation = {
         'id': {'readonly': True},
         'name': {'readonly': True},
         'type': {'readonly': True},
         'provisioning_state': {'readonly': True},
+        'status': {'readonly': True},
         'created_at': {'readonly': True},
         'updated_at': {'readonly': True},
         'service_bus_endpoint': {'readonly': True},
         'metric_id': {'readonly': True},
         'maximum_throughput_units': {'maximum': 20, 'minimum': 0},
     }
 
@@ -777,14 +780,15 @@
         'name': {'key': 'name', 'type': 'str'},
         'type': {'key': 'type', 'type': 'str'},
         'location': {'key': 'location', 'type': 'str'},
         'tags': {'key': 'tags', 'type': '{str}'},
         'sku': {'key': 'sku', 'type': 'Sku'},
         'identity': {'key': 'identity', 'type': 'Identity'},
         'provisioning_state': {'key': 'properties.provisioningState', 'type': 'str'},
+        'status': {'key': 'properties.status', 'type': 'str'},
         'created_at': {'key': 'properties.createdAt', 'type': 'iso-8601'},
         'updated_at': {'key': 'properties.updatedAt', 'type': 'iso-8601'},
         'service_bus_endpoint': {'key': 'properties.serviceBusEndpoint', 'type': 'str'},
         'cluster_arm_id': {'key': 'properties.clusterArmId', 'type': 'str'},
         'metric_id': {'key': 'properties.metricId', 'type': 'str'},
         'is_auto_inflate_enabled': {'key': 'properties.isAutoInflateEnabled', 'type': 'bool'},
         'maximum_throughput_units': {'key': 'properties.maximumThroughputUnits', 'type': 'int'},
@@ -797,14 +801,15 @@
         self,
         **kwargs
     ):
         super(EHNamespace, self).__init__(**kwargs)
         self.sku = kwargs.get('sku', None)
         self.identity = kwargs.get('identity', None)
         self.provisioning_state = None
+        self.status = None
         self.created_at = None
         self.updated_at = None
         self.service_bus_endpoint = None
         self.cluster_arm_id = kwargs.get('cluster_arm_id', None)
         self.metric_id = None
         self.is_auto_inflate_enabled = kwargs.get('is_auto_inflate_enabled', None)
         self.maximum_throughput_units = kwargs.get('maximum_throughput_units', None)
@@ -874,41 +879,35 @@
         self.value = kwargs.get('value', None)
         self.next_link = kwargs.get('next_link', None)
 
 
 class Encryption(msrest.serialization.Model):
     """Properties to configure Encryption.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     :param key_vault_properties: Properties of KeyVault.
     :type key_vault_properties:
      list[~azure.mgmt.eventhub.v2018_01_01_preview.models.KeyVaultProperties]
-    :ivar key_source: Enumerates the possible value of keySource for Encryption. Default value:
+    :param key_source: Enumerates the possible value of keySource for Encryption. The only
+     acceptable values to pass in are None and "Microsoft.KeyVault". The default value is
      "Microsoft.KeyVault".
-    :vartype key_source: str
+    :type key_source: str
     """
 
-    _validation = {
-        'key_source': {'constant': True},
-    }
-
     _attribute_map = {
         'key_vault_properties': {'key': 'keyVaultProperties', 'type': '[KeyVaultProperties]'},
         'key_source': {'key': 'keySource', 'type': 'str'},
     }
 
-    key_source = "Microsoft.KeyVault"
-
     def __init__(
         self,
         **kwargs
     ):
         super(Encryption, self).__init__(**kwargs)
         self.key_vault_properties = kwargs.get('key_vault_properties', None)
+        self.key_source = kwargs.get('key_source', "Microsoft.KeyVault")
 
 
 class ErrorResponse(msrest.serialization.Model):
     """Error response indicates Event Hub service is not able to process the incoming request. The reason is provided in the error message.
 
     :param code: Error code.
     :type code: str
@@ -1022,44 +1021,38 @@
         self.value = kwargs.get('value', None)
         self.next_link = kwargs.get('next_link', None)
 
 
 class Identity(msrest.serialization.Model):
     """Properties to configure Identity for Bring your Own Keys.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     :param principal_id: ObjectId from the KeyVault.
     :type principal_id: str
     :param tenant_id: TenantId from the KeyVault.
     :type tenant_id: str
-    :ivar type: Enumerates the possible value Identity type, which currently supports only
-     'SystemAssigned'. Default value: "SystemAssigned".
-    :vartype type: str
+    :param type: Enumerates the possible value Identity type, which currently supports only
+     'SystemAssigned'. The only acceptable values to pass in are None and "SystemAssigned". The
+     default value is "SystemAssigned".
+    :type type: str
     """
 
-    _validation = {
-        'type': {'constant': True},
-    }
-
     _attribute_map = {
         'principal_id': {'key': 'principalId', 'type': 'str'},
         'tenant_id': {'key': 'tenantId', 'type': 'str'},
         'type': {'key': 'type', 'type': 'str'},
     }
 
-    type = "SystemAssigned"
-
     def __init__(
         self,
         **kwargs
     ):
         super(Identity, self).__init__(**kwargs)
         self.principal_id = kwargs.get('principal_id', None)
         self.tenant_id = kwargs.get('tenant_id', None)
+        self.type = kwargs.get('type', "SystemAssigned")
 
 
 class IpFilterRule(Resource):
     """Single item in a List or Get IpFilterRules operation.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -1642,15 +1635,15 @@
     :type tier: str or ~azure.mgmt.eventhub.v2018_01_01_preview.models.SkuTier
     :param capacity: The Event Hubs throughput units, value should be 0 to 20 throughput units.
     :type capacity: int
     """
 
     _validation = {
         'name': {'required': True},
-        'capacity': {'maximum': 20, 'minimum': 0},
+        'capacity': {'minimum': 0},
     }
 
     _attribute_map = {
         'name': {'key': 'name', 'type': 'str'},
         'tier': {'key': 'tier', 'type': 'str'},
         'capacity': {'key': 'capacity', 'type': 'int'},
     }
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models_py3.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/models/_models_py3.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,15 +604,15 @@
     :type name: str or ~azure.mgmt.eventhub.v2018_01_01_preview.models.ClusterSkuName
     :param capacity: The quantity of Event Hubs Cluster Capacity Units contained in this cluster.
     :type capacity: int
     """
 
     _validation = {
         'name': {'required': True},
-        'capacity': {'maximum': 32, 'minimum': 1},
+        'capacity': {'minimum': 1},
     }
 
     _attribute_map = {
         'name': {'key': 'name', 'type': 'str'},
         'capacity': {'key': 'capacity', 'type': 'int'},
     }
 
@@ -789,14 +789,16 @@
     :type tags: dict[str, str]
     :param sku: Properties of sku resource.
     :type sku: ~azure.mgmt.eventhub.v2018_01_01_preview.models.Sku
     :param identity: Properties of BYOK Identity description.
     :type identity: ~azure.mgmt.eventhub.v2018_01_01_preview.models.Identity
     :ivar provisioning_state: Provisioning state of the Namespace.
     :vartype provisioning_state: str
+    :ivar status: Status of the Namespace.
+    :vartype status: str
     :ivar created_at: The time the Namespace was created.
     :vartype created_at: ~datetime.datetime
     :ivar updated_at: The time the Namespace was updated.
     :vartype updated_at: ~datetime.datetime
     :ivar service_bus_endpoint: Endpoint you can use to perform Service Bus operations.
     :vartype service_bus_endpoint: str
     :param cluster_arm_id: Cluster ARM ID of the Namespace.
@@ -819,14 +821,15 @@
     """
 
     _validation = {
         'id': {'readonly': True},
         'name': {'readonly': True},
         'type': {'readonly': True},
         'provisioning_state': {'readonly': True},
+        'status': {'readonly': True},
         'created_at': {'readonly': True},
         'updated_at': {'readonly': True},
         'service_bus_endpoint': {'readonly': True},
         'metric_id': {'readonly': True},
         'maximum_throughput_units': {'maximum': 20, 'minimum': 0},
     }
 
@@ -835,14 +838,15 @@
         'name': {'key': 'name', 'type': 'str'},
         'type': {'key': 'type', 'type': 'str'},
         'location': {'key': 'location', 'type': 'str'},
         'tags': {'key': 'tags', 'type': '{str}'},
         'sku': {'key': 'sku', 'type': 'Sku'},
         'identity': {'key': 'identity', 'type': 'Identity'},
         'provisioning_state': {'key': 'properties.provisioningState', 'type': 'str'},
+        'status': {'key': 'properties.status', 'type': 'str'},
         'created_at': {'key': 'properties.createdAt', 'type': 'iso-8601'},
         'updated_at': {'key': 'properties.updatedAt', 'type': 'iso-8601'},
         'service_bus_endpoint': {'key': 'properties.serviceBusEndpoint', 'type': 'str'},
         'cluster_arm_id': {'key': 'properties.clusterArmId', 'type': 'str'},
         'metric_id': {'key': 'properties.metricId', 'type': 'str'},
         'is_auto_inflate_enabled': {'key': 'properties.isAutoInflateEnabled', 'type': 'bool'},
         'maximum_throughput_units': {'key': 'properties.maximumThroughputUnits', 'type': 'int'},
@@ -866,14 +870,15 @@
         encryption: Optional["Encryption"] = None,
         **kwargs
     ):
         super(EHNamespace, self).__init__(location=location, tags=tags, **kwargs)
         self.sku = sku
         self.identity = identity
         self.provisioning_state = None
+        self.status = None
         self.created_at = None
         self.updated_at = None
         self.service_bus_endpoint = None
         self.cluster_arm_id = cluster_arm_id
         self.metric_id = None
         self.is_auto_inflate_enabled = is_auto_inflate_enabled
         self.maximum_throughput_units = maximum_throughput_units
@@ -950,43 +955,38 @@
         self.value = value
         self.next_link = next_link
 
 
 class Encryption(msrest.serialization.Model):
     """Properties to configure Encryption.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     :param key_vault_properties: Properties of KeyVault.
     :type key_vault_properties:
      list[~azure.mgmt.eventhub.v2018_01_01_preview.models.KeyVaultProperties]
-    :ivar key_source: Enumerates the possible value of keySource for Encryption. Default value:
+    :param key_source: Enumerates the possible value of keySource for Encryption. The only
+     acceptable values to pass in are None and "Microsoft.KeyVault". The default value is
      "Microsoft.KeyVault".
-    :vartype key_source: str
+    :type key_source: str
     """
 
-    _validation = {
-        'key_source': {'constant': True},
-    }
-
     _attribute_map = {
         'key_vault_properties': {'key': 'keyVaultProperties', 'type': '[KeyVaultProperties]'},
         'key_source': {'key': 'keySource', 'type': 'str'},
     }
 
-    key_source = "Microsoft.KeyVault"
-
     def __init__(
         self,
         *,
         key_vault_properties: Optional[List["KeyVaultProperties"]] = None,
+        key_source: Optional[str] = "Microsoft.KeyVault",
         **kwargs
     ):
         super(Encryption, self).__init__(**kwargs)
         self.key_vault_properties = key_vault_properties
+        self.key_source = key_source
 
 
 class ErrorResponse(msrest.serialization.Model):
     """Error response indicates Event Hub service is not able to process the incoming request. The reason is provided in the error message.
 
     :param code: Error code.
     :type code: str
@@ -1111,47 +1111,42 @@
         self.value = value
         self.next_link = next_link
 
 
 class Identity(msrest.serialization.Model):
     """Properties to configure Identity for Bring your Own Keys.
 
-    Variables are only populated by the server, and will be ignored when sending a request.
-
     :param principal_id: ObjectId from the KeyVault.
     :type principal_id: str
     :param tenant_id: TenantId from the KeyVault.
     :type tenant_id: str
-    :ivar type: Enumerates the possible value Identity type, which currently supports only
-     'SystemAssigned'. Default value: "SystemAssigned".
-    :vartype type: str
+    :param type: Enumerates the possible value Identity type, which currently supports only
+     'SystemAssigned'. The only acceptable values to pass in are None and "SystemAssigned". The
+     default value is "SystemAssigned".
+    :type type: str
     """
 
-    _validation = {
-        'type': {'constant': True},
-    }
-
     _attribute_map = {
         'principal_id': {'key': 'principalId', 'type': 'str'},
         'tenant_id': {'key': 'tenantId', 'type': 'str'},
         'type': {'key': 'type', 'type': 'str'},
     }
 
-    type = "SystemAssigned"
-
     def __init__(
         self,
         *,
         principal_id: Optional[str] = None,
         tenant_id: Optional[str] = None,
+        type: Optional[str] = "SystemAssigned",
         **kwargs
     ):
         super(Identity, self).__init__(**kwargs)
         self.principal_id = principal_id
         self.tenant_id = tenant_id
+        self.type = type
 
 
 class IpFilterRule(Resource):
     """Single item in a List or Get IpFilterRules operation.
 
     Variables are only populated by the server, and will be ignored when sending a request.
 
@@ -1786,15 +1781,15 @@
     :type tier: str or ~azure.mgmt.eventhub.v2018_01_01_preview.models.SkuTier
     :param capacity: The Event Hubs throughput units, value should be 0 to 20 throughput units.
     :type capacity: int
     """
 
     _validation = {
         'name': {'required': True},
-        'capacity': {'maximum': 20, 'minimum': 0},
+        'capacity': {'minimum': 0},
     }
 
     _attribute_map = {
         'name': {'key': 'name', 'type': 'str'},
         'tier': {'key': 'tier', 'type': 'str'},
         'capacity': {'key': 'capacity', 'type': 'int'},
     }
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_link_resources_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_consumer_groups_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_consumer_groups_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_configuration_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_configuration_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_event_hubs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_event_hubs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_namespaces_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_namespaces_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_regions_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_regions_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_disaster_recovery_configs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_disaster_recovery_configs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_clusters_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/operations/_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_configuration.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy
 
+from .._version import VERSION
+
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
-VERSION = "unknown"
 
 class EventHubManagementClientConfiguration(Configuration):
     """Configuration for EventHubManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_event_hub_management_client.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/_event_hub_management_client.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_link_resources_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_link_resources_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_consumer_groups_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_consumer_groups_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_configuration_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_configuration_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_endpoint_connections_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_private_endpoint_connections_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/__init__.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_event_hubs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_event_hubs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_namespaces_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_namespaces_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_regions_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_regions_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_clusters_operations.py` & `azure-mgmt-eventhub-9.1.0/azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_clusters_operations.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/SOURCES.txt` & `azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 azure/mgmt/eventhub/models.py
 azure/mgmt/eventhub/aio/__init__.py
 azure/mgmt/eventhub/aio/_configuration.py
 azure/mgmt/eventhub/aio/_event_hub_management_client.py
 azure/mgmt/eventhub/v2015_08_01/__init__.py
 azure/mgmt/eventhub/v2015_08_01/_configuration.py
 azure/mgmt/eventhub/v2015_08_01/_event_hub_management_client.py
+azure/mgmt/eventhub/v2015_08_01/_version.py
 azure/mgmt/eventhub/v2015_08_01/aio/__init__.py
 azure/mgmt/eventhub/v2015_08_01/aio/_configuration.py
 azure/mgmt/eventhub/v2015_08_01/aio/_event_hub_management_client.py
 azure/mgmt/eventhub/v2015_08_01/aio/operations/__init__.py
 azure/mgmt/eventhub/v2015_08_01/aio/operations/_consumer_groups_operations.py
 azure/mgmt/eventhub/v2015_08_01/aio/operations/_event_hubs_operations.py
 azure/mgmt/eventhub/v2015_08_01/aio/operations/_namespaces_operations.py
@@ -33,14 +34,15 @@
 azure/mgmt/eventhub/v2015_08_01/operations/_consumer_groups_operations.py
 azure/mgmt/eventhub/v2015_08_01/operations/_event_hubs_operations.py
 azure/mgmt/eventhub/v2015_08_01/operations/_namespaces_operations.py
 azure/mgmt/eventhub/v2015_08_01/operations/_operations.py
 azure/mgmt/eventhub/v2017_04_01/__init__.py
 azure/mgmt/eventhub/v2017_04_01/_configuration.py
 azure/mgmt/eventhub/v2017_04_01/_event_hub_management_client.py
+azure/mgmt/eventhub/v2017_04_01/_version.py
 azure/mgmt/eventhub/v2017_04_01/aio/__init__.py
 azure/mgmt/eventhub/v2017_04_01/aio/_configuration.py
 azure/mgmt/eventhub/v2017_04_01/aio/_event_hub_management_client.py
 azure/mgmt/eventhub/v2017_04_01/aio/operations/__init__.py
 azure/mgmt/eventhub/v2017_04_01/aio/operations/_consumer_groups_operations.py
 azure/mgmt/eventhub/v2017_04_01/aio/operations/_disaster_recovery_configs_operations.py
 azure/mgmt/eventhub/v2017_04_01/aio/operations/_event_hubs_operations.py
@@ -57,14 +59,15 @@
 azure/mgmt/eventhub/v2017_04_01/operations/_event_hubs_operations.py
 azure/mgmt/eventhub/v2017_04_01/operations/_namespaces_operations.py
 azure/mgmt/eventhub/v2017_04_01/operations/_operations.py
 azure/mgmt/eventhub/v2017_04_01/operations/_regions_operations.py
 azure/mgmt/eventhub/v2018_01_01_preview/__init__.py
 azure/mgmt/eventhub/v2018_01_01_preview/_configuration.py
 azure/mgmt/eventhub/v2018_01_01_preview/_event_hub_management_client.py
+azure/mgmt/eventhub/v2018_01_01_preview/_version.py
 azure/mgmt/eventhub/v2018_01_01_preview/aio/__init__.py
 azure/mgmt/eventhub/v2018_01_01_preview/aio/_configuration.py
 azure/mgmt/eventhub/v2018_01_01_preview/aio/_event_hub_management_client.py
 azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/__init__.py
 azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_clusters_operations.py
 azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_configuration_operations.py
 azure/mgmt/eventhub/v2018_01_01_preview/aio/operations/_consumer_groups_operations.py
@@ -89,14 +92,15 @@
 azure/mgmt/eventhub/v2018_01_01_preview/operations/_operations.py
 azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_endpoint_connections_operations.py
 azure/mgmt/eventhub/v2018_01_01_preview/operations/_private_link_resources_operations.py
 azure/mgmt/eventhub/v2018_01_01_preview/operations/_regions_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/__init__.py
 azure/mgmt/eventhub/v2021_01_01_preview/_configuration.py
 azure/mgmt/eventhub/v2021_01_01_preview/_event_hub_management_client.py
+azure/mgmt/eventhub/v2021_01_01_preview/_version.py
 azure/mgmt/eventhub/v2021_01_01_preview/aio/__init__.py
 azure/mgmt/eventhub/v2021_01_01_preview/aio/_configuration.py
 azure/mgmt/eventhub/v2021_01_01_preview/aio/_event_hub_management_client.py
 azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/__init__.py
 azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_consumer_groups_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_disaster_recovery_configs_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/aio/operations/_event_hubs_operations.py
@@ -112,14 +116,45 @@
 azure/mgmt/eventhub/v2021_01_01_preview/operations/_consumer_groups_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/operations/_disaster_recovery_configs_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/operations/_event_hubs_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/operations/_namespaces_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/operations/_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_endpoint_connections_operations.py
 azure/mgmt/eventhub/v2021_01_01_preview/operations/_private_link_resources_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/__init__.py
+azure/mgmt/eventhub/v2021_06_01_preview/_configuration.py
+azure/mgmt/eventhub/v2021_06_01_preview/_event_hub_management_client.py
+azure/mgmt/eventhub/v2021_06_01_preview/_version.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/__init__.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/_configuration.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/_event_hub_management_client.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/__init__.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_clusters_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_configuration_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_consumer_groups_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_disaster_recovery_configs_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_event_hubs_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_namespaces_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_private_endpoint_connections_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/aio/operations/_private_link_resources_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/models/__init__.py
+azure/mgmt/eventhub/v2021_06_01_preview/models/_event_hub_management_client_enums.py
+azure/mgmt/eventhub/v2021_06_01_preview/models/_models.py
+azure/mgmt/eventhub/v2021_06_01_preview/models/_models_py3.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/__init__.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_clusters_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_configuration_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_consumer_groups_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_disaster_recovery_configs_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_event_hubs_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_namespaces_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_private_endpoint_connections_operations.py
+azure/mgmt/eventhub/v2021_06_01_preview/operations/_private_link_resources_operations.py
 azure_mgmt_eventhub.egg-info/PKG-INFO
 azure_mgmt_eventhub.egg-info/SOURCES.txt
 azure_mgmt_eventhub.egg-info/dependency_links.txt
 azure_mgmt_eventhub.egg-info/not-zip-safe
 azure_mgmt_eventhub.egg-info/requires.txt
 azure_mgmt_eventhub.egg-info/top_level.txt
 tests/_aio_testcase.py
```

## Comparing `azure-mgmt-eventhub-9.0.0/azure_mgmt_eventhub.egg-info/PKG-INFO` & `azure-mgmt-eventhub-9.1.0/azure_mgmt_eventhub.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-eventhub
-Version: 9.0.0
+Version: 9.1.0
 Summary: Microsoft Azure EventHub Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Description: # Microsoft Azure SDK for Python
         
@@ -27,14 +27,24 @@
         
         
         ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fazure-mgmt-eventhub%2FREADME.png)
         
         
         # Release History
         
+        ## 9.1.0 (2021-09-17)
+        
+        **Features**
+        
+          - Model Cluster has a new parameter system_data
+          - Model EHNamespace has a new parameter disable_local_auth
+          - Model EHNamespace has a new parameter status
+          - Model NetworkRuleSet has a new parameter public_network_access
+          - Added operation ClustersOperations.list_by_subscription
+        
         ## 9.0.0 (2021-05-25)
         
         **Features**
         
           - Model NetworkRuleSet has a new parameter system_data
           - Model ConsumerGroup has a new parameter system_data
           - Model PrivateEndpointConnection has a new parameter system_data
@@ -76,29 +86,29 @@
         
         - Credential system has been completly revamped:
         
           - `azure.common.credentials` or `msrestazure.azure_active_directory` instances are no longer supported, use the `azure-identity` classes instead: https://pypi.org/project/azure-identity/
           - `credentials` parameter has been renamed `credential`
         
         - The `config` attribute no longer exists on a client, configuration should be passed as kwarg. Example: `MyClient(credential, subscription_id, enable_logging=True)`. For a complete set of
-          supported options, see the [parameters accept in init documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
+          supported options, see the [parameters accept in init documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
         - You can't import a `version` module anymore, use `__version__` instead
         - Operations that used to return a `msrest.polling.LROPoller` now returns a `azure.core.polling.LROPoller` and are prefixed with `begin_`.
         - Exceptions tree have been simplified and most exceptions are now `azure.core.exceptions.HttpResponseError` (`CloudError` has been removed).
         - Most of the operation kwarg have changed. Some of the most noticeable:
         
           - `raw` has been removed. Equivalent feature can be found using `cls`, a callback that will give access to internal HTTP response for advanced user
           - For a complete set of
-          supported options, see the [parameters accept in Request documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/master/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
+          supported options, see the [parameters accept in Request documentation of azure-core](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/core/azure-core/CLIENT_LIBRARY_DEVELOPER.md#available-policies)
         
         **General new features**
         
         - Type annotations support using `typing`. SDKs are mypy ready.
         - This client has now stable and official support for async. Check the `aio` namespace of your package to find the async client.
-        - This client now support natively tracing library like OpenCensus or OpenTelemetry. See this [tracing quickstart](https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/core/azure-core-tracing-opentelemetry) for an overview.
+        - This client now support natively tracing library like OpenCensus or OpenTelemetry. See this [tracing quickstart](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-tracing-opentelemetry) for an overview.
         
         ## 4.0.0 (2020-06-12)
         
         **Features**
         
           - Model Cluster has a new parameter updated_at
           - Model Cluster has a new parameter created_at
```

## Comparing `azure-mgmt-eventhub-9.0.0/tests/conftest.py` & `azure-mgmt-eventhub-9.1.0/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/tests/_aio_testcase.py` & `azure-mgmt-eventhub-9.1.0/tests/_aio_testcase.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/tests/test_cli_mgmt_eventhub_async.py` & `azure-mgmt-eventhub-9.1.0/tests/test_cli_mgmt_eventhub_async.py`

 * *Files identical despite different names*

## Comparing `azure-mgmt-eventhub-9.0.0/tests/test_cli_mgmt_eventhub.py` & `azure-mgmt-eventhub-9.1.0/tests/test_cli_mgmt_eventhub.py`

 * *Files identical despite different names*

