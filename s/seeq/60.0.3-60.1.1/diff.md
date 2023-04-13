# Comparing `tmp/seeq-60.0.3.tar.gz` & `tmp/seeq-60.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seeq-60.0.3.tar", last modified: Tue Mar  7 21:47:13 2023, max compression
+gzip compressed data, was "dist\seeq-60.1.1.tar", last modified: Tue Mar 21 19:02:00 2023, max compression
```

## Comparing `seeq-60.0.3.tar` & `seeq-60.1.1.tar`

### file list

```diff
@@ -1,375 +1,375 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 21:47:13.000000 seeq-60.0.3/
--rw-rw-rw-   0        0        0    33551 2022-12-22 20:30:35.000000 seeq-60.0.3/LICENSE
--rw-rw-rw-   0        0        0       19 2023-01-30 20:12:10.000000 seeq-60.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3899 2023-03-07 21:47:13.000000 seeq-60.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3399 2023-01-30 20:12:10.000000 seeq-60.0.3/README.md
--rw-rw-rw-   0        0        0        0 2022-12-22 20:30:35.000000 seeq-60.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-07 21:47:12.000000 seeq-60.0.3/seeq/
-drwxrwxrwx   0        0        0        0 2023-03-07 21:47:12.000000 seeq-60.0.3/seeq/sdk/
--rw-rw-rw-   0        0        0    22319 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 21:47:12.000000 seeq-60.0.3/seeq/sdk/api/
--rw-rw-rw-   0        0        0     1926 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/__init__.py
--rw-rw-rw-   0        0        0    15283 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/access_keys_api.py
--rw-rw-rw-   0        0        0    29040 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/add_ons_api.py
--rw-rw-rw-   0        0        0   114203 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/agents_api.py
--rw-rw-rw-   0        0        0    54586 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/annotations_api.py
--rw-rw-rw-   0        0        0    23866 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/assets_api.py
--rw-rw-rw-   0        0        0     8213 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/audit_api.py
--rw-rw-rw-   0        0        0    13540 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/auth_api.py
--rw-rw-rw-   0        0        0    27068 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/condition_monitors_api.py
--rw-rw-rw-   0        0        0    51672 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/conditions_api.py
--rw-rw-rw-   0        0        0   124777 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/content_api.py
--rw-rw-rw-   0        0        0    34214 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/datafiles_api.py
--rw-rw-rw-   0        0        0    41068 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/datasources_api.py
--rw-rw-rw-   0        0        0    24826 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/display_templates_api.py
--rw-rw-rw-   0        0        0    24099 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/displays_api.py
--rw-rw-rw-   0        0        0    29830 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/export_api.py
--rw-rw-rw-   0        0        0    49756 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/folders_api.py
--rw-rw-rw-   0        0        0   102750 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/formulas_api.py
--rw-rw-rw-   0        0        0   155303 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/items_api.py
--rw-rw-rw-   0        0        0    29740 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/jobs_api.py
--rw-rw-rw-   0        0        0    21182 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/logs_api.py
--rw-rw-rw-   0        0        0    24406 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/metrics_api.py
--rw-rw-rw-   0        0        0    31687 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/monitors_api.py
--rw-rw-rw-   0        0        0     5941 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/networks_api.py
--rw-rw-rw-   0        0        0    26044 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/notification_configurations_api.py
--rw-rw-rw-   0        0        0    21303 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/plugins_api.py
--rw-rw-rw-   0        0        0    35172 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/projects_api.py
--rw-rw-rw-   0        0        0    24398 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/report_templates_api.py
--rw-rw-rw-   0        0        0     5736 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/reports_api.py
--rw-rw-rw-   0        0        0    37825 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/requests_api.py
--rw-rw-rw-   0        0        0    28228 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/scalars_api.py
--rw-rw-rw-   0        0        0   111043 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/signals_api.py
--rw-rw-rw-   0        0        0    20428 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/subscriptions_api.py
--rw-rw-rw-   0        0        0    99316 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/system_api.py
--rw-rw-rw-   0        0        0    65360 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/trees_api.py
--rw-rw-rw-   0        0        0    12493 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/usage_api.py
--rw-rw-rw-   0        0        0    51919 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/user_groups_api.py
--rw-rw-rw-   0        0        0    49412 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/users_api.py
--rw-rw-rw-   0        0        0    93533 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api/workbooks_api.py
--rw-rw-rw-   0        0        0    30256 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/api_client.py
--rw-rw-rw-   0        0        0     9431 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/configuration.py
-drwxrwxrwx   0        0        0        0 2023-03-07 21:47:13.000000 seeq-60.0.3/seeq/sdk/models/
--rw-rw-rw-   0        0        0    18310 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/__init__.py
--rw-rw-rw-   0        0        0     4424 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/access_key_input_v1.py
--rw-rw-rw-   0        0        0     7578 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/access_key_output_list_v1.py
--rw-rw-rw-   0        0        0    14950 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/access_key_output_v1.py
--rw-rw-rw-   0        0        0     4247 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/ace_input_v1.py
--rw-rw-rw-   0        0        0     5948 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/ace_output_v1.py
--rw-rw-rw-   0        0        0     6980 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/acl_input_v1.py
--rw-rw-rw-   0        0        0     6783 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/acl_output_v1.py
--rw-rw-rw-   0        0        0     3713 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/activity_graph_output_v1.py
--rw-rw-rw-   0        0        0     7607 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/activity_output_v1.py
--rw-rw-rw-   0        0        0     8832 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/add_on_input_v1.py
--rw-rw-rw-   0        0        0     7521 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/add_on_output_list_v1.py
--rw-rw-rw-   0        0        0    14831 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/add_on_output_v1.py
--rw-rw-rw-   0        0        0     7763 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/add_on_preview_output_list_v1.py
--rw-rw-rw-   0        0        0     6748 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/add_on_preview_v1.py
--rw-rw-rw-   0        0        0    11430 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/add_on_tool_input_v1.py
--rw-rw-rw-   0        0        0    16207 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/add_on_tool_output_v1.py
--rw-rw-rw-   0        0        0     4285 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/administrator_contact_information_v1.py
--rw-rw-rw-   0        0        0     5019 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/agent_input_v1.py
--rw-rw-rw-   0        0        0     3238 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/agent_key_output_v1.py
--rw-rw-rw-   0        0        0    12658 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/agent_output_v1.py
--rw-rw-rw-   0        0        0     8084 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/agent_status_output_v1.py
--rw-rw-rw-   0        0        0     8091 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/agent_status_v1.py
--rw-rw-rw-   0        0        0     4420 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/annotation_image_link_output_v1.py
--rw-rw-rw-   0        0        0    11395 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/annotation_input_v1.py
--rw-rw-rw-   0        0        0     4365 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/annotation_interest_input_v1.py
--rw-rw-rw-   0        0        0     3884 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/annotation_interest_output_v1.py
--rw-rw-rw-   0        0        0     7642 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/annotation_list_output_v1.py
--rw-rw-rw-   0        0        0    28089 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/annotation_output_v1.py
--rw-rw-rw-   0        0        0     4571 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/archive_output_v1.py
--rw-rw-rw-   0        0        0     4316 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_batch_input_v1.py
--rw-rw-rw-   0        0        0     4853 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_error.py
--rw-rw-rw-   0        0        0    15161 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_group_asset_input_v1.py
--rw-rw-rw-   0        0        0     4174 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_group_input_v1.py
--rw-rw-rw-   0        0        0     4105 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_group_output_v1.py
--rw-rw-rw-   0        0        0    14208 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_group_root_input_v1.py
--rw-rw-rw-   0        0        0     6682 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_group_tree_output_v1.py
--rw-rw-rw-   0        0        0    12120 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_input_v1.py
--rw-rw-rw-   0        0        0    18126 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_output_v1.py
--rw-rw-rw-   0        0        0     8745 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_selection_input_v1.py
--rw-rw-rw-   0        0        0    14359 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_selection_output_v1.py
--rw-rw-rw-   0        0        0     9597 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_tree_batch_input_v1.py
--rw-rw-rw-   0        0        0    11597 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_tree_output_v1.py
--rw-rw-rw-   0        0        0     4570 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/asset_tree_single_input_v1.py
--rw-rw-rw-   0        0        0     8470 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/audit_output_list_v1.py
--rw-rw-rw-   0        0        0     9984 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/audit_output_v1.py
--rw-rw-rw-   0        0        0     7325 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/auth_input_v1.py
--rw-rw-rw-   0        0        0     3554 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/auth_providers_output_v1.py
--rw-rw-rw-   0        0        0     4227 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/cache_info_v1.py
--rw-rw-rw-   0        0        0    21392 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/calculated_item_output_v1.py
--rw-rw-rw-   0        0        0     5502 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/capsule_input_v1.py
--rw-rw-rw-   0        0        0     4490 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/capsule_property_input_v1.py
--rw-rw-rw-   0        0        0     4301 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/capsule_property_output_v1.py
--rw-rw-rw-   0        0        0     8310 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/capsule_v1.py
--rw-rw-rw-   0        0        0     3371 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/capsules_input_v1.py
--rw-rw-rw-   0        0        0    10722 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/capsules_output_v1.py
--rw-rw-rw-   0        0        0     4158 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/capsules_overwrite_input_v1.py
--rw-rw-rw-   0        0        0     7478 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/channel_output_v1.py
--rw-rw-rw-   0        0        0     3521 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/condition_batch_input_v1.py
--rw-rw-rw-   0        0        0    21085 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/condition_input_v1.py
--rw-rw-rw-   0        0        0     9108 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/condition_monitor_input_v1.py
--rw-rw-rw-   0        0        0    11175 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py
--rw-rw-rw-   0        0        0    17800 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/condition_monitor_output_v1.py
--rw-rw-rw-   0        0        0    25193 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/condition_output_v1.py
--rw-rw-rw-   0        0        0    24419 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/condition_update_input_v1.py
--rw-rw-rw-   0        0        0     4198 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/configuration_input_v1.py
--rw-rw-rw-   0        0        0     4436 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/configuration_option_input_v1.py
--rw-rw-rw-   0        0        0     3882 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/configuration_option_output_simple_v1.py
--rw-rw-rw-   0        0        0    12749 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/configuration_option_output_v1.py
--rw-rw-rw-   0        0        0     8957 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/configuration_output_v1.py
--rw-rw-rw-   0        0        0     5125 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/configured_directives_output_v1.py
--rw-rw-rw-   0        0        0     8805 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/connection_input_v1.py
--rw-rw-rw-   0        0        0    22910 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/connection_output_v1.py
--rw-rw-rw-   0        0        0    17645 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/connection_status_output_v1.py
--rw-rw-rw-   0        0        0    17370 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/connection_status_v1.py
--rw-rw-rw-   0        0        0     3363 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/connections_output_v1.py
--rw-rw-rw-   0        0        0     5107 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/connector_input_v1.py
--rw-rw-rw-   0        0        0    13652 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/connector_output_v1.py
--rw-rw-rw-   0        0        0     3383 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/connectors_output_v1.py
--rw-rw-rw-   0        0        0    16191 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/content_input_v1.py
--rw-rw-rw-   0        0        0    24079 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/content_output_v1.py
--rw-rw-rw-   0        0        0     5464 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/content_with_metadata_list_output_v1.py
--rw-rw-rw-   0        0        0    30123 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/content_with_metadata_output_v1.py
--rw-rw-rw-   0        0        0     3558 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/csv_datafile_output_v1.py
--rw-rw-rw-   0        0        0    51259 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datafile_input_v1.py
--rw-rw-rw-   0        0        0    55080 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datafile_output_v1.py
--rw-rw-rw-   0        0        0     3227 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datafiles_csv_body.py
--rw-rw-rw-   0        0        0     9859 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_clean_up_input_v1.py
--rw-rw-rw-   0        0        0     3665 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_clean_up_output_v1.py
--rw-rw-rw-   0        0        0    13625 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_input_v1.py
--rw-rw-rw-   0        0        0     7754 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_output_list_v1.py
--rw-rw-rw-   0        0        0    20696 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_output_v1.py
--rw-rw-rw-   0        0        0     9118 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_preview_v1.py
--rw-rw-rw-   0        0        0    16264 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_statistics_v1.py
--rw-rw-rw-   0        0        0     8969 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_status_output_v1.py
--rw-rw-rw-   0        0        0     9422 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_status_v1.py
--rw-rw-rw-   0        0        0    25599 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasource_summary_status_output_v1.py
--rw-rw-rw-   0        0        0    10331 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/datasources_status_output_v1.py
--rw-rw-rw-   0        0        0    10061 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/date_range_input_v1.py
--rw-rw-rw-   0        0        0    17474 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/date_range_output_v1.py
--rw-rw-rw-   0        0        0     5034 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/detailed_meter_output_v1.py
--rw-rw-rw-   0        0        0     5921 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/detailed_timer_output_v1.py
--rw-rw-rw-   0        0        0     5213 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/directive_input_v1.py
--rw-rw-rw-   0        0        0     5410 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/display_input_v1.py
--rw-rw-rw-   0        0        0     7604 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/display_output_list_v1.py
--rw-rw-rw-   0        0        0    15213 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/display_output_v1.py
--rw-rw-rw-   0        0        0     9715 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/display_template_input_v1.py
--rw-rw-rw-   0        0        0     8041 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/display_template_output_list_v1.py
--rw-rw-rw-   0        0        0    16432 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/display_template_output_v1.py
--rw-rw-rw-   0        0        0     5065 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/document_backup_output_v1.py
--rw-rw-rw-   0        0        0     5511 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/email_notification_recipient_output_v1.py
--rw-rw-rw-   0        0        0     5516 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/export_item_v1.py
--rw-rw-rw-   0        0        0    19425 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/export_items_output_v1.py
--rw-rw-rw-   0        0        0    19068 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/export_items_v1.py
--rw-rw-rw-   0        0        0     7536 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/export_preview_list_v1.py
--rw-rw-rw-   0        0        0    11091 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/export_preview_v1.py
--rw-rw-rw-   0        0        0     6728 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/folded_stack_node_v1.py
--rw-rw-rw-   0        0        0     7908 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/folder_input_v1.py
--rw-rw-rw-   0        0        0     5896 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/folder_navigation_output_v1.py
--rw-rw-rw-   0        0        0    16393 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/folder_output_v1.py
--rw-rw-rw-   0        0        0     7095 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_compile_output_v1.py
--rw-rw-rw-   0        0        0     8391 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_compiler_error_output_v1.py
--rw-rw-rw-   0        0        0     4472 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_dependency_input_v1.py
--rw-rw-rw-   0        0        0     4144 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_doc_example_input_v1.py
--rw-rw-rw-   0        0        0     3576 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_doc_example_list_input_v1.py
--rw-rw-rw-   0        0        0     7635 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_doc_input_v1.py
--rw-rw-rw-   0        0        0     3527 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_doc_keyword_list_input_v1.py
--rw-rw-rw-   0        0        0    22305 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_doc_output_v1.py
--rw-rw-rw-   0        0        0     3336 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_doc_summaries_output_v1.py
--rw-rw-rw-   0        0        0     8541 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_doc_summary_output_v1.py
--rw-rw-rw-   0        0        0     8499 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_error_output_v1.py
--rw-rw-rw-   0        0        0     4090 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_example_output_v1.py
--rw-rw-rw-   0        0        0    19458 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_item_input_v1.py
--rw-rw-rw-   0        0        0    19412 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_item_output_v1.py
--rw-rw-rw-   0        0        0     4067 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_log_entry.py
--rw-rw-rw-   0        0        0     3852 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_log_entry_details.py
--rw-rw-rw-   0        0        0     4593 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_log_v1.py
--rw-rw-rw-   0        0        0     6969 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_package_import_input_v1.py
--rw-rw-rw-   0        0        0     6252 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_package_import_output_v1.py
--rw-rw-rw-   0        0        0     9638 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_package_input_v1.py
--rw-rw-rw-   0        0        0    18453 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_package_output_v1.py
--rw-rw-rw-   0        0        0     6385 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_parameter_input_v1.py
--rw-rw-rw-   0        0        0     5766 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_parameter_output_v1.py
--rw-rw-rw-   0        0        0    13985 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_run_input_v1.py
--rw-rw-rw-   0        0        0    12686 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_run_output_v1.py
--rw-rw-rw-   0        0        0     4237 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_token.py
--rw-rw-rw-   0        0        0     4204 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_update_input_v1.py
--rw-rw-rw-   0        0        0     4246 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_upgrade_change_v1.py
--rw-rw-rw-   0        0        0     5098 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/formula_upgrade_output_v1.py
--rw-rw-rw-   0        0        0    14037 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/function_input_v1.py
--rw-rw-rw-   0        0        0     4760 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/function_parameter_output_v1.py
--rw-rw-rw-   0        0        0     6549 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/function_variant_output_v1.py
--rw-rw-rw-   0        0        0     5004 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/gauge_datum_v1.py
--rw-rw-rw-   0        0        0     4299 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/generic_table_output_v1.py
--rw-rw-rw-   0        0        0     3396 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_add_on_tools_output_v1.py
--rw-rw-rw-   0        0        0     7594 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_channels_output_v1.py
--rw-rw-rw-   0        0        0     9468 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_condition_monitor_items_output_v1.py
--rw-rw-rw-   0        0        0     7811 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_content_items_output_v1.py
--rw-rw-rw-   0        0        0     7719 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_date_ranges_output_v1.py
--rw-rw-rw-   0        0        0     7386 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_jobs_output_v1.py
--rw-rw-rw-   0        0        0     7569 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_metrics_output_v1.py
--rw-rw-rw-   0        0        0     7598 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_projects_output_v1.py
--rw-rw-rw-   0        0        0     4327 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_request_output_v1.py
--rw-rw-rw-   0        0        0     3230 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_requests_output_v1.py
--rw-rw-rw-   0        0        0     6413 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_sample_output_v1.py
--rw-rw-rw-   0        0        0    11687 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_samples_output_v1.py
--rw-rw-rw-   0        0        0     7542 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/get_signals_output_v1.py
--rw-rw-rw-   0        0        0     3199 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/id_images_body.py
--rw-rw-rw-   0        0        0     3651 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/identity_mapping_list_v1.py
--rw-rw-rw-   0        0        0     6419 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/identity_mapping_v1.py
--rw-rw-rw-   0        0        0     8628 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/identity_preview_list_v1.py
--rw-rw-rw-   0        0        0    12439 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/identity_preview_v1.py
--rw-rw-rw-   0        0        0     4350 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/indexing_parameters_input_v1.py
--rw-rw-rw-   0        0        0     5113 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/installer_output_v1.py
--rw-rw-rw-   0        0        0     4274 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/interval_v1.py
--rw-rw-rw-   0        0        0     3105 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/invalid_swap_out_v1.py
--rw-rw-rw-   0        0        0     4628 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_batch_output_v1.py
--rw-rw-rw-   0        0        0    11919 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_dependency_output_v1.py
--rw-rw-rw-   0        0        0     3280 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_id_list_input_v1.py
--rw-rw-rw-   0        0        0    15155 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_output_v1.py
--rw-rw-rw-   0        0        0    11643 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_parameter_of_output_v1.py
--rw-rw-rw-   0        0        0     8458 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_preview_list_v1.py
--rw-rw-rw-   0        0        0     7190 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_preview_v1.py
--rw-rw-rw-   0        0        0     9797 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_preview_with_assets_v1.py
--rw-rw-rw-   0        0        0     4334 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_search_preview_list_v1.py
--rw-rw-rw-   0        0        0     8941 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_search_preview_paginated_list_v1.py
--rw-rw-rw-   0        0        0    14582 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_search_preview_v1.py
--rw-rw-rw-   0        0        0     4870 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_swap_result_output_v1.py
--rw-rw-rw-   0        0        0     6757 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_update_output_v1.py
--rw-rw-rw-   0        0        0     4356 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_user_attributes_input_v1.py
--rw-rw-rw-   0        0        0     6082 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_user_attributes_output_v1.py
--rw-rw-rw-   0        0        0     5314 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/item_with_swap_pairs_v1.py
--rw-rw-rw-   0        0        0    11915 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/job_output_v1.py
--rw-rw-rw-   0        0        0     5011 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/json_backup_output_v1.py
--rw-rw-rw-   0        0        0     4519 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/license_importer_output_v1.py
--rw-rw-rw-   0        0        0    12972 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/license_status_output_v1.py
--rw-rw-rw-   0        0        0     6391 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/licensed_feature_status_output_v1.py
--rw-rw-rw-   0        0        0     4854 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/log_message.py
--rw-rw-rw-   0        0        0     4861 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/meter_datum_v1.py
--rw-rw-rw-   0        0        0     3287 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/migrate_editor_input_v1.py
--rw-rw-rw-   0        0        0     4917 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/monitor_definition_output_v1.py
--rw-rw-rw-   0        0        0     3528 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/monitor_definitions_output_v1.py
--rw-rw-rw-   0        0        0     4686 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/monitor_input_v1.py
--rw-rw-rw-   0        0        0     3297 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/monitor_output_v1.py
--rw-rw-rw-   0        0        0    12784 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/monitor_values.py
--rw-rw-rw-   0        0        0     3272 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/monitors_output_v1.py
--rw-rw-rw-   0        0        0     9208 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/notifiable_report_output_list_v1.py
--rw-rw-rw-   0        0        0     8353 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/notifiable_report_output_v1.py
--rw-rw-rw-   0        0        0    12225 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/notification_configuration_output_v1.py
--rw-rw-rw-   0        0        0     6259 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/optional_report_input_v1.py
--rw-rw-rw-   0        0        0     6428 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/parameter_doc_output_v1.py
--rw-rw-rw-   0        0        0     4284 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/permissions_v1.py
--rw-rw-rw-   0        0        0     8516 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/plugin_output_list_v1.py
--rw-rw-rw-   0        0        0    17190 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/plugin_output_v1.py
--rw-rw-rw-   0        0        0     3196 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/plugins_body.py
--rw-rw-rw-   0        0        0     5101 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/priority_v1.py
--rw-rw-rw-   0        0        0     4145 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/progress_information_output_v1.py
--rw-rw-rw-   0        0        0    10448 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/project_input_v1.py
--rw-rw-rw-   0        0        0    21442 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/project_output_v1.py
--rw-rw-rw-   0        0        0     4395 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/property_href_output_v1.py
--rw-rw-rw-   0        0        0     4722 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/property_input_v1.py
--rw-rw-rw-   0        0        0     6718 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/property_output_v1.py
--rw-rw-rw-   0        0        0    13708 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/put_asset_input_v1.py
--rw-rw-rw-   0        0        0    19916 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/put_scalar_input_v1.py
--rw-rw-rw-   0        0        0     5969 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/put_scalars_input_v1.py
--rw-rw-rw-   0        0        0     3400 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/put_signals_input_v1.py
--rw-rw-rw-   0        0        0     3525 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/put_user_groups_input_v1.py
--rw-rw-rw-   0        0        0     3386 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/referenced_items_output_v1.py
--rw-rw-rw-   0        0        0    11559 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/regression_output_v1.py
--rw-rw-rw-   0        0        0     4713 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/remote_agent_directives_output_v1.py
--rw-rw-rw-   0        0        0    17039 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/remote_agent_status_input_v1.py
--rw-rw-rw-   0        0        0    17188 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/remote_agent_status_output_v1.py
--rw-rw-rw-   0        0        0     5303 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/report_input_item_v1.py
--rw-rw-rw-   0        0        0     4980 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/report_input_v1.py
--rw-rw-rw-   0        0        0     8317 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/report_notification_configuration_input_v1.py
--rw-rw-rw-   0        0        0     6423 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/report_template_input_v1.py
--rw-rw-rw-   0        0        0    15725 2023-03-07 21:47:07.000000 seeq-60.0.3/seeq/sdk/models/report_template_output_v1.py
--rw-rw-rw-   0        0        0    15680 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/request_output_v1.py
--rw-rw-rw-   0        0        0     4525 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/sample_input_v1.py
--rw-rw-rw-   0        0        0     4619 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/sample_output_v1.py
--rw-rw-rw-   0        0        0     3349 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/samples_input_v1.py
--rw-rw-rw-   0        0        0     3611 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/samples_output_v1.py
--rw-rw-rw-   0        0        0     4132 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/samples_overwrite_input_v1.py
--rw-rw-rw-   0        0        0    11589 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/scalar_evaluate_output_v1.py
--rw-rw-rw-   0        0        0    18252 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/scalar_input_v1.py
--rw-rw-rw-   0        0        0     5430 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/scalar_property_v1.py
--rw-rw-rw-   0        0        0     4918 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/scalar_value_output_v1.py
--rw-rw-rw-   0        0        0     4680 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/scale_across_tree_output_v1.py
--rw-rw-rw-   0        0        0     8794 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/schedulable_admin_list_output_v1.py
--rw-rw-rw-   0        0        0    16596 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/schedulable_admin_output_v1.py
--rw-rw-rw-   0        0        0     4354 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/schedulable_summary_day_output_v1.py
--rw-rw-rw-   0        0        0     3441 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/schedulable_summary_week_output_v1.py
--rw-rw-rw-   0        0        0     4354 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/schedule_input_v1.py
--rw-rw-rw-   0        0        0     5140 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/schedule_output_v1.py
--rw-rw-rw-   0        0        0     9294 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/scheduled_notebook_input_v1.py
--rw-rw-rw-   0        0        0     4749 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/scheduled_notebook_list_output_v1.py
--rw-rw-rw-   0        0        0    18032 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/scheduled_notebook_output_v1.py
--rw-rw-rw-   0        0        0     4463 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/screenshot_output_v1.py
--rw-rw-rw-   0        0        0     5893 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/see_also_doc_output_v1.py
--rw-rw-rw-   0        0        0     4852 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/send_logs_input_v1.py
--rw-rw-rw-   0        0        0     3459 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/server_build_info_output_v1.py
--rw-rw-rw-   0        0        0     4779 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/server_load_output_v1.py
--rw-rw-rw-   0        0        0     6642 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/server_spec_output_v1.py
--rw-rw-rw-   0        0        0    11298 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/server_status_output_v1.py
--rw-rw-rw-   0        0        0    18579 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/signal_input_v1.py
--rw-rw-rw-   0        0        0    28601 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/signal_output_v1.py
--rw-rw-rw-   0        0        0    23676 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/signal_with_id_input_v1.py
--rw-rw-rw-   0        0        0     3625 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/status_message_base.py
--rw-rw-rw-   0        0        0     4508 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/subscription_input_v1.py
--rw-rw-rw-   0        0        0     5009 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/subscription_output_v1.py
--rw-rw-rw-   0        0        0     3501 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/subscription_update_input_v1.py
--rw-rw-rw-   0        0        0     4440 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/supported_units_output_v1.py
--rw-rw-rw-   0        0        0     4347 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/swap_input_v1.py
--rw-rw-rw-   0        0        0     3669 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/swap_option_list_v1.py
--rw-rw-rw-   0        0        0     5739 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/swap_option_v1.py
--rw-rw-rw-   0        0        0     3922 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/swap_output_v1.py
--rw-rw-rw-   0        0        0    12118 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/sync_progress.py
--rw-rw-rw-   0        0        0    18435 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/sync_progress_output_v1.py
--rw-rw-rw-   0        0        0     3234 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/system_license_body.py
--rw-rw-rw-   0        0        0     4970 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/table_column_output_v1.py
--rw-rw-rw-   0        0        0    19657 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/threshold_metric_input_v1.py
--rw-rw-rw-   0        0        0    29029 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/threshold_metric_output_v1.py
--rw-rw-rw-   0        0        0     5228 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/threshold_output_v1.py
--rw-rw-rw-   0        0        0     4963 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/timer_datum_v1.py
--rw-rw-rw-   0        0        0    20741 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/tree_item_output_v1.py
--rw-rw-rw-   0        0        0     7490 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/treemap_item_output_v1.py
--rw-rw-rw-   0        0        0    10520 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/treemap_output_v1.py
--rw-rw-rw-   0        0        0     3665 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/units_of_measure_batch_input_v1.py
--rw-rw-rw-   0        0        0     4189 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/units_of_measure_item_v1.py
--rw-rw-rw-   0        0        0     3582 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/units_of_measure_output_v1.py
--rw-rw-rw-   0        0        0     4335 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/usage_output_list_v1.py
--rw-rw-rw-   0        0        0     9422 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/usage_output_v1.py
--rw-rw-rw-   0        0        0     3165 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/usage_types_v1.py
--rw-rw-rw-   0        0        0    10192 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/user_group_input_v1.py
--rw-rw-rw-   0        0        0    20240 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/user_group_output_v1.py
--rw-rw-rw-   0        0        0    13558 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/user_group_with_id_input_v1.py
--rw-rw-rw-   0        0        0    18567 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/user_input_v1.py
--rw-rw-rw-   0        0        0     8404 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/user_output_list_v1.py
--rw-rw-rw-   0        0        0    27119 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/user_output_v1.py
--rw-rw-rw-   0        0        0     4381 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/user_password_input_v1.py
--rw-rw-rw-   0        0        0     5631 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/validate_cron_list_input_v1.py
--rw-rw-rw-   0        0        0     3442 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/validate_cron_list_output_v1.py
--rw-rw-rw-   0        0        0     7318 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/validate_cron_output_v1.py
--rw-rw-rw-   0        0        0     9636 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/workbench_item_output_list_v1.py
--rw-rw-rw-   0        0        0    21275 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/workbench_search_result_preview_v1.py
--rw-rw-rw-   0        0        0     8518 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/workbook_input_v1.py
--rw-rw-rw-   0        0        0     7650 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/workbook_output_list_v1.py
--rw-rw-rw-   0        0        0    17362 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/workbook_output_v1.py
--rw-rw-rw-   0        0        0     4423 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/worksheet_input_v1.py
--rw-rw-rw-   0        0        0     7702 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/worksheet_output_list_v1.py
--rw-rw-rw-   0        0        0    13509 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/worksheet_output_v1.py
--rw-rw-rw-   0        0        0     3344 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/workstep_input_v1.py
--rw-rw-rw-   0        0        0    14298 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/models/workstep_output_v1.py
--rw-rw-rw-   0        0        0    13595 2023-03-07 21:47:08.000000 seeq-60.0.3/seeq/sdk/rest.py
-drwxrwxrwx   0        0        0        0 2023-03-07 21:47:12.000000 seeq-60.0.3/seeq.egg-info/
--rw-rw-rw-   0        0        0     3899 2023-03-07 21:47:11.000000 seeq-60.0.3/seeq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14625 2023-03-07 21:47:12.000000 seeq-60.0.3/seeq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 21:47:11.000000 seeq-60.0.3/seeq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 21:47:11.000000 seeq-60.0.3/seeq.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2023-03-07 21:47:11.000000 seeq-60.0.3/seeq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-07 21:47:11.000000 seeq-60.0.3/seeq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-07 21:47:13.000000 seeq-60.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1153 2023-03-07 21:44:12.000000 seeq-60.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-21 19:02:00.000000 seeq-60.1.1/
+-rw-rw-rw-   0        0        0    33551 2022-12-22 20:30:35.000000 seeq-60.1.1/LICENSE
+-rw-rw-rw-   0        0        0       19 2023-01-30 20:12:10.000000 seeq-60.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3899 2023-03-21 19:02:00.000000 seeq-60.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3399 2023-01-30 20:12:10.000000 seeq-60.1.1/README.md
+-rw-rw-rw-   0        0        0        0 2022-12-22 20:30:35.000000 seeq-60.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq/
+drwxrwxrwx   0        0        0        0 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq/sdk/
+-rw-rw-rw-   0        0        0    22319 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq/sdk/api/
+-rw-rw-rw-   0        0        0     1926 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/__init__.py
+-rw-rw-rw-   0        0        0    15283 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/access_keys_api.py
+-rw-rw-rw-   0        0        0    29040 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/add_ons_api.py
+-rw-rw-rw-   0        0        0   114203 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/agents_api.py
+-rw-rw-rw-   0        0        0    54586 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/annotations_api.py
+-rw-rw-rw-   0        0        0    23866 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/assets_api.py
+-rw-rw-rw-   0        0        0     8213 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/audit_api.py
+-rw-rw-rw-   0        0        0    13540 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/auth_api.py
+-rw-rw-rw-   0        0        0    27068 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/condition_monitors_api.py
+-rw-rw-rw-   0        0        0    51672 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/conditions_api.py
+-rw-rw-rw-   0        0        0   124777 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/content_api.py
+-rw-rw-rw-   0        0        0    34214 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/datafiles_api.py
+-rw-rw-rw-   0        0        0    41068 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/datasources_api.py
+-rw-rw-rw-   0        0        0    24826 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/display_templates_api.py
+-rw-rw-rw-   0        0        0    24099 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/displays_api.py
+-rw-rw-rw-   0        0        0    29830 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/export_api.py
+-rw-rw-rw-   0        0        0    49756 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/folders_api.py
+-rw-rw-rw-   0        0        0   102750 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/formulas_api.py
+-rw-rw-rw-   0        0        0   155303 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/items_api.py
+-rw-rw-rw-   0        0        0    29740 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/jobs_api.py
+-rw-rw-rw-   0        0        0    21182 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/logs_api.py
+-rw-rw-rw-   0        0        0    24406 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/metrics_api.py
+-rw-rw-rw-   0        0        0    31687 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/monitors_api.py
+-rw-rw-rw-   0        0        0     5941 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/networks_api.py
+-rw-rw-rw-   0        0        0    26044 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/notification_configurations_api.py
+-rw-rw-rw-   0        0        0    21303 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/plugins_api.py
+-rw-rw-rw-   0        0        0    35172 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/projects_api.py
+-rw-rw-rw-   0        0        0    24398 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/report_templates_api.py
+-rw-rw-rw-   0        0        0     5736 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/reports_api.py
+-rw-rw-rw-   0        0        0    37825 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/requests_api.py
+-rw-rw-rw-   0        0        0    28228 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/scalars_api.py
+-rw-rw-rw-   0        0        0   111043 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/signals_api.py
+-rw-rw-rw-   0        0        0    20428 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/subscriptions_api.py
+-rw-rw-rw-   0        0        0    99316 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/system_api.py
+-rw-rw-rw-   0        0        0    65360 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/trees_api.py
+-rw-rw-rw-   0        0        0    12493 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/usage_api.py
+-rw-rw-rw-   0        0        0    51919 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/user_groups_api.py
+-rw-rw-rw-   0        0        0    49412 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/users_api.py
+-rw-rw-rw-   0        0        0    93533 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api/workbooks_api.py
+-rw-rw-rw-   0        0        0    30256 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/api_client.py
+-rw-rw-rw-   0        0        0     9431 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/configuration.py
+drwxrwxrwx   0        0        0        0 2023-03-21 19:02:00.000000 seeq-60.1.1/seeq/sdk/models/
+-rw-rw-rw-   0        0        0    18310 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/__init__.py
+-rw-rw-rw-   0        0        0     4424 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/access_key_input_v1.py
+-rw-rw-rw-   0        0        0     7578 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/access_key_output_list_v1.py
+-rw-rw-rw-   0        0        0    14950 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/access_key_output_v1.py
+-rw-rw-rw-   0        0        0     4247 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/ace_input_v1.py
+-rw-rw-rw-   0        0        0     5948 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/ace_output_v1.py
+-rw-rw-rw-   0        0        0     6980 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/acl_input_v1.py
+-rw-rw-rw-   0        0        0     6783 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/acl_output_v1.py
+-rw-rw-rw-   0        0        0     3713 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/activity_graph_output_v1.py
+-rw-rw-rw-   0        0        0     7607 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/activity_output_v1.py
+-rw-rw-rw-   0        0        0     8832 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/add_on_input_v1.py
+-rw-rw-rw-   0        0        0     7521 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/add_on_output_list_v1.py
+-rw-rw-rw-   0        0        0    14831 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/add_on_output_v1.py
+-rw-rw-rw-   0        0        0     7763 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/add_on_preview_output_list_v1.py
+-rw-rw-rw-   0        0        0     6748 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/add_on_preview_v1.py
+-rw-rw-rw-   0        0        0    11430 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/add_on_tool_input_v1.py
+-rw-rw-rw-   0        0        0    16207 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/add_on_tool_output_v1.py
+-rw-rw-rw-   0        0        0     4285 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/administrator_contact_information_v1.py
+-rw-rw-rw-   0        0        0     5019 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/agent_input_v1.py
+-rw-rw-rw-   0        0        0     3238 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/agent_key_output_v1.py
+-rw-rw-rw-   0        0        0    12658 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/agent_output_v1.py
+-rw-rw-rw-   0        0        0     8084 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/agent_status_output_v1.py
+-rw-rw-rw-   0        0        0     8091 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/agent_status_v1.py
+-rw-rw-rw-   0        0        0     4420 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/annotation_image_link_output_v1.py
+-rw-rw-rw-   0        0        0    11395 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/annotation_input_v1.py
+-rw-rw-rw-   0        0        0     4365 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/annotation_interest_input_v1.py
+-rw-rw-rw-   0        0        0     3884 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/annotation_interest_output_v1.py
+-rw-rw-rw-   0        0        0     7642 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/annotation_list_output_v1.py
+-rw-rw-rw-   0        0        0    28089 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/annotation_output_v1.py
+-rw-rw-rw-   0        0        0     4571 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/archive_output_v1.py
+-rw-rw-rw-   0        0        0     4316 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_batch_input_v1.py
+-rw-rw-rw-   0        0        0     4853 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_error.py
+-rw-rw-rw-   0        0        0    15161 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_group_asset_input_v1.py
+-rw-rw-rw-   0        0        0     4174 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_group_input_v1.py
+-rw-rw-rw-   0        0        0     4105 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_group_output_v1.py
+-rw-rw-rw-   0        0        0    14208 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_group_root_input_v1.py
+-rw-rw-rw-   0        0        0     6682 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_group_tree_output_v1.py
+-rw-rw-rw-   0        0        0    12120 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_input_v1.py
+-rw-rw-rw-   0        0        0    18126 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_output_v1.py
+-rw-rw-rw-   0        0        0     8745 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_selection_input_v1.py
+-rw-rw-rw-   0        0        0    14359 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_selection_output_v1.py
+-rw-rw-rw-   0        0        0     9597 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_tree_batch_input_v1.py
+-rw-rw-rw-   0        0        0    11597 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_tree_output_v1.py
+-rw-rw-rw-   0        0        0     4570 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/asset_tree_single_input_v1.py
+-rw-rw-rw-   0        0        0     8470 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/audit_output_list_v1.py
+-rw-rw-rw-   0        0        0     9984 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/audit_output_v1.py
+-rw-rw-rw-   0        0        0     7325 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/auth_input_v1.py
+-rw-rw-rw-   0        0        0     3554 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/auth_providers_output_v1.py
+-rw-rw-rw-   0        0        0     4227 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/cache_info_v1.py
+-rw-rw-rw-   0        0        0    21392 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/calculated_item_output_v1.py
+-rw-rw-rw-   0        0        0     5502 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/capsule_input_v1.py
+-rw-rw-rw-   0        0        0     4490 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/capsule_property_input_v1.py
+-rw-rw-rw-   0        0        0     4301 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/capsule_property_output_v1.py
+-rw-rw-rw-   0        0        0     8310 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/capsule_v1.py
+-rw-rw-rw-   0        0        0     3371 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/capsules_input_v1.py
+-rw-rw-rw-   0        0        0    10722 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/capsules_output_v1.py
+-rw-rw-rw-   0        0        0     4158 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/capsules_overwrite_input_v1.py
+-rw-rw-rw-   0        0        0     7478 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/channel_output_v1.py
+-rw-rw-rw-   0        0        0     3521 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/condition_batch_input_v1.py
+-rw-rw-rw-   0        0        0    21085 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/condition_input_v1.py
+-rw-rw-rw-   0        0        0     9108 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/condition_monitor_input_v1.py
+-rw-rw-rw-   0        0        0    11175 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py
+-rw-rw-rw-   0        0        0    17800 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/condition_monitor_output_v1.py
+-rw-rw-rw-   0        0        0    25193 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/condition_output_v1.py
+-rw-rw-rw-   0        0        0    24419 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/condition_update_input_v1.py
+-rw-rw-rw-   0        0        0     4198 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/configuration_input_v1.py
+-rw-rw-rw-   0        0        0     4436 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/configuration_option_input_v1.py
+-rw-rw-rw-   0        0        0     3882 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/configuration_option_output_simple_v1.py
+-rw-rw-rw-   0        0        0    12749 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/configuration_option_output_v1.py
+-rw-rw-rw-   0        0        0     8957 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/configuration_output_v1.py
+-rw-rw-rw-   0        0        0     5125 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/configured_directives_output_v1.py
+-rw-rw-rw-   0        0        0     8805 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/connection_input_v1.py
+-rw-rw-rw-   0        0        0    22910 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/connection_output_v1.py
+-rw-rw-rw-   0        0        0    17645 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/connection_status_output_v1.py
+-rw-rw-rw-   0        0        0    17370 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/connection_status_v1.py
+-rw-rw-rw-   0        0        0     3363 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/connections_output_v1.py
+-rw-rw-rw-   0        0        0     5107 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/connector_input_v1.py
+-rw-rw-rw-   0        0        0    13652 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/connector_output_v1.py
+-rw-rw-rw-   0        0        0     3383 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/connectors_output_v1.py
+-rw-rw-rw-   0        0        0    16191 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/content_input_v1.py
+-rw-rw-rw-   0        0        0    24079 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/content_output_v1.py
+-rw-rw-rw-   0        0        0     5464 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/content_with_metadata_list_output_v1.py
+-rw-rw-rw-   0        0        0    30123 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/content_with_metadata_output_v1.py
+-rw-rw-rw-   0        0        0     3558 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/csv_datafile_output_v1.py
+-rw-rw-rw-   0        0        0    51259 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datafile_input_v1.py
+-rw-rw-rw-   0        0        0    55080 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datafile_output_v1.py
+-rw-rw-rw-   0        0        0     3227 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datafiles_csv_body.py
+-rw-rw-rw-   0        0        0     9859 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_clean_up_input_v1.py
+-rw-rw-rw-   0        0        0     3665 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_clean_up_output_v1.py
+-rw-rw-rw-   0        0        0    13625 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_input_v1.py
+-rw-rw-rw-   0        0        0     7754 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_output_list_v1.py
+-rw-rw-rw-   0        0        0    20696 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_output_v1.py
+-rw-rw-rw-   0        0        0     9118 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_preview_v1.py
+-rw-rw-rw-   0        0        0    16264 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_statistics_v1.py
+-rw-rw-rw-   0        0        0     8969 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_status_output_v1.py
+-rw-rw-rw-   0        0        0     9422 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_status_v1.py
+-rw-rw-rw-   0        0        0    25599 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasource_summary_status_output_v1.py
+-rw-rw-rw-   0        0        0    10331 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/datasources_status_output_v1.py
+-rw-rw-rw-   0        0        0    10061 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/date_range_input_v1.py
+-rw-rw-rw-   0        0        0    17474 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/date_range_output_v1.py
+-rw-rw-rw-   0        0        0     5034 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/detailed_meter_output_v1.py
+-rw-rw-rw-   0        0        0     5921 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/detailed_timer_output_v1.py
+-rw-rw-rw-   0        0        0     5213 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/directive_input_v1.py
+-rw-rw-rw-   0        0        0     5410 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/display_input_v1.py
+-rw-rw-rw-   0        0        0     7604 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/display_output_list_v1.py
+-rw-rw-rw-   0        0        0    15213 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/display_output_v1.py
+-rw-rw-rw-   0        0        0     9715 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/display_template_input_v1.py
+-rw-rw-rw-   0        0        0     8041 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/display_template_output_list_v1.py
+-rw-rw-rw-   0        0        0    16432 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/display_template_output_v1.py
+-rw-rw-rw-   0        0        0     5065 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/document_backup_output_v1.py
+-rw-rw-rw-   0        0        0     5511 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/email_notification_recipient_output_v1.py
+-rw-rw-rw-   0        0        0     5516 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/export_item_v1.py
+-rw-rw-rw-   0        0        0    19425 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/export_items_output_v1.py
+-rw-rw-rw-   0        0        0    19068 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/export_items_v1.py
+-rw-rw-rw-   0        0        0     7536 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/export_preview_list_v1.py
+-rw-rw-rw-   0        0        0    11091 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/export_preview_v1.py
+-rw-rw-rw-   0        0        0     6728 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/folded_stack_node_v1.py
+-rw-rw-rw-   0        0        0     7908 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/folder_input_v1.py
+-rw-rw-rw-   0        0        0     5896 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/folder_navigation_output_v1.py
+-rw-rw-rw-   0        0        0    16393 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/folder_output_v1.py
+-rw-rw-rw-   0        0        0     7095 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_compile_output_v1.py
+-rw-rw-rw-   0        0        0     8391 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_compiler_error_output_v1.py
+-rw-rw-rw-   0        0        0     4472 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_dependency_input_v1.py
+-rw-rw-rw-   0        0        0     4144 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_doc_example_input_v1.py
+-rw-rw-rw-   0        0        0     3576 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_doc_example_list_input_v1.py
+-rw-rw-rw-   0        0        0     7635 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_doc_input_v1.py
+-rw-rw-rw-   0        0        0     3527 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_doc_keyword_list_input_v1.py
+-rw-rw-rw-   0        0        0    22305 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_doc_output_v1.py
+-rw-rw-rw-   0        0        0     3336 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_doc_summaries_output_v1.py
+-rw-rw-rw-   0        0        0     8541 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_doc_summary_output_v1.py
+-rw-rw-rw-   0        0        0     8499 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_error_output_v1.py
+-rw-rw-rw-   0        0        0     4090 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_example_output_v1.py
+-rw-rw-rw-   0        0        0    19458 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_item_input_v1.py
+-rw-rw-rw-   0        0        0    19412 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_item_output_v1.py
+-rw-rw-rw-   0        0        0     4067 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_log_entry.py
+-rw-rw-rw-   0        0        0     3852 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_log_entry_details.py
+-rw-rw-rw-   0        0        0     4593 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_log_v1.py
+-rw-rw-rw-   0        0        0     6969 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_package_import_input_v1.py
+-rw-rw-rw-   0        0        0     6252 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_package_import_output_v1.py
+-rw-rw-rw-   0        0        0     9638 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_package_input_v1.py
+-rw-rw-rw-   0        0        0    18453 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_package_output_v1.py
+-rw-rw-rw-   0        0        0     6385 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_parameter_input_v1.py
+-rw-rw-rw-   0        0        0     5766 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_parameter_output_v1.py
+-rw-rw-rw-   0        0        0    13985 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_run_input_v1.py
+-rw-rw-rw-   0        0        0    12686 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_run_output_v1.py
+-rw-rw-rw-   0        0        0     4237 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_token.py
+-rw-rw-rw-   0        0        0     4204 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_update_input_v1.py
+-rw-rw-rw-   0        0        0     4246 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_upgrade_change_v1.py
+-rw-rw-rw-   0        0        0     5098 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/formula_upgrade_output_v1.py
+-rw-rw-rw-   0        0        0    14037 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/function_input_v1.py
+-rw-rw-rw-   0        0        0     4760 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/function_parameter_output_v1.py
+-rw-rw-rw-   0        0        0     6549 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/function_variant_output_v1.py
+-rw-rw-rw-   0        0        0     5004 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/gauge_datum_v1.py
+-rw-rw-rw-   0        0        0     4299 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/generic_table_output_v1.py
+-rw-rw-rw-   0        0        0     3396 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_add_on_tools_output_v1.py
+-rw-rw-rw-   0        0        0     7594 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_channels_output_v1.py
+-rw-rw-rw-   0        0        0     9468 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_condition_monitor_items_output_v1.py
+-rw-rw-rw-   0        0        0     7811 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_content_items_output_v1.py
+-rw-rw-rw-   0        0        0     7719 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_date_ranges_output_v1.py
+-rw-rw-rw-   0        0        0     7386 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_jobs_output_v1.py
+-rw-rw-rw-   0        0        0     7569 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_metrics_output_v1.py
+-rw-rw-rw-   0        0        0     7598 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_projects_output_v1.py
+-rw-rw-rw-   0        0        0     4327 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_request_output_v1.py
+-rw-rw-rw-   0        0        0     3230 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_requests_output_v1.py
+-rw-rw-rw-   0        0        0     6413 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_sample_output_v1.py
+-rw-rw-rw-   0        0        0    11687 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_samples_output_v1.py
+-rw-rw-rw-   0        0        0     7542 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/get_signals_output_v1.py
+-rw-rw-rw-   0        0        0     3199 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/id_images_body.py
+-rw-rw-rw-   0        0        0     3651 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/identity_mapping_list_v1.py
+-rw-rw-rw-   0        0        0     6419 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/identity_mapping_v1.py
+-rw-rw-rw-   0        0        0     8628 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/identity_preview_list_v1.py
+-rw-rw-rw-   0        0        0    12439 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/identity_preview_v1.py
+-rw-rw-rw-   0        0        0     4350 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/indexing_parameters_input_v1.py
+-rw-rw-rw-   0        0        0     5113 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/installer_output_v1.py
+-rw-rw-rw-   0        0        0     4274 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/interval_v1.py
+-rw-rw-rw-   0        0        0     3105 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/invalid_swap_out_v1.py
+-rw-rw-rw-   0        0        0     4628 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_batch_output_v1.py
+-rw-rw-rw-   0        0        0    11919 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_dependency_output_v1.py
+-rw-rw-rw-   0        0        0     3280 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_id_list_input_v1.py
+-rw-rw-rw-   0        0        0    15155 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_output_v1.py
+-rw-rw-rw-   0        0        0    11643 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_parameter_of_output_v1.py
+-rw-rw-rw-   0        0        0     8458 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_preview_list_v1.py
+-rw-rw-rw-   0        0        0     7190 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_preview_v1.py
+-rw-rw-rw-   0        0        0     9797 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_preview_with_assets_v1.py
+-rw-rw-rw-   0        0        0     4334 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_search_preview_list_v1.py
+-rw-rw-rw-   0        0        0     8941 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_search_preview_paginated_list_v1.py
+-rw-rw-rw-   0        0        0    14582 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_search_preview_v1.py
+-rw-rw-rw-   0        0        0     4870 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_swap_result_output_v1.py
+-rw-rw-rw-   0        0        0     6757 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_update_output_v1.py
+-rw-rw-rw-   0        0        0     4356 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_user_attributes_input_v1.py
+-rw-rw-rw-   0        0        0     6082 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_user_attributes_output_v1.py
+-rw-rw-rw-   0        0        0     5314 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/item_with_swap_pairs_v1.py
+-rw-rw-rw-   0        0        0    11915 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/job_output_v1.py
+-rw-rw-rw-   0        0        0     5011 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/json_backup_output_v1.py
+-rw-rw-rw-   0        0        0     4519 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/license_importer_output_v1.py
+-rw-rw-rw-   0        0        0    12972 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/license_status_output_v1.py
+-rw-rw-rw-   0        0        0     6391 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/licensed_feature_status_output_v1.py
+-rw-rw-rw-   0        0        0     4854 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/log_message.py
+-rw-rw-rw-   0        0        0     4861 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/meter_datum_v1.py
+-rw-rw-rw-   0        0        0     3287 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/migrate_editor_input_v1.py
+-rw-rw-rw-   0        0        0     4917 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/monitor_definition_output_v1.py
+-rw-rw-rw-   0        0        0     3528 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/monitor_definitions_output_v1.py
+-rw-rw-rw-   0        0        0     4686 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/monitor_input_v1.py
+-rw-rw-rw-   0        0        0     3297 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/monitor_output_v1.py
+-rw-rw-rw-   0        0        0    12784 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/monitor_values.py
+-rw-rw-rw-   0        0        0     3272 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/monitors_output_v1.py
+-rw-rw-rw-   0        0        0     9208 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/notifiable_report_output_list_v1.py
+-rw-rw-rw-   0        0        0     8353 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/notifiable_report_output_v1.py
+-rw-rw-rw-   0        0        0    12225 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/notification_configuration_output_v1.py
+-rw-rw-rw-   0        0        0     6259 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/optional_report_input_v1.py
+-rw-rw-rw-   0        0        0     6428 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/parameter_doc_output_v1.py
+-rw-rw-rw-   0        0        0     4284 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/permissions_v1.py
+-rw-rw-rw-   0        0        0     8516 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/plugin_output_list_v1.py
+-rw-rw-rw-   0        0        0    17190 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/plugin_output_v1.py
+-rw-rw-rw-   0        0        0     3196 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/plugins_body.py
+-rw-rw-rw-   0        0        0     5101 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/priority_v1.py
+-rw-rw-rw-   0        0        0     4145 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/progress_information_output_v1.py
+-rw-rw-rw-   0        0        0    10448 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/project_input_v1.py
+-rw-rw-rw-   0        0        0    21442 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/project_output_v1.py
+-rw-rw-rw-   0        0        0     4395 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/property_href_output_v1.py
+-rw-rw-rw-   0        0        0     4722 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/property_input_v1.py
+-rw-rw-rw-   0        0        0     6718 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/property_output_v1.py
+-rw-rw-rw-   0        0        0    13708 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/put_asset_input_v1.py
+-rw-rw-rw-   0        0        0    19916 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/put_scalar_input_v1.py
+-rw-rw-rw-   0        0        0     5969 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/put_scalars_input_v1.py
+-rw-rw-rw-   0        0        0     3400 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/put_signals_input_v1.py
+-rw-rw-rw-   0        0        0     3525 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/put_user_groups_input_v1.py
+-rw-rw-rw-   0        0        0     3386 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/referenced_items_output_v1.py
+-rw-rw-rw-   0        0        0    11559 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/regression_output_v1.py
+-rw-rw-rw-   0        0        0     4713 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/remote_agent_directives_output_v1.py
+-rw-rw-rw-   0        0        0    17039 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/remote_agent_status_input_v1.py
+-rw-rw-rw-   0        0        0    17188 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/remote_agent_status_output_v1.py
+-rw-rw-rw-   0        0        0     5303 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/report_input_item_v1.py
+-rw-rw-rw-   0        0        0     4980 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/report_input_v1.py
+-rw-rw-rw-   0        0        0     8317 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/report_notification_configuration_input_v1.py
+-rw-rw-rw-   0        0        0     6423 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/report_template_input_v1.py
+-rw-rw-rw-   0        0        0    15725 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/report_template_output_v1.py
+-rw-rw-rw-   0        0        0    15680 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/request_output_v1.py
+-rw-rw-rw-   0        0        0     4525 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/sample_input_v1.py
+-rw-rw-rw-   0        0        0     4619 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/sample_output_v1.py
+-rw-rw-rw-   0        0        0     3349 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/samples_input_v1.py
+-rw-rw-rw-   0        0        0     3611 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/samples_output_v1.py
+-rw-rw-rw-   0        0        0     4132 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/samples_overwrite_input_v1.py
+-rw-rw-rw-   0        0        0    11589 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/scalar_evaluate_output_v1.py
+-rw-rw-rw-   0        0        0    18252 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/scalar_input_v1.py
+-rw-rw-rw-   0        0        0     5430 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/scalar_property_v1.py
+-rw-rw-rw-   0        0        0     4918 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/scalar_value_output_v1.py
+-rw-rw-rw-   0        0        0     4680 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/scale_across_tree_output_v1.py
+-rw-rw-rw-   0        0        0     8794 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/schedulable_admin_list_output_v1.py
+-rw-rw-rw-   0        0        0    16596 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/schedulable_admin_output_v1.py
+-rw-rw-rw-   0        0        0     4354 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/schedulable_summary_day_output_v1.py
+-rw-rw-rw-   0        0        0     3441 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/schedulable_summary_week_output_v1.py
+-rw-rw-rw-   0        0        0     4354 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/schedule_input_v1.py
+-rw-rw-rw-   0        0        0     5140 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/schedule_output_v1.py
+-rw-rw-rw-   0        0        0     9294 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/scheduled_notebook_input_v1.py
+-rw-rw-rw-   0        0        0     4749 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/scheduled_notebook_list_output_v1.py
+-rw-rw-rw-   0        0        0    18032 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/scheduled_notebook_output_v1.py
+-rw-rw-rw-   0        0        0     4463 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/screenshot_output_v1.py
+-rw-rw-rw-   0        0        0     5893 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/see_also_doc_output_v1.py
+-rw-rw-rw-   0        0        0     4852 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/send_logs_input_v1.py
+-rw-rw-rw-   0        0        0     3459 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/server_build_info_output_v1.py
+-rw-rw-rw-   0        0        0     4779 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/server_load_output_v1.py
+-rw-rw-rw-   0        0        0     6642 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/server_spec_output_v1.py
+-rw-rw-rw-   0        0        0    11298 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/server_status_output_v1.py
+-rw-rw-rw-   0        0        0    18579 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/signal_input_v1.py
+-rw-rw-rw-   0        0        0    28601 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/signal_output_v1.py
+-rw-rw-rw-   0        0        0    23676 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/signal_with_id_input_v1.py
+-rw-rw-rw-   0        0        0     3625 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/status_message_base.py
+-rw-rw-rw-   0        0        0     4508 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/subscription_input_v1.py
+-rw-rw-rw-   0        0        0     5009 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/subscription_output_v1.py
+-rw-rw-rw-   0        0        0     3501 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/subscription_update_input_v1.py
+-rw-rw-rw-   0        0        0     4440 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/supported_units_output_v1.py
+-rw-rw-rw-   0        0        0     4347 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/swap_input_v1.py
+-rw-rw-rw-   0        0        0     3669 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/swap_option_list_v1.py
+-rw-rw-rw-   0        0        0     5739 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/swap_option_v1.py
+-rw-rw-rw-   0        0        0     3922 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/swap_output_v1.py
+-rw-rw-rw-   0        0        0    12118 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/sync_progress.py
+-rw-rw-rw-   0        0        0    18435 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/sync_progress_output_v1.py
+-rw-rw-rw-   0        0        0     3234 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/system_license_body.py
+-rw-rw-rw-   0        0        0     4970 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/table_column_output_v1.py
+-rw-rw-rw-   0        0        0    19657 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/threshold_metric_input_v1.py
+-rw-rw-rw-   0        0        0    29029 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/threshold_metric_output_v1.py
+-rw-rw-rw-   0        0        0     5228 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/threshold_output_v1.py
+-rw-rw-rw-   0        0        0     4963 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/timer_datum_v1.py
+-rw-rw-rw-   0        0        0    20741 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/tree_item_output_v1.py
+-rw-rw-rw-   0        0        0     7490 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/treemap_item_output_v1.py
+-rw-rw-rw-   0        0        0    10520 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/treemap_output_v1.py
+-rw-rw-rw-   0        0        0     3665 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/units_of_measure_batch_input_v1.py
+-rw-rw-rw-   0        0        0     4189 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/units_of_measure_item_v1.py
+-rw-rw-rw-   0        0        0     3582 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/units_of_measure_output_v1.py
+-rw-rw-rw-   0        0        0     4335 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/usage_output_list_v1.py
+-rw-rw-rw-   0        0        0     9422 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/usage_output_v1.py
+-rw-rw-rw-   0        0        0     3165 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/usage_types_v1.py
+-rw-rw-rw-   0        0        0    10192 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/user_group_input_v1.py
+-rw-rw-rw-   0        0        0    20240 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/user_group_output_v1.py
+-rw-rw-rw-   0        0        0    13558 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/user_group_with_id_input_v1.py
+-rw-rw-rw-   0        0        0    18567 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/user_input_v1.py
+-rw-rw-rw-   0        0        0     8404 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/user_output_list_v1.py
+-rw-rw-rw-   0        0        0    27119 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/user_output_v1.py
+-rw-rw-rw-   0        0        0     4381 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/user_password_input_v1.py
+-rw-rw-rw-   0        0        0     5631 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/validate_cron_list_input_v1.py
+-rw-rw-rw-   0        0        0     3442 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/validate_cron_list_output_v1.py
+-rw-rw-rw-   0        0        0     7318 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/validate_cron_output_v1.py
+-rw-rw-rw-   0        0        0     9636 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/workbench_item_output_list_v1.py
+-rw-rw-rw-   0        0        0    21275 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/workbench_search_result_preview_v1.py
+-rw-rw-rw-   0        0        0     8518 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/workbook_input_v1.py
+-rw-rw-rw-   0        0        0     7650 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/workbook_output_list_v1.py
+-rw-rw-rw-   0        0        0    17362 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/workbook_output_v1.py
+-rw-rw-rw-   0        0        0     4423 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/worksheet_input_v1.py
+-rw-rw-rw-   0        0        0     7702 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/worksheet_output_list_v1.py
+-rw-rw-rw-   0        0        0    13509 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/worksheet_output_v1.py
+-rw-rw-rw-   0        0        0     3344 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/workstep_input_v1.py
+-rw-rw-rw-   0        0        0    14298 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/models/workstep_output_v1.py
+-rw-rw-rw-   0        0        0    13595 2023-03-21 19:01:57.000000 seeq-60.1.1/seeq/sdk/rest.py
+drwxrwxrwx   0        0        0        0 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq.egg-info/
+-rw-rw-rw-   0        0        0     3899 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14625 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-03-21 19:01:59.000000 seeq-60.1.1/seeq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-21 19:02:00.000000 seeq-60.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1153 2023-03-21 18:59:54.000000 seeq-60.1.1/setup.py
```

### Comparing `seeq-60.0.3/LICENSE` & `seeq-60.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-60.0.3/PKG-INFO` & `seeq-60.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq
-Version: 60.0.3
+Version: 60.1.1
 Summary: The Seeq SDK for Python
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-60.0.3/README.md` & `seeq-60.1.1/README.md`

 * *Files identical despite different names*

### Comparing `seeq-60.0.3/seeq/sdk/__init__.py` & `seeq-60.1.1/seeq/sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "60.0.3"
+__version__ = "60.1.1"
 
 # import apis into sdk package
 from .api.access_keys_api import AccessKeysApi
 from .api.add_ons_api import AddOnsApi
 from .api.agents_api import AgentsApi
 from .api.annotations_api import AnnotationsApi
 from .api.assets_api import AssetsApi
```

### Comparing `seeq-60.0.3/seeq/sdk/api/__init__.py` & `seeq-60.1.1/seeq/sdk/api/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "60.0.3"
+__version__ = "60.1.1"
 
 # import apis into sdk package
 from .access_keys_api import AccessKeysApi
 from .add_ons_api import AddOnsApi
 from .agents_api import AgentsApi
 from .annotations_api import AnnotationsApi
 from .assets_api import AssetsApi
```

### Comparing `seeq-60.0.3/seeq/sdk/api/access_keys_api.py` & `seeq-60.1.1/seeq/sdk/api/access_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/add_ons_api.py` & `seeq-60.1.1/seeq/sdk/api/add_ons_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/agents_api.py` & `seeq-60.1.1/seeq/sdk/api/agents_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/annotations_api.py` & `seeq-60.1.1/seeq/sdk/api/annotations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/assets_api.py` & `seeq-60.1.1/seeq/sdk/api/assets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/audit_api.py` & `seeq-60.1.1/seeq/sdk/api/audit_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/auth_api.py` & `seeq-60.1.1/seeq/sdk/api/auth_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/condition_monitors_api.py` & `seeq-60.1.1/seeq/sdk/api/condition_monitors_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/conditions_api.py` & `seeq-60.1.1/seeq/sdk/api/conditions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/content_api.py` & `seeq-60.1.1/seeq/sdk/api/content_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/datafiles_api.py` & `seeq-60.1.1/seeq/sdk/api/datafiles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/datasources_api.py` & `seeq-60.1.1/seeq/sdk/api/datasources_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/display_templates_api.py` & `seeq-60.1.1/seeq/sdk/api/display_templates_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/displays_api.py` & `seeq-60.1.1/seeq/sdk/api/displays_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/export_api.py` & `seeq-60.1.1/seeq/sdk/api/export_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/folders_api.py` & `seeq-60.1.1/seeq/sdk/api/folders_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/formulas_api.py` & `seeq-60.1.1/seeq/sdk/api/formulas_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 00000050: 2062 7920 5377 6167 6765 7220 436f 6465   by Swagger Code
 00000060: 6765 6e20 6874 7470 733a 2f2f 6769 7468  gen https://gith
 00000070: 7562 2e63 6f6d 2f73 7761 6767 6572 2d61  ub.com/swagger-a
 00000080: 7069 2f73 7761 6767 6572 2d63 6f64 6567  pi/swagger-codeg
 00000090: 656e 2920 2023 206e 6f71 613a 2045 3530  en)  # noqa: E50
 000000a0: 310a 0a20 2020 204f 7065 6e41 5049 2073  1..    OpenAPI s
 000000b0: 7065 6320 7665 7273 696f 6e3a 2036 302e  pec version: 60.
-000000c0: 302e 332d 534e 4150 5348 4f54 0a20 2020  0.3-SNAPSHOT.   
+000000c0: 312e 312d 534e 4150 5348 4f54 0a20 2020  1.1-SNAPSHOT.   
 000000d0: 200a 2020 2020 4765 6e65 7261 7465 6420   .    Generated 
 000000e0: 6279 3a20 6874 7470 733a 2f2f 6769 7468  by: https://gith
 000000f0: 7562 2e63 6f6d 2f73 7761 6767 6572 2d61  ub.com/swagger-a
 00000100: 7069 2f73 7761 6767 6572 2d63 6f64 6567  pi/swagger-codeg
 00000110: 656e 2e67 6974 0a22 2222 0a0d 0a66 726f  en.git."""...fro
 00000120: 6d20 5f5f 6675 7475 7265 5f5f 2069 6d70  m __future__ imp
 00000130: 6f72 7420 6162 736f 6c75 7465 5f69 6d70  ort absolute_imp
```

### Comparing `seeq-60.0.3/seeq/sdk/api/items_api.py` & `seeq-60.1.1/seeq/sdk/api/items_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/jobs_api.py` & `seeq-60.1.1/seeq/sdk/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/logs_api.py` & `seeq-60.1.1/seeq/sdk/api/logs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/metrics_api.py` & `seeq-60.1.1/seeq/sdk/api/metrics_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/monitors_api.py` & `seeq-60.1.1/seeq/sdk/api/monitors_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/networks_api.py` & `seeq-60.1.1/seeq/sdk/api/networks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/notification_configurations_api.py` & `seeq-60.1.1/seeq/sdk/api/notification_configurations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/plugins_api.py` & `seeq-60.1.1/seeq/sdk/api/plugins_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/projects_api.py` & `seeq-60.1.1/seeq/sdk/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/report_templates_api.py` & `seeq-60.1.1/seeq/sdk/api/report_templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/reports_api.py` & `seeq-60.1.1/seeq/sdk/api/reports_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/requests_api.py` & `seeq-60.1.1/seeq/sdk/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/scalars_api.py` & `seeq-60.1.1/seeq/sdk/api/scalars_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/signals_api.py` & `seeq-60.1.1/seeq/sdk/api/signals_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/subscriptions_api.py` & `seeq-60.1.1/seeq/sdk/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/system_api.py` & `seeq-60.1.1/seeq/sdk/api/system_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/trees_api.py` & `seeq-60.1.1/seeq/sdk/api/trees_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/usage_api.py` & `seeq-60.1.1/seeq/sdk/api/usage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/user_groups_api.py` & `seeq-60.1.1/seeq/sdk/api/user_groups_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/users_api.py` & `seeq-60.1.1/seeq/sdk/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api/workbooks_api.py` & `seeq-60.1.1/seeq/sdk/api/workbooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-60.0.3/seeq/sdk/api_client.py` & `seeq-60.1.1/seeq/sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import json
 import mimetypes
@@ -72,15 +72,15 @@
             self.default_headers[header_name] = header_value
         if host is None:
             self.host = self.configuration.host
         else:
             self.host = host
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/60.0.3/python'
+        self.user_agent = 'Swagger-Codegen/60.1.1/python'
         self.auth_token = None
         self.csrf_token = None
 
     @property
     def user_agent(self):
         """
         Gets user agent.
```

### Comparing `seeq-60.0.3/seeq/sdk/configuration.py` & `seeq-60.1.1/seeq/sdk/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import urllib3
@@ -250,16 +250,16 @@
         Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 60.0.3-SNAPSHOT\n"\
-               "SDK Package Version: 60.0.3".\
+               "Version of the API: 60.1.1-SNAPSHOT\n"\
+               "SDK Package Version: 60.1.1".\
                format(env=sys.platform, pyversion=sys.version)
 
 
 default_configuration = ClientConfiguration()
 
 
 def Configuration():
```

### Comparing `seeq-60.0.3/seeq/sdk/models/__init__.py` & `seeq-60.1.1/seeq/sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "60.0.3"
+__version__ = "60.1.1"
 
 # import models into sdk package
 from .access_key_input_v1 import AccessKeyInputV1
 from .access_key_output_list_v1 import AccessKeyOutputListV1
 from .access_key_output_v1 import AccessKeyOutputV1
 from .ace_input_v1 import AceInputV1
 from .ace_output_v1 import AceOutputV1
```

### Comparing `seeq-60.0.3/seeq/sdk/models/access_key_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/access_key_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/access_key_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/access_key_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/access_key_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/access_key_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/ace_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/ace_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/ace_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/ace_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/acl_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/acl_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/acl_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/acl_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/activity_graph_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/activity_graph_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/activity_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/activity_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/add_on_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/add_on_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/add_on_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/add_on_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/add_on_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/add_on_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/add_on_preview_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/add_on_preview_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/add_on_preview_v1.py` & `seeq-60.1.1/seeq/sdk/models/add_on_preview_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/add_on_tool_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/add_on_tool_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/add_on_tool_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/add_on_tool_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/administrator_contact_information_v1.py` & `seeq-60.1.1/seeq/sdk/models/administrator_contact_information_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/agent_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/agent_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/agent_key_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/agent_key_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/agent_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/agent_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/agent_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/agent_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/agent_status_v1.py` & `seeq-60.1.1/seeq/sdk/models/agent_status_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/annotation_image_link_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/annotation_image_link_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/annotation_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/annotation_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/annotation_interest_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/annotation_interest_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/annotation_interest_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/annotation_interest_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/annotation_list_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/annotation_list_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/annotation_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/annotation_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/archive_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/archive_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_batch_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_batch_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_error.py` & `seeq-60.1.1/seeq/sdk/models/asset_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_group_asset_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_group_asset_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_group_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_group_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_group_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_group_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_group_root_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_group_root_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_group_tree_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_group_tree_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_selection_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_selection_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_selection_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_selection_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_tree_batch_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_tree_batch_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_tree_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_tree_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/asset_tree_single_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/asset_tree_single_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/audit_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/audit_output_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/audit_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/audit_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/auth_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/auth_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/auth_providers_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/auth_providers_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/cache_info_v1.py` & `seeq-60.1.1/seeq/sdk/models/cache_info_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/calculated_item_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/calculated_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/capsule_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/capsule_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/capsule_property_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/capsule_property_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/capsule_property_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/capsule_property_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/capsule_v1.py` & `seeq-60.1.1/seeq/sdk/models/capsule_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/capsules_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/capsules_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/capsules_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/capsules_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/capsules_overwrite_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/capsules_overwrite_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/channel_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/channel_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/condition_batch_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/condition_batch_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/condition_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/condition_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/condition_monitor_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/condition_monitor_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/condition_monitor_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/condition_monitor_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/condition_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/condition_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/condition_update_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/condition_update_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/configuration_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/configuration_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/configuration_option_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/configuration_option_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/configuration_option_output_simple_v1.py` & `seeq-60.1.1/seeq/sdk/models/configuration_option_output_simple_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/configuration_option_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/configuration_option_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/configuration_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/configuration_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/configured_directives_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/configured_directives_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/connection_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/connection_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/connection_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/connection_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/connection_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/connection_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/connection_status_v1.py` & `seeq-60.1.1/seeq/sdk/models/connection_status_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/connections_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/connections_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/connector_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/connector_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/connector_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/connector_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/connectors_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/connectors_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/content_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/content_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/content_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/content_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/content_with_metadata_list_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/content_with_metadata_list_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/content_with_metadata_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/content_with_metadata_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/csv_datafile_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/csv_datafile_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datafile_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/datafile_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datafile_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/datafile_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datafiles_csv_body.py` & `seeq-60.1.1/seeq/sdk/models/datafiles_csv_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_clean_up_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_clean_up_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_clean_up_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_clean_up_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_preview_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_statistics_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_statistics_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_status_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_status_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasource_summary_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasource_summary_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/datasources_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/datasources_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/date_range_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/date_range_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/date_range_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/date_range_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/detailed_meter_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/detailed_meter_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/detailed_timer_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/detailed_timer_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/directive_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/directive_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/display_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/display_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/display_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/display_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/display_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/display_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/display_template_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/display_template_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/display_template_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/display_template_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/display_template_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/display_template_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/document_backup_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/document_backup_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/email_notification_recipient_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/email_notification_recipient_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/export_item_v1.py` & `seeq-60.1.1/seeq/sdk/models/export_item_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/export_items_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/export_items_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/export_items_v1.py` & `seeq-60.1.1/seeq/sdk/models/export_items_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/export_preview_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/export_preview_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/export_preview_v1.py` & `seeq-60.1.1/seeq/sdk/models/export_preview_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/folded_stack_node_v1.py` & `seeq-60.1.1/seeq/sdk/models/folded_stack_node_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/folder_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/folder_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/folder_navigation_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/folder_navigation_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/folder_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/folder_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_compile_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_compile_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_compiler_error_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_compiler_error_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_dependency_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_dependency_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_doc_example_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_doc_example_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_doc_example_list_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_doc_example_list_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_doc_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_doc_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_doc_keyword_list_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_doc_keyword_list_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_doc_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_doc_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_doc_summaries_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_doc_summaries_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_doc_summary_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_doc_summary_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_error_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_error_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_example_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_example_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_item_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_item_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_item_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_log_entry.py` & `seeq-60.1.1/seeq/sdk/models/formula_log_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_log_entry_details.py` & `seeq-60.1.1/seeq/sdk/models/formula_log_entry_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_log_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_log_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_package_import_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_package_import_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_package_import_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_package_import_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_package_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_package_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_package_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_package_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_parameter_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_parameter_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_parameter_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_parameter_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_run_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_run_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_run_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_run_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_token.py` & `seeq-60.1.1/seeq/sdk/models/formula_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_update_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_update_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_upgrade_change_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_upgrade_change_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/formula_upgrade_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/formula_upgrade_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/function_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/function_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/function_parameter_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/function_parameter_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/function_variant_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/function_variant_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/gauge_datum_v1.py` & `seeq-60.1.1/seeq/sdk/models/gauge_datum_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/generic_table_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/generic_table_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_add_on_tools_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_add_on_tools_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_channels_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_channels_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_condition_monitor_items_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_condition_monitor_items_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_content_items_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_content_items_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_date_ranges_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_date_ranges_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_jobs_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_jobs_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_metrics_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_metrics_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_projects_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_projects_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_request_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_requests_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_requests_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_sample_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_sample_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_samples_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_samples_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/get_signals_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/get_signals_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/id_images_body.py` & `seeq-60.1.1/seeq/sdk/models/id_images_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/identity_mapping_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/identity_mapping_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/identity_mapping_v1.py` & `seeq-60.1.1/seeq/sdk/models/identity_mapping_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/identity_preview_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/identity_preview_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/identity_preview_v1.py` & `seeq-60.1.1/seeq/sdk/models/identity_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/indexing_parameters_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/indexing_parameters_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/installer_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/installer_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/interval_v1.py` & `seeq-60.1.1/seeq/sdk/models/interval_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/invalid_swap_out_v1.py` & `seeq-60.1.1/seeq/sdk/models/invalid_swap_out_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_batch_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_batch_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_dependency_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_dependency_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_id_list_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_id_list_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_parameter_of_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_parameter_of_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_preview_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_preview_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_preview_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_preview_with_assets_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_preview_with_assets_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_search_preview_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_search_preview_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_search_preview_paginated_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_search_preview_paginated_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_search_preview_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_search_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_swap_result_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_swap_result_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_update_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_update_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_user_attributes_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_user_attributes_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_user_attributes_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_user_attributes_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/item_with_swap_pairs_v1.py` & `seeq-60.1.1/seeq/sdk/models/item_with_swap_pairs_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/job_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/job_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/json_backup_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/json_backup_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/license_importer_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/license_importer_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/license_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/license_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/licensed_feature_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/licensed_feature_status_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/log_message.py` & `seeq-60.1.1/seeq/sdk/models/log_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/meter_datum_v1.py` & `seeq-60.1.1/seeq/sdk/models/meter_datum_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/migrate_editor_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/migrate_editor_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/monitor_definition_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/monitor_definition_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/monitor_definitions_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/monitor_definitions_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/monitor_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/monitor_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/monitor_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/monitor_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/monitor_values.py` & `seeq-60.1.1/seeq/sdk/models/monitor_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/monitors_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/monitors_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/notifiable_report_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/notifiable_report_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/notifiable_report_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/notifiable_report_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/notification_configuration_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/notification_configuration_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/optional_report_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/optional_report_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/parameter_doc_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/parameter_doc_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/permissions_v1.py` & `seeq-60.1.1/seeq/sdk/models/permissions_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/plugin_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/plugin_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/plugin_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/plugin_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/plugins_body.py` & `seeq-60.1.1/seeq/sdk/models/plugins_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/priority_v1.py` & `seeq-60.1.1/seeq/sdk/models/priority_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/progress_information_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/progress_information_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/project_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/project_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/project_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/project_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/property_href_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/property_href_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/property_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/property_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/property_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/property_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/put_asset_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/put_asset_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/put_scalar_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/put_scalar_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/put_scalars_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/put_scalars_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/put_signals_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/put_signals_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/put_user_groups_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/put_user_groups_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/referenced_items_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/referenced_items_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/regression_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/regression_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/remote_agent_directives_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/remote_agent_directives_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/remote_agent_status_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/remote_agent_status_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/remote_agent_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/remote_agent_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/report_input_item_v1.py` & `seeq-60.1.1/seeq/sdk/models/report_input_item_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/report_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/report_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/report_notification_configuration_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/report_notification_configuration_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/report_template_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/report_template_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/report_template_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/report_template_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/request_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/sample_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/sample_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/sample_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/sample_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/samples_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/samples_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/samples_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/samples_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/samples_overwrite_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/samples_overwrite_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/scalar_evaluate_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/scalar_evaluate_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/scalar_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/scalar_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/scalar_property_v1.py` & `seeq-60.1.1/seeq/sdk/models/scalar_property_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/scalar_value_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/scalar_value_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/scale_across_tree_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/scale_across_tree_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/schedulable_admin_list_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/schedulable_admin_list_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/schedulable_admin_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/schedulable_admin_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/schedulable_summary_day_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/schedulable_summary_day_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/schedulable_summary_week_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/schedulable_summary_week_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/schedule_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/schedule_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/schedule_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/schedule_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/scheduled_notebook_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/scheduled_notebook_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/scheduled_notebook_list_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/scheduled_notebook_list_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/scheduled_notebook_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/scheduled_notebook_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/screenshot_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/screenshot_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/see_also_doc_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/see_also_doc_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/send_logs_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/send_logs_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/server_build_info_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/server_build_info_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/server_load_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/server_load_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/server_spec_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/server_spec_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/server_status_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/server_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/signal_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/signal_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/signal_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/signal_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/signal_with_id_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/signal_with_id_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/status_message_base.py` & `seeq-60.1.1/seeq/sdk/models/status_message_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/subscription_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/subscription_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/subscription_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/subscription_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/subscription_update_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/subscription_update_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/supported_units_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/supported_units_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/swap_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/swap_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/swap_option_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/swap_option_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/swap_option_v1.py` & `seeq-60.1.1/seeq/sdk/models/swap_option_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/swap_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/swap_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/sync_progress.py` & `seeq-60.1.1/seeq/sdk/models/sync_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/sync_progress_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/sync_progress_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/system_license_body.py` & `seeq-60.1.1/seeq/sdk/models/system_license_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/table_column_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/table_column_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/threshold_metric_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/threshold_metric_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/threshold_metric_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/threshold_metric_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/threshold_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/threshold_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/timer_datum_v1.py` & `seeq-60.1.1/seeq/sdk/models/timer_datum_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/tree_item_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/tree_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/treemap_item_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/treemap_item_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/treemap_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/treemap_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/units_of_measure_batch_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/units_of_measure_batch_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/units_of_measure_item_v1.py` & `seeq-60.1.1/seeq/sdk/models/units_of_measure_item_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/units_of_measure_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/units_of_measure_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/usage_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/usage_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/usage_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/usage_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/usage_types_v1.py` & `seeq-60.1.1/seeq/sdk/models/usage_types_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/user_group_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/user_group_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/user_group_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/user_group_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/user_group_with_id_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/user_group_with_id_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/user_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/user_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/user_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/user_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/user_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/user_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/user_password_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/user_password_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/validate_cron_list_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/validate_cron_list_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/validate_cron_list_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/validate_cron_list_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/validate_cron_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/validate_cron_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/workbench_item_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/workbench_item_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/workbench_search_result_preview_v1.py` & `seeq-60.1.1/seeq/sdk/models/workbench_search_result_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/workbook_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/workbook_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/workbook_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/workbook_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/workbook_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/workbook_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/worksheet_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/worksheet_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/worksheet_output_list_v1.py` & `seeq-60.1.1/seeq/sdk/models/worksheet_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/worksheet_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/worksheet_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/workstep_input_v1.py` & `seeq-60.1.1/seeq/sdk/models/workstep_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/models/workstep_output_v1.py` & `seeq-60.1.1/seeq/sdk/models/workstep_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-60.0.3/seeq/sdk/rest.py` & `seeq-60.1.1/seeq/sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 60.0.3-SNAPSHOT
+    OpenAPI spec version: 60.1.1-SNAPSHOT
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `seeq-60.0.3/seeq.egg-info/PKG-INFO` & `seeq-60.1.1/seeq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq
-Version: 60.0.3
+Version: 60.1.1
 Summary: The Seeq SDK for Python
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-60.0.3/seeq.egg-info/SOURCES.txt` & `seeq-60.1.1/seeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeq-60.0.3/setup.py` & `seeq-60.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq",
-    version="60.0.3",
+    version="60.1.1",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="The Seeq SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

